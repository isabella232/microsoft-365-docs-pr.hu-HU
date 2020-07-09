---
title: Tartományi felhasználók szinkronizálása a Microsoft 365-tel
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
description: Szinkronizálja a tartományvezérelt felhasználókat a Microsoft 365 vállalati verzióval.
ms.openlocfilehash: af9cb7c9b2b639edc2375679a73ab41c4cf6de71
ms.sourcegitcommit: 5b769f74bcc76ac8d38aad815d1728824783cd9f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081910"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a><span data-ttu-id="1b2c8-103">Tartományi felhasználók szinkronizálása a Microsoft 365-tel</span><span class="sxs-lookup"><span data-stu-id="1b2c8-103">Synchronize domain users to Microsoft 365</span></span>

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="1b2c8-104">1. Felkészülés a címtár-szinkronizálásra</span><span class="sxs-lookup"><span data-stu-id="1b2c8-104">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="1b2c8-105">Mielőtt szinkronizálja a felhasználókat és a számítógépeket a helyi Active Directory tartományból, tekintse át [a Felkészülés a Microsoft 365-tel a címtár-szinkronizálásra](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization)című részt.</span><span class="sxs-lookup"><span data-stu-id="1b2c8-105">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Microsoft 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="1b2c8-106">Különösen:</span><span class="sxs-lookup"><span data-stu-id="1b2c8-106">In particular:</span></span>

   - <span data-ttu-id="1b2c8-107">Győződjön meg arról, hogy a következő attribútumokhoz nem találhatók ismétlődések a könyvtárban: **mail**, **proxyAddresses**és **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="1b2c8-107">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="1b2c8-108">Ezeknek az értékeknek egyedieknek kell lenniük, és minden ismétlődést el kell távolítani.</span><span class="sxs-lookup"><span data-stu-id="1b2c8-108">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="1b2c8-109">Azt javasoljuk, hogy minden helyi felhasználói fiókhoz konfigurálja a **userPrincipalName** (UPN) attribútumot úgy, hogy az megfeleljen a licencelt Microsoft 365-felhasználónak megfelelő elsődleges e-mail címnek.</span><span class="sxs-lookup"><span data-stu-id="1b2c8-109">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="1b2c8-110">Például: *mary.shelley@contoso.com* helyett *mary@contoso.local*</span><span class="sxs-lookup"><span data-stu-id="1b2c8-110">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="1b2c8-111">Ha az Active Directory tartomány nem irányítható utótaggal végződik, például *.local* vagy *.lan*, az internetes irányítható utótag (például *.com* vagy *.org)* helyett, állítsa be először a helyi felhasználói fiókok UPN-utónevét a [Címtár-szinkronizálásra](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization)nem irányítható tartomány előkészítése című részben leírtak szerint.</span><span class="sxs-lookup"><span data-stu-id="1b2c8-111">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

<span data-ttu-id="1b2c8-112">A **Run IdFix** az alábbi negyedik (4) lépésben azt is győződjön meg arról, hogy a helyszíni Active Directory készen áll a dir sync.</span><span class="sxs-lookup"><span data-stu-id="1b2c8-112">The **Run IdFix** in step four (4) below, will also make sure your on-premises Active Directory is ready for dir sync.</span></span>

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="1b2c8-113">2. Az Azure AD Connect telepítése és konfigurálása</span><span class="sxs-lookup"><span data-stu-id="1b2c8-113">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="1b2c8-114">Ha szinkronizálni szeretné a felhasználókat, csoportokat és névjegyeket a helyi Active Directoryból az Azure Active Directoryba, telepítse az Azure Active Directory Connectet, és állítsa be a címtár-szinkronizálást.</span><span class="sxs-lookup"><span data-stu-id="1b2c8-114">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> 

 1. <span data-ttu-id="1b2c8-115">A felügyeleti központban válassza a <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **telepítő lehetőséget** a bal oldali navigációs eszközben.</span><span class="sxs-lookup"><span data-stu-id="1b2c8-115">In the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> select **Setup** in the left nav.</span></span>

 2. <span data-ttu-id="1b2c8-116">A **Bejelentkezés és biztonság csoportban**válassza a **Nézet** lehetőséget a **szervezeti címtár felhasználók szinkronizálása csoportban.**</span><span class="sxs-lookup"><span data-stu-id="1b2c8-116">Under **Sign-in and security**, choose **View**  under **Sync users from your org's directory**.</span></span>

 3. <span data-ttu-id="1b2c8-117">A **felhasználók szinkronizálása a szervezet címtárlapján** válassza az **Első lépések**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="1b2c8-117">On the **Sync users from your org's directory** page, choose **Get started**.</span></span>

 4. <span data-ttu-id="1b2c8-118">Az első lépésben futtassa az IdFix eszközt a címtár-szinkronizáláselőkészítéséhez.</span><span class="sxs-lookup"><span data-stu-id="1b2c8-118">In the first step  run IdFix tool to prepare for Directory sync.</span></span>

 5. <span data-ttu-id="1b2c8-119">Kövesse a varázsló lépéseit az Azure AD Connect letöltéséhez, és használja azt a tartományáltal vezérelt felhasználók microsoft 365-tel való szinkronizálásához.</span><span class="sxs-lookup"><span data-stu-id="1b2c8-119">Follow the wizard steps to download Azure AD Connect and use it to synchronize your domain-controlled users to Microsoft 365.</span></span>


<span data-ttu-id="1b2c8-120">További információ A [Microsoft 365 címtár-szinkronizálásának beállítása.](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization)</span><span class="sxs-lookup"><span data-stu-id="1b2c8-120">See [Set up directory synchronization for Microsoft 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) to learn more.</span></span>

<span data-ttu-id="1b2c8-121">Az Azure AD Connect beállításainak konfigurálásakor azt javasoljuk, hogy engedélyezze **a jelszó-szinkronizálást**, a zökkenőmentes egyszeri bejelentkezést és a **jelszó-visszaírási** funkciót, amelyet a Microsoft 365 vállalati verzió is támogat. **Seamless Single Sign-On**</span><span class="sxs-lookup"><span data-stu-id="1b2c8-121">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="1b2c8-122">Az Azure AD Connect jelölőnégyzetén túl további lépések is bevannak téve a jelszó-visszaíráshoz.</span><span class="sxs-lookup"><span data-stu-id="1b2c8-122">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="1b2c8-123">További információ: [Útmutató: jelszó-visszaírás konfigurálása.](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="1b2c8-123">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

<span data-ttu-id="1b2c8-124">Ha tartományhoz csatlakozó Windows 10-eszközöket is kezelni szeretne, olvassa el [a Microsoft 365 Business Premium által felügyelt, tartományhoz csatlakozó Windows 10-eszközök engedélyezése](manage-windows-devices.md) hibrid Azure AD-csatlakozás beállításához című témakört.</span><span class="sxs-lookup"><span data-stu-id="1b2c8-124">If you want to manage domain-joined Windows 10 devices also, see [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set up a hybrid Azure AD Join.</span></span> 
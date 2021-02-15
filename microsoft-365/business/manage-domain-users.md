---
title: Tartományfelhasználók szinkronizálása a Microsoft 365-be
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
description: Szinkronizálja a tartományvezérelt felhasználókat a Microsoft 365 Vállalati verzióval.
ms.openlocfilehash: b40a995a1723808d2fd171c534e9131a891840ba
ms.sourcegitcommit: e56894917d2aae05705c3b9447388d10e2156183
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48841359"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a><span data-ttu-id="60e47-103">Tartományfelhasználók szinkronizálása a Microsoft 365-be</span><span class="sxs-lookup"><span data-stu-id="60e47-103">Synchronize domain users to Microsoft 365</span></span>

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="60e47-104">1. Felkészülés a címtár-szinkronizálásra</span><span class="sxs-lookup"><span data-stu-id="60e47-104">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="60e47-105">Mielőtt szinkronizálja a felhasználókat és a számítógépeket a helyi Active Directory-tartományból, tekintse át a Felkészülés a Címtár-szinkronizálásra a [Microsoft 365-ben.](https://docs.microsoft.com/microsoft-365/enterprise/prepare-for-directory-synchronization)</span><span class="sxs-lookup"><span data-stu-id="60e47-105">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="60e47-106">Különösen:</span><span class="sxs-lookup"><span data-stu-id="60e47-106">In particular:</span></span>

   - <span data-ttu-id="60e47-107">Győződjön meg arról, hogy a címtárban nincsenek ismétlődő attribútumok a következő attribútumok esetén: **mail,** **proxyAddresses** és **userPrincipalName.**</span><span class="sxs-lookup"><span data-stu-id="60e47-107">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="60e47-108">Ezeknek az értékeknek egyedinek kell lennie, az ismétlődő értékeket pedig el kell távolítani.</span><span class="sxs-lookup"><span data-stu-id="60e47-108">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="60e47-109">Azt javasoljuk, hogy állítsa be a **userPrincipalName** (UPN) attribútumot az egyes helyi felhasználói fiókokhoz úgy, hogy megegyeznek a licencelt Microsoft 365-felhasználónak megfelelő elsődleges e-mail-címmel.</span><span class="sxs-lookup"><span data-stu-id="60e47-109">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="60e47-110">Például: *mary.shelley@contoso.com* a *mary@contoso.local helyett*</span><span class="sxs-lookup"><span data-stu-id="60e47-110">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="60e47-111">Ha az Active Directory-tartomány egy nem átirányítható utótaggal (például *.local* vagy *.lan)* végződik egy internetes átirányítható utótag (például *.com* vagy *.org)* helyett, először módosítsa a helyi felhasználói fiókok UPN-utótagját a Nem átirányítható tartomány előkészítése [címtár-szinkronizálásra](https://docs.microsoft.com/microsoft-365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization)leírásának megfelelően.</span><span class="sxs-lookup"><span data-stu-id="60e47-111">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/microsoft-365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

<span data-ttu-id="60e47-112">Az alábbi, 4. lépésben lefutott **IdFix** futtatása azt is meg fogja győződni arról, hogy a helyszíni Active Directory készen áll a címtár-szinkronizálásra.</span><span class="sxs-lookup"><span data-stu-id="60e47-112">The **Run IdFix** in step four (4) below, will also make sure your on-premises Active Directory is ready for directory synchronization.</span></span>

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="60e47-113">2. Az Azure AD Connect telepítése és konfigurálása</span><span class="sxs-lookup"><span data-stu-id="60e47-113">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="60e47-114">Ha szinkronizálni szeretné a felhasználókat, csoportokat és névjegyeket a helyi Active Directoryból az Azure Active Directoryba, telepítse az Azure Active Directory Connectet, és állítsa be a címtár-szinkronizálást.</span><span class="sxs-lookup"><span data-stu-id="60e47-114">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> 

 1. <span data-ttu-id="60e47-115">A Felügyeleti [központban válassza](https://go.microsoft.com/fwlink/p/?linkid=2024339)a **bal** oldali navigációs sávOn a Beállítás lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="60e47-115">In the [admin center](https://go.microsoft.com/fwlink/p/?linkid=2024339), select **Setup** in the left nav.</span></span>

 2. <span data-ttu-id="60e47-116">A **Bejelentkezés és biztonság** csoportban válassza a **Nézet** lehetőséget a Felhasználók szinkronizálása csoportban a szervezet **címtárában.**</span><span class="sxs-lookup"><span data-stu-id="60e47-116">Under **Sign-in and security**, choose **View**  under **Sync users from your org's directory**.</span></span>

 3. <span data-ttu-id="60e47-117">A felhasználók **szinkronizálása a** szervezet címtárlapján válassza az **Első lépések lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="60e47-117">On the **Sync users from your org's directory** page, choose **Get started**.</span></span>

 4. <span data-ttu-id="60e47-118">Az első lépésben futtassa az IdFix eszközt a címtár-szinkronizálás előkészítéséhez.</span><span class="sxs-lookup"><span data-stu-id="60e47-118">In the first step  run IdFix tool to prepare for Directory sync.</span></span>

 5. <span data-ttu-id="60e47-119">A varázsló lépéseit követve töltse le az Azure AD Connectet, és ezzel szinkronizálja a tartományvezérelt felhasználókat a Microsoft 365-be.</span><span class="sxs-lookup"><span data-stu-id="60e47-119">Follow the wizard steps to download Azure AD Connect and use it to synchronize your domain-controlled users to Microsoft 365.</span></span>


<span data-ttu-id="60e47-120">További [információ: Címtár-szinkronizálás beállítása a Microsoft 365-ben.](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization)</span><span class="sxs-lookup"><span data-stu-id="60e47-120">See [Set up directory synchronization for Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) to learn more.</span></span>

<span data-ttu-id="60e47-121">Az Azure AD Connect beállításainak konfigurálásakor azt javasoljuk, hogy engedélyezze a  jelszó-szinkronizálást, a zökkenőmentes egyszeri bejelentkezést és a jelszóvisszaírási funkciót, amelyet a Microsoft 365 Vállalati verzió is támogat. </span><span class="sxs-lookup"><span data-stu-id="60e47-121">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="60e47-122">Az Azure AD Connect jelölőnégyzete után további lépésekkel is visszaírhatja a jelszavakat.</span><span class="sxs-lookup"><span data-stu-id="60e47-122">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="60e47-123">További információt a ["How-to: configure password writeback" (Jelszóvisszaírás konfigurálása)](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="60e47-123">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

<span data-ttu-id="60e47-124">Ha a tartományhoz csatlakozott Windows 10-es eszközöket is kezelni szeretné, a Tartományhoz csatlakozott [Windows 10-es](manage-windows-devices.md) eszközök kezelése a Microsoft 365 Vállalati prémium verzióval a hibrid Azure AD Join beállításához.</span><span class="sxs-lookup"><span data-stu-id="60e47-124">If you also want to manage domain-joined Windows 10 devices, see [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set up a hybrid Azure AD Join.</span></span> 
---
title: Tartományfelhasználók szinkronizálása a Microsoft 365-be
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: Szinkronizálja a tartomány által vezérelt felhasználókat a Microsoft 365 Vállalati verzióval.
ms.openlocfilehash: b477b8a1f35a790d6c49937c973c141ad9f90ad4
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578407"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a><span data-ttu-id="5565a-103">Tartományfelhasználók szinkronizálása a Microsoft 365-be</span><span class="sxs-lookup"><span data-stu-id="5565a-103">Synchronize domain users to Microsoft 365</span></span>

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="5565a-104">1. Felkészülés a címtár-szinkronizálásra</span><span class="sxs-lookup"><span data-stu-id="5565a-104">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="5565a-105">Mielőtt szinkronizálja a felhasználókat és a számítógépeket a helyi Active Directory-tartományból, tekintse át a Felkészülés a Címtár-szinkronizálásra a [Microsoft 365-bencímtár-szinkronizálásracímet.](../enterprise/prepare-for-directory-synchronization.md)</span><span class="sxs-lookup"><span data-stu-id="5565a-105">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Microsoft 365](../enterprise/prepare-for-directory-synchronization.md).</span></span> <span data-ttu-id="5565a-106">Különösen:</span><span class="sxs-lookup"><span data-stu-id="5565a-106">In particular:</span></span>

   - <span data-ttu-id="5565a-107">Győződjön meg arról, hogy a címtárban nem léteznek ismétlődő attribútumok a **következő** attribútumok esetén: mail , **proxyAddresses** és **userPrincipalName.**</span><span class="sxs-lookup"><span data-stu-id="5565a-107">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="5565a-108">Ezeknek az értékeknek egyedinek kell lennie, és az ismétlődéseket el kell távolítani.</span><span class="sxs-lookup"><span data-stu-id="5565a-108">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="5565a-109">Azt javasoljuk, hogy minden helyi felhasználói fiók **userPrincipalName** (UPN) attribútumát úgy konfigurálja, hogy megegyezzon a licencelt Microsoft 365-felhasználónak megfelelő elsődleges e-mail-címmel.</span><span class="sxs-lookup"><span data-stu-id="5565a-109">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="5565a-110">Például: *mary.shelley@contoso.com.local* mary@contoso *helyett*</span><span class="sxs-lookup"><span data-stu-id="5565a-110">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="5565a-111">Ha az Active Directory-tartomány egy nem átirányítható utótaggal végződik , például *.local* vagy *.lan*, internetes átirányítható utótag (például *.com* vagy *.org)* helyett, módosítsa a helyi felhasználói fiókok UPN-utótagját a Nem átirányítható tartomány előkészítése a [címtár-szinkronizáláshoz](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md)leírt módon.</span><span class="sxs-lookup"><span data-stu-id="5565a-111">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md).</span></span> 

<span data-ttu-id="5565a-112">Az **idFix futtatása** az alábbi negyedik lépésben (4) azt is meg kell győződni arról, hogy a helyszíni Active Directory készen áll-e a címtár-szinkronizálásra.</span><span class="sxs-lookup"><span data-stu-id="5565a-112">The **Run IdFix** in step four (4) below, will also make sure your on-premises Active Directory is ready for directory synchronization.</span></span>

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="5565a-113">2. Az Azure AD Connect telepítése és konfigurálása</span><span class="sxs-lookup"><span data-stu-id="5565a-113">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="5565a-114">Ha szinkronizálni szeretné a felhasználókat, csoportokat és névjegyeket a helyi Active Directoryból az Azure Active Directoryba, telepítse az Azure Active Directory Connect alkalmazást, és állítsa be a címtár-szinkronizálást.</span><span class="sxs-lookup"><span data-stu-id="5565a-114">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> 

 1. <span data-ttu-id="5565a-115">A Felügyeleti [központban válassza](https://go.microsoft.com/fwlink/p/?linkid=2024339)a bal oldali navigációs **sávon** a Beállítás lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="5565a-115">In the [admin center](https://go.microsoft.com/fwlink/p/?linkid=2024339), select **Setup** in the left nav.</span></span>

 2. <span data-ttu-id="5565a-116">A **Bejelentkezés és biztonság csoportban** válassza a Megtekintés lehetőséget a Felhasználók szinkronizálása a szervezet **címtárában csoportban.** </span><span class="sxs-lookup"><span data-stu-id="5565a-116">Under **Sign-in and security**, choose **View**  under **Sync users from your org's directory**.</span></span>

 3. <span data-ttu-id="5565a-117">A Felhasználók **szinkronizálása a szervezeti** címtárból lapon válassza az Első **lépések lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="5565a-117">On the **Sync users from your org's directory** page, choose **Get started**.</span></span>

 4. <span data-ttu-id="5565a-118">Az első lépésben futtassa az IdFix eszközt a címtár-szinkronizálásra való felkészüléshez.</span><span class="sxs-lookup"><span data-stu-id="5565a-118">In the first step  run IdFix tool to prepare for Directory sync.</span></span>

 5. <span data-ttu-id="5565a-119">A varázsló lépéseit követve töltse le az Azure AD Connectet, és szinkronizálja vele a tartomány által szabályozott felhasználókat a Microsoft 365-be.</span><span class="sxs-lookup"><span data-stu-id="5565a-119">Follow the wizard steps to download Azure AD Connect and use it to synchronize your domain-controlled users to Microsoft 365.</span></span>


<span data-ttu-id="5565a-120">További [információ: Címtár-szinkronizálás beállítása a Microsoft 365-ben.](../enterprise/set-up-directory-synchronization.md)</span><span class="sxs-lookup"><span data-stu-id="5565a-120">See [Set up directory synchronization for Microsoft 365](../enterprise/set-up-directory-synchronization.md) to learn more.</span></span>

<span data-ttu-id="5565a-121">Az Azure AD Connect beállításainak konfigurálásakor azt javasoljuk, hogy engedélyezze a  jelszó-szinkronizálást, a zökkenőmentes egyszeri bejelentkezést és a jelszóvisszaírási funkciót, amelyet a Microsoft 365 Vállalati verzió is támogat. </span><span class="sxs-lookup"><span data-stu-id="5565a-121">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="5565a-122">Az Azure AD Connect jelölőnégyzete után további lépésekkel is visszaírhatja a jelszavakat.</span><span class="sxs-lookup"><span data-stu-id="5565a-122">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="5565a-123">További információért lásd: [Hogyan: jelszóvisszaírás konfigurálása](/azure/active-directory/authentication/howto-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="5565a-123">For more information, see [How-to: configure password writeback](/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

<span data-ttu-id="5565a-124">Ha a tartományhoz csatlakozott Windows 10-es eszközöket is kezelni szeretné, tekintse át A tartományhoz csatlakozott [Windows 10-es](manage-windows-devices.md) eszközök microsoft 365 Vállalati prémium verzió által történő kezelése hibrid Azure AD-csatlakozás beállítását engedélyező cikkeket.</span><span class="sxs-lookup"><span data-stu-id="5565a-124">If you also want to manage domain-joined Windows 10 devices, see [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set up a hybrid Azure AD Join.</span></span>
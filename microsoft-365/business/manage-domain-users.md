---
title: A tartományi felhasználók szinkronizálása a Microsoft 365
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
description: Tartomány által felügyelt felhasználók szinkronizálása a Microsoft 365 vállalati verzióval.
ms.openlocfilehash: b40a995a1723808d2fd171c534e9131a891840ba
ms.sourcegitcommit: e56894917d2aae05705c3b9447388d10e2156183
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48841359"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a><span data-ttu-id="c7773-103">A tartományi felhasználók szinkronizálása a Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c7773-103">Synchronize domain users to Microsoft 365</span></span>

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="c7773-104">1. Felkészülés a címtár-szinkronizálásra</span><span class="sxs-lookup"><span data-stu-id="c7773-104">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="c7773-105">Mielőtt szinkronizálni szeretné a felhasználókat és a számítógépeket a helyi Active Directory-tartományból, tanulmányozza a [címtár-szinkronizálás előkészítése a Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/prepare-for-directory-synchronization)-ra című részt.</span><span class="sxs-lookup"><span data-stu-id="c7773-105">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="c7773-106">Különösen:</span><span class="sxs-lookup"><span data-stu-id="c7773-106">In particular:</span></span>

   - <span data-ttu-id="c7773-107">Győződjön meg arról, hogy a címtárban nincsenek ismétlődések a következő attribútumok esetében: **posta** , **ProxyAddresses** és **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="c7773-107">Make sure that no duplicates exist in your directory for the following attributes: **mail** , **proxyAddresses** , and **userPrincipalName**.</span></span> <span data-ttu-id="c7773-108">Ezeknek az értékeknek egyedinek kell lenniük, és minden ismétlődést el kell távolítani.</span><span class="sxs-lookup"><span data-stu-id="c7773-108">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="c7773-109">Azt javasoljuk, hogy állítsa be az **userPrincipalName** (UPN) attribútumot mindegyik helyi felhasználói fiókhoz, hogy megegyezzen a licenccel rendelkező Microsoft 365-felhasználóhoz tartozó elsődleges e-mail-címmel.</span><span class="sxs-lookup"><span data-stu-id="c7773-109">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="c7773-110">Például: *Mary.Shelley@contoso.com* helyett *Mary@contoso. local*</span><span class="sxs-lookup"><span data-stu-id="c7773-110">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="c7773-111">Ha az Active Directory-tartomány nem átirányítható (például. com vagy *. org* ) (például. *com* vagy. org) végződésű útválasztással *végződik, a* helyi felhasználói fiókokhoz tartozó UPN-utótagot a [címtár-szinkronizáláshoz nem útválasztásos tartomány](https://docs.microsoft.com/microsoft-365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization)létrehozása című témakörben leírtak szerint állítsa *be.*</span><span class="sxs-lookup"><span data-stu-id="c7773-111">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan* , instead of an internet routable suffix such as *.com* or *.org* , adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/microsoft-365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

<span data-ttu-id="c7773-112">A **Futtatás IdFix** az alábbi négy lépésben (4) az alábbi lépésekkel gondoskodhat arról is, hogy a helyszíni Active Directory készen áll a címtár-szinkronizálásra.</span><span class="sxs-lookup"><span data-stu-id="c7773-112">The **Run IdFix** in step four (4) below, will also make sure your on-premises Active Directory is ready for directory synchronization.</span></span>

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="c7773-113">2. az Azure AD Connect telepítése és beállítása</span><span class="sxs-lookup"><span data-stu-id="c7773-113">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="c7773-114">Ha a helyi Active Directoryból szeretné szinkronizálni a felhasználókat, a csoportokat és a névjegyeket az Azure Active Directoryhoz, telepítse az Azure Active Directory Connect alkalmazást, és állítsa be a címtár-szinkronizálást.</span><span class="sxs-lookup"><span data-stu-id="c7773-114">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> 

 1. <span data-ttu-id="c7773-115">A [felügyeleti központban](https://go.microsoft.com/fwlink/p/?linkid=2024339)válassza a **Setup (beállítás** ) lehetőséget a bal oldali navigációs sávon.</span><span class="sxs-lookup"><span data-stu-id="c7773-115">In the [admin center](https://go.microsoft.com/fwlink/p/?linkid=2024339), select **Setup** in the left nav.</span></span>

 2. <span data-ttu-id="c7773-116">A **Bejelentkezés és biztonság** csoportban válassza **a szervezet címtárában lévő felhasználók szinkronizálása** csoportban a **nézet** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c7773-116">Under **Sign-in and security** , choose **View**  under **Sync users from your org's directory**.</span></span>

 3. <span data-ttu-id="c7773-117">A **felhasználók szinkronizálása a szervezeti címtárból** lapon válassza az első **lépések** elemet.</span><span class="sxs-lookup"><span data-stu-id="c7773-117">On the **Sync users from your org's directory** page, choose **Get started**.</span></span>

 4. <span data-ttu-id="c7773-118">Az első lépésben futtassa a IdFix eszközt a címtár-szinkronizálásra való felkészüléshez.</span><span class="sxs-lookup"><span data-stu-id="c7773-118">In the first step  run IdFix tool to prepare for Directory sync.</span></span>

 5. <span data-ttu-id="c7773-119">Kövesse a varázsló lépéseit az Azure AD Connect letöltéséhez, és használja azt a tartományba tartozó felhasználók szinkronizálásához a Microsoft 365-ban.</span><span class="sxs-lookup"><span data-stu-id="c7773-119">Follow the wizard steps to download Azure AD Connect and use it to synchronize your domain-controlled users to Microsoft 365.</span></span>


<span data-ttu-id="c7773-120">További információt a [címtár-szinkronizálás beállítása a Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) -hoz című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="c7773-120">See [Set up directory synchronization for Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) to learn more.</span></span>

<span data-ttu-id="c7773-121">Az Azure AD Connect beállításainak beállításakor javasoljuk, hogy engedélyezze a **Jelszó-szinkronizálást** , a **zökkenőmentes egyszeri bejelentkezést** és a jelszó- **writeback** szolgáltatást, amelyet a Microsoft 365 vállalati verzió is támogat.</span><span class="sxs-lookup"><span data-stu-id="c7773-121">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization** , **Seamless Single Sign-On** , and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="c7773-122">Az Azure AD Connect writeback kívül további lépéseket is találhat a jelszavakkal kapcsolatos további lépésekhez.</span><span class="sxs-lookup"><span data-stu-id="c7773-122">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="c7773-123">További információt a [jelszó-writeback beállítása](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="c7773-123">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

<span data-ttu-id="c7773-124">Ha a tartományhoz csatlakoztatott Windows 10-es eszközök kezelését is szeretné használni, olvassa el a [tartományhoz csatlakoztatott Windows 10-es eszközök kezelésének engedélyezése a Microsoft 365 vállalati prémium](manage-windows-devices.md) verzióban című témakört a hibrid Azure ad-illesztések beállításához.</span><span class="sxs-lookup"><span data-stu-id="c7773-124">If you also want to manage domain-joined Windows 10 devices, see [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set up a hybrid Azure AD Join.</span></span> 
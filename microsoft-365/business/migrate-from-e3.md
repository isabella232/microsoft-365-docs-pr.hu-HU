---
title: Áttelepítés Microsoft 365 Vállalati verzióba Office 365 E3 csomag
f1.keywords:
- NOCSH
ms.author: cmcatee
author: cmcatee-MSFT
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
- AdminTemplateSet
search.appverid:
- BCS160
- MET150
description: Ha van előfizetése Office 365 E3 csomag, de nincs több mint 300 alkalmazottja, fontolja meg a váltást a Microsoft 365 Vállalati prémium verzió.
ms.openlocfilehash: c1b4da07b3bf28cce1a48424ab45cde6ea54d367
ms.sourcegitcommit: 00f001019c653269d85718d410f970887d904304
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/12/2021
ms.locfileid: "53394171"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a><span data-ttu-id="d0a0d-103">Áttelepítés Office 365 E3 csomag Microsoft 365 Vállalati prémium verzió</span><span class="sxs-lookup"><span data-stu-id="d0a0d-103">Migrating from Office 365 E3 to Microsoft 365 Business Premium</span></span>

<span data-ttu-id="d0a0d-104">Microsoft 365 Vállalati prémium verzió rendelkezik mindennel, ami a kisvállalata számára szükséges, a legjobb, felhőalapú hatékonyságnövelő appokat egyszerű eszközkezeléssel és biztonsággal kombinálva.</span><span class="sxs-lookup"><span data-stu-id="d0a0d-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security.</span></span> <span data-ttu-id="d0a0d-105">Ha jelenleg Office 365 E3 csomag rendelkezik, de nincs több mint 300 alkalmazottja, fontolja meg a Microsoft 365 Vállalati prémium verzió-re való váltást a további biztonsági funkciókért.</span><span class="sxs-lookup"><span data-stu-id="d0a0d-105">If you currently have an Office 365 E3 subscription, but don't have more than 300 employees, consider switching to Microsoft 365 Business Premium for added security features.</span></span>

<span data-ttu-id="d0a0d-106">Az áttelepítés egyszerű: Először váltson a licencek között, és az aktuális előfizetésében lévő összes adata és felhasználói adata megmarad.</span><span class="sxs-lookup"><span data-stu-id="d0a0d-106">Migrating is easy: First you switch licenses and all your data and user information in your current subscription is maintained.</span></span> <span data-ttu-id="d0a0d-107">Az áttelepítés után be kell állítania a Microsoft 365 Vállalati prémium verzió.</span><span class="sxs-lookup"><span data-stu-id="d0a0d-107">After the migration, you'll need to set up the features that are added in Microsoft 365 Business Premium.</span></span>

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a><span data-ttu-id="d0a0d-108">Különbségek a Office 365 E3 csomag és a Microsoft 365 Vállalati prémium verzió</span><span class="sxs-lookup"><span data-stu-id="d0a0d-108">Differences between Office 365 E3 and Microsoft 365 Business Premium</span></span>

<span data-ttu-id="d0a0d-109">Az alábbi táblázat a két táblázatban Microsoft 365 Vállalati prémium verzió és a Office 365 E3 csomag.</span><span class="sxs-lookup"><span data-stu-id="d0a0d-109">This table shows the differences between Microsoft 365 Business Premium and Office 365 E3.</span></span>

| <span data-ttu-id="d0a0d-110">Funkció</span><span class="sxs-lookup"><span data-stu-id="d0a0d-110">Feature</span></span>    | <span data-ttu-id="d0a0d-111">Támogatás a Microsoft 365 Vállalati prémium verzió</span><span class="sxs-lookup"><span data-stu-id="d0a0d-111">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="d0a0d-112">Támogatás a Office 365 E3 csomag</span><span class="sxs-lookup"><span data-stu-id="d0a0d-112">Support in Office 365 E3</span></span> |
|:-------|:-----|:-----|
| <span data-ttu-id="d0a0d-113">**Helyszíni**</span><span class="sxs-lookup"><span data-stu-id="d0a0d-113">**On-premises**</span></span>        | | |
| <span data-ttu-id="d0a0d-114">Office alkalmazások<sup>1</sup></span><span class="sxs-lookup"><span data-stu-id="d0a0d-114">Office apps<sup>1</sup></span></span>    | <span data-ttu-id="d0a0d-115">Üzleti Microsoft 365-alkalmazások</span><span class="sxs-lookup"><span data-stu-id="d0a0d-115">Microsoft 365 Apps for business</span></span>    | <span data-ttu-id="d0a0d-116">Microsoft 365 Vállalati alkalmazások</span><span class="sxs-lookup"><span data-stu-id="d0a0d-116">Microsoft 365 Apps for enterprise</span></span> |
| <span data-ttu-id="d0a0d-117">**Felhőbeli hatékonyságnövelő alkalmazások**</span><span class="sxs-lookup"><span data-stu-id="d0a0d-117">**Cloud productivity apps**</span></span>        | | |
| <span data-ttu-id="d0a0d-118">Exchange Online és Outlook</span><span class="sxs-lookup"><span data-stu-id="d0a0d-118">Exchange Online and Outlook</span></span>    | <span data-ttu-id="d0a0d-119">Postaládánként 50 GB tárterületkorlát és korlátlan Exchange Online Archiválás</span><span class="sxs-lookup"><span data-stu-id="d0a0d-119">50 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span>    | <span data-ttu-id="d0a0d-120">Postaládánként 100 GB tárterületkorlát és korlátlan Exchange Online Archiválás</span><span class="sxs-lookup"><span data-stu-id="d0a0d-120">100 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span> |
| <span data-ttu-id="d0a0d-121">Teams</span><span class="sxs-lookup"><span data-stu-id="d0a0d-121">Teams</span></span>    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![Az Office 365 E3 csomag](../media/check-mark.png) | 
| <span data-ttu-id="d0a0d-124">OneDrive Vállalati verzió</span><span class="sxs-lookup"><span data-stu-id="d0a0d-124">OneDrive for Business</span></span>    | <span data-ttu-id="d0a0d-125">Felhasználónként 1 TB tárterületkorlát</span><span class="sxs-lookup"><span data-stu-id="d0a0d-125">1 TB storage limit per user</span></span>    | <span data-ttu-id="d0a0d-126">Korlátlan</span><span class="sxs-lookup"><span data-stu-id="d0a0d-126">Unlimited</span></span> | 
| <span data-ttu-id="d0a0d-127">Yammer, SharePoint, Planner, Stream</span><span class="sxs-lookup"><span data-stu-id="d0a0d-127">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![Az Office 365 E3 csomag](../media/check-mark.png) | 
| <span data-ttu-id="d0a0d-130">StaffHub</span><span class="sxs-lookup"><span data-stu-id="d0a0d-130">StaffHub</span></span>    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![Az Office 365 E3 csomag](../media/check-mark.png) |
| <span data-ttu-id="d0a0d-133">**Veszélyforrások elleni védelem**</span><span class="sxs-lookup"><span data-stu-id="d0a0d-133">**Threat Protection**</span></span>        | | |
| <span data-ttu-id="d0a0d-134">Defender a Office 365 1. csomaghoz</span><span class="sxs-lookup"><span data-stu-id="d0a0d-134">Defender for Office 365 Plan 1</span></span> | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | <span data-ttu-id="d0a0d-136">Nem tartalmazza, de a következőn használhatja:</span><span class="sxs-lookup"><span data-stu-id="d0a0d-136">Not included, but can be added on</span></span> |
| <span data-ttu-id="d0a0d-137">**Identitáskezelés**</span><span class="sxs-lookup"><span data-stu-id="d0a0d-137">**Identity management**</span></span>        | | |
| <span data-ttu-id="d0a0d-138">Önkiszolgáló jelszó-visszaállítás hibrid Azure Active Directory -fiókokhoz (Azure AD-fiókokhoz), Azure AD többtényezős hitelesítés (MFA), feltételes hozzáférés, jelszóvisszaírás a helyszíni identitásokhoz</span><span class="sxs-lookup"><span data-stu-id="d0a0d-138">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure AD multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    |  |
| <span data-ttu-id="d0a0d-140">**Eszköz- és alkalmazáskezelés**</span><span class="sxs-lookup"><span data-stu-id="d0a0d-140">**Device and app management**</span></span>        | | |
| <span data-ttu-id="d0a0d-141">Microsoft Intune, Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="d0a0d-141">Microsoft Intune, Windows AutoPilot</span></span>|     ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    |  |
| <span data-ttu-id="d0a0d-143">Megosztott számítógép aktiválása</span><span class="sxs-lookup"><span data-stu-id="d0a0d-143">Shared computer activation</span></span>|     ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![Az Office 365 E3 csomag](../media/check-mark.png)| 
| <span data-ttu-id="d0a0d-146">Frissítési jogok Windows 10 Pro Windows 7/8.1 verziós Pro verzióról</span><span class="sxs-lookup"><span data-stu-id="d0a0d-146">Upgrade rights to Windows 10 Pro from Win 7/8.1 Pro licenses</span></span>|     ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    ||
| <span data-ttu-id="d0a0d-148">**Információvédelem**</span><span class="sxs-lookup"><span data-stu-id="d0a0d-148">**Information protection**</span></span>        | | |
|<span data-ttu-id="d0a0d-149">Office 365 Adatveszteség-megelőzés</span><span class="sxs-lookup"><span data-stu-id="d0a0d-149">Office 365 Data Loss Prevention</span></span>|    ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)|![Az Office 365 E3 csomag](../media/check-mark.png)|
|<span data-ttu-id="d0a0d-152">Azure Information Protection Plan 1, BitLocker enforcement</span><span class="sxs-lookup"><span data-stu-id="d0a0d-152">Azure Information Protection Plan 1, BitLocker enforcement</span></span>|![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)||
|<span data-ttu-id="d0a0d-154">Azure Information Protection Plan 1, Bizalmasság-címkék</span><span class="sxs-lookup"><span data-stu-id="d0a0d-154">Azure Information Protection Plan 1, Sensitivity labels</span></span>|![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)||
|<span data-ttu-id="d0a0d-156">**Ügyfélelérési licenc (CAL-jogok)**</span><span class="sxs-lookup"><span data-stu-id="d0a0d-156">**Client Access License (CAL rights)**</span></span>|||
|<span data-ttu-id="d0a0d-157">Nagyvállalati CAL csomag (Exchange, SharePoint, Skype)</span><span class="sxs-lookup"><span data-stu-id="d0a0d-157">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span></span>||![Az Office 365 E3 csomag](../media/check-mark.png)|

<span data-ttu-id="d0a0d-159"><sup>1</sup> A Microsoft 365 Vállalati prémium verzió appok Office nem tartalmazza a mennyiségi aktiválást csoportházirenden, alkalmazás telemetrián, frissítési vezérlőn, számolótábla-összehasonlításon és -lekérdezésen keresztül, illetve az üzleti intelligencia segítségével.</span><span class="sxs-lookup"><span data-stu-id="d0a0d-159"><sup>1</sup> The Microsoft 365 Business Premium version of the Office apps doesn't include volume activation through Group Policy, app telemetry, update controls, spreadsheet compare and inquire, or business Intelligence.</span></span>

## <a name="migration"></a><span data-ttu-id="d0a0d-160">Áttelepítés</span><span class="sxs-lookup"><span data-stu-id="d0a0d-160">Migration</span></span>

<span data-ttu-id="d0a0d-161">Ha csak néhány embert [](../commerce/subscriptions/change-plans-manually.md) szeretne áthelyezni a csomagváltásba, az előfizetés áttelepítéséhez olvassa el a Csomagváltás manuálisan Microsoft 365 Vállalati prémium verzió.</span><span class="sxs-lookup"><span data-stu-id="d0a0d-161">To migrate your subscription, see [Change plans manually](../commerce/subscriptions/change-plans-manually.md) for instructions if you want to move just a few people to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="d0a0d-162">Automatikusan is [frissíthet](../commerce/subscriptions/upgrade-to-different-plan.md)mindenkit , vagy egy partnerrel együtt áthelyezheti az E3-előfizetését és -licenceit egy Microsoft 365 Vállalati prémium verzió előfizetésbe.</span><span class="sxs-lookup"><span data-stu-id="d0a0d-162">You can also [upgrade everyone automatically](../commerce/subscriptions/upgrade-to-different-plan.md), or work with a partner to move your E3 subscription and licenses to a Microsoft 365 Business Premium subscription.</span></span>
<span data-ttu-id="d0a0d-163">Az alábbi szakaszok ismertetik az esetlegesen szükséges módosításokat, valamint azt, hogy mit lehet tenni az áttelepítés után.</span><span class="sxs-lookup"><span data-stu-id="d0a0d-163">The following sections describe the changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="office-365-e3-subscription-configuration-and-data"></a><span data-ttu-id="d0a0d-164">Office 365 E3 csomag-előfizetés beállítása és adatai</span><span class="sxs-lookup"><span data-stu-id="d0a0d-164">Office 365 E3 subscription configuration and data</span></span>
<span data-ttu-id="d0a0d-165">Az áttelepítés előtt semmit sem kell változtatnia az aktuális előfizetésen vagy az adatain, beleértve az alábbi adatokat:</span><span class="sxs-lookup"><span data-stu-id="d0a0d-165">You don't need to do any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="d0a0d-166">Előfizetés-konfiguráció, például DNS-rekordok és tartománynevek.</span><span class="sxs-lookup"><span data-stu-id="d0a0d-166">Subscription configuration, such as DNS records and domain names.</span></span>
- <span data-ttu-id="d0a0d-167">Felhasználói és csoportfiókok, valamint hitelesítési beállítások, például többtényezős hitelesítés vagy feltételes hozzáférési házirendek.</span><span class="sxs-lookup"><span data-stu-id="d0a0d-167">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="d0a0d-168">Hatékonyságnövelő szolgáltatáskonfigurációk és adataik , például Teams, Exchange Online-postaládák, SharePoint Online webhelyek, OneDrive Vállalati verzió mappák és OneNote jegyzetfüzetek.</span><span class="sxs-lookup"><span data-stu-id="d0a0d-168">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>
- <span data-ttu-id="d0a0d-169">Office alkalmazások méretezése automatikusan megtörténik.</span><span class="sxs-lookup"><span data-stu-id="d0a0d-169">Office applications will scale automatically.</span></span> <span data-ttu-id="d0a0d-170">Office 365 a modern licencelés 72 óránként ellenőrzi a felhasználó licenc-hozzárendelését, és a Office-alkalmazásokat a felhasználói előfizetésnek megfelelő verzióra konvertálja.</span><span class="sxs-lookup"><span data-stu-id="d0a0d-170">Office 365 modern licensing will check the user’s license assignment every 72 hours and will convert Office applications to the version that matches the user subscription.</span></span>

### <a name="windows-10"></a><span data-ttu-id="d0a0d-171">Windows 10 rendszer esetén</span><span class="sxs-lookup"><span data-stu-id="d0a0d-171">Windows 10</span></span>

<span data-ttu-id="d0a0d-172">Ha a Windows még nem frissítette a Windows Pro alkotói frissítést, frissítse őket [a Windows Pro alkotói frissítésre.](upgrade-to-windows-pro-creators-update.md)</span><span class="sxs-lookup"><span data-stu-id="d0a0d-172">If your Windows aren't already on Windows Pro Creator update, [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

### <a name="set-up-policies-to-protect-user-devices-and-files"></a><span data-ttu-id="d0a0d-173">Házirendek beállítása a felhasználói eszközök és fájlok védelméhez</span><span class="sxs-lookup"><span data-stu-id="d0a0d-173">Set up policies to protect user devices and files</span></span>

> [!NOTE]
> <span data-ttu-id="d0a0d-174">Ha több MDM Office 365-házirendet és -eszközt is beállított,  ezek az eszközök az Eszközök lapon fognak Microsoft 365 Felügyeleti központ.</span><span class="sxs-lookup"><span data-stu-id="d0a0d-174">If you set up Office 365 MDM policies and devices, those devices will be listed on the **Devices** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="d0a0d-175">Az Ön által beállított házirendek az Intune portál klasszikus házirendek [listájában megjelenik.](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)</span><span class="sxs-lookup"><span data-stu-id="d0a0d-175">Any policies you set up will show up in the list of classic policies in the [Intune portal](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span></span>

<span data-ttu-id="d0a0d-176">Miután hozzárendelt licenceket a Microsoft 365 Vállalati prémium verzió, elkezdheti védeni a felhasználók eszközeit és fájljait.</span><span class="sxs-lookup"><span data-stu-id="d0a0d-176">After you have assigned licenses to Microsoft 365 Business Premium, you can start protecting the users' devices and files.</span></span>

<span data-ttu-id="d0a0d-177">Ha szervezetében mindenkit frissített a Microsoft 365 Vállalati prémium verzió-frissítésre, a kezdőlapon használhatja a beállítási varázslót, és a telepítővarázsló lépéseit követve védheti a fájlokat és a mobileszközeket a [Microsoft 365 Vállalati prémium verzió](set-up.md) beállítási varázslóban.</span><span class="sxs-lookup"><span data-stu-id="d0a0d-177">If you upgraded everyone in your organization to Microsoft 365 Business Premium, you'll see the setup wizard on the Home page, and can follow the [Set up Microsoft 365 Business Premium in the setup wizard](set-up.md) steps to protect files and mobile devices.</span></span>

<span data-ttu-id="d0a0d-178">Az Eszközök lapon az alábbi lépéseket is végre tudja tenni:</span><span class="sxs-lookup"><span data-stu-id="d0a0d-178">You can also complete these steps on the Devices page:</span></span>
  
1. <span data-ttu-id="d0a0d-179">A felügyeleti központ bal oldali navigációs  sávjában menjen az Eszköz \> **házirendek lapra.**</span><span class="sxs-lookup"><span data-stu-id="d0a0d-179">In the admin center, in the left nav, go to **Devices** \> **Policies**.</span></span>

2. <span data-ttu-id="d0a0d-180">Az Eszköz **házirendek lapon** válassza a Hozzáadás **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="d0a0d-180">On the **Device policies** page, choose **Add**.</span></span>

3. <span data-ttu-id="d0a0d-181">A Házirend **hozzáadása ablaktáblában** nevezze el a házirendet, majd válasszon **egy** Házirendtípust a legördülő menüből.</span><span class="sxs-lookup"><span data-stu-id="d0a0d-181">In the **Add policy** pane give the policy a name, and then choose a **Policy type** from the drop-down.</span></span>

     <span data-ttu-id="d0a0d-182">Alkalmazás-konfigurációs házirendeket állíthat be az Android- és iPhone-eszközökön, valamint az Windows 10-ban lévő fájlok védelmére, valamint eszközkonfigurációs házirendeket állíthat be a vállalati tulajdonú Windows 10 eszközökön.</span><span class="sxs-lookup"><span data-stu-id="d0a0d-182">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="d0a0d-183">A részleteket az alábbi hivatkozásokra kattintva olvashatja el:</span><span class="sxs-lookup"><span data-stu-id="d0a0d-183">See the following links for details:</span></span>

  - [<span data-ttu-id="d0a0d-184">Appvédelmi beállítások megadása androidos vagy iOS-es eszközökhöz</span><span class="sxs-lookup"><span data-stu-id="d0a0d-184">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)

  - [<span data-ttu-id="d0a0d-185">Alkalmazásvédelmi beállítások megadása Windows 10-es eszközökhöz</span><span class="sxs-lookup"><span data-stu-id="d0a0d-185">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)

  - [<span data-ttu-id="d0a0d-186">Eszközvédelmi beállítások megadása Windows 10 PC-khez</span><span class="sxs-lookup"><span data-stu-id="d0a0d-186">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  
4. <span data-ttu-id="d0a0d-187">A házirendek beállítása után Ön és alkalmazottai eszközeiket is beállíthatja:</span><span class="sxs-lookup"><span data-stu-id="d0a0d-187">Once you set up policies, you and your employees can set up devices:</span></span>

  - <span data-ttu-id="d0a0d-188">Az [eszköz Windows beállítása Microsoft 365 Vállalati prémium verzió felhasználók](set-up-windows-devices.md) számára Windows lépéseket.</span><span class="sxs-lookup"><span data-stu-id="d0a0d-188">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 

  - <span data-ttu-id="d0a0d-189">Az [Android-telefonok és](set-up-mobile-devices.md) iPhone-ok használatának Microsoft 365 Vállalati prémium verzió beállítása a mobileszközök számára.</span><span class="sxs-lookup"><span data-stu-id="d0a0d-189">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 
  
### <a name="mailbox-size"></a><span data-ttu-id="d0a0d-190">Postaláda mérete</span><span class="sxs-lookup"><span data-stu-id="d0a0d-190">Mailbox Size</span></span>

<span data-ttu-id="d0a0d-191">Microsoft 365 Vállalati prémium verzió 50 GB-os tárterületkorlátot használ az 1. Exchange Online használ.</span><span class="sxs-lookup"><span data-stu-id="d0a0d-191">Microsoft 365 Business Premium has a 50 GB storage limit as it uses Exchange Online Plan 1.</span></span> <span data-ttu-id="d0a0d-192">Az Microsoft 365 Vállalati prémium verzió-re való áttelepítés során, ha a felhasználók bármelyike meghaladja az 50 GB-os postaláda-tárterületet, javasoljuk, hogy rendeljen a felhasználóhoz egy Exchange Online 2. csomaggal, és távolítsa el az Exchange Online 1. csomagját, mivel mindkettőt nem lehet hozzárendelni.</span><span class="sxs-lookup"><span data-stu-id="d0a0d-192">While migrating to Microsoft 365 Business Premium, if any of your users exceed 50 GB of mailbox storage, it is recommended that you assign this user an Exchange Online Plan 2 and remove the Exchange Online Plan 1 as it's not feasible to assign both.</span></span>

### <a name="threat-protection"></a><span data-ttu-id="d0a0d-193">Veszélyforrások elleni védelem</span><span class="sxs-lookup"><span data-stu-id="d0a0d-193">Threat protection</span></span>

<span data-ttu-id="d0a0d-194">Az áttelepítés után Microsoft 365 Vállalati prémium verzió Defender Office 365.</span><span class="sxs-lookup"><span data-stu-id="d0a0d-194">After migrating to Microsoft 365 Business Premium, you have Defender for Office 365.</span></span> <span data-ttu-id="d0a0d-195">További [áttekintést a Microsoft Defender Office 365](../security/office-365-security/defender-for-office-365.md) talál.</span><span class="sxs-lookup"><span data-stu-id="d0a0d-195">See [Microsoft Defender for Office 365](../security/office-365-security/defender-for-office-365.md) for an overview.</span></span> <span data-ttu-id="d0a0d-196">A beállításról [](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)további Széf, a mellékletek Széf [és](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)az Adathalászat elleni védelem beállítása a [Defenderben a](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)Office 365.</span><span class="sxs-lookup"><span data-stu-id="d0a0d-196">To set up, see [set up Safe Links](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [set up Safe Attachments](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), and [set up Anti-phishing in Defender for Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span></span>

### <a name="sensitivity-labels"></a><span data-ttu-id="d0a0d-197">Érzékenységi címkék</span><span class="sxs-lookup"><span data-stu-id="d0a0d-197">Sensitivity labels</span></span>

<span data-ttu-id="d0a0d-198">A bizalmasság-címkék használatának elkezdését a Bizalmasság-címkék áttekintése és a bizalmasság-címkék létrehozása és [kezelése videóban](../business-video/create-sensitivity-labels.md) olvashatja. [](../compliance/sensitivity-labels.md)</span><span class="sxs-lookup"><span data-stu-id="d0a0d-198">To start using sensitivity labels, see [Overview of sensitivity labels](../compliance/sensitivity-labels.md) and [create and manage sensitivity labels](../business-video/create-sensitivity-labels.md) video.</span></span>

## <a name="related-content"></a><span data-ttu-id="d0a0d-199">Kapcsolódó tartalom</span><span class="sxs-lookup"><span data-stu-id="d0a0d-199">Related content</span></span>

<span data-ttu-id="d0a0d-200">[Csomagváltás kézzel](../commerce/subscriptions/change-plans-manually.md) (cikk)</span><span class="sxs-lookup"><span data-stu-id="d0a0d-200">[Change plans manually](../commerce/subscriptions/change-plans-manually.md) (article)</span></span>\
<span data-ttu-id="d0a0d-201">[Az Windows-eszközök frissítése Windows 10 Pro](upgrade-to-windows-pro-creators-update.md) (videó)</span><span class="sxs-lookup"><span data-stu-id="d0a0d-201">[Upgrade Windows devices to Windows 10 Pro](upgrade-to-windows-pro-creators-update.md) (video)</span></span>\
<span data-ttu-id="d0a0d-202">[Appvédelmi beállítások megadása Android- és iOS-eszközökön](app-protection-settings-for-android-and-ios.md) (cikk)</span><span class="sxs-lookup"><span data-stu-id="d0a0d-202">[Set app protection settings for Android or iOS devices](app-protection-settings-for-android-and-ios.md) (article)</span></span>\
<span data-ttu-id="d0a0d-203">[Alkalmazásvédelmi beállítások](protection-settings-for-windows-10-devices.md) megadása és szerkesztése Windows 10 eszközökön (cikk)</span><span class="sxs-lookup"><span data-stu-id="d0a0d-203">[Set or edit application protection settings for Windows 10 devices](protection-settings-for-windows-10-devices.md) (article)</span></span>\
<span data-ttu-id="d0a0d-204">[]</span><span class="sxs-lookup"><span data-stu-id="d0a0d-204">[]</span></span>


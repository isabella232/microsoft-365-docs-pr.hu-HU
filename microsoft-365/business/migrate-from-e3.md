---
title: Áttelepítés a Microsoft 365 Vállalati verzióra az Office 365 E3-ból
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
description: Megtudhatja, hogy miként helyezheti át vállalkozását a Microsoft 365 Vállalati Prémium verzióra az Office 365 E3-ból.
ms.openlocfilehash: d72f0c52a745ff973868b6fdaa95efa1a37a3dbd
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/18/2020
ms.locfileid: "45081879"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a><span data-ttu-id="103a1-103">Áttérés az Office 365 E3-ról a Microsoft 365 Vállalati Prémium verzióra</span><span class="sxs-lookup"><span data-stu-id="103a1-103">Migrating from Office 365 E3 to Microsoft 365 Business Premium</span></span> 

<span data-ttu-id="103a1-104">A Microsoft 365 Business Premium mindent tartalmaz, amire szüksége lehet a kisvállalkozásához, kombinálva a kategóriájában legjobb felhőalapú hatékonyságnövelő alkalmazásokat az egyszerű eszközkezeléssel és biztonsággal.</span><span class="sxs-lookup"><span data-stu-id="103a1-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security.</span></span> <span data-ttu-id="103a1-105">Ha jelenleg Office 365 E3-előfizetéssel rendelkezik, de nem rendelkezik 300-nál több alkalmazottal, érdemes lehet átváltani a Microsoft 365 Vállalati Prémium verzióra a további biztonsági funkciók érdekében.</span><span class="sxs-lookup"><span data-stu-id="103a1-105">If you currently have an Office 365 E3 subscription, but don't have more than 300 employees, consider switching to Microsoft 365 Business Premium for added security features.</span></span>

<span data-ttu-id="103a1-106">Az áttelepítés egyszerű: Először licencet vált, és az aktuális előfizetésben lévő összes adat és felhasználói információ megmarad.</span><span class="sxs-lookup"><span data-stu-id="103a1-106">Migrating is easy: First you switch licenses and all your data and user information in your current subscription is maintained.</span></span> <span data-ttu-id="103a1-107">Az áttelepítés után be kell állítania a Microsoft 365 Vállalati prémium verzióban hozzáadott funkciókat.</span><span class="sxs-lookup"><span data-stu-id="103a1-107">After the migration, you'll need to set up the features that are added in Microsoft 365 Business Premium.</span></span>

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a><span data-ttu-id="103a1-108">Az Office 365 E3 és a Microsoft 365 Vállalati Prémium verzió közötti különbségek</span><span class="sxs-lookup"><span data-stu-id="103a1-108">Differences between Office 365 E3 and Microsoft 365 Business Premium</span></span>

<span data-ttu-id="103a1-109">Ez a táblázat a Microsoft 365 Vállalati Prémium verzió és az Office 365 E3 közötti különbségeket mutatja be.</span><span class="sxs-lookup"><span data-stu-id="103a1-109">This table shows the differences between Microsoft 365 Business Premium and Office 365 E3.</span></span>

| <span data-ttu-id="103a1-110">Funkció</span><span class="sxs-lookup"><span data-stu-id="103a1-110">Feature</span></span>    | <span data-ttu-id="103a1-111">Támogatás a Microsoft 365 Vállalati prémium verzióban</span><span class="sxs-lookup"><span data-stu-id="103a1-111">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="103a1-112">Támogatás az Office 365 E3-ban</span><span class="sxs-lookup"><span data-stu-id="103a1-112">Support in Office 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="103a1-113">**Helyszíni**</span><span class="sxs-lookup"><span data-stu-id="103a1-113">**On-premises**</span></span>        | | | 
| <span data-ttu-id="103a1-114">Office-alkalmazások<sup>1</sup></span><span class="sxs-lookup"><span data-stu-id="103a1-114">Office apps<sup>1</sup></span></span>    | <span data-ttu-id="103a1-115">Microsoft 365 alkalmazások üzleti célokra</span><span class="sxs-lookup"><span data-stu-id="103a1-115">Microsoft 365 Apps for business</span></span>    | <span data-ttu-id="103a1-116">Microsoft 365 nagyvállalati alkalmazások</span><span class="sxs-lookup"><span data-stu-id="103a1-116">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="103a1-117">**Felhőalapú hatékonyságnövelő alkalmazások**</span><span class="sxs-lookup"><span data-stu-id="103a1-117">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="103a1-118">Exchange Online és Outlook</span><span class="sxs-lookup"><span data-stu-id="103a1-118">Exchange Online and Outlook</span></span>    | <span data-ttu-id="103a1-119">50 GB tárhelykorlát postaládánként és korlátlan Exchange Online archiválás</span><span class="sxs-lookup"><span data-stu-id="103a1-119">50 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span>    | <span data-ttu-id="103a1-120">100 GB tárhelykorlát postafiókonként és korlátlan Exchange Online archiválás</span><span class="sxs-lookup"><span data-stu-id="103a1-120">100 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span> | 
| <span data-ttu-id="103a1-121">Csapat</span><span class="sxs-lookup"><span data-stu-id="103a1-121">Teams</span></span>    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![Az Office 365 E3 része](../media/check-mark.png) | 
| <span data-ttu-id="103a1-124">OneDrive Vállalati verzió</span><span class="sxs-lookup"><span data-stu-id="103a1-124">OneDrive for Business</span></span>    | <span data-ttu-id="103a1-125">Felhasználónként 1 TB tárhelykorlát</span><span class="sxs-lookup"><span data-stu-id="103a1-125">1 TB storage limit per user</span></span>    | <span data-ttu-id="103a1-126">Korlátlan</span><span class="sxs-lookup"><span data-stu-id="103a1-126">Unlimited</span></span> | 
| <span data-ttu-id="103a1-127">Yammer, SharePoint Online, Planner, Adatfolyam</span><span class="sxs-lookup"><span data-stu-id="103a1-127">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![Az Office 365 E3 része](../media/check-mark.png) | 
| <span data-ttu-id="103a1-130">StaffHub</span><span class="sxs-lookup"><span data-stu-id="103a1-130">StaffHub</span></span>    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![Az Office 365 E3 része](../media/check-mark.png) | 
| <span data-ttu-id="103a1-133">Outlook ügyfélmenedzser, MileIQ</span><span class="sxs-lookup"><span data-stu-id="103a1-133">Outlook Customer Manager, MileIQ</span></span>    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | | 
| <span data-ttu-id="103a1-135">**Veszélyforrások elleni védelem**</span><span class="sxs-lookup"><span data-stu-id="103a1-135">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="103a1-136">Office 365 Komplex veszélyforrások elleni védelem (ATP) 1.</span><span class="sxs-lookup"><span data-stu-id="103a1-136">Office 365 Advanced Threat Protection (ATP) Plan 1</span></span> | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | <span data-ttu-id="103a1-138">Nem tartalmazza, de hozzáadható a</span><span class="sxs-lookup"><span data-stu-id="103a1-138">Not included, but can be added on</span></span> | 
| <span data-ttu-id="103a1-139">**Identitáskezelés**</span><span class="sxs-lookup"><span data-stu-id="103a1-139">**Identity management**</span></span>        | | | 
| <span data-ttu-id="103a1-140">Önkiszolgáló jelszó-visszaállítás hibrid Azure Active Directory (Azure AD) fiókokhoz, Azure többtényezős hitelesítéshez (MFA), feltételes hozzáféréshez, jelszó-visszaírás a helyszíni identitásokhoz</span><span class="sxs-lookup"><span data-stu-id="103a1-140">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    |  | 
| <span data-ttu-id="103a1-142">**Eszköz- és alkalmazáskezelés**</span><span class="sxs-lookup"><span data-stu-id="103a1-142">**Device and app management**</span></span>        | | |
| <span data-ttu-id="103a1-143">Microsoft Intune, Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="103a1-143">Microsoft Intune, Windows AutoPilot</span></span>|     ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    |  |
| <span data-ttu-id="103a1-145">Megosztott számítógép aktiválása</span><span class="sxs-lookup"><span data-stu-id="103a1-145">Shared computer activation</span></span>|     ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![Az Office 365 E3 része](../media/check-mark.png)| 
| <span data-ttu-id="103a1-148">Frissítési jogok a Windows 10 Pro rendszerre a Win 7/8.1 Pro licencekből</span><span class="sxs-lookup"><span data-stu-id="103a1-148">Upgrade rights to Windows 10 Pro from Win 7/8.1 Pro licenses</span></span>|     ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    || 
| <span data-ttu-id="103a1-150">**Információvédelem**</span><span class="sxs-lookup"><span data-stu-id="103a1-150">**Information protection**</span></span>        | | |
|<span data-ttu-id="103a1-151">Az Office 365 adatvesztés-megelőzési megelőzése</span><span class="sxs-lookup"><span data-stu-id="103a1-151">Office 365 Data Loss Prevention</span></span>|    ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)|![Az Office 365 E3 része](../media/check-mark.png)|
|<span data-ttu-id="103a1-154">Azure Information Protection Plan 1, Bitlocker kényszerítés</span><span class="sxs-lookup"><span data-stu-id="103a1-154">Azure Information Protection Plan 1, Bitlocker enforcement</span></span>|![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)||
|<span data-ttu-id="103a1-156">Azure Information Protection Plan 1, Érzékenységi címkék</span><span class="sxs-lookup"><span data-stu-id="103a1-156">Azure Information Protection Plan 1, Sensitivity labels</span></span>|![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)||
|<span data-ttu-id="103a1-158">**Ügyféllicenc (CAL-jogok)**</span><span class="sxs-lookup"><span data-stu-id="103a1-158">**Client Access License (CAL rights)**</span></span>|||
|<span data-ttu-id="103a1-159">Vállalati CAL Suite (Exchange, SharePoint, Skype)</span><span class="sxs-lookup"><span data-stu-id="103a1-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span></span>||![Az Office 365 E3 része](../media/check-mark.png)|

<span data-ttu-id="103a1-161"><sup>1</sup> Az Office-alkalmazások Microsoft 365 Vállalati Prémium verziója nem tartalmazza a mennyiségi aktiválást a csoportházirenden, az alkalmazástelemetriai adatokon, a frissítésvezérlőkön, a számolótábla-összehasonlításon és -lekérdezésen, illetve az üzleti intelligencián keresztül.</span><span class="sxs-lookup"><span data-stu-id="103a1-161"><sup>1</sup> The Microsoft 365 Business Premium version of the Office apps doesn't include volume activation through Group Policy, app telemetry, update controls, spreadsheet compare and inquire, or business Intelligence.</span></span>

## <a name="migration"></a><span data-ttu-id="103a1-162">Áttelepítési</span><span class="sxs-lookup"><span data-stu-id="103a1-162">Migration</span></span>

<span data-ttu-id="103a1-163">Az előfizetés áttelepítéséhez olvassa el a [Csomagküldő manuális átváltása](../commerce/subscriptions/change-plans-manually.md) című témakört, ha csak néhány embert szeretne áthelyezni a Microsoft 365 Business Premium szolgáltatásba.</span><span class="sxs-lookup"><span data-stu-id="103a1-163">To migrate your subscription, see [Change plans manually](../commerce/subscriptions/change-plans-manually.md) for instructions if you want to move just a few people to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="103a1-164">Emellett [mindenkit automatikusan](../commerce/subscriptions/upgrade-to-different-plan.md)frissíthet, vagy partnerrel együttműködve áthelyezheti e3-előfizetését és licenceit Microsoft 365 Business Premium előfizetésbe.</span><span class="sxs-lookup"><span data-stu-id="103a1-164">You can also [upgrade everyone automatically](../commerce/subscriptions/upgrade-to-different-plan.md), or work with a partner to move your E3 subscription and licenses to a Microsoft 365 Business Premium subscription.</span></span>
<span data-ttu-id="103a1-165">A következő szakaszok ismertetik a módosításokat, ha vannak ilyenek, és mit tehet az áttelepítés után.</span><span class="sxs-lookup"><span data-stu-id="103a1-165">The following sections describe the changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="office-365-e3-subscription-configuration-and-data"></a><span data-ttu-id="103a1-166">Az Office 365 E3 előfizetés konfigurációja és adatai</span><span class="sxs-lookup"><span data-stu-id="103a1-166">Office 365 E3 subscription configuration and data</span></span>
<span data-ttu-id="103a1-167">Az áttelepítés előtt nem kell módosítania az aktuális előfizetését vagy adatait, amely a következőket tartalmazza:</span><span class="sxs-lookup"><span data-stu-id="103a1-167">You don't need to do any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="103a1-168">Előfizetés-konfiguráció, például DNS-rekordok és tartománynevek.</span><span class="sxs-lookup"><span data-stu-id="103a1-168">Subscription configuration, such as DNS records and domain names.</span></span>
- <span data-ttu-id="103a1-169">Felhasználói és csoportfiókok és hitelesítési beállítások, például többtényezős hitelesítés vagy feltételes hozzáférési házirendek.</span><span class="sxs-lookup"><span data-stu-id="103a1-169">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="103a1-170">A hatékonyságnövelő szolgáltatás konfigurációi és adataik, például a Teams, az Exchange Online-postaládák, a SharePoint Online-webhelyek, a OneDrive Vállalati verzió mappái és a OneNote-jegyzetfüzetek.</span><span class="sxs-lookup"><span data-stu-id="103a1-170">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>
- <span data-ttu-id="103a1-171">Az Office-alkalmazások automatikusan méreteződnek.</span><span class="sxs-lookup"><span data-stu-id="103a1-171">Office applications will scale automatically.</span></span> <span data-ttu-id="103a1-172">Az Office 365 modern licencelése 72 óránként ellenőrzi a felhasználó licenchozzárendelését, és az Office-alkalmazásokat a felhasználói előfizetésnek megfelelő verzióra konvertálja.</span><span class="sxs-lookup"><span data-stu-id="103a1-172">Office 365 modern licensing will check the user’s license assignment every 72 hours and will convert Office applications to the version that matches the user subscription.</span></span>

### <a name="windows-10"></a><span data-ttu-id="103a1-173">Windows 10</span><span class="sxs-lookup"><span data-stu-id="103a1-173">Windows 10</span></span>

<span data-ttu-id="103a1-174">Ha a Windows még nem rendelkezik a Windows Pro Creator frissítésével, [frissítse őket a Windows Pro Alkotók frissítésére.](upgrade-to-windows-pro-creators-update.md)</span><span class="sxs-lookup"><span data-stu-id="103a1-174">If your Windows aren't already on Windows Pro Creator update, [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

### <a name="set-up-policies-to-protect-user-devices-and-files"></a><span data-ttu-id="103a1-175">Házirendek beállítása a felhasználói eszközök és fájlok védelmére</span><span class="sxs-lookup"><span data-stu-id="103a1-175">Set up policies to protect user devices and files</span></span>

> [!NOTE]
> <span data-ttu-id="103a1-176">Ha office 365 MDM-házirendeket és -eszközöket állít be, ezek az eszközök megjelennek a Microsoft 365 Felügyeleti központ **Eszközök** lapján.</span><span class="sxs-lookup"><span data-stu-id="103a1-176">If you set up Office 365 MDM policies and devices, those devices will be listed on the **Devices** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="103a1-177">A beállított házirendek megjelennek az [Intune portál](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)klasszikus szabályzatainak listájában.</span><span class="sxs-lookup"><span data-stu-id="103a1-177">Any policies you set up will show up in the list of classic policies in the [Intune portal](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span></span>

<span data-ttu-id="103a1-178">Miután licenceket rendelt a Microsoft 365 Business Premium szolgáltatáshoz, megkezdheti a felhasználók eszközeinek és fájljainak védelmét.</span><span class="sxs-lookup"><span data-stu-id="103a1-178">After you have assigned licenses to Microsoft 365 Business Premium, you can start protecting the users' devices and files.</span></span>

<span data-ttu-id="103a1-179">Ha a szervezet minden tagjára frissített microsoft 365 Vállalati prémium verzióra, a kezdőlapon megjelenik a beállítási varázsló, és a [telepítővarázsló lépéseiben a Microsoft 365 Business Premium beállítása](set-up.md) a telepítővarázsló lépéseit követve megvédheti a fájlokat és a mobileszközöket.</span><span class="sxs-lookup"><span data-stu-id="103a1-179">If you upgraded everyone in your organization to Microsoft 365 Business Premium, you'll see the setup wizard on the Home page, and can follow the [Set up Microsoft 365 Business Premium in the setup wizard](set-up.md) steps to protect files and mobile devices.</span></span>

<span data-ttu-id="103a1-180">Ezeket a lépéseket az Eszközök lapon is elvégezheti:</span><span class="sxs-lookup"><span data-stu-id="103a1-180">You can also complete these steps on the Devices page:</span></span>
  
1. <span data-ttu-id="103a1-181">A felügyeleti központban a bal oldali navigációs sávon nyissa meg az **Eszközök** \> **házirendje it.**</span><span class="sxs-lookup"><span data-stu-id="103a1-181">In the admin center, in the left nav, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="103a1-182">Az **Eszközházirendek** lapon válassza a **Hozzáadás gombot.**</span><span class="sxs-lookup"><span data-stu-id="103a1-182">On the **Device policies** page, choose **Add**.</span></span>
    
3. <span data-ttu-id="103a1-183">A **Házirend hozzáadása** ablaktáblán adjon nevet a házirendnek, majd válasszon egy **házirendtípust** a legördülő menüből.</span><span class="sxs-lookup"><span data-stu-id="103a1-183">In the **Add policy** pane give the policy a name, and then choose a **Policy type** from the drop-down.</span></span> 
    
     <span data-ttu-id="103a1-184">Beállíthat alkalmazásházirendeket az Android és iPhone eszközökön, valamint a Windows 10-en lévő fájlok védelmére, és eszközkonfigurációs házirendeket állíthat be a vállalat tulajdonában lévő Windows 10-es eszközökhöz.</span><span class="sxs-lookup"><span data-stu-id="103a1-184">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="103a1-185">A részleteket az alábbi linkeken találja:</span><span class="sxs-lookup"><span data-stu-id="103a1-185">See the following links for details:</span></span>
    
  - [<span data-ttu-id="103a1-186">Appvédelmi beállítások megadása androidos vagy iOS-es eszközökhöz</span><span class="sxs-lookup"><span data-stu-id="103a1-186">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="103a1-187">Alkalmazásvédelmi beállítások megadása Windows 10-es eszközökhöz</span><span class="sxs-lookup"><span data-stu-id="103a1-187">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="103a1-188">A Windows 10 rendszerű számítógépek eszközvédelmi beállításainak megadása</span><span class="sxs-lookup"><span data-stu-id="103a1-188">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  
4. <span data-ttu-id="103a1-189">A házirendek beállítása után Ön és az alkalmazottak beállíthatják az eszközöket:</span><span class="sxs-lookup"><span data-stu-id="103a1-189">Once you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="103a1-190">A [Windows-eszközök beállítása A Microsoft 365 Business Premium-felhasználók számára](set-up-windows-devices.md) a Windows-eszközökhöz szükséges lépéseket lásd.</span><span class="sxs-lookup"><span data-stu-id="103a1-190">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="103a1-191">Az Android-telefonokra és iPhone-okra vonatkozó lépésekért olvassa el [A mobileszközök beállítása Microsoft 365 Business Premium-felhasználók számára.](set-up-mobile-devices.md)</span><span class="sxs-lookup"><span data-stu-id="103a1-191">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 

### <a name="threat-protection"></a><span data-ttu-id="103a1-192">Veszélyforrások elleni védelem</span><span class="sxs-lookup"><span data-stu-id="103a1-192">Threat protection</span></span>

<span data-ttu-id="103a1-193">Miután áttelepítette a Microsoft 365 Vállalati Prémium verzióra, office 365 ATP-vel rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="103a1-193">After migrating to Microsoft 365 Business Premium, you have Office 365 ATP.</span></span> <span data-ttu-id="103a1-194">Az [Office 365 ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) című témakörben olvashat.</span><span class="sxs-lookup"><span data-stu-id="103a1-194">See [Office 365 ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) for an overview.</span></span> <span data-ttu-id="103a1-195">A beállításról az [ATP-biztonságos hivatkozások beállítása](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [az ATP-biztonságos mellékletek beállítása](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)és az [ATP adathalászat elleni beállítása.](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)</span><span class="sxs-lookup"><span data-stu-id="103a1-195">To set up, see [set up ATP safe links](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [set up ATP safe attachments](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), and [set up ATP anti-phishing](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span></span>

### <a name="sensitivity-labels"></a><span data-ttu-id="103a1-196">Érzékenységi címkék</span><span class="sxs-lookup"><span data-stu-id="103a1-196">Sensitivity labels</span></span>

<span data-ttu-id="103a1-197">Az érzékenységi címkék használatának megkezdéséhez olvassa [el az érzékenységi címkék áttekintése,](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) valamint [az érzékenységi címkék létrehozása és kezelése](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) című videót.</span><span class="sxs-lookup"><span data-stu-id="103a1-197">To start using sensitivity labels, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) and [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>

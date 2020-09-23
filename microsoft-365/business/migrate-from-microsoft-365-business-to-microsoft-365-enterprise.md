---
title: Áttérés a Microsoft 365 Business webhelyről a Microsoft 365 E3 csomagra
f1.keywords:
- NOCSH
ms.author: josephd
author: JoeDavies-MSFT
manager: laurawi
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: Megtudhatja, hogy miként helyezheti át vállalkozását a Microsoft 365 Business Premiumból a Microsoft 365 E3 csomagra.
ms.openlocfilehash: fbd5c0710bffa92cfc17447094bb9b2683641d5f
ms.sourcegitcommit: c083602dda3cdcb5b58cb8aa070d77019075f765
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48195519"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a><span data-ttu-id="ba0bb-103">Áttérés a Microsoft 365 Business premiumról a Microsoft 365 E3 csomagra</span><span class="sxs-lookup"><span data-stu-id="ba0bb-103">Migrate from Microsoft 365 Business Premium to Microsoft 365 E3</span></span>

<span data-ttu-id="ba0bb-104">A Microsoft 365 vállalati prémium verzióban mindent meg kell tennie a kisvállalati verzióhoz, amely egyesíti a legalkalmasabb felhőalapú hatékonyságnövelő alkalmazásokat az egyszerű eszközkezelés és-biztonság segítségével, amelyek lehetővé teszik az alkalmazottak számára a legmegfelelőbb munkát.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security that enable your employees to do their best work.</span></span> <span data-ttu-id="ba0bb-105">Bizonyos esetekben azonban előfordulhat, hogy a Microsoft 365 vállalati prémium verzióra szóló előfizetést át kell telepítenie a Microsoft 365 E3 csomagra.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-105">In some cases, however, you may need to migrate your Microsoft 365 Business Premium subscription to Microsoft 365 E3.</span></span> 

<span data-ttu-id="ba0bb-106">Üzleti tevékenysége például több mint 300-licenccel (Gratulálunk) bővült és szükséges.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-106">For example, your business has grown and needs more than 300 licenses (congratulations, by the way).</span></span>

<span data-ttu-id="ba0bb-107">Vagy az üzleti igények nagyvállalati funkciókat, többek között a Microsoft 365-alkalmazásokat, a Windows 10-es nagyvállalati E3 verziót vagy az Enterprise ügyfél-hozzáférési licenceket (CAL) kell megadniuk.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-107">Or, your business needs enterprise features, such as Microsoft 365 Apps for enterprise, Windows 10 Enterprise E3, or Enterprise Client Access Licenses (CALs).</span></span>

<span data-ttu-id="ba0bb-108">A frissítés egyszerű: a frissítés [a felügyeleti központból](../commerce/subscriptions/upgrade-to-different-plan.md)indítható el.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-108">Upgrading is easy: you can start the upgrade [from the Admin center](../commerce/subscriptions/upgrade-to-different-plan.md).</span></span> <span data-ttu-id="ba0bb-109">A jelenlegi előfizetésben lévő összes adatot és konfigurációt karbantartja.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-109">All your data and configuration in your current subscription is maintained.</span></span> <span data-ttu-id="ba0bb-110">Nem kell semmit sem tennie az áttelepítésre való felkészüléshez, és semmi teendőt sem kell tennie, kivéve az új funkciók előnyeit.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-110">There's nothing for you to do to prepare for the migration and nothing to do afterward, except take advantage of the new features.</span></span>

>[!Note]
><span data-ttu-id="ba0bb-111">A Microsoft 365 vállalati prémium verzióra szóló előfizetéssel akár 300 helyet is elérheti, és Microsoft 365 E3-előfizetést szerezhet a több mint 300 helyhez.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-111">You can also use a Microsoft 365 Business Premium subscription for up to 300 seats and get a Microsoft 365 E3 subscription for more than 300 seats.</span></span> <span data-ttu-id="ba0bb-112">Az Office 365 ATP azonban nem része a Microsoft 365 E3 csomagnak.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-112">However, Office 365 ATP is not included with Microsoft 365 E3.</span></span> <span data-ttu-id="ba0bb-113">A fenyegetések elleni védelem érdekében további Office 365-ös ATP-licenceket kell felvennie, hogy az Office 365-ös ATP-rendőrei minden felhasználója licenccel rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-113">For continued threat protection, you should add additional Office 365 ATP licenses so that all of the users in scope of your Office 365 ATP polices are licensed.</span></span>
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a><span data-ttu-id="ba0bb-114">A Microsoft 365 vállalati prémium verzió és a Microsoft 365 Enterprise közötti különbségek</span><span class="sxs-lookup"><span data-stu-id="ba0bb-114">Differences between Microsoft 365 Business Premium and Microsoft 365 Enterprise</span></span>

<span data-ttu-id="ba0bb-115">Ez a táblázat a Microsoft 365 Business Premium és a Microsoft 365 E3 közötti különbségeket mutatja be.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-115">This table shows the differences between Microsoft 365 Business Premium and Microsoft 365 E3.</span></span>

| <span data-ttu-id="ba0bb-116">Funkció</span><span class="sxs-lookup"><span data-stu-id="ba0bb-116">Feature</span></span>    | <span data-ttu-id="ba0bb-117">Támogatás a Microsoft 365 vállalati prémium verzióban</span><span class="sxs-lookup"><span data-stu-id="ba0bb-117">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="ba0bb-118">Támogatás a Microsoft 365 E3 csomaghoz</span><span class="sxs-lookup"><span data-stu-id="ba0bb-118">Support in Microsoft 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="ba0bb-119">**Helyszíni**</span><span class="sxs-lookup"><span data-stu-id="ba0bb-119">**On-premises**</span></span>        | | | 
| <span data-ttu-id="ba0bb-120">Windows 10</span><span class="sxs-lookup"><span data-stu-id="ba0bb-120">Windows 10</span></span>    | <span data-ttu-id="ba0bb-121">Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="ba0bb-121">Windows 10 Business</span></span>  |     <span data-ttu-id="ba0bb-122">Windows 10 nagyvállalati E3 csomag</span><span class="sxs-lookup"><span data-stu-id="ba0bb-122">Windows 10 Enterprise E3</span></span>| 
| <span data-ttu-id="ba0bb-123">Office-alkalmazások \*</span><span class="sxs-lookup"><span data-stu-id="ba0bb-123">Office apps\*</span></span>    | [<span data-ttu-id="ba0bb-124">Microsoft 365-alkalmazások vállalati verzió</span><span class="sxs-lookup"><span data-stu-id="ba0bb-124">Microsoft 365 Apps for business</span></span>](#office-365-business)    | <span data-ttu-id="ba0bb-125">Nagyvállalati Microsoft 365-alkalmazások</span><span class="sxs-lookup"><span data-stu-id="ba0bb-125">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="ba0bb-126">**Felhőbeli hatékonyságnövelő alkalmazások**</span><span class="sxs-lookup"><span data-stu-id="ba0bb-126">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="ba0bb-127">Exchange Online és Outlook</span><span class="sxs-lookup"><span data-stu-id="ba0bb-127">Exchange Online and Outlook</span></span>    | <span data-ttu-id="ba0bb-128">50 GB tárolási korlát egy postaládában és korlátlan Exchange Online archiválás</span><span class="sxs-lookup"><span data-stu-id="ba0bb-128">50 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span>    | <span data-ttu-id="ba0bb-129">100 GB tárolási korlát egy postaládában és korlátlan Exchange Online archiválás</span><span class="sxs-lookup"><span data-stu-id="ba0bb-129">100 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span> | 
| <span data-ttu-id="ba0bb-130">Teams</span><span class="sxs-lookup"><span data-stu-id="ba0bb-130">Teams</span></span>    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| <span data-ttu-id="ba0bb-133">OneDrive Vállalati verzió</span><span class="sxs-lookup"><span data-stu-id="ba0bb-133">OneDrive for Business</span></span>    | <span data-ttu-id="ba0bb-134">1 TB tárterület felhasználónként</span><span class="sxs-lookup"><span data-stu-id="ba0bb-134">1 TB storage limit per user</span></span>    | <span data-ttu-id="ba0bb-135">Korlátlan</span><span class="sxs-lookup"><span data-stu-id="ba0bb-135">Unlimited</span></span> | 
| <span data-ttu-id="ba0bb-136">Yammer, SharePoint Online, Planner, Stream</span><span class="sxs-lookup"><span data-stu-id="ba0bb-136">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| <span data-ttu-id="ba0bb-139">Outlook Customer Manager, MileIQ</span><span class="sxs-lookup"><span data-stu-id="ba0bb-139">Outlook Customer Manager, MileIQ</span></span>    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | | 
| <span data-ttu-id="ba0bb-141">**Veszélyforrások elleni védelem**</span><span class="sxs-lookup"><span data-stu-id="ba0bb-141">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="ba0bb-142">A támadási felület csökkentési lehetőségei</span><span class="sxs-lookup"><span data-stu-id="ba0bb-142">Attack surface reduction capabilities</span></span>    | [<span data-ttu-id="ba0bb-143">A lista megtekintése</span><span class="sxs-lookup"><span data-stu-id="ba0bb-143">See this list</span></span>](#threat-protection) | <span data-ttu-id="ba0bb-144">A Microsoft Edge hardver-alapú elkülönítésének vállalati kezelése</span><span class="sxs-lookup"><span data-stu-id="ba0bb-144">Enterprise management of hardware-based isolation for Microsoft Edge</span></span> | 
| <span data-ttu-id="ba0bb-145">Office 365 Advanced Threat Protection (ATP) csomag 1</span><span class="sxs-lookup"><span data-stu-id="ba0bb-145">Office 365 Advanced Threat Protection (ATP) Plan 1</span></span> | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | <span data-ttu-id="ba0bb-147">Nem szerepelnek, de hozzáadhatók</span><span class="sxs-lookup"><span data-stu-id="ba0bb-147">Not included, but can be added on</span></span> | 
| <span data-ttu-id="ba0bb-148">**Személyazonosság-kezelés**</span><span class="sxs-lookup"><span data-stu-id="ba0bb-148">**Identity management**</span></span>        | | | 
| <span data-ttu-id="ba0bb-149">Önkiszolgáló jelszó-visszaállítás a hibrid Azure Active Directory (Azure AD) fiókokhoz, Azure multi-Factor Authentication (MFA), feltételes hozzáférés, jelszó-writeback a helyszíni identitásokhoz</span><span class="sxs-lookup"><span data-stu-id="ba0bb-149">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| <span data-ttu-id="ba0bb-152">Felhőbeli app-felderítés, Azure AD Connect Health</span><span class="sxs-lookup"><span data-stu-id="ba0bb-152">Cloud App Discovery, Azure AD Connect Health</span></span>    |     | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| <span data-ttu-id="ba0bb-154">Azure AD Office 365-alkalmazások egyszeri bejelentkezés (SSO): 10 app felhasználónként (Gallery SaaS-alkalmazások, például Salesforce) \*</span><span class="sxs-lookup"><span data-stu-id="ba0bb-154">Azure AD Office 365 apps Single Sign-On (SSO): 10 apps per user (Gallery SaaS apps such as Salesforce)\*</span></span> | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| <span data-ttu-id="ba0bb-157">Azure AD prémium 1 egyszeri bejelentkezés: nincs korlátozás (helyszíni alkalmazások Azure AD Application proxyn és nem gyűjteményes alkalmazásokon keresztül, önkiszolgáló app-integrációs sablonok használatával)</span><span class="sxs-lookup"><span data-stu-id="ba0bb-157">Azure AD Premium 1 SSO: no limit (On-premises apps through Azure AD Application Proxy and non-gallery apps using Self-Service App Integration templates)</span></span>    |     | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| <span data-ttu-id="ba0bb-159">**Eszközök és alkalmazások kezelése**</span><span class="sxs-lookup"><span data-stu-id="ba0bb-159">**Device and app management**</span></span>        | | | 
| <span data-ttu-id="ba0bb-160">Microsoft Intune, Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="ba0bb-160">Microsoft Intune, Windows Autopilot</span></span>|     ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
|<span data-ttu-id="ba0bb-163">Virtuális asztali hozzáférés (VDA)</span><span class="sxs-lookup"><span data-stu-id="ba0bb-163">Virtual Desktop Access (VDA)</span></span>    |  |     ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
|<span data-ttu-id="ba0bb-165">Windows Virtual Desktop (WVD)</span><span class="sxs-lookup"><span data-stu-id="ba0bb-165">Windows Virtual Desktop (WVD)</span></span>    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png) |     ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
|<span data-ttu-id="ba0bb-168">Megosztott számítógép-aktiválás (SCA)</span><span class="sxs-lookup"><span data-stu-id="ba0bb-168">Shared Computer Activation (SCA)</span></span>    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png) |     ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| <span data-ttu-id="ba0bb-171">Microsoft asztali optimalizálási csomag</span><span class="sxs-lookup"><span data-stu-id="ba0bb-171">Microsoft Desktop Optimization Package</span></span>    | |     ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| <span data-ttu-id="ba0bb-173">**Adatvédelem**</span><span class="sxs-lookup"><span data-stu-id="ba0bb-173">**Information protection**</span></span>        | | | 
| <span data-ttu-id="ba0bb-174">Az Office 365 adatvesztés-megelőzése, Azure Information Protection Plan 1</span><span class="sxs-lookup"><span data-stu-id="ba0bb-174">Office 365 Data Loss Prevention, Azure Information Protection Plan 1</span></span>    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| <span data-ttu-id="ba0bb-177">Window Information Protection for Endpoint DLP</span><span class="sxs-lookup"><span data-stu-id="ba0bb-177">Window Information Protection for endpoint DLP</span></span>    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| <span data-ttu-id="ba0bb-180">**Ügyfél-hozzáférési licenc (CAL-jogok)**</span><span class="sxs-lookup"><span data-stu-id="ba0bb-180">**Client Access License (CAL rights)**</span></span>    | | |     
| <span data-ttu-id="ba0bb-181">Nagyvállalati CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)</span><span class="sxs-lookup"><span data-stu-id="ba0bb-181">Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)</span></span>| |         ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| <span data-ttu-id="ba0bb-183">**Megfelelőségi**</span><span class="sxs-lookup"><span data-stu-id="ba0bb-183">**Compliance**</span></span>        | | | 
| <span data-ttu-id="ba0bb-184">Korlátlan e-mail-archiválás</span><span class="sxs-lookup"><span data-stu-id="ba0bb-184">Unlimited email archiving</span></span>    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| <span data-ttu-id="ba0bb-187">Megfelelőségi vezető</span><span class="sxs-lookup"><span data-stu-id="ba0bb-187">Compliance Manager</span></span>    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| <span data-ttu-id="ba0bb-190">eDiscovery</span><span class="sxs-lookup"><span data-stu-id="ba0bb-190">eDiscovery</span></span>    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| <span data-ttu-id="ba0bb-193">Helyi visszatartás és jogi célú mentesség</span><span class="sxs-lookup"><span data-stu-id="ba0bb-193">In-place hold and litigation hold</span></span>    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| <span data-ttu-id="ba0bb-196">Üzenetküldési rekordok kezelése (MRM) adatmegőrzési címkék és adatmegőrzési házirendek</span><span class="sxs-lookup"><span data-stu-id="ba0bb-196">Messaging Records Management (MRM) retention tags and retention policies</span></span>    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
||||

<span data-ttu-id="ba0bb-199">\* Azok a felhasználók, akik hozzáféréssel rendelkeznek a SaaS-alkalmazásokhoz, beszerezhetnek egyszeri bejelentkezést, akár 10 alkalmazásba is.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-199">\* Users who have been assigned access to SaaS apps can get SSO access to up to 10 apps.</span></span> <span data-ttu-id="ba0bb-200">A rendszergazdák beállíthatják az egyszeri bejelentkezést, és módosíthatják a felhasználók hozzáférését a különböző SaaS-alkalmazásokhoz, az SSO-hozzáférés azonban csak felhasználónként 10 alkalmazásban engedélyezett egyszerre.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-200">Admins can configure SSO and change user access to different SaaS apps, but SSO access is only allowed for 10 apps per user at a time.</span></span> <span data-ttu-id="ba0bb-201">Minden Office 365-alkalmazás egyetlen alkalmazásként számítja ki.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-201">All Office 365 apps are counted as a single app.</span></span>

## <a name="migration"></a><span data-ttu-id="ba0bb-202">Áttelepítési</span><span class="sxs-lookup"><span data-stu-id="ba0bb-202">Migration</span></span>

<span data-ttu-id="ba0bb-203">A partnerekkel való áttelepítés érdekében a Microsoft 365 vállalati prémium verzióra szóló előfizetését és licenceit egy megfelelő Microsoft 365 E3-előfizetésre kell áthelyeznie a licencekkel.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-203">To migrate, work with your partner to move your Microsoft 365 Business Premium subscription and licenses to a suitable Microsoft 365 E3 subscription with its licenses.</span></span>

<span data-ttu-id="ba0bb-204">Az alábbi szakaszok ismertetik, hogy milyen módosításokat kell végrehajtania, ha vannak ilyenek, és hogy mit tehet az áttelepítés után.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-204">The following sections describe what changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="microsoft-365-subscription-configuration-and-data"></a><span data-ttu-id="ba0bb-205">Microsoft 365-előfizetés konfigurációja és adatainak</span><span class="sxs-lookup"><span data-stu-id="ba0bb-205">Microsoft 365 subscription configuration and data</span></span>

<span data-ttu-id="ba0bb-206">Az áttelepítés előtt nem kell módosítania a jelenlegi előfizetést vagy adatot, beleértve az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="ba0bb-206">You don't need to make any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="ba0bb-207">Előfizetés konfigurációja (például DNS-tartománynevek)</span><span class="sxs-lookup"><span data-stu-id="ba0bb-207">Subscription configuration, such as DNS domain names.</span></span>
- <span data-ttu-id="ba0bb-208">Felhasználók és csoportok fiókjai és hitelesítési beállításai, például többtényezős hitelesítés vagy feltételes hozzáférésű házirendek.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-208">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="ba0bb-209">A hatékonyságnövelő szolgáltatások konfigurációi és adatai, többek között a Teams, az Exchange Online-postaládák, a SharePoint Online-webhelyek, a OneDrive vállalati verziós mappák és a OneNote-jegyzetfüzetek.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-209">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>

<span data-ttu-id="ba0bb-210">A felhasználók mostantól korlátlan tárhelyet élvezhetnek az Exchange Online-postaládák és a OneDrive vállalati verzió mappáiban.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-210">Your users can now enjoy unlimited storage in the Exchange Online mailboxes and OneDrive for Business folders.</span></span>

<span data-ttu-id="ba0bb-211">Használhatja a Cloud app Discovery, az Azure AD Connect Health és az SSO több mint 10 alkalmazást.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-211">You can begin using Cloud App Discovery, Azure AD Connect Health, and SSO for more than 10 apps.</span></span>

>[!Note]
><span data-ttu-id="ba0bb-212">A Microsoft 365 E3-ba áttelepített felhasználók már nem használhatják az Outlook Customer Managert és a MileIQ.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-212">Users migrated to Microsoft 365 E3 can no longer use Outlook Customer Manager and MileIQ.</span></span>
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a><span data-ttu-id="ba0bb-213">Veszélyforrások elleni védelem</span><span class="sxs-lookup"><span data-stu-id="ba0bb-213">Threat protection</span></span>

<span data-ttu-id="ba0bb-214">A Windows 10 Business a következő védelmet foglalja magában:</span><span class="sxs-lookup"><span data-stu-id="ba0bb-214">Windows 10 Business includes these protections:</span></span>

- <span data-ttu-id="ba0bb-215">Az operációs rendszer indítási folyamatának integritása</span><span class="sxs-lookup"><span data-stu-id="ba0bb-215">Integrity enforcement of operating system boot up process</span></span>
- <span data-ttu-id="ba0bb-216">Az érzékeny operációs összetevők sértetlenségének érvényesítése</span><span class="sxs-lookup"><span data-stu-id="ba0bb-216">Integrity enforcement of sensitive operating components</span></span>
- <span data-ttu-id="ba0bb-217">Speciális biztonsági rések és a nulladik napi hibák enyhítése</span><span class="sxs-lookup"><span data-stu-id="ba0bb-217">Advanced vulnerability and zero-day exploit mitigations</span></span>
- <span data-ttu-id="ba0bb-218">Jó hírű hálózati védelem a Microsoft Edge, az Internet Explorer és a Chrome számára</span><span class="sxs-lookup"><span data-stu-id="ba0bb-218">Reputation-based network protection for Microsoft Edge, Internet Explorer, and Chrome</span></span>
- <span data-ttu-id="ba0bb-219">Host-alapú tűzfal</span><span class="sxs-lookup"><span data-stu-id="ba0bb-219">Host-based firewall</span></span>
- <span data-ttu-id="ba0bb-220">Ransomware enyhítése</span><span class="sxs-lookup"><span data-stu-id="ba0bb-220">Ransomware mitigations</span></span>
- <span data-ttu-id="ba0bb-221">Hardveres elkülönítés a Microsoft Edge-ben</span><span class="sxs-lookup"><span data-stu-id="ba0bb-221">Hardware-based isolation for Microsoft Edge</span></span>
- <span data-ttu-id="ba0bb-222">Az intelligens biztonsági diagram által működtetett alkalmazás-vezérlés</span><span class="sxs-lookup"><span data-stu-id="ba0bb-222">Application control powered by the Intelligent Security Graph</span></span>
- <span data-ttu-id="ba0bb-223">Device Control (USB)</span><span class="sxs-lookup"><span data-stu-id="ba0bb-223">Device control (USB)</span></span>
- <span data-ttu-id="ba0bb-224">Webes fenyegetések hálózati védelme</span><span class="sxs-lookup"><span data-stu-id="ba0bb-224">Network protection for web-based threats</span></span>
- <span data-ttu-id="ba0bb-225">A fogadó Behatolás-megelőzési szabályok</span><span class="sxs-lookup"><span data-stu-id="ba0bb-225">Host intrusion prevention rules</span></span>

<span data-ttu-id="ba0bb-226">A Windows 10 nagyvállalati E3 csomag a Microsoft Edge hardveres elkülönítésének vállalati kezelését is tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-226">Windows 10 Enterprise E3 also includes enterprise management of hardware-based isolation for Microsoft Edge.</span></span>

>[!Note]
><span data-ttu-id="ba0bb-227">A Microsoft 365 E3 rendszerre áttelepített felhasználók az Office 365 ATP-licencet igénylik a folyamatos fenyegetettség elleni védelemhez.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-227">Users migrated to Microsoft 365 E3 will each require an Office 365 ATP license for continued threat protection.</span></span> <span data-ttu-id="ba0bb-228">Ügyeljen arra, hogy további Office 365 ATP-licenceket vásároljon, hogy az Office 365-ös ATP-rendőrségi partnerei minden felhasználója licenccel rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-228">Be sure to purchase additional Office 365 ATP licenses so that all of the users in scope of your Office 365 ATP polices are licensed.</span></span> 
>

### <a name="device-management-with-intune"></a><span data-ttu-id="ba0bb-229">Eszközkezelés az Intune segítségével</span><span class="sxs-lookup"><span data-stu-id="ba0bb-229">Device management with Intune</span></span>

<span data-ttu-id="ba0bb-230">A áttelepítés előtt nem kell módosítania a jelenlegi Intune-konfigurációt, beleértve a regisztrált eszközöket, valamint az eszközök és az App beállításait is.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-230">You don't need to make any changes to your current Intune configuration before migrating, which includes enrolled devices and device and app settings.</span></span>

### <a name="windows-10"></a><span data-ttu-id="ba0bb-231">Windows 10</span><span class="sxs-lookup"><span data-stu-id="ba0bb-231">Windows 10</span></span>

<span data-ttu-id="ba0bb-232">A Microsoft 365 vállalati prémium verzió tartalmazza a Windows 10 Business verziót, amelyet a Windows Autopilot segítségével telepíthet.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-232">Microsoft 365 Business Premium includes Windows 10 Business, which you can install with Windows AutoPilot.</span></span> <span data-ttu-id="ba0bb-233">A Microsoft 365 E3-ra történő áttelepítéskor minden felhasználói licenc tartalmazza a Windows 10 nagyvállalati E3 verziót, amelyet a Windows Autopilot segítségével is telepíthet.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-233">When you migrate to Microsoft 365 E3, each user license includes Windows 10 Enterprise E3, which you can also install with Windows Autopilot.</span></span>

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a><span data-ttu-id="ba0bb-234">Microsoft 365-alkalmazások vállalati verzió</span><span class="sxs-lookup"><span data-stu-id="ba0bb-234">Microsoft 365 Apps for business</span></span>

<span data-ttu-id="ba0bb-235">A Microsoft 365-alapú Office-alkalmazások telepítése automatikusan megkezdődik a Microsoft 365-alkalmazások nagyvállalatoknak funkcióinak használatához.</span><span class="sxs-lookup"><span data-stu-id="ba0bb-235">Your Microsoft 365 Apps for business client installed on your devices will automatically begin to use the features of Microsoft 365 Apps for enterprise.</span></span> <span data-ttu-id="ba0bb-236">Az áttelepítés után mostantól használhatja a következőt:</span><span class="sxs-lookup"><span data-stu-id="ba0bb-236">After migration, you can now use:</span></span>

 - <span data-ttu-id="ba0bb-237">A mennyiségi aktiválás csoportházirenden keresztül</span><span class="sxs-lookup"><span data-stu-id="ba0bb-237">Volume activation through Group Policy</span></span>
 - <span data-ttu-id="ba0bb-238">App telemetriai</span><span class="sxs-lookup"><span data-stu-id="ba0bb-238">App telemetry</span></span>
 - <span data-ttu-id="ba0bb-239">Vezérlők frissítése</span><span class="sxs-lookup"><span data-stu-id="ba0bb-239">Update controls</span></span>
 - <span data-ttu-id="ba0bb-240">Számolótábla összehasonlítása és lekérdezése</span><span class="sxs-lookup"><span data-stu-id="ba0bb-240">Spreadsheet compare and inquire</span></span>
 - <span data-ttu-id="ba0bb-241">Üzleti intelligencia</span><span class="sxs-lookup"><span data-stu-id="ba0bb-241">Business intelligence</span></span>


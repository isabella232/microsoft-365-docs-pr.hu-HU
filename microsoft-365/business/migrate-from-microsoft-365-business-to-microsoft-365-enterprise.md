---
title: Áttelepítés a Microsoft 365 Vállalati verzióról a Microsoft 365 E3 szolgáltatásra
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
description: Megtudhatja, hogy miként helyezheti át vállalkozását a Microsoft 365 Business Premium szolgáltatásról a Microsoft 365 E3 szolgáltatásra.
ms.openlocfilehash: 6a795d96ccae7e054e7e52d4fd60a4e73b3c71dd
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/27/2020
ms.locfileid: "45081832"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a><span data-ttu-id="c20d7-103">Áttelepítés a Microsoft 365 Business Premium szolgáltatásról a Microsoft 365 E3 szolgáltatásra</span><span class="sxs-lookup"><span data-stu-id="c20d7-103">Migrate from Microsoft 365 Business Premium to Microsoft 365 E3</span></span>

<span data-ttu-id="c20d7-104">A Microsoft 365 Business Premium mindent tartalmaz, amire szüksége lehet a kisvállalkozásához, kombinálva a kategóriájában legjobb felhőalapú hatékonyságnövelő alkalmazásokat az egyszerű eszközkezeléssel és biztonsággal, amelyek lehetővé teszik az alkalmazottak számára, hogy a legjobb munkát végezzék.</span><span class="sxs-lookup"><span data-stu-id="c20d7-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security that enable your employees to do their best work.</span></span> <span data-ttu-id="c20d7-105">Bizonyos esetekben azonban előfordulhat, hogy át kell telepítenie a Microsoft 365 Business Premium előfizetését a Microsoft 365 E3 programba.</span><span class="sxs-lookup"><span data-stu-id="c20d7-105">In some cases, however, you may need to migrate your Microsoft 365 Business Premium subscription to Microsoft 365 E3.</span></span> 

<span data-ttu-id="c20d7-106">Például a vállalkozásod nőtt, és több mint 300 licencre van szüksége (egyébként gratulálok).</span><span class="sxs-lookup"><span data-stu-id="c20d7-106">For example, your business has grown and needs more than 300 licenses (congratulations, by the way).</span></span>

<span data-ttu-id="c20d7-107">Üzleti környezetének vállalati funkciókra is szüksége van, például nagyvállalati Microsoft 365-alkalmazásokra, Windows 10 Nagyvállalati E3-ra vagy vállalati ügyféllicencre.</span><span class="sxs-lookup"><span data-stu-id="c20d7-107">Or, your business needs enterprise features, such as Microsoft 365 Apps for enterprise, Windows 10 Enterprise E3, or Enterprise Client Access Licenses (CALs).</span></span>

<span data-ttu-id="c20d7-108">A frissítés egyszerű: a frissítést [a Felügyeleti központból indíthatja](../commerce/subscriptions/upgrade-to-different-plan.md)el.</span><span class="sxs-lookup"><span data-stu-id="c20d7-108">Upgrading is easy: you can start the upgrade [from the Admin center](../commerce/subscriptions/upgrade-to-different-plan.md).</span></span> <span data-ttu-id="c20d7-109">Az aktuális előfizetésben lévő összes adat és konfiguráció megmarad.</span><span class="sxs-lookup"><span data-stu-id="c20d7-109">All your data and configuration in your current subscription is maintained.</span></span> <span data-ttu-id="c20d7-110">Nincs mit tennie, hogy felkészüljenek a migráció, és semmi köze utána, kivéve, hogy kihasználják az új funkciókat.</span><span class="sxs-lookup"><span data-stu-id="c20d7-110">There's nothing for you to do to prepare for the migration and nothing to do afterward, except take advantage of the new features.</span></span>

>[!Note]
><span data-ttu-id="c20d7-111">Akár 300 férőhelyes Microsoft 365 Business Premium előfizetést is használhat, és több mint 300 férőhelyes Microsoft 365 E3-előfizetést is kaphat.</span><span class="sxs-lookup"><span data-stu-id="c20d7-111">You can also use a Microsoft 365 Business Premium subscription for up to 300 seats and get a Microsoft 365 E3 subscription for more than 300 seats.</span></span> <span data-ttu-id="c20d7-112">Az Office 365 ATP azonban nem része a Microsoft 365 E3 szolgáltatásnak.</span><span class="sxs-lookup"><span data-stu-id="c20d7-112">However, Office 365 ATP is not included with Microsoft 365 E3.</span></span> <span data-ttu-id="c20d7-113">A folyamatos veszélyforrások elleni védelem érdekében további Office 365 ATP-licenceket kell hozzáadnia, hogy az Office 365 ATP-rendszerében lévő összes felhasználó licenccel rendelkezhessen.</span><span class="sxs-lookup"><span data-stu-id="c20d7-113">For continued threat protection, you should add additional Office 365 ATP licenses so that all of the users in scope of your Office 365 ATP polices are licensed.</span></span>
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a><span data-ttu-id="c20d7-114">A Microsoft 365 Business Premium és a Microsoft 365 Enterprise közötti különbségek</span><span class="sxs-lookup"><span data-stu-id="c20d7-114">Differences between Microsoft 365 Business Premium and Microsoft 365 Enterprise</span></span>

<span data-ttu-id="c20d7-115">Ez a táblázat a Microsoft 365 Business Premium és a Microsoft 365 E3 közötti különbségeket mutatja be.</span><span class="sxs-lookup"><span data-stu-id="c20d7-115">This table shows the differences between Microsoft 365 Business Premium and Microsoft 365 E3.</span></span>

| <span data-ttu-id="c20d7-116">Funkció</span><span class="sxs-lookup"><span data-stu-id="c20d7-116">Feature</span></span>    | <span data-ttu-id="c20d7-117">Támogatás a Microsoft 365 Vállalati prémium verzióban</span><span class="sxs-lookup"><span data-stu-id="c20d7-117">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="c20d7-118">Támogatás a Microsoft 365 E3-ban</span><span class="sxs-lookup"><span data-stu-id="c20d7-118">Support in Microsoft 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="c20d7-119">**Helyszíni**</span><span class="sxs-lookup"><span data-stu-id="c20d7-119">**On-premises**</span></span>        | | | 
| <span data-ttu-id="c20d7-120">Windows 10</span><span class="sxs-lookup"><span data-stu-id="c20d7-120">Windows 10</span></span>    | <span data-ttu-id="c20d7-121">Windows 10 Üzleti Verzió</span><span class="sxs-lookup"><span data-stu-id="c20d7-121">Windows 10 Business</span></span>  |     <span data-ttu-id="c20d7-122">Windows 10 Nagyvállalati E3</span><span class="sxs-lookup"><span data-stu-id="c20d7-122">Windows 10 Enterprise E3</span></span>| 
| <span data-ttu-id="c20d7-123">Office-alkalmazások\*</span><span class="sxs-lookup"><span data-stu-id="c20d7-123">Office apps\*</span></span>    | [<span data-ttu-id="c20d7-124">Microsoft 365 alkalmazások üzleti célokra</span><span class="sxs-lookup"><span data-stu-id="c20d7-124">Microsoft 365 Apps for business</span></span>](#office-365-business)    | <span data-ttu-id="c20d7-125">Microsoft 365 nagyvállalati alkalmazások</span><span class="sxs-lookup"><span data-stu-id="c20d7-125">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="c20d7-126">**Felhőalapú hatékonyságnövelő alkalmazások**</span><span class="sxs-lookup"><span data-stu-id="c20d7-126">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="c20d7-127">Exchange Online és Outlook</span><span class="sxs-lookup"><span data-stu-id="c20d7-127">Exchange Online and Outlook</span></span>    | <span data-ttu-id="c20d7-128">50 GB tárhelykorlát postaládánként és korlátlan Exchange Online archiválás</span><span class="sxs-lookup"><span data-stu-id="c20d7-128">50 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span>    | <span data-ttu-id="c20d7-129">100 GB tárhelykorlát postafiókonként és korlátlan Exchange Online archiválás</span><span class="sxs-lookup"><span data-stu-id="c20d7-129">100 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span> | 
| <span data-ttu-id="c20d7-130">Csapat</span><span class="sxs-lookup"><span data-stu-id="c20d7-130">Teams</span></span>    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| <span data-ttu-id="c20d7-133">OneDrive Vállalati verzió</span><span class="sxs-lookup"><span data-stu-id="c20d7-133">OneDrive for Business</span></span>    | <span data-ttu-id="c20d7-134">Felhasználónként 1 TB tárhelykorlát</span><span class="sxs-lookup"><span data-stu-id="c20d7-134">1 TB storage limit per user</span></span>    | <span data-ttu-id="c20d7-135">Korlátlan</span><span class="sxs-lookup"><span data-stu-id="c20d7-135">Unlimited</span></span> | 
| <span data-ttu-id="c20d7-136">Yammer, SharePoint Online, Planner, Adatfolyam</span><span class="sxs-lookup"><span data-stu-id="c20d7-136">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| <span data-ttu-id="c20d7-139">Outlook ügyfélmenedzser, MileIQ</span><span class="sxs-lookup"><span data-stu-id="c20d7-139">Outlook Customer Manager, MileIQ</span></span>    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | | 
| <span data-ttu-id="c20d7-141">**Veszélyforrások elleni védelem**</span><span class="sxs-lookup"><span data-stu-id="c20d7-141">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="c20d7-142">A támadási felület csökkentésének képességei</span><span class="sxs-lookup"><span data-stu-id="c20d7-142">Attack surface reduction capabilities</span></span>    | [<span data-ttu-id="c20d7-143">A lista megtekintése</span><span class="sxs-lookup"><span data-stu-id="c20d7-143">See this list</span></span>](#threat-protection) | <span data-ttu-id="c20d7-144">A Microsoft Edge hardveralapú elkülönítésének vállalati kezelése</span><span class="sxs-lookup"><span data-stu-id="c20d7-144">Enterprise management of hardware-based isolation for Microsoft Edge</span></span> | 
| <span data-ttu-id="c20d7-145">Office 365 Komplex veszélyforrások elleni védelem (ATP) 1.</span><span class="sxs-lookup"><span data-stu-id="c20d7-145">Office 365 Advanced Threat Protection (ATP) Plan 1</span></span> | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | <span data-ttu-id="c20d7-147">Nem tartalmazza, de hozzáadható a</span><span class="sxs-lookup"><span data-stu-id="c20d7-147">Not included, but can be added on</span></span> | 
| <span data-ttu-id="c20d7-148">**Identitáskezelés**</span><span class="sxs-lookup"><span data-stu-id="c20d7-148">**Identity management**</span></span>        | | | 
| <span data-ttu-id="c20d7-149">Önkiszolgáló jelszó-visszaállítás hibrid Azure Active Directory (Azure AD) fiókokhoz, Azure többtényezős hitelesítéshez (MFA), feltételes hozzáféréshez, jelszó-visszaírás a helyszíni identitásokhoz</span><span class="sxs-lookup"><span data-stu-id="c20d7-149">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| <span data-ttu-id="c20d7-152">Cloud App Discovery, Azure AD Connect állapota</span><span class="sxs-lookup"><span data-stu-id="c20d7-152">Cloud App Discovery, Azure AD Connect Health</span></span>    |     | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| <span data-ttu-id="c20d7-154">Azure AD Office 365 alkalmazások egyszeri bejelentkezés (SSO): 10 alkalmazás felhasználónként (Gallery SaaS-alkalmazások, például a Salesforce)\*</span><span class="sxs-lookup"><span data-stu-id="c20d7-154">Azure AD Office 365 apps Single Sign-On (SSO): 10 apps per user (Gallery SaaS apps such as Salesforce)\*</span></span> | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| <span data-ttu-id="c20d7-157">Azure AD Premium 1 egyszeri szolgáltató: nincs korlátozás (helyszíni alkalmazások az Azure AD alkalmazásproxyn keresztül és nem galéria alkalmazások önkiszolgáló alkalmazásintegrációs sablonok használatával)</span><span class="sxs-lookup"><span data-stu-id="c20d7-157">Azure AD Premium 1 SSO: no limit (On-premises apps through Azure AD Application Proxy and non-gallery apps using Self-Service App Integration templates)</span></span>    |     | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| <span data-ttu-id="c20d7-159">**Eszköz- és alkalmazáskezelés**</span><span class="sxs-lookup"><span data-stu-id="c20d7-159">**Device and app management**</span></span>        | | | 
| <span data-ttu-id="c20d7-160">Microsoft Intune, Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="c20d7-160">Microsoft Intune, Windows Autopilot</span></span>|     ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
|<span data-ttu-id="c20d7-163">Virtuális asztali hozzáférés (VDA)</span><span class="sxs-lookup"><span data-stu-id="c20d7-163">Virtual Desktop Access (VDA)</span></span>    |  |     ![A Microsoft 365 E3 része](../media/check-mark.png) | 
|<span data-ttu-id="c20d7-165">Windows virtuális asztal (WVD)</span><span class="sxs-lookup"><span data-stu-id="c20d7-165">Windows Virtual Desktop (WVD)</span></span>    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png) |     ![A Microsoft 365 E3 része](../media/check-mark.png) | 
|<span data-ttu-id="c20d7-168">Megosztott számítógép aktiválása (SCA)</span><span class="sxs-lookup"><span data-stu-id="c20d7-168">Shared Computer Activation (SCA)</span></span>    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png) |     ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| <span data-ttu-id="c20d7-171">Microsoft asztali optimalizálási csomag</span><span class="sxs-lookup"><span data-stu-id="c20d7-171">Microsoft Desktop Optimization Package</span></span>    | |     ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| <span data-ttu-id="c20d7-173">**Információvédelem**</span><span class="sxs-lookup"><span data-stu-id="c20d7-173">**Information protection**</span></span>        | | | 
| <span data-ttu-id="c20d7-174">Az Office 365 adatvesztés-megelőzési terve, Azure-információvédelmi csomag 1</span><span class="sxs-lookup"><span data-stu-id="c20d7-174">Office 365 Data Loss Prevention, Azure Information Protection Plan 1</span></span>    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| <span data-ttu-id="c20d7-177">Ablakinformáció-védelem a DLP végponthoz</span><span class="sxs-lookup"><span data-stu-id="c20d7-177">Window Information Protection for endpoint DLP</span></span>    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| <span data-ttu-id="c20d7-180">**Ügyféllicenc (CAL-jogok)**</span><span class="sxs-lookup"><span data-stu-id="c20d7-180">**Client Access License (CAL rights)**</span></span>    | | |     
| <span data-ttu-id="c20d7-181">Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)</span><span class="sxs-lookup"><span data-stu-id="c20d7-181">Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)</span></span>| |         ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| <span data-ttu-id="c20d7-183">**Megfelelés**</span><span class="sxs-lookup"><span data-stu-id="c20d7-183">**Compliance**</span></span>        | | | 
| <span data-ttu-id="c20d7-184">Korlátlan e-mail archiválás</span><span class="sxs-lookup"><span data-stu-id="c20d7-184">Unlimited email archiving</span></span>    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| <span data-ttu-id="c20d7-187">Megfelelőségi pontszám/megfelelőségi vezető</span><span class="sxs-lookup"><span data-stu-id="c20d7-187">Compliance Score/Compliance Manager</span></span>    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| <span data-ttu-id="c20d7-190">elektronikus adatfeltárás</span><span class="sxs-lookup"><span data-stu-id="c20d7-190">eDiscovery</span></span>    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| <span data-ttu-id="c20d7-193">Helybeni tartás és peres eljárás miatti tartás</span><span class="sxs-lookup"><span data-stu-id="c20d7-193">In-place hold and litigation hold</span></span>    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| <span data-ttu-id="c20d7-196">Üzenetkezelési rekordok kezelése (MRM) adatmegőrzési címkék és adatmegőrzési házirendek</span><span class="sxs-lookup"><span data-stu-id="c20d7-196">Messaging Records Management (MRM) retention tags and retention policies</span></span>    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
||||

<span data-ttu-id="c20d7-199">\*A SaaS-alkalmazásokhoz hozzáféréssel rendelkező felhasználók akár 10 alkalmazáshoz is hozzáférhetnek az Sso-alkalmazásokhoz.</span><span class="sxs-lookup"><span data-stu-id="c20d7-199">\* Users who have been assigned access to SaaS apps can get SSO access to up to 10 apps.</span></span> <span data-ttu-id="c20d7-200">A rendszergazdák konfigurálhatják az egyszeri hozzáférést, és módosíthatják a felhasználói hozzáférést a különböző SaaS-alkalmazásokhoz, de az Egyszeri szolgáltatás hozzáférése felhasználónként csak 10 alkalmazáshoz engedélyezett egyszerre.</span><span class="sxs-lookup"><span data-stu-id="c20d7-200">Admins can configure SSO and change user access to different SaaS apps, but SSO access is only allowed for 10 apps per user at a time.</span></span> <span data-ttu-id="c20d7-201">Minden Office 365-alkalmazás egyetlen alkalmazásnak számít.</span><span class="sxs-lookup"><span data-stu-id="c20d7-201">All Office 365 apps are counted as a single app.</span></span>

## <a name="migration"></a><span data-ttu-id="c20d7-202">Áttelepítési</span><span class="sxs-lookup"><span data-stu-id="c20d7-202">Migration</span></span>

<span data-ttu-id="c20d7-203">Az áttelepítéshez a partnerével együttműködve helyezze át Microsoft 365 Business Premium előfizetését és licenceit egy megfelelő Microsoft 365 E3-előfizetésbe a licencekkel.</span><span class="sxs-lookup"><span data-stu-id="c20d7-203">To migrate, work with your partner to move your Microsoft 365 Business Premium subscription and licenses to a suitable Microsoft 365 E3 subscription with its licenses.</span></span>

<span data-ttu-id="c20d7-204">A következő szakaszok ismertetik, hogy milyen módosításokat kell végrehajtania, ha vannak ilyenek, és mit tehet az áttelepítés után.</span><span class="sxs-lookup"><span data-stu-id="c20d7-204">The following sections describe what changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="microsoft-365-subscription-configuration-and-data"></a><span data-ttu-id="c20d7-205">Microsoft 365 előfizetés konfigurációja és adatai</span><span class="sxs-lookup"><span data-stu-id="c20d7-205">Microsoft 365 subscription configuration and data</span></span>

<span data-ttu-id="c20d7-206">Az áttelepítés előtt nem kell módosítania az aktuális előfizetését vagy adatait, amely a következőket tartalmazza:</span><span class="sxs-lookup"><span data-stu-id="c20d7-206">You don't need to make any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="c20d7-207">Előfizetés-konfiguráció, például DNS-tartománynevek.</span><span class="sxs-lookup"><span data-stu-id="c20d7-207">Subscription configuration, such as DNS domain names.</span></span>
- <span data-ttu-id="c20d7-208">Felhasználói és csoportfiókok és hitelesítési beállítások, például többtényezős hitelesítés vagy feltételes hozzáférési házirendek.</span><span class="sxs-lookup"><span data-stu-id="c20d7-208">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="c20d7-209">A hatékonyságnövelő szolgáltatás konfigurációi és adataik, például a Teams, az Exchange Online-postaládák, a SharePoint Online-webhelyek, a OneDrive Vállalati verzió mappái és a OneNote-jegyzetfüzetek.</span><span class="sxs-lookup"><span data-stu-id="c20d7-209">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>

<span data-ttu-id="c20d7-210">A felhasználók mostantól korlátlan tárhelyet élvezhetnek az Exchange Online-postaládákban és a OneDrive Vállalati verzióban lévő mappákban.</span><span class="sxs-lookup"><span data-stu-id="c20d7-210">Your users can now enjoy unlimited storage in the Exchange Online mailboxes and OneDrive for Business folders.</span></span>

<span data-ttu-id="c20d7-211">A Cloud App Discovery, az Azure AD Connect Health és az SSO több mint 10 alkalmazáshoz használható.</span><span class="sxs-lookup"><span data-stu-id="c20d7-211">You can begin using Cloud App Discovery, Azure AD Connect Health, and SSO for more than 10 apps.</span></span>

>[!Note]
><span data-ttu-id="c20d7-212">A Microsoft 365 E3 rendszerre áttelepített felhasználók már nem használhatják az Outlook Customer Manager és a MileIQ alkalmazást.</span><span class="sxs-lookup"><span data-stu-id="c20d7-212">Users migrated to Microsoft 365 E3 can no longer use Outlook Customer Manager and MileIQ.</span></span>
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a><span data-ttu-id="c20d7-213">Veszélyforrások elleni védelem</span><span class="sxs-lookup"><span data-stu-id="c20d7-213">Threat protection</span></span>

<span data-ttu-id="c20d7-214">A Windows 10 Business a következő védelmet tartalmazza:</span><span class="sxs-lookup"><span data-stu-id="c20d7-214">Windows 10 Business includes these protections:</span></span>

- <span data-ttu-id="c20d7-215">Az operációs rendszer rendszerindítási folyamatának integritásérvényesítési rendszere</span><span class="sxs-lookup"><span data-stu-id="c20d7-215">Integrity enforcement of operating system boot up process</span></span>
- <span data-ttu-id="c20d7-216">Az érzékeny üzemi elemek integritásának érvényesítése</span><span class="sxs-lookup"><span data-stu-id="c20d7-216">Integrity enforcement of sensitive operating components</span></span>
- <span data-ttu-id="c20d7-217">Speciális biztonsági rés és nulladik napi biztonsági rés-kockázatcsökkentés</span><span class="sxs-lookup"><span data-stu-id="c20d7-217">Advanced vulnerability and zero-day exploit mitigations</span></span>
- <span data-ttu-id="c20d7-218">Hírnévalapú hálózatvédelem a Microsoft Edge, az Internet Explorer és a Chrome számára</span><span class="sxs-lookup"><span data-stu-id="c20d7-218">Reputation-based network protection for Microsoft Edge, Internet Explorer, and Chrome</span></span>
- <span data-ttu-id="c20d7-219">Gazdagépalapú tűzfal</span><span class="sxs-lookup"><span data-stu-id="c20d7-219">Host-based firewall</span></span>
- <span data-ttu-id="c20d7-220">Zsarolóprogramok enyhítése</span><span class="sxs-lookup"><span data-stu-id="c20d7-220">Ransomware mitigations</span></span>
- <span data-ttu-id="c20d7-221">Hardveralapú elkülönítés a Microsoft Edge számára</span><span class="sxs-lookup"><span data-stu-id="c20d7-221">Hardware-based isolation for Microsoft Edge</span></span>
- <span data-ttu-id="c20d7-222">Az alkalmazásvezérlés az intelligens biztonsági grafikonon hajtva</span><span class="sxs-lookup"><span data-stu-id="c20d7-222">Application control powered by the Intelligent Security Graph</span></span>
- <span data-ttu-id="c20d7-223">Eszközvezérlés (USB)</span><span class="sxs-lookup"><span data-stu-id="c20d7-223">Device control (USB)</span></span>
- <span data-ttu-id="c20d7-224">Hálózatvédelem a webalapú fenyegetések számára</span><span class="sxs-lookup"><span data-stu-id="c20d7-224">Network protection for web-based threats</span></span>
- <span data-ttu-id="c20d7-225">A gazdabehatolás-megelőzési szabályok</span><span class="sxs-lookup"><span data-stu-id="c20d7-225">Host intrusion prevention rules</span></span>

<span data-ttu-id="c20d7-226">A Windows 10 Enterprise E3 a Microsoft Edge hardveralapú elkülönítésének vállalati kezelését is tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="c20d7-226">Windows 10 Enterprise E3 also includes enterprise management of hardware-based isolation for Microsoft Edge.</span></span>

>[!Note]
><span data-ttu-id="c20d7-227">A Microsoft 365 E3 rendszerre áttelepített felhasználóknak office 365 ATP-licencre lesz szükségük a folyamatos veszélyforrások elleni védelemhez.</span><span class="sxs-lookup"><span data-stu-id="c20d7-227">Users migrated to Microsoft 365 E3 will each require an Office 365 ATP license for continued threat protection.</span></span> <span data-ttu-id="c20d7-228">Mindenképpen vásároljon további Office 365 ATP-licenceket, hogy az Office 365 ATP-rendszerében lévő összes felhasználó licenccel rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="c20d7-228">Be sure to purchase additional Office 365 ATP licenses so that all of the users in scope of your Office 365 ATP polices are licensed.</span></span> 
>

### <a name="device-management-with-intune"></a><span data-ttu-id="c20d7-229">Eszközkezelés az Intune-nal</span><span class="sxs-lookup"><span data-stu-id="c20d7-229">Device management with Intune</span></span>

<span data-ttu-id="c20d7-230">Az áttelepítés előtt nem kell módosítania az aktuális Intune-konfigurációt, amely tartalmazza a regisztrált eszközöket, valamint az eszköz- és alkalmazásbeállításokat.</span><span class="sxs-lookup"><span data-stu-id="c20d7-230">You don't need to make any changes to your current Intune configuration before migrating, which includes enrolled devices and device and app settings.</span></span>

### <a name="windows-10"></a><span data-ttu-id="c20d7-231">Windows 10</span><span class="sxs-lookup"><span data-stu-id="c20d7-231">Windows 10</span></span>

<span data-ttu-id="c20d7-232">A Microsoft 365 Business Premium tartalmazza a Windows 10 Business rendszert, amelyet a Windows AutoPilot programmal telepíthet.</span><span class="sxs-lookup"><span data-stu-id="c20d7-232">Microsoft 365 Business Premium includes Windows 10 Business, which you can install with Windows AutoPilot.</span></span> <span data-ttu-id="c20d7-233">Amikor áttelepíti a Microsoft 365 E3 rendszert, minden felhasználói licenc tartalmazza a Windows 10 Enterprise E3 rendszert, amelyet a Windows Autopilot segítségével is telepíthet.</span><span class="sxs-lookup"><span data-stu-id="c20d7-233">When you migrate to Microsoft 365 E3, each user license includes Windows 10 Enterprise E3, which you can also install with Windows Autopilot.</span></span>

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a><span data-ttu-id="c20d7-234">Microsoft 365 alkalmazások üzleti célokra</span><span class="sxs-lookup"><span data-stu-id="c20d7-234">Microsoft 365 Apps for business</span></span>

<span data-ttu-id="c20d7-235">Az eszközökre telepített Microsoft 365 vállalati alkalmazások automatikusan elkezdik használni a Microsoft 365 vállalati verzióinak funkcióit.</span><span class="sxs-lookup"><span data-stu-id="c20d7-235">Your Microsoft 365 Apps for business client installed on your devices will automatically begin to use the features of Microsoft 365 Apps for enterprise.</span></span> <span data-ttu-id="c20d7-236">Az áttelepítés után a következőket használhatja:</span><span class="sxs-lookup"><span data-stu-id="c20d7-236">After migration, you can now use:</span></span>

 - <span data-ttu-id="c20d7-237">Mennyiségi aktiválás csoportházirenddel</span><span class="sxs-lookup"><span data-stu-id="c20d7-237">Volume activation through Group Policy</span></span>
 - <span data-ttu-id="c20d7-238">Alkalmazástelemetria</span><span class="sxs-lookup"><span data-stu-id="c20d7-238">App telemetry</span></span>
 - <span data-ttu-id="c20d7-239">Vezérlők frissítése</span><span class="sxs-lookup"><span data-stu-id="c20d7-239">Update controls</span></span>
 - <span data-ttu-id="c20d7-240">Számolótábla összehasonlítása és lekérdezése</span><span class="sxs-lookup"><span data-stu-id="c20d7-240">Spreadsheet compare and inquire</span></span>
 - <span data-ttu-id="c20d7-241">Üzleti intelligencia</span><span class="sxs-lookup"><span data-stu-id="c20d7-241">Business intelligence</span></span>


---
title: Áttelepítés az Microsoft 365 Vállalati verzióból Microsoft 365 E3
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
description: Megtudhatja, hogy miként mozgathat cége új Microsoft 365 Vállalati prémium verzió-Microsoft 365 E3.
ms.openlocfilehash: 6502d79dbb283db37b00e4fccf89b15ab4291ce5
ms.sourcegitcommit: 48195345b21b409b175d68acdc25d9f2fc4fc5f1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53227619"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a><span data-ttu-id="1e513-103">Áttelepítés Microsoft 365 Vállalati prémium verzió Microsoft 365 E3</span><span class="sxs-lookup"><span data-stu-id="1e513-103">Migrate from Microsoft 365 Business Premium to Microsoft 365 E3</span></span>

<span data-ttu-id="1e513-104">Microsoft 365 Vállalati prémium verzió rendelkezik mindennel, ami a kisvállalata számára szükséges, a legjobb, felhőalapú hatékonyságnövelő alkalmazásokat egyszerű eszközkezelési és biztonsági megoldásokkal kombinálva, ami lehetővé teszi, hogy alkalmazottai a lehető legjobb munkát el tudjaják látni.</span><span class="sxs-lookup"><span data-stu-id="1e513-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security that enable your employees to do their best work.</span></span> <span data-ttu-id="1e513-105">Bizonyos esetekben azonban előfordulhat, hogy át kell Microsoft 365 Vállalati prémium verzió a Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="1e513-105">In some cases, however, you may need to migrate your Microsoft 365 Business Premium subscription to Microsoft 365 E3.</span></span>

<span data-ttu-id="1e513-106">A vállalkozása például több mint 300 licencre van szüksége (egyébként gratulálunk).</span><span class="sxs-lookup"><span data-stu-id="1e513-106">For example, your business has grown and needs more than 300 licenses (congratulations, by the way).</span></span>

<span data-ttu-id="1e513-107">Az is lehet, hogy cégének nagyvállalati szolgáltatásokra van szüksége, például Nagyvállalati Microsoft 365-alkalmazások, Windows 10 Enterprise E3 vagy Nagyvállalati ügyfélelérési licencek (CAL-ek).</span><span class="sxs-lookup"><span data-stu-id="1e513-107">Or, your business needs enterprise features, such as Microsoft 365 Apps for enterprise, Windows 10 Enterprise E3, or Enterprise Client Access Licenses (CALs).</span></span>

<span data-ttu-id="1e513-108">A frissítés egyszerű: a frissítést a [Felügyeleti központból elindíthatja.](../commerce/subscriptions/upgrade-to-different-plan.md)</span><span class="sxs-lookup"><span data-stu-id="1e513-108">Upgrading is easy: you can start the upgrade [from the Admin center](../commerce/subscriptions/upgrade-to-different-plan.md).</span></span> <span data-ttu-id="1e513-109">Jelenlegi előfizetésében minden adata és konfigurációja megmarad.</span><span class="sxs-lookup"><span data-stu-id="1e513-109">All your data and configuration in your current subscription is maintained.</span></span> <span data-ttu-id="1e513-110">Semmit sem kell tennie az áttelepítésre való felkészüléshez, és később semmit sem kell tennie, az új funkciók előnyeinek kihasználásán kívül.</span><span class="sxs-lookup"><span data-stu-id="1e513-110">There's nothing for you to do to prepare for the migration and nothing to do afterward, except take advantage of the new features.</span></span>

> [!NOTE]
> <span data-ttu-id="1e513-111">Akár 300 Microsoft 365 Vállalati prémium verzió is használhat előfizetést, és több mint 300 Microsoft 365 E3 előfizetést is kaphat.</span><span class="sxs-lookup"><span data-stu-id="1e513-111">You can also use a Microsoft 365 Business Premium subscription for up to 300 seats and get a Microsoft 365 E3 subscription for more than 300 seats.</span></span> <span data-ttu-id="1e513-112">A Microsoft Defender Office 365 azonban nem része a Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="1e513-112">However, Microsoft Defender for Office 365 is not included with Microsoft 365 E3.</span></span> <span data-ttu-id="1e513-113">A további veszélyforrások elleni védelem érdekében további Defendert kell hozzáadni a Office 365-licencekhez, hogy az Office 365 Defenderrel hatókörben rendelkező összes felhasználónak legyen licence.</span><span class="sxs-lookup"><span data-stu-id="1e513-113">For continued threat protection, you should add additional Defender for Office 365 licenses so that all of the users in scope of your Defender for Office 365 polices are licensed.</span></span>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a><span data-ttu-id="1e513-114">Különbségek a Microsoft 365 Vállalati prémium verzió és a Microsoft 365 Nagyvállalati verzió</span><span class="sxs-lookup"><span data-stu-id="1e513-114">Differences between Microsoft 365 Business Premium and Microsoft 365 Enterprise</span></span>

<span data-ttu-id="1e513-115">Az alábbi táblázatban a két táblázatban Microsoft 365 Vállalati prémium verzió és a Microsoft 365 E3.</span><span class="sxs-lookup"><span data-stu-id="1e513-115">This table shows the differences between Microsoft 365 Business Premium and Microsoft 365 E3.</span></span>

| <span data-ttu-id="1e513-116">Funkció</span><span class="sxs-lookup"><span data-stu-id="1e513-116">Feature</span></span>    | <span data-ttu-id="1e513-117">Támogatás a Microsoft 365 Vállalati prémium verzió</span><span class="sxs-lookup"><span data-stu-id="1e513-117">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="1e513-118">Támogatás a Microsoft 365 E3</span><span class="sxs-lookup"><span data-stu-id="1e513-118">Support in Microsoft 365 E3</span></span> |
|:-------|:-----|:-----|
| <span data-ttu-id="1e513-119">**Helyszíni**</span><span class="sxs-lookup"><span data-stu-id="1e513-119">**On-premises**</span></span>        | | |
| <span data-ttu-id="1e513-120">Windows 10 rendszer esetén</span><span class="sxs-lookup"><span data-stu-id="1e513-120">Windows 10</span></span>    | <span data-ttu-id="1e513-121">Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="1e513-121">Windows 10 Business</span></span>  |     <span data-ttu-id="1e513-122">Windows 10 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="1e513-122">Windows 10 Enterprise E3</span></span>|
| <span data-ttu-id="1e513-123">Office alkalmazások\*</span><span class="sxs-lookup"><span data-stu-id="1e513-123">Office apps\*</span></span>    | [<span data-ttu-id="1e513-124">Üzleti Microsoft 365-alkalmazások</span><span class="sxs-lookup"><span data-stu-id="1e513-124">Microsoft 365 Apps for business</span></span>](#office-365-business)    | <span data-ttu-id="1e513-125">Microsoft 365 Vállalati alkalmazások</span><span class="sxs-lookup"><span data-stu-id="1e513-125">Microsoft 365 Apps for enterprise</span></span> |
| <span data-ttu-id="1e513-126">**Felhőbeli hatékonyságnövelő alkalmazások**</span><span class="sxs-lookup"><span data-stu-id="1e513-126">**Cloud productivity apps**</span></span>        | | |
| <span data-ttu-id="1e513-127">Exchange Online és Outlook</span><span class="sxs-lookup"><span data-stu-id="1e513-127">Exchange Online and Outlook</span></span>    | <span data-ttu-id="1e513-128">Postaládánként 50 GB tárterületkorlát és korlátlan Exchange Online archiválás</span><span class="sxs-lookup"><span data-stu-id="1e513-128">50 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span>    | <span data-ttu-id="1e513-129">Postaládánként 100 GB tárterületkorlát és korlátlan Exchange Online archiválás</span><span class="sxs-lookup"><span data-stu-id="1e513-129">100 GB storage limit per mailbox and unlimited Exchange Online archiving</span></span> |
| <span data-ttu-id="1e513-130">Teams</span><span class="sxs-lookup"><span data-stu-id="1e513-130">Teams</span></span>    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![A Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="1e513-133">OneDrive Vállalati verzió</span><span class="sxs-lookup"><span data-stu-id="1e513-133">OneDrive for Business</span></span>    | <span data-ttu-id="1e513-134">Felhasználónként 1 TB tárterületkorlát</span><span class="sxs-lookup"><span data-stu-id="1e513-134">1 TB storage limit per user</span></span>    | <span data-ttu-id="1e513-135">Korlátlan</span><span class="sxs-lookup"><span data-stu-id="1e513-135">Unlimited</span></span> |
| <span data-ttu-id="1e513-136">Yammer, SharePoint, Planner, Stream</span><span class="sxs-lookup"><span data-stu-id="1e513-136">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![A Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="1e513-139">**Veszélyforrások elleni védelem**</span><span class="sxs-lookup"><span data-stu-id="1e513-139">**Threat Protection**</span></span>        | | |
| <span data-ttu-id="1e513-140">Támadásifelület-csökkentés lehetőségei</span><span class="sxs-lookup"><span data-stu-id="1e513-140">Attack surface reduction capabilities</span></span>    | [<span data-ttu-id="1e513-141">A lista</span><span class="sxs-lookup"><span data-stu-id="1e513-141">See this list</span></span>](#threat-protection) | <span data-ttu-id="1e513-142">A hardveralapú elkülönítés nagyvállalati kezelése Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="1e513-142">Enterprise management of hardware-based isolation for Microsoft Edge</span></span> |
| <span data-ttu-id="1e513-143">Defender a Office 365 1. csomaghoz</span><span class="sxs-lookup"><span data-stu-id="1e513-143">Defender for Office 365 Plan 1</span></span> | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | <span data-ttu-id="1e513-145">Nem tartalmazza, de a következőn használhatja:</span><span class="sxs-lookup"><span data-stu-id="1e513-145">Not included, but can be added on</span></span> |
| <span data-ttu-id="1e513-146">**Identitáskezelés**</span><span class="sxs-lookup"><span data-stu-id="1e513-146">**Identity management**</span></span>        | | |
| <span data-ttu-id="1e513-147">Önkiszolgáló jelszó-visszaállítás hibrid Azure Active Directory -fiókokhoz (Azure AD-fiókokhoz), Azure AD többtényezős hitelesítés (MFA), feltételes hozzáférés, jelszóvisszaírás a helyszíni identitásokhoz</span><span class="sxs-lookup"><span data-stu-id="1e513-147">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure AD multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![A Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="1e513-150">Cloud App Discovery, Azure AD Csatlakozás Health</span><span class="sxs-lookup"><span data-stu-id="1e513-150">Cloud App Discovery, Azure AD Connect Health</span></span>    |     | ![A Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="1e513-152">Azure AD Office 365 -Sign-On (SSO): Felhasználónként 10 app (Gallery SaaS-appok, például Salesforce)\*</span><span class="sxs-lookup"><span data-stu-id="1e513-152">Azure AD Office 365 apps Single Sign-On (SSO): 10 apps per user (Gallery SaaS apps such as Salesforce)\*</span></span> | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![A Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="1e513-155">prémium szintű Azure AD 1 SSO: nincs korlátozás (helyszíni appok az Azure AD-alkalmazásproxyn keresztül és a nem galériaalkalmazások az Self-Service-integrációs sablonokkal)</span><span class="sxs-lookup"><span data-stu-id="1e513-155">Azure AD Premium 1 SSO: no limit (On-premises apps through Azure AD Application Proxy and non-gallery apps using Self-Service App Integration templates)</span></span>    |     | ![A Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="1e513-157">**Eszköz- és alkalmazáskezelés**</span><span class="sxs-lookup"><span data-stu-id="1e513-157">**Device and app management**</span></span>        | | |
| <span data-ttu-id="1e513-158">Microsoft Intune, Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="1e513-158">Microsoft Intune, Windows Autopilot</span></span>|     ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![A Microsoft 365 E3](../media/check-mark.png) |
|<span data-ttu-id="1e513-161">Virtual Desktop Access (VDA)</span><span class="sxs-lookup"><span data-stu-id="1e513-161">Virtual Desktop Access (VDA)</span></span>    |  |     ![A Microsoft 365 E3](../media/check-mark.png) |
|<span data-ttu-id="1e513-163">Windows Virtual Desktop (WVD)</span><span class="sxs-lookup"><span data-stu-id="1e513-163">Windows Virtual Desktop (WVD)</span></span>    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png) |     ![A Microsoft 365 E3](../media/check-mark.png) |
|<span data-ttu-id="1e513-166">Megosztott számítógép aktiválása (SCA)</span><span class="sxs-lookup"><span data-stu-id="1e513-166">Shared Computer Activation (SCA)</span></span>    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png) |     ![A Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="1e513-169">A Microsoft asztali optimalizálási csomagja</span><span class="sxs-lookup"><span data-stu-id="1e513-169">Microsoft Desktop Optimization Package</span></span>    | |     ![A Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="1e513-171">**Információvédelem**</span><span class="sxs-lookup"><span data-stu-id="1e513-171">**Information protection**</span></span>        | | |
| <span data-ttu-id="1e513-172">Office 365 Adatveszteség-megelőzés, Azure Information Protection 1. csomag</span><span class="sxs-lookup"><span data-stu-id="1e513-172">Office 365 Data Loss Prevention, Azure Information Protection Plan 1</span></span>    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![A Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="1e513-175">Window Information Protection for endpoint DLP</span><span class="sxs-lookup"><span data-stu-id="1e513-175">Window Information Protection for endpoint DLP</span></span>    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![A Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="1e513-178">**Ügyfélelérési licenc (CAL-jogok)**</span><span class="sxs-lookup"><span data-stu-id="1e513-178">**Client Access License (CAL rights)**</span></span>    | | |
| <span data-ttu-id="1e513-179">Nagyvállalati CAL csomag (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)</span><span class="sxs-lookup"><span data-stu-id="1e513-179">Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)</span></span>| |         ![A Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="1e513-181">**Megfelelőség**</span><span class="sxs-lookup"><span data-stu-id="1e513-181">**Compliance**</span></span>        | | |
| <span data-ttu-id="1e513-182">Korlátlan e-mail archiválás</span><span class="sxs-lookup"><span data-stu-id="1e513-182">Unlimited email archiving</span></span>    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![A Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="1e513-185">Megfelelőségkezelő</span><span class="sxs-lookup"><span data-stu-id="1e513-185">Compliance Manager</span></span>    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![A Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="1e513-188">Elektronikus észlelés</span><span class="sxs-lookup"><span data-stu-id="1e513-188">eDiscovery</span></span>    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![A Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="1e513-191">A helytől való hely- és jogi tartás</span><span class="sxs-lookup"><span data-stu-id="1e513-191">In-place hold and litigation hold</span></span>    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![A Microsoft 365 E3](../media/check-mark.png) |
| <span data-ttu-id="1e513-194">Üzenetrekord-kezelési (MRM) adatmegőrzési címkék és adatmegőrzési házirendek</span><span class="sxs-lookup"><span data-stu-id="1e513-194">Messaging Records Management (MRM) retention tags and retention policies</span></span>    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![A Microsoft 365 E3](../media/check-mark.png) |
||||

<span data-ttu-id="1e513-197">\* A SaaS-alkalmazásokhoz hozzáféréssel társított felhasználók legfeljebb 10 apphoz kaphatnak SSO-hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="1e513-197">\* Users who have been assigned access to SaaS apps can get SSO access to up to 10 apps.</span></span> <span data-ttu-id="1e513-198">A rendszergazdák konfigurálhatnak SSO-t, és módosíthatják a felhasználók hozzáférését a különböző SaaS-alkalmazásokhoz, az SSO-hozzáférés azonban felhasználónként csak 10 app számára engedélyezett.</span><span class="sxs-lookup"><span data-stu-id="1e513-198">Admins can configure SSO and change user access to different SaaS apps, but SSO access is only allowed for 10 apps per user at a time.</span></span> <span data-ttu-id="1e513-199">Minden Office 365 alkalmazás egyetlen alkalmazásnak számít.</span><span class="sxs-lookup"><span data-stu-id="1e513-199">All Office 365 apps are counted as a single app.</span></span>

## <a name="migration"></a><span data-ttu-id="1e513-200">Áttelepítés</span><span class="sxs-lookup"><span data-stu-id="1e513-200">Migration</span></span>

<span data-ttu-id="1e513-201">Az áttelepítéshez a partnerével együtt helyezze át Microsoft 365 Vállalati prémium verzió előfizetését és licenceit egy megfelelő előfizetésbe Microsoft 365 E3 licencekkel együtt.</span><span class="sxs-lookup"><span data-stu-id="1e513-201">To migrate, work with your partner to move your Microsoft 365 Business Premium subscription and licenses to a suitable Microsoft 365 E3 subscription with its licenses.</span></span>

<span data-ttu-id="1e513-202">Az alábbi szakaszokban ismertetheti, hogy milyen módosításokat kell, ha van, és hogy mit lehet tenni az áttelepítés után.</span><span class="sxs-lookup"><span data-stu-id="1e513-202">The following sections describe what changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="microsoft-365-subscription-configuration-and-data"></a><span data-ttu-id="1e513-203">Microsoft 365-előfizetés konfigurációjának és adatainak beállítása</span><span class="sxs-lookup"><span data-stu-id="1e513-203">Microsoft 365 subscription configuration and data</span></span>

<span data-ttu-id="1e513-204">Az áttelepítés előtt semmit sem kell változtatnia az aktuális előfizetésen vagy adatokon, beleértve az alábbi adatokat:</span><span class="sxs-lookup"><span data-stu-id="1e513-204">You don't need to make any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="1e513-205">Előfizetés-konfiguráció, például DNS-tartománynevek.</span><span class="sxs-lookup"><span data-stu-id="1e513-205">Subscription configuration, such as DNS domain names.</span></span>
- <span data-ttu-id="1e513-206">Felhasználói és csoportfiókok, valamint hitelesítési beállítások, például többtényezős hitelesítés vagy feltételes hozzáférési házirendek.</span><span class="sxs-lookup"><span data-stu-id="1e513-206">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="1e513-207">Hatékonyságnövelő szolgáltatáskonfigurációk és adataik , például Teams, Exchange Online-postaládák, SharePoint Online webhelyek, OneDrive Vállalati verzió mappák és OneNote jegyzetfüzetek.</span><span class="sxs-lookup"><span data-stu-id="1e513-207">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>

<span data-ttu-id="1e513-208">A felhasználók mostantól korlátlan tárterületet élvezhetnek a Exchange Online és a OneDrive Vállalati verzió mappáiban.</span><span class="sxs-lookup"><span data-stu-id="1e513-208">Your users can now enjoy unlimited storage in the Exchange Online mailboxes and OneDrive for Business folders.</span></span>

<span data-ttu-id="1e513-209">A Cloud App Discovery, az Azure AD Csatlakozás Health és az SSO több mint 10 appot is használhat.</span><span class="sxs-lookup"><span data-stu-id="1e513-209">You can begin using Cloud App Discovery, Azure AD Connect Health, and SSO for more than 10 apps.</span></span>

<a name="threat-protection"></a>
### <a name="threat-protection"></a><span data-ttu-id="1e513-210">Veszélyforrások elleni védelem</span><span class="sxs-lookup"><span data-stu-id="1e513-210">Threat protection</span></span>

<span data-ttu-id="1e513-211">Windows 10 Business az alábbi védelemeket tartalmazza:</span><span class="sxs-lookup"><span data-stu-id="1e513-211">Windows 10 Business includes these protections:</span></span>

- <span data-ttu-id="1e513-212">Az operációs rendszerindítási folyamat integritási kényszerítési eljárása</span><span class="sxs-lookup"><span data-stu-id="1e513-212">Integrity enforcement of operating system boot up process</span></span>
- <span data-ttu-id="1e513-213">Bizalmas működési összetevők integritási kényszerítése</span><span class="sxs-lookup"><span data-stu-id="1e513-213">Integrity enforcement of sensitive operating components</span></span>
- <span data-ttu-id="1e513-214">Speciális biztonsági rés és a biztonsági rés kiaknázása elleni nulla napos megoldások</span><span class="sxs-lookup"><span data-stu-id="1e513-214">Advanced vulnerability and zero-day exploit mitigations</span></span>
- <span data-ttu-id="1e513-215">A Microsoft Edge, az Internet Explorer és a Chrome jó hírnevén alapuló hálózatvédelem</span><span class="sxs-lookup"><span data-stu-id="1e513-215">Reputation-based network protection for Microsoft Edge, Internet Explorer, and Chrome</span></span>
- <span data-ttu-id="1e513-216">Állomásalapú tűzfal</span><span class="sxs-lookup"><span data-stu-id="1e513-216">Host-based firewall</span></span>
- <span data-ttu-id="1e513-217">Zsarolóvírusok elleni megoldások</span><span class="sxs-lookup"><span data-stu-id="1e513-217">Ransomware mitigations</span></span>
- <span data-ttu-id="1e513-218">Hardveralapú elkülönítés a Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="1e513-218">Hardware-based isolation for Microsoft Edge</span></span>
- <span data-ttu-id="1e513-219">Alkalmazásvezérlő az intelligens biztonsági Graph</span><span class="sxs-lookup"><span data-stu-id="1e513-219">Application control powered by the Intelligent Security Graph</span></span>
- <span data-ttu-id="1e513-220">Eszközvezérlő (USB)</span><span class="sxs-lookup"><span data-stu-id="1e513-220">Device control (USB)</span></span>
- <span data-ttu-id="1e513-221">Hálózatvédelem a webes veszélyforrások számára</span><span class="sxs-lookup"><span data-stu-id="1e513-221">Network protection for web-based threats</span></span>
- <span data-ttu-id="1e513-222">Host intrusion prevention rules</span><span class="sxs-lookup"><span data-stu-id="1e513-222">Host intrusion prevention rules</span></span>

<span data-ttu-id="1e513-223">Windows 10 Enterprise Az E3 csomag magában foglalja a hardveralapú elkülönítés nagyvállalati kezelését is Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="1e513-223">Windows 10 Enterprise E3 also includes enterprise management of hardware-based isolation for Microsoft Edge.</span></span>

> [!NOTE]
> <span data-ttu-id="1e513-224">Az új rendszerbe áttelepített Microsoft 365 E3 a további veszélyforrások elleni védelem érdekében Office 365 Microsoft Defender szükséges.</span><span class="sxs-lookup"><span data-stu-id="1e513-224">Users migrated to Microsoft 365 E3 will each require a Microsoft Defender for Office 365 license for continued threat protection.</span></span> <span data-ttu-id="1e513-225">Ne mindenképpen vásároljon további Defender Office 365, hogy a rendszer a saját defendere által Office 365 összes felhasználónak licencet vásároljon.</span><span class="sxs-lookup"><span data-stu-id="1e513-225">Be sure to purchase additional Defender for Office 365 licenses so that all of the users in scope of your Defender for Office 365 polices are licensed.</span></span>

### <a name="device-management-with-intune"></a><span data-ttu-id="1e513-226">Eszközkezelés az Intune-nal</span><span class="sxs-lookup"><span data-stu-id="1e513-226">Device management with Intune</span></span>

<span data-ttu-id="1e513-227">Az áttelepítés előtt nem kell módosítania az aktuális Intune-konfigurációt, beleértve a regisztrált eszközöket, eszköz- és alkalmazásbeállításokat.</span><span class="sxs-lookup"><span data-stu-id="1e513-227">You don't need to make any changes to your current Intune configuration before migrating, which includes enrolled devices and device and app settings.</span></span>

### <a name="windows-10"></a><span data-ttu-id="1e513-228">Windows 10 rendszer esetén</span><span class="sxs-lookup"><span data-stu-id="1e513-228">Windows 10</span></span>

<span data-ttu-id="1e513-229">Microsoft 365 Vállalati prémium verzió autopilottal Windows 10 Business, amelyek az AutoPilottal Windows telepíthetők.</span><span class="sxs-lookup"><span data-stu-id="1e513-229">Microsoft 365 Business Premium includes Windows 10 Business, which you can install with Windows AutoPilot.</span></span> <span data-ttu-id="1e513-230">Az áttelepítési Microsoft 365 E3 minden felhasználói licenc tartalmazza az Windows 10 Enterprise E3-t, amelyet az Autopilottal is Windows telepíthet.</span><span class="sxs-lookup"><span data-stu-id="1e513-230">When you migrate to Microsoft 365 E3, each user license includes Windows 10 Enterprise E3, which you can also install with Windows Autopilot.</span></span>

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a><span data-ttu-id="1e513-231">Üzleti Microsoft 365-alkalmazások</span><span class="sxs-lookup"><span data-stu-id="1e513-231">Microsoft 365 Apps for business</span></span>

<span data-ttu-id="1e513-232">Az Üzleti Microsoft 365-alkalmazások telepített ügyfélprogram automatikusan elkezdi használni a Nagyvállalati Microsoft 365-alkalmazások.</span><span class="sxs-lookup"><span data-stu-id="1e513-232">Your Microsoft 365 Apps for business client installed on your devices will automatically begin to use the features of Microsoft 365 Apps for enterprise.</span></span> <span data-ttu-id="1e513-233">Az áttelepítés után a következőt használhatja:</span><span class="sxs-lookup"><span data-stu-id="1e513-233">After migration, you can now use:</span></span>

- <span data-ttu-id="1e513-234">Csoportházirend-támogatás</span><span class="sxs-lookup"><span data-stu-id="1e513-234">Group Policy support</span></span>
- <span data-ttu-id="1e513-235">Spreadsheet compare and inquire</span><span class="sxs-lookup"><span data-stu-id="1e513-235">Spreadsheet compare and inquire</span></span>
- <span data-ttu-id="1e513-236">Üzleti intelligencia</span><span class="sxs-lookup"><span data-stu-id="1e513-236">Business intelligence</span></span>

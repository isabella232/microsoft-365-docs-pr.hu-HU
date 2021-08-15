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
ms.openlocfilehash: d3030518f7f4467c7b2e16897dc7b100764d9d5a36c50169b58f1adcd7bef209
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53837653"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Áttelepítés Microsoft 365 Vállalati prémium verzió Microsoft 365 E3

Microsoft 365 Vállalati prémium verzió rendelkezik mindennel, ami a kisvállalata számára szükséges, a legjobb, felhőalapú hatékonyságnövelő alkalmazásokat egyszerű eszközkezelési és biztonsági megoldásokkal kombinálva, ami lehetővé teszi, hogy alkalmazottai a lehető legjobb munkát el tudjaják látni. Bizonyos esetekben azonban előfordulhat, hogy át kell Microsoft 365 Vállalati prémium verzió a Microsoft 365 E3.

A vállalkozása például több mint 300 licencre van szüksége (egyébként gratulálunk).

Az is lehet, hogy cégének nagyvállalati szolgáltatásokra van szüksége, például Nagyvállalati Microsoft 365-alkalmazások, Windows 10 Enterprise E3 vagy Nagyvállalati ügyfélelérési licencek (CAL-ek).

A frissítés egyszerű: a frissítést a [Felügyeleti központból elindíthatja.](../commerce/subscriptions/upgrade-to-different-plan.md) Jelenlegi előfizetésében minden adata és konfigurációja megmarad. Semmit sem kell tennie az áttelepítésre való felkészüléshez, és később semmit sem kell tennie, az új funkciók előnyeinek kihasználásán kívül.

> [!NOTE]
> Akár 300 Microsoft 365 Vállalati prémium verzió is használhat előfizetést, és több mint 300 Microsoft 365 E3 előfizetést is kaphat. A Microsoft Defender Office 365 azonban nem része a Microsoft 365 E3. A további veszélyforrások elleni védelem érdekében további Defendert kell hozzáadni a Office 365-licencekhez, hogy az Office 365 Defenderrel hatókörben rendelkező összes felhasználónak legyen licence.

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>Különbségek a Microsoft 365 Vállalati prémium verzió és a Microsoft 365 Nagyvállalati verzió

Az alábbi táblázatban a két táblázatban Microsoft 365 Vállalati prémium verzió és a Microsoft 365 E3.

| Funkció    | Támogatás a Microsoft 365 Vállalati prémium verzió    | Támogatás a Microsoft 365 E3 |
|:-------|:-----|:-----|
| **Helyszíni**        | | |
| Windows 10 rendszer esetén    | Windows 10 Business  |     Windows 10 Enterprise E3|
| Office alkalmazások*    | [Üzleti Microsoft 365-alkalmazások](#office-365-business)    | Microsoft 365 Vállalati alkalmazások |
| **Felhőbeli hatékonyságnövelő alkalmazások**        | | |
| Exchange Online és Outlook    | Postaládánként 50 GB tárterületkorlát és korlátlan Exchange Online archiválás    | Postaládánként 100 GB tárterületkorlát és korlátlan Exchange Online archiválás |
| Teams    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![A Microsoft 365 E3](../media/check-mark.png) |
| OneDrive Vállalati verzió    | Felhasználónként 1 TB tárterületkorlát    | Korlátlan |
| Yammer, SharePoint, Planner, Stream    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![A Microsoft 365 E3](../media/check-mark.png) |
| **Veszélyforrások elleni védelem**        | | |
| Támadásifelület-csökkentés lehetőségei    | [A lista](#threat-protection) | A hardveralapú elkülönítés nagyvállalati kezelése Microsoft Edge |
| Defender a Office 365 1. csomaghoz | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | Nem tartalmazza, de a következőn használhatja: |
| **Identitáskezelés**        | | |
| Önkiszolgáló jelszó-visszaállítás hibrid Azure Active Directory -fiókokhoz (Azure AD-fiókokhoz), Azure AD többtényezős hitelesítés (MFA), feltételes hozzáférés, jelszóvisszaírás a helyszíni identitásokhoz|     ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![A Microsoft 365 E3](../media/check-mark.png) |
| Cloud App Discovery, Azure AD Csatlakozás Health    |     | ![A Microsoft 365 E3](../media/check-mark.png) |
| Azure AD Office 365 -Sign-On (SSO): Felhasználónként 10 app (Gallery SaaS-appok, például Salesforce)* | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![A Microsoft 365 E3](../media/check-mark.png) |
| prémium szintű Azure AD 1 SSO: nincs korlátozás (helyszíni appok az Azure AD-alkalmazásproxyn keresztül és a nem galériaalkalmazások az Self-Service-integrációs sablonokkal)    |     | ![A Microsoft 365 E3](../media/check-mark.png) |
| **Eszköz- és alkalmazáskezelés**        | | |
| Microsoft Intune, Windows Autopilot|     ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![A Microsoft 365 E3](../media/check-mark.png) |
|Virtual Desktop Access (VDA)    |  |     ![A Microsoft 365 E3](../media/check-mark.png) |
|Windows Virtual Desktop (WVD)    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png) |     ![A Microsoft 365 E3](../media/check-mark.png) |
|Megosztott számítógép aktiválása (SCA)    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png) |     ![A Microsoft 365 E3](../media/check-mark.png) |
| A Microsoft asztali optimalizálási csomagja    | |     ![A Microsoft 365 E3](../media/check-mark.png) |
| **Információvédelem**        | | |
| Office 365 Adatveszteség-megelőzés, Azure Information Protection 1. csomag    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![A Microsoft 365 E3](../media/check-mark.png) |
| Window Information Protection for endpoint DLP    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![A Microsoft 365 E3](../media/check-mark.png) |
| **Ügyfélelérési licenc (CAL-jogok)**    | | |
| Nagyvállalati CAL csomag (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)| |         ![A Microsoft 365 E3](../media/check-mark.png) |
| **Megfelelőség**        | | |
| Korlátlan e-mail archiválás    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![A Microsoft 365 E3](../media/check-mark.png) |
| Megfelelőségkezelő    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![A Microsoft 365 E3](../media/check-mark.png) |
| Elektronikus észlelés    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![A Microsoft 365 E3](../media/check-mark.png) |
| A helytől való hely- és jogi tartás    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![A Microsoft 365 E3](../media/check-mark.png) |
| Üzenetrekord-kezelési (MRM) adatmegőrzési címkék és adatmegőrzési házirendek    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![A Microsoft 365 E3](../media/check-mark.png) |
||||

\* A SaaS-alkalmazásokhoz hozzáféréssel társított felhasználók legfeljebb 10 apphoz kaphatnak SSO-hozzáférést. A rendszergazdák konfigurálhatnak SSO-t, és módosíthatják a felhasználók hozzáférését a különböző SaaS-alkalmazásokhoz, az SSO-hozzáférés azonban felhasználónként csak 10 app számára engedélyezett. Minden Office 365 alkalmazás egyetlen alkalmazásnak számít.

## <a name="migration"></a>Áttelepítés

Az áttelepítéshez a partnerével együtt helyezze át Microsoft 365 Vállalati prémium verzió előfizetését és licenceit egy megfelelő előfizetésbe Microsoft 365 E3 licencekkel együtt.

Az alábbi szakaszokban ismertetheti, hogy milyen módosításokat kell, ha van, és hogy mit lehet tenni az áttelepítés után.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Microsoft 365-előfizetés konfigurációjának és adatainak beállítása

Az áttelepítés előtt semmit sem kell változtatnia az aktuális előfizetésen vagy adatokon, beleértve az alábbi adatokat:

- Előfizetés-konfiguráció, például DNS-tartománynevek.
- Felhasználói és csoportfiókok, valamint hitelesítési beállítások, például többtényezős hitelesítés vagy feltételes hozzáférési házirendek.
- Hatékonyságnövelő szolgáltatáskonfigurációk és adataik , például Teams, Exchange Online-postaládák, SharePoint Online webhelyek, OneDrive Vállalati verzió mappák és OneNote jegyzetfüzetek.

A felhasználók mostantól korlátlan tárterületet élvezhetnek a Exchange Online és a OneDrive Vállalati verzió mappáiban.

A Cloud App Discovery, az Azure AD Csatlakozás Health és az SSO több mint 10 appot is használhat.

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Veszélyforrások elleni védelem

Windows 10 Business az alábbi védelemeket tartalmazza:

- Az operációs rendszerindítási folyamat integritási kényszerítési eljárása
- Bizalmas működési összetevők integritási kényszerítése
- Speciális biztonsági rés és a biztonsági rés kiaknázása elleni nulla napos megoldások
- A Microsoft Edge, az Internet Explorer és a Chrome jó hírnevén alapuló hálózatvédelem
- Állomásalapú tűzfal
- Zsarolóvírusok elleni megoldások
- Hardveralapú elkülönítés a Microsoft Edge
- Alkalmazásvezérlő az intelligens biztonsági Graph
- Eszközvezérlő (USB)
- Hálózatvédelem a webes veszélyforrások számára
- Host intrusion prevention rules

Windows 10 Enterprise Az E3 csomag magában foglalja a hardveralapú elkülönítés nagyvállalati kezelését is Microsoft Edge.

> [!NOTE]
> Az új rendszerbe áttelepített Microsoft 365 E3 a további veszélyforrások elleni védelem érdekében Office 365 Microsoft Defender szükséges. Ne mindenképpen vásároljon további Defender Office 365, hogy a rendszer a saját defendere által Office 365 összes felhasználónak licencet vásároljon.

### <a name="device-management-with-intune"></a>Eszközkezelés az Intune-nal

Az áttelepítés előtt nem kell módosítania az aktuális Intune-konfigurációt, beleértve a regisztrált eszközöket, eszköz- és alkalmazásbeállításokat.

### <a name="windows-10"></a>Windows 10 rendszer esetén

Microsoft 365 Vállalati prémium verzió autopilottal Windows 10 Business, amelyek az AutoPilottal Windows telepíthetők. Az áttelepítési Microsoft 365 E3 minden felhasználói licenc tartalmazza az Windows 10 Enterprise E3-t, amelyet az Autopilottal is Windows telepíthet.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>Üzleti Microsoft 365-alkalmazások

Az Üzleti Microsoft 365-alkalmazások telepített ügyfélprogram automatikusan elkezdi használni a Nagyvállalati Microsoft 365-alkalmazások. Az áttelepítés után a következőt használhatja:

- Csoportházirend-támogatás
- Spreadsheet compare and inquire
- Üzleti intelligencia

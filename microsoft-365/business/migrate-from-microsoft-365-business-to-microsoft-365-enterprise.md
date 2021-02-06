---
title: Áttelepítés a Microsoft 365 Vállalati verzióról a Microsoft 365 E3 verzióra
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
description: Megtudhatja, hogy miként helyezze át vállalkozását a Microsoft 365 Vállalati prémium verzióról a Microsoft 365 E3 csomagra.
ms.openlocfilehash: 019a422bb879389f42a32cf30f9a8094f776078a
ms.sourcegitcommit: eac5d9f759f290d3c51cafaf335a1a1c43ded927
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50126201"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Áttelepítés a Microsoft 365 Vállalati prémium verzióról a Microsoft 365 E3 csomagra

A Microsoft 365 Vállalati prémium verzió mindennel rendelkezik, ami a kisvállalati verzióhoz szükséges, a legjobb, felhőalapú hatékonyságnövelő alkalmazásokat egyszerű eszközkezelési és biztonsági funkciókkal kombinálva, amelyek lehetővé teszik az alkalmazottaknak, hogy a lehető legjobb munkájukat tetsszen. Bizonyos esetekben azonban előfordulhat, hogy át kell áttelepítése a Microsoft 365 Vállalati prémium verziós előfizetését a Microsoft 365 E3 csomagra. 

A vállalkozása például több mint 300 licencre van szüksége (egyébként gratulálunk!

A vállalatnak nagyvállalati funkciókra is szüksége van, például a Nagyvállalati Microsoft 365-alkalmazásokra, a Windows 10 Nagyvállalati E3 verzióra vagy a Nagyvállalati ügyfélelérési licencekre (CAL-ek).

A frissítés egyszerű: a frissítést a Felügyeleti [központból indíthatja el.](../commerce/subscriptions/upgrade-to-different-plan.md) Az aktuális előfizetésében lévő összes adata és konfigurációja megmarad. Az áttelepítésre való felkészüléshez semmit sem kell tennie, és később semmit sem kell tennie, csak ki kell használnia az új funkciók előnyeit.

>[!Note]
>Microsoft 365 Vállalati prémium verziós előfizetéssel akár 300-as verziós előfizetést is használhat, és Microsoft 365 E3-előfizetést is kaphat több mint 300 csomaghoz. A Microsoft Defender az Office 365-hez azonban nem része a Microsoft 365 E3-nak. A további veszélyforrások elleni védelem érdekében további Office 365-licenceket kell hozzáadnia, hogy az Office 365-ös Defenderrel rendelkező összes felhasználónak legyen licence.
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>Különbségek a Microsoft 365 Vállalati prémium verzió és a Microsoft 365 Nagyvállalati verzió között

Az alábbi táblázat a Microsoft 365 Vállalati prémium verzió és a Microsoft 365 E3 közötti különbségeket mutatja be.

| Funkció    | Támogatás a Microsoft 365 Vállalati prémium verzióban    | Támogatás a Microsoft 365 E3-ban | 
|:-------|:-----|:-----|
| **Helyszíni**        | | | 
| Windows 10    | Windows 10 Business  |     Windows 10 Enterprise E3| 
| Office-appok*    | [Microsoft 365-alkalmazások vállalati verzió](#office-365-business)    | Nagyvállalati Microsoft 365-alkalmazások | 
| **Felhőbeli hatékonyságnövelő alkalmazások**        | | | 
| Exchange Online és Outlook    | Postaládánként 50 GB tárterületkorlát és korlátlan Exchange Online-archiválás    | Postaládánként 100 GB tárterületkorlát és korlátlan Exchange Online-archiválás | 
| Teams    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomagban](../media/check-mark.png) | 
| OneDrive Vállalati verzió    | Felhasználónként 1 TB tárterületkorlát    | Korlátlan | 
| Yammer, SharePoint Online, Planner, Stream    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomagban](../media/check-mark.png) | 
| MileIQ    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | | 
| **Veszélyforrások elleni védelem**        | | | 
| Támadásifelület-csökkentés lehetőségei    | [A lista](#threat-protection) | Hardveralapú elkülönítés nagyvállalati kezelése a Microsoft Edge-ben | 
| Defender az Office 365 1. csomaghoz | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | Nem szerepel a csomagban, de hozzáadható | 
| **Identitáskezelés**        | | | 
| Önkiszolgáló jelszó-visszaállítás a hibrid Azure Active Directory -fiókokhoz (Azure AD), Azure AD többtényezős hitelesítéshez (MFA), feltételes hozzáféréshez, jelszóvisszaírás helyszíni identitásokhoz|     ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomagban](../media/check-mark.png) | 
| Cloud App Discovery, Azure AD Connect Health    |     | ![A Microsoft 365 E3 csomagban](../media/check-mark.png) | 
| Azure AD Office 365-appok Sign-On (SSO): Felhasználónként 10 app (Gallery SaaS-appok, például Salesforce)* | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomagban](../media/check-mark.png) | 
| Azure AD Premium 1 SSO: nincs korlát (helyszíni appok az Azure AD alkalmazásproxyn keresztül és nem galériaalkalmazások az Self-Service appintegrációs sablonokkal)    |     | ![A Microsoft 365 E3 csomagban](../media/check-mark.png) | 
| **Eszköz- és alkalmazáskezelés**        | | | 
| Microsoft Intune, Windows Autopilot|     ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomagban](../media/check-mark.png) | 
|Virtual Desktop Access (VDA)    |  |     ![A Microsoft 365 E3 csomagban](../media/check-mark.png) | 
|Windows Virtuális asztal (WVD)    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png) |     ![A Microsoft 365 E3 csomagban](../media/check-mark.png) | 
|Megosztott számítógép aktiválása (SCA)    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png) |     ![A Microsoft 365 E3 csomagban](../media/check-mark.png) | 
| A Microsoft asztali optimalizálási csomagja    | |     ![A Microsoft 365 E3 csomagban](../media/check-mark.png) | 
| **Információvédelem**        | | | 
| Office 365 Adatveszteség-megelőzés, Azure Information Protection 1. csomag    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomagban](../media/check-mark.png) | 
| Window Information Protection for endpoint DLP    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomagban](../media/check-mark.png) | 
| **Ügyfélelérési licenc (CAL-jogok)**    | | |     
| Nagyvállalati CAL csomag (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)| |         ![A Microsoft 365 E3 csomagban](../media/check-mark.png) | 
| **Megfelelőség**        | | | 
| Korlátlan e-mail archiválás    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomagban](../media/check-mark.png) | 
| Megfelelőségkezelő    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomagban](../media/check-mark.png) | 
| Elektronikus észlelés    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomagban](../media/check-mark.png) | 
| Helybeli és jogi tartás    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomagban](../media/check-mark.png) | 
| Üzenetrekord-kezelési (MRM) adatmegőrzési címkék és adatmegőrzési házirendek    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomagban](../media/check-mark.png) | 
||||

\* Azok a felhasználók, akik hozzáféréssel vannak a SaaS-alkalmazásokhoz, SSO-hozzáférést kaphatnak legfeljebb 10 apphoz. A rendszergazdák konfigurálhatnak SSO-t, és módosíthatják a különböző SaaS-appok felhasználói hozzáférését, de az SSO-hozzáférés felhasználónként csak 10 app számára engedélyezett. Minden Office 365-app egyetlen alkalmazásnak számít.

## <a name="migration"></a>Áttelepítés

Az áttelepítéshez a partnerével együtt helyezze át Microsoft 365 Vállalati prémium verziós előfizetését és licencét egy megfelelő Microsoft 365 E3-előfizetésbe a licencével együtt.

Az alábbi szakaszok ismertetik, hogy milyen módosításokat kell megtennie (ha van ilyen) és milyen lehetőségeket kell követnie az áttelepítés után.

### <a name="microsoft-365-subscription-configuration-and-data"></a>A Microsoft 365-előfizetés konfigurációja és adatai

Az áttelepítés előtt semmit sem kell változtatnia az aktuális előfizetésen vagy az adatokon, beleértve az alábbi adatokat:

- Előfizetés-konfiguráció, például DNS-tartománynevek.
- Felhasználói és csoportos fiókok és hitelesítési beállítások, például többtényezős hitelesítés vagy feltételes hozzáférési házirendek.
- Hatékonyságnövelő szolgáltatáskonfigurációk és adataik, például Teams, Exchange Online-postaládák, SharePoint Online-webhelyek, OneDrive Vállalati verziós mappák és OneNote-jegyzetfüzetek.

A felhasználók mostantól korlátlan tárterületet használhatjanak az Exchange Online-postaládákban és a OneDrive Vállalati verzió mappáiban.

Több mint 10 alkalmazáshoz használhatja a Cloud App Discovery, az Azure AD Connect Health és az SSO alkalmazást.

>[!Note]
>A Microsoft 365 E3-ra áttelepített felhasználók már nem használhatják a MileIQ-t.
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Veszélyforrások elleni védelem

A Windows 10 Business az alábbi védelmet tartalmazza:

- Az operációs rendszerindítási folyamat integritási kényszerítési eljárása
- Bizalmas működési összetevők integritási kényszerítése
- Fejlett biztonsági rés és nulla napos kiaknázás elleni megoldások
- A Microsoft Edge, az Internet Explorer és a Chrome jó hírnevén alapuló hálózatvédelem
- Host-based firewall
- Zsarolóvírusok elleni megoldások
- Hardveralapú elkülönítés a Microsoft Edge-hez
- Az Intelligens biztonsági grafikonon vezérelt alkalmazásvezérlő
- Eszközvezérlő (USB)
- A webes veszélyforrások hálózatvédelemmel való védelme
- Host intrusion prevention rules

A Windows 10 Nagyvállalati E3 csomag a Microsoft Edge hardveralapú elkülönítésének nagyvállalati kezelését is magában foglalja.

>[!Note]
>A Microsoft 365 E3-ra áttelepített felhasználóknak szükségük lesz egy Microsoft Defender Office 365-licencre a további veszélyforrások elleni védelem érdekében. Mindenképpen vásároljon további Office 365-ös Office 365-licenceket, hogy az Office 365-ös Defenderrel rendelkező összes felhasználónak legyen licence. 
>

### <a name="device-management-with-intune"></a>Eszközkezelés az Intune-nal

Az áttelepítés előtt nem kell módosítania az aktuális Intune-konfigurációját, beleértve a regisztrált eszközöket, valamint az eszköz- és alkalmazásbeállításokat.

### <a name="windows-10"></a>Windows 10

A Microsoft 365 Vállalati prémium verzió tartalmazza a Windows 10 Businesst, amelyet a Windows AutoPilottal telepíthet. A Microsoft 365 E3 csomagra való áttelepítéskor minden felhasználói licenc tartalmazza a Windows 10 Nagyvállalati E3 rendszert, amelyet a Windows Autopilottal is telepíthet.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>Microsoft 365-alkalmazások vállalati verzió

Az eszközeire telepített Microsoft 365-alkalmazások vállalati ügyfélalkalmazások automatikusan megkezdik a Nagyvállalati Microsoft 365-alkalmazások funkcióinak használatát. Az áttelepítés után a következőt használhatja:

 - Csoportházirend támogatása
 - Spreadsheet compare and inquire
 - Üzleti intelligencia


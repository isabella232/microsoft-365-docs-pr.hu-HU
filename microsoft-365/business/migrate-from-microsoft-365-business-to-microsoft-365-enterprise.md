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
ms.openlocfilehash: 10630671f3deb7eff0ad0f601d301b90743ee35f
ms.sourcegitcommit: 2a708650b7e30a53d10a2fe3164c6ed5ea37d868
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/24/2021
ms.locfileid: "51164513"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Áttelepítés a Microsoft 365 Vállalati prémium verzióról a Microsoft 365 E3 csomagra

A Microsoft 365 Vállalati prémium verzió mindennel rendelkezik, ami a kisvállalati verzióhoz szükséges. A kategóriában legjobb felhőalapú hatékonyságnövelő alkalmazásokat egyszerű eszközkezelési és biztonsági funkciókkal kombinálva lehetővé teszi, hogy alkalmazottai a lehető legjobb munkát el tudjaják látni. Bizonyos esetekben azonban előfordulhat, hogy át kell áttelepítése a Microsoft 365 Vállalati prémium verziós előfizetését a Microsoft 365 E3 csomagra. 

A vállalkozása például több mint 300 licencre van szüksége (egyébként gratulálunk).

A vállalatnak nagyvállalati funkciókra is szüksége van, például nagyvállalati Microsoft 365-alkalmazásokra, Windows 10 Nagyvállalati E3 vagy Nagyvállalati ügyfélelérési licencekre (CAL-ek).

A frissítés egyszerű: a frissítést a [Felügyeleti központból elindíthatja.](../commerce/subscriptions/upgrade-to-different-plan.md) Jelenlegi előfizetésében minden adata és konfigurációja megmarad. Semmit sem kell tennie az áttelepítésre való felkészüléshez, és később semmit sem kell tennie, az új funkciók előnyeinek kihasználásán kívül.

>[!Note]
>Microsoft 365 Vállalati prémium verziós előfizetéssel akár 300-as előfizetést is használhat, és Microsoft 365 E3-előfizetést is kaphat több mint 300 helyért. Az Office 365-hez való Microsoft Defendert azonban nem tartalmazza a Microsoft 365 E3. A további veszélyforrások elleni védelem érdekében további Office 365-licenceket kell hozzáadnia, hogy az Office 365-ös Defenderrel rendelkező minden felhasználónak legyen licence.
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>A Microsoft 365 Vállalati prémium verzió és a Microsoft 365 Nagyvállalati verzió közötti különbségek

Az alábbi táblázatban a Microsoft 365 Vállalati prémium verzió és a Microsoft 365 E3 csomag közötti különbségeket mutatjuk be.

| Funkció    | Támogatás a Microsoft 365 Vállalati prémium verzióban    | Támogatás a Microsoft 365 E3-ban | 
|:-------|:-----|:-----|
| **Helyszíni**        | | | 
| Windows 10    | Windows 10 Business  |     Windows 10 Nagyvállalati E3| 
| Office-appok*    | [Microsoft 365-alkalmazások vállalati verzióhoz](#office-365-business)    | Microsoft 365 Vállalati alkalmazások | 
| **Felhőbeli hatékonyságnövelő alkalmazások**        | | | 
| Exchange Online és Outlook    | Postaládánként 50 GB tárterületkorlát és korlátlan Exchange Online-archiválás    | Postaládánként 100 GB tárterületkorlát és korlátlan Exchange Online-archiválás | 
| Teams    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| OneDrive Vállalati verzió    | Felhasználónként 1 TB tárterületkorlát    | Korlátlan | 
| Yammer, SharePoint Online, Planner, Stream    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| **Veszélyforrások elleni védelem**        | | | 
| Támadásifelület-csökkentés lehetőségei    | [A lista](#threat-protection) | A Hardveralapú elkülönítés nagyvállalati kezelése a Microsoft Edge-ben | 
| Defender az Office 365 1. csomaghoz | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | Nem tartalmazza, de a következőn használhatja: | 
| **Identitáskezelés**        | | | 
| Önkiszolgáló jelszó-visszaállítás hibrid Azure Active Directory-(Azure AD-) fiókokban, Azure AD többtényezős hitelesítés (MFA), feltételes hozzáférés, jelszóvisszaírás a helyszíni identitásokhoz|     ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| Cloud App Discovery, Azure AD Connect Health    |     | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| Azure AD Office 365-appok egyszeri Sign-On (SSO): Felhasználónként 10 app (Gallery SaaS-appok, például Salesforce)* | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| Azure AD Premium 1 SSO: nincs korlátozás (helyszíni appok az Azure AD-alkalmazásproxyn keresztül és a nem galériaalkalmazások az Self-Service-integrációs sablonokkal)    |     | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| **Eszköz- és alkalmazáskezelés**        | | | 
| Microsoft Intune, Windows Autopilot|     ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
|Virtual Desktop Access (VDA)    |  |     ![A Microsoft 365 E3 része](../media/check-mark.png) | 
|Windows Virtual Desktop (WVD)    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png) |     ![A Microsoft 365 E3 része](../media/check-mark.png) | 
|Megosztott számítógép aktiválása (SCA)    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png) |     ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| A Microsoft asztali optimalizálási csomagja    | |     ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| **Információvédelem**        | | | 
| Office 365 Adatveszteség-megelőzés, Azure Information Protection 1. csomag    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| Window Information Protection for endpoint DLP    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| **Ügyfélelérési licenc (CAL-jogok)**    | | |     
| Nagyvállalati CAL csomag (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)| |         ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| **Megfelelőség**        | | | 
| Korlátlan e-mail archiválás    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| Megfelelőségkezelő    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| Elektronikus észlelés    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| A helytől való hely- és jogi tartás    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| Üzenetrekord-kezelési (MRM) adatmegőrzési címkék és adatmegőrzési házirendek    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
||||

\* A SaaS-alkalmazásokhoz hozzáféréssel társított felhasználók legfeljebb 10 apphoz kaphatnak SSO-hozzáférést. A rendszergazdák konfigurálhatnak SSO-t, és módosíthatják a felhasználók hozzáférését a különböző SaaS-alkalmazásokhoz, az SSO-hozzáférés azonban felhasználónként csak 10 app számára engedélyezett. Minden Office 365-app egyetlen alkalmazásnak számít.

## <a name="migration"></a>Áttelepítés

Az áttelepítéshez a partnerével együtt helyezze át Microsoft 365 Business Premium-előfizetését és -licenceit egy megfelelő, licencekkel rendelkező Microsoft 365 E3-előfizetésbe.

Az alábbi szakaszokban ismertetheti, hogy milyen módosításokat kell, ha van, és hogy mit lehet tenni az áttelepítés után.

### <a name="microsoft-365-subscription-configuration-and-data"></a>A Microsoft 365-előfizetés konfigurációja és adatai

Az áttelepítés előtt semmit sem kell változtatnia az aktuális előfizetésen vagy adatokon, beleértve az alábbi adatokat:

- Előfizetés-konfiguráció, például DNS-tartománynevek.
- Felhasználói és csoportfiókok, valamint hitelesítési beállítások, például többtényezős hitelesítés vagy feltételes hozzáférési házirendek.
- Hatékonyságnövelő szolgáltatáskonfigurációk és adataik, például Teams, Exchange Online-postaládák, SharePoint Online-webhelyek, OneDrive Vállalati verziós mappák és OneNote-jegyzetfüzetek.

A felhasználók mostantól korlátlan tárterületet használhatjanak az Exchange Online-postaládákban és a OneDrive Vállalati verzió mappáiban.

A Cloud App Discovery, az Azure AD Connect Health és az SSO használatával több mint 10 appot használhat.

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Veszélyforrások elleni védelem

A Windows 10 Business az alábbi védelemeket tartalmazza:

- Az operációs rendszerindítási folyamat integritási kényszerítési eljárása
- Bizalmas működési összetevők integritási kényszerítése
- Speciális biztonsági rés és a biztonsági rés kiaknázása elleni nulla napos megoldások
- A Microsoft Edge, az Internet Explorer és a Chrome jó hírnevén alapuló hálózatvédelem
- Állomásalapú tűzfal
- Zsarolóvírusok elleni megoldások
- Hardveralapú elkülönítés a Microsoft Edge-hez
- Az Intelligens biztonsági grafikon által vezérelt alkalmazásvezérlő
- Eszközvezérlő (USB)
- Hálózatvédelem a webes veszélyforrások számára
- Host intrusion prevention rules

A Windows 10 Nagyvállalati E3 csomag a Microsoft Edge hardveralapú elkülönítésének nagyvállalati kezelését is magában foglalja.

>[!Note]
>A Microsoft 365 E3-ra áttelepített felhasználóknak szükségük lesz egy Microsoft Defender Office 365-licencre a további veszélyforrások elleni védelem érdekében. Mindenképpen vásároljon további Office 365-licenceket a Defenderrel, hogy az Office 365-ös defenderrel rendelkező minden felhasználónak legyen licence. 
>

### <a name="device-management-with-intune"></a>Eszközkezelés az Intune-nal

Az áttelepítés előtt nem kell módosítania az aktuális Intune-konfigurációt, beleértve a regisztrált eszközöket, eszköz- és alkalmazásbeállításokat.

### <a name="windows-10"></a>Windows 10

A Microsoft 365 Vállalati prémium verzió tartalmazza a Windows 10 Businesst, amelyet a Windows AutoPilottal telepíthet. A Microsoft 365 E3 csomagra való áttelepítéskor minden felhasználói licenc tartalmazza a Windows 10 Enterprise E3 rendszert, amelyet a Windows Autopilottal is telepíthet.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>Microsoft 365-alkalmazások vállalati verzióhoz

Az eszközeire telepített Microsoft 365-ös vállalati ügyfélalkalmazások automatikusan megkezdik a Nagyvállalati Microsoft 365-alkalmazások funkcióinak használatát. Az áttelepítés után a következőt használhatja:

 - Csoportházirend-támogatás
 - Spreadsheet compare and inquire
 - Üzleti intelligencia


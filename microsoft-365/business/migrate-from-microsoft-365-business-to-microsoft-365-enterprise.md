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
ms.openlocfilehash: 2b15d20e3ae1ad0bef871b139e61abf3ba260729
ms.sourcegitcommit: 34ebec8e2bd54ba3d4ccfd9724797665c965c17f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/13/2020
ms.locfileid: "49071427"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Áttérés a Microsoft 365 Business premiumról a Microsoft 365 E3 csomagra

A Microsoft 365 vállalati prémium verzióban mindent meg kell tennie a kisvállalati verzióhoz, amely egyesíti a legalkalmasabb felhőalapú hatékonyságnövelő alkalmazásokat az egyszerű eszközkezelés és-biztonság segítségével, amelyek lehetővé teszik az alkalmazottak számára a legmegfelelőbb munkát. Bizonyos esetekben azonban előfordulhat, hogy a Microsoft 365 vállalati prémium verzióra szóló előfizetést át kell telepítenie a Microsoft 365 E3 csomagra. 

Üzleti tevékenysége például több mint 300-licenccel (Gratulálunk) bővült és szükséges.

Vagy az üzleti igények nagyvállalati funkciókat, többek között a Microsoft 365-alkalmazásokat, a Windows 10-es nagyvállalati E3 verziót vagy az Enterprise ügyfél-hozzáférési licenceket (CAL) kell megadniuk.

A frissítés egyszerű: a frissítés [a felügyeleti központból](../commerce/subscriptions/upgrade-to-different-plan.md)indítható el. A jelenlegi előfizetésben lévő összes adatot és konfigurációt karbantartja. Nem kell semmit sem tennie az áttelepítésre való felkészüléshez, és semmi teendőt sem kell tennie, kivéve az új funkciók előnyeit.

>[!Note]
>A Microsoft 365 vállalati prémium verzióra szóló előfizetéssel akár 300 helyet is elérheti, és Microsoft 365 E3-előfizetést szerezhet a több mint 300 helyhez. A Microsoft Defender for Office 365 azonban nem része a Microsoft 365 E3 csomagnak. A további veszélyforrások elleni védelem érdekében további Office 365-licenceket kell hozzáadnia, hogy az Office 365-ös felügyelői által biztosított összes felhasználó rendelkezik licenccel.
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>A Microsoft 365 vállalati prémium verzió és a Microsoft 365 Enterprise közötti különbségek

Ez a táblázat a Microsoft 365 Business Premium és a Microsoft 365 E3 közötti különbségeket mutatja be.

| Funkció    | Támogatás a Microsoft 365 vállalati prémium verzióban    | Támogatás a Microsoft 365 E3 csomaghoz | 
|:-------|:-----|:-----|
| **Helyszíni**        | | | 
| Windows 10    | Windows 10 Business  |     Windows 10 nagyvállalati E3 csomag| 
| Office-alkalmazások *    | [Microsoft 365-alkalmazások vállalati verzió](#office-365-business)    | Microsoft 365 Vállalati alkalmazások | 
| **Felhőbeli hatékonyságnövelő alkalmazások**        | | | 
| Exchange Online és Outlook    | 50 GB tárolási korlát egy postaládában és korlátlan Exchange Online archiválás    | 100 GB tárolási korlát egy postaládában és korlátlan Exchange Online archiválás | 
| Teams    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| OneDrive Vállalati verzió    | 1 TB tárterület felhasználónként    | Korlátlan | 
| Yammer, SharePoint Online, Planner, Stream    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| MileIQ    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | | 
| **Veszélyforrások elleni védelem**        | | | 
| A támadási felület csökkentési lehetőségei    | [A lista megtekintése](#threat-protection) | A Microsoft Edge hardver-alapú elkülönítésének vállalati kezelése | 
| Defender for Office 365-es csomag 1 | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | Nem szerepelnek, de hozzáadhatók | 
| **Személyazonosság-kezelés**        | | | 
| Önkiszolgáló jelszó-visszaállítás a hibrid Azure Active Directory (Azure AD) fiókokhoz, Azure multi-Factor Authentication (MFA), feltételes hozzáférés, jelszó-writeback a helyszíni identitásokhoz|     ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| Felhőbeli app-felderítés, Azure AD Connect Health    |     | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| Azure AD Office 365-alkalmazások egyetlen Sign-On (SSO): 10 app felhasználónként (Gallery SaaS-alkalmazások, például Salesforce) * | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| Azure AD prémium 1 egyszeri bejelentkezés: nincs korlátozás (helyszíni alkalmazások Azure AD alkalmazásproxy-és nem-gyűjteményes alkalmazásokon keresztül Self-Service app-integrációs sablonok használatával)    |     | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| **Eszközök és alkalmazások kezelése**        | | | 
| Microsoft Intune, Windows Autopilot|     ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
|Virtuális asztali hozzáférés (VDA)    |  |     ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
|Windows Virtual Desktop (WVD)    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png) |     ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
|Megosztott számítógép-aktiválás (SCA)    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png) |     ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| Microsoft asztali optimalizálási csomag    | |     ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| **Adatvédelem**        | | | 
| Az Office 365 adatvesztés-megelőzése, Azure Information Protection Plan 1    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| Window Information Protection for Endpoint DLP    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| **Ügyfél-hozzáférési licenc (CAL-jogok)**    | | |     
| Nagyvállalati CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)| |         ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| **Megfelelőségi**        | | | 
| Korlátlan e-mail-archiválás    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| Megfelelőségi vezető    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| eDiscovery    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| Helyi visszatartás és jogi célú mentesség    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
| Üzenetküldési rekordok kezelése (MRM) adatmegőrzési címkék és adatmegőrzési házirendek    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![A Microsoft 365 E3 csomag része](../media/check-mark.png) | 
||||

\* Azok a felhasználók, akik hozzáféréssel rendelkeznek a SaaS-alkalmazásokhoz, beszerezhetnek egyszeri bejelentkezést, akár 10 alkalmazásba is. A rendszergazdák beállíthatják az egyszeri bejelentkezést, és módosíthatják a felhasználók hozzáférését a különböző SaaS-alkalmazásokhoz, az SSO-hozzáférés azonban csak felhasználónként 10 alkalmazásban engedélyezett egyszerre. Minden Office 365-alkalmazás egyetlen alkalmazásként számítja ki.

## <a name="migration"></a>Áttelepítési

A partnerekkel való áttelepítés érdekében a Microsoft 365 vállalati prémium verzióra szóló előfizetését és licenceit egy megfelelő Microsoft 365 E3-előfizetésre kell áthelyeznie a licencekkel.

Az alábbi szakaszok ismertetik, hogy milyen módosításokat kell végrehajtania, ha vannak ilyenek, és hogy mit tehet az áttelepítés után.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Microsoft 365-előfizetés konfigurációja és adatainak

Az áttelepítés előtt nem kell módosítania a jelenlegi előfizetést vagy adatot, beleértve az alábbiakat:

- Előfizetés konfigurációja (például DNS-tartománynevek)
- Felhasználók és csoportok fiókjai és hitelesítési beállításai, például többtényezős hitelesítés vagy feltételes hozzáférésű házirendek.
- A hatékonyságnövelő szolgáltatások konfigurációi és adatai, többek között a Teams, az Exchange Online-postaládák, a SharePoint Online-webhelyek, a OneDrive vállalati verziós mappák és a OneNote-jegyzetfüzetek.

A felhasználók mostantól korlátlan tárhelyet élvezhetnek az Exchange Online-postaládák és a OneDrive vállalati verzió mappáiban.

Használhatja a Cloud app Discovery, az Azure AD Connect Health és az SSO több mint 10 alkalmazást.

>[!Note]
>A Microsoft 365 E3-ra áttelepített felhasználók már nem használhatják a MileIQ.
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Veszélyforrások elleni védelem

A Windows 10 Business a következő védelmet foglalja magában:

- Az operációs rendszer indítási folyamatának integritása
- Az érzékeny operációs összetevők sértetlenségének érvényesítése
- Speciális biztonsági rések és a nulladik napi hibák enyhítése
- Jó hírű hálózati védelem a Microsoft Edge, az Internet Explorer és a Chrome számára
- Host-alapú tűzfal
- Ransomware enyhítése
- Hardveres elkülönítés a Microsoft Edge-ben
- Az intelligens biztonsági diagram által működtetett alkalmazás-vezérlés
- Device Control (USB)
- Webes fenyegetések hálózati védelme
- A fogadó Behatolás-megelőzési szabályok

A Windows 10 nagyvállalati E3 csomag a Microsoft Edge hardveres elkülönítésének vállalati kezelését is tartalmazza.

>[!Note]
>A Microsoft 365 E3 rendszerre áttelepített felhasználók a további veszélyforrások elleni védelemhez a Microsoft Defender for Office 365 licencet igénylik. Ügyeljen arra, hogy további Office 365-licenceket vásároljon, hogy az Office 365-ös felügyelői által biztosított összes felhasználó rendelkezik licenccel. 
>

### <a name="device-management-with-intune"></a>Eszközkezelés az Intune segítségével

A áttelepítés előtt nem kell módosítania a jelenlegi Intune-konfigurációt, beleértve a regisztrált eszközöket, valamint az eszközök és az App beállításait is.

### <a name="windows-10"></a>Windows 10

A Microsoft 365 vállalati prémium verzió tartalmazza a Windows 10 Business verziót, amelyet a Windows Autopilot segítségével telepíthet. A Microsoft 365 E3-ra történő áttelepítéskor minden felhasználói licenc tartalmazza a Windows 10 nagyvállalati E3 verziót, amelyet a Windows Autopilot segítségével is telepíthet.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>Microsoft 365-alkalmazások vállalati verzió

A Microsoft 365-alapú Office-alkalmazások telepítése automatikusan megkezdődik a Microsoft 365-alkalmazások nagyvállalatoknak funkcióinak használatához. Az áttelepítés után mostantól használhatja a következőt:

 - A mennyiségi aktiválás csoportházirenden keresztül
 - App telemetriai
 - Vezérlők frissítése
 - Számolótábla összehasonlítása és lekérdezése
 - Üzleti intelligencia


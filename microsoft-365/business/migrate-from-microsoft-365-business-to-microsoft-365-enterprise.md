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
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Áttelepítés a Microsoft 365 Business Premium szolgáltatásról a Microsoft 365 E3 szolgáltatásra

A Microsoft 365 Business Premium mindent tartalmaz, amire szüksége lehet a kisvállalkozásához, kombinálva a kategóriájában legjobb felhőalapú hatékonyságnövelő alkalmazásokat az egyszerű eszközkezeléssel és biztonsággal, amelyek lehetővé teszik az alkalmazottak számára, hogy a legjobb munkát végezzék. Bizonyos esetekben azonban előfordulhat, hogy át kell telepítenie a Microsoft 365 Business Premium előfizetését a Microsoft 365 E3 programba. 

Például a vállalkozásod nőtt, és több mint 300 licencre van szüksége (egyébként gratulálok).

Üzleti környezetének vállalati funkciókra is szüksége van, például nagyvállalati Microsoft 365-alkalmazásokra, Windows 10 Nagyvállalati E3-ra vagy vállalati ügyféllicencre.

A frissítés egyszerű: a frissítést [a Felügyeleti központból indíthatja](../commerce/subscriptions/upgrade-to-different-plan.md)el. Az aktuális előfizetésben lévő összes adat és konfiguráció megmarad. Nincs mit tennie, hogy felkészüljenek a migráció, és semmi köze utána, kivéve, hogy kihasználják az új funkciókat.

>[!Note]
>Akár 300 férőhelyes Microsoft 365 Business Premium előfizetést is használhat, és több mint 300 férőhelyes Microsoft 365 E3-előfizetést is kaphat. Az Office 365 ATP azonban nem része a Microsoft 365 E3 szolgáltatásnak. A folyamatos veszélyforrások elleni védelem érdekében további Office 365 ATP-licenceket kell hozzáadnia, hogy az Office 365 ATP-rendszerében lévő összes felhasználó licenccel rendelkezhessen.
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>A Microsoft 365 Business Premium és a Microsoft 365 Enterprise közötti különbségek

Ez a táblázat a Microsoft 365 Business Premium és a Microsoft 365 E3 közötti különbségeket mutatja be.

| Funkció    | Támogatás a Microsoft 365 Vállalati prémium verzióban    | Támogatás a Microsoft 365 E3-ban | 
|:-------|:-----|:-----|
| **Helyszíni**        | | | 
| Windows 10    | Windows 10 Üzleti Verzió  |     Windows 10 Nagyvállalati E3| 
| Office-alkalmazások*    | [Microsoft 365 alkalmazások üzleti célokra](#office-365-business)    | Microsoft 365 nagyvállalati alkalmazások | 
| **Felhőalapú hatékonyságnövelő alkalmazások**        | | | 
| Exchange Online és Outlook    | 50 GB tárhelykorlát postaládánként és korlátlan Exchange Online archiválás    | 100 GB tárhelykorlát postafiókonként és korlátlan Exchange Online archiválás | 
| Csapat    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| OneDrive Vállalati verzió    | Felhasználónként 1 TB tárhelykorlát    | Korlátlan | 
| Yammer, SharePoint Online, Planner, Adatfolyam    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| Outlook ügyfélmenedzser, MileIQ    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | | 
| **Veszélyforrások elleni védelem**        | | | 
| A támadási felület csökkentésének képességei    | [A lista megtekintése](#threat-protection) | A Microsoft Edge hardveralapú elkülönítésének vállalati kezelése | 
| Office 365 Komplex veszélyforrások elleni védelem (ATP) 1. | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | Nem tartalmazza, de hozzáadható a | 
| **Identitáskezelés**        | | | 
| Önkiszolgáló jelszó-visszaállítás hibrid Azure Active Directory (Azure AD) fiókokhoz, Azure többtényezős hitelesítéshez (MFA), feltételes hozzáféréshez, jelszó-visszaírás a helyszíni identitásokhoz|     ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| Cloud App Discovery, Azure AD Connect állapota    |     | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| Azure AD Office 365 alkalmazások egyszeri bejelentkezés (SSO): 10 alkalmazás felhasználónként (Gallery SaaS-alkalmazások, például a Salesforce)* | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| Azure AD Premium 1 egyszeri szolgáltató: nincs korlátozás (helyszíni alkalmazások az Azure AD alkalmazásproxyn keresztül és nem galéria alkalmazások önkiszolgáló alkalmazásintegrációs sablonok használatával)    |     | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| **Eszköz- és alkalmazáskezelés**        | | | 
| Microsoft Intune, Windows Autopilot|     ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
|Virtuális asztali hozzáférés (VDA)    |  |     ![A Microsoft 365 E3 része](../media/check-mark.png) | 
|Windows virtuális asztal (WVD)    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png) |     ![A Microsoft 365 E3 része](../media/check-mark.png) | 
|Megosztott számítógép aktiválása (SCA)    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png) |     ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| Microsoft asztali optimalizálási csomag    | |     ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| **Információvédelem**        | | | 
| Az Office 365 adatvesztés-megelőzési terve, Azure-információvédelmi csomag 1    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| Ablakinformáció-védelem a DLP végponthoz    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| **Ügyféllicenc (CAL-jogok)**    | | |     
| Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)| |         ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| **Megfelelés**        | | | 
| Korlátlan e-mail archiválás    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| Megfelelőségi pontszám/megfelelőségi vezető    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| elektronikus adatfeltárás    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| Helybeni tartás és peres eljárás miatti tartás    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
| Üzenetkezelési rekordok kezelése (MRM) adatmegőrzési címkék és adatmegőrzési házirendek    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![A Microsoft 365 E3 része](../media/check-mark.png) | 
||||

\*A SaaS-alkalmazásokhoz hozzáféréssel rendelkező felhasználók akár 10 alkalmazáshoz is hozzáférhetnek az Sso-alkalmazásokhoz. A rendszergazdák konfigurálhatják az egyszeri hozzáférést, és módosíthatják a felhasználói hozzáférést a különböző SaaS-alkalmazásokhoz, de az Egyszeri szolgáltatás hozzáférése felhasználónként csak 10 alkalmazáshoz engedélyezett egyszerre. Minden Office 365-alkalmazás egyetlen alkalmazásnak számít.

## <a name="migration"></a>Áttelepítési

Az áttelepítéshez a partnerével együttműködve helyezze át Microsoft 365 Business Premium előfizetését és licenceit egy megfelelő Microsoft 365 E3-előfizetésbe a licencekkel.

A következő szakaszok ismertetik, hogy milyen módosításokat kell végrehajtania, ha vannak ilyenek, és mit tehet az áttelepítés után.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Microsoft 365 előfizetés konfigurációja és adatai

Az áttelepítés előtt nem kell módosítania az aktuális előfizetését vagy adatait, amely a következőket tartalmazza:

- Előfizetés-konfiguráció, például DNS-tartománynevek.
- Felhasználói és csoportfiókok és hitelesítési beállítások, például többtényezős hitelesítés vagy feltételes hozzáférési házirendek.
- A hatékonyságnövelő szolgáltatás konfigurációi és adataik, például a Teams, az Exchange Online-postaládák, a SharePoint Online-webhelyek, a OneDrive Vállalati verzió mappái és a OneNote-jegyzetfüzetek.

A felhasználók mostantól korlátlan tárhelyet élvezhetnek az Exchange Online-postaládákban és a OneDrive Vállalati verzióban lévő mappákban.

A Cloud App Discovery, az Azure AD Connect Health és az SSO több mint 10 alkalmazáshoz használható.

>[!Note]
>A Microsoft 365 E3 rendszerre áttelepített felhasználók már nem használhatják az Outlook Customer Manager és a MileIQ alkalmazást.
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Veszélyforrások elleni védelem

A Windows 10 Business a következő védelmet tartalmazza:

- Az operációs rendszer rendszerindítási folyamatának integritásérvényesítési rendszere
- Az érzékeny üzemi elemek integritásának érvényesítése
- Speciális biztonsági rés és nulladik napi biztonsági rés-kockázatcsökkentés
- Hírnévalapú hálózatvédelem a Microsoft Edge, az Internet Explorer és a Chrome számára
- Gazdagépalapú tűzfal
- Zsarolóprogramok enyhítése
- Hardveralapú elkülönítés a Microsoft Edge számára
- Az alkalmazásvezérlés az intelligens biztonsági grafikonon hajtva
- Eszközvezérlés (USB)
- Hálózatvédelem a webalapú fenyegetések számára
- A gazdabehatolás-megelőzési szabályok

A Windows 10 Enterprise E3 a Microsoft Edge hardveralapú elkülönítésének vállalati kezelését is tartalmazza.

>[!Note]
>A Microsoft 365 E3 rendszerre áttelepített felhasználóknak office 365 ATP-licencre lesz szükségük a folyamatos veszélyforrások elleni védelemhez. Mindenképpen vásároljon további Office 365 ATP-licenceket, hogy az Office 365 ATP-rendszerében lévő összes felhasználó licenccel rendelkezik. 
>

### <a name="device-management-with-intune"></a>Eszközkezelés az Intune-nal

Az áttelepítés előtt nem kell módosítania az aktuális Intune-konfigurációt, amely tartalmazza a regisztrált eszközöket, valamint az eszköz- és alkalmazásbeállításokat.

### <a name="windows-10"></a>Windows 10

A Microsoft 365 Business Premium tartalmazza a Windows 10 Business rendszert, amelyet a Windows AutoPilot programmal telepíthet. Amikor áttelepíti a Microsoft 365 E3 rendszert, minden felhasználói licenc tartalmazza a Windows 10 Enterprise E3 rendszert, amelyet a Windows Autopilot segítségével is telepíthet.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>Microsoft 365 alkalmazások üzleti célokra

Az eszközökre telepített Microsoft 365 vállalati alkalmazások automatikusan elkezdik használni a Microsoft 365 vállalati verzióinak funkcióit. Az áttelepítés után a következőket használhatja:

 - Mennyiségi aktiválás csoportházirenddel
 - Alkalmazástelemetria
 - Vezérlők frissítése
 - Számolótábla összehasonlítása és lekérdezése
 - Üzleti intelligencia


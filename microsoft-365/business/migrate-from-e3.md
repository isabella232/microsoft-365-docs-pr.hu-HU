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
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>Áttérés az Office 365 E3-ról a Microsoft 365 Vállalati Prémium verzióra 

A Microsoft 365 Business Premium mindent tartalmaz, amire szüksége lehet a kisvállalkozásához, kombinálva a kategóriájában legjobb felhőalapú hatékonyságnövelő alkalmazásokat az egyszerű eszközkezeléssel és biztonsággal. Ha jelenleg Office 365 E3-előfizetéssel rendelkezik, de nem rendelkezik 300-nál több alkalmazottal, érdemes lehet átváltani a Microsoft 365 Vállalati Prémium verzióra a további biztonsági funkciók érdekében.

Az áttelepítés egyszerű: Először licencet vált, és az aktuális előfizetésben lévő összes adat és felhasználói információ megmarad. Az áttelepítés után be kell állítania a Microsoft 365 Vállalati prémium verzióban hozzáadott funkciókat.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>Az Office 365 E3 és a Microsoft 365 Vállalati Prémium verzió közötti különbségek

Ez a táblázat a Microsoft 365 Vállalati Prémium verzió és az Office 365 E3 közötti különbségeket mutatja be.

| Funkció    | Támogatás a Microsoft 365 Vállalati prémium verzióban    | Támogatás az Office 365 E3-ban | 
|:-------|:-----|:-----|
| **Helyszíni**        | | | 
| Office-alkalmazások<sup>1</sup>    | Microsoft 365 alkalmazások üzleti célokra    | Microsoft 365 nagyvállalati alkalmazások | 
| **Felhőalapú hatékonyságnövelő alkalmazások**        | | | 
| Exchange Online és Outlook    | 50 GB tárhelykorlát postaládánként és korlátlan Exchange Online archiválás    | 100 GB tárhelykorlát postafiókonként és korlátlan Exchange Online archiválás | 
| Csapat    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![Az Office 365 E3 része](../media/check-mark.png) | 
| OneDrive Vállalati verzió    | Felhasználónként 1 TB tárhelykorlát    | Korlátlan | 
| Yammer, SharePoint Online, Planner, Adatfolyam    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![Az Office 365 E3 része](../media/check-mark.png) | 
| StaffHub    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![Az Office 365 E3 része](../media/check-mark.png) | 
| Outlook ügyfélmenedzser, MileIQ    | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | | 
| **Veszélyforrások elleni védelem**        | | | 
| Office 365 Komplex veszélyforrások elleni védelem (ATP) 1. | ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | Nem tartalmazza, de hozzáadható a | 
| **Identitáskezelés**        | | | 
| Önkiszolgáló jelszó-visszaállítás hibrid Azure Active Directory (Azure AD) fiókokhoz, Azure többtényezős hitelesítéshez (MFA), feltételes hozzáféréshez, jelszó-visszaírás a helyszíni identitásokhoz|     ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    |  | 
| **Eszköz- és alkalmazáskezelés**        | | |
| Microsoft Intune, Windows AutoPilot|     ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    |  |
| Megosztott számítógép aktiválása|     ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    | ![Az Office 365 E3 része](../media/check-mark.png)| 
| Frissítési jogok a Windows 10 Pro rendszerre a Win 7/8.1 Pro licencekből|     ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)    || 
| **Információvédelem**        | | |
|Az Office 365 adatvesztés-megelőzési megelőzése|    ![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)|![Az Office 365 E3 része](../media/check-mark.png)|
|Azure Information Protection Plan 1, Bitlocker kényszerítés|![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)||
|Azure Information Protection Plan 1, Érzékenységi címkék|![A Microsoft 365 Business Premium csomag része](../media/check-mark.png)||
|**Ügyféllicenc (CAL-jogok)**|||
|Vállalati CAL Suite (Exchange, SharePoint, Skype)||![Az Office 365 E3 része](../media/check-mark.png)|

<sup>1</sup> Az Office-alkalmazások Microsoft 365 Vállalati Prémium verziója nem tartalmazza a mennyiségi aktiválást a csoportházirenden, az alkalmazástelemetriai adatokon, a frissítésvezérlőkön, a számolótábla-összehasonlításon és -lekérdezésen, illetve az üzleti intelligencián keresztül.

## <a name="migration"></a>Áttelepítési

Az előfizetés áttelepítéséhez olvassa el a [Csomagküldő manuális átváltása](../commerce/subscriptions/change-plans-manually.md) című témakört, ha csak néhány embert szeretne áthelyezni a Microsoft 365 Business Premium szolgáltatásba. Emellett [mindenkit automatikusan](../commerce/subscriptions/upgrade-to-different-plan.md)frissíthet, vagy partnerrel együttműködve áthelyezheti e3-előfizetését és licenceit Microsoft 365 Business Premium előfizetésbe.
A következő szakaszok ismertetik a módosításokat, ha vannak ilyenek, és mit tehet az áttelepítés után.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Az Office 365 E3 előfizetés konfigurációja és adatai
Az áttelepítés előtt nem kell módosítania az aktuális előfizetését vagy adatait, amely a következőket tartalmazza:

- Előfizetés-konfiguráció, például DNS-rekordok és tartománynevek.
- Felhasználói és csoportfiókok és hitelesítési beállítások, például többtényezős hitelesítés vagy feltételes hozzáférési házirendek.
- A hatékonyságnövelő szolgáltatás konfigurációi és adataik, például a Teams, az Exchange Online-postaládák, a SharePoint Online-webhelyek, a OneDrive Vállalati verzió mappái és a OneNote-jegyzetfüzetek.
- Az Office-alkalmazások automatikusan méreteződnek. Az Office 365 modern licencelése 72 óránként ellenőrzi a felhasználó licenchozzárendelését, és az Office-alkalmazásokat a felhasználói előfizetésnek megfelelő verzióra konvertálja.

### <a name="windows-10"></a>Windows 10

Ha a Windows még nem rendelkezik a Windows Pro Creator frissítésével, [frissítse őket a Windows Pro Alkotók frissítésére.](upgrade-to-windows-pro-creators-update.md)

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>Házirendek beállítása a felhasználói eszközök és fájlok védelmére

> [!NOTE]
> Ha office 365 MDM-házirendeket és -eszközöket állít be, ezek az eszközök megjelennek a Microsoft 365 Felügyeleti központ **Eszközök** lapján. A beállított házirendek megjelennek az [Intune portál](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)klasszikus szabályzatainak listájában.

Miután licenceket rendelt a Microsoft 365 Business Premium szolgáltatáshoz, megkezdheti a felhasználók eszközeinek és fájljainak védelmét.

Ha a szervezet minden tagjára frissített microsoft 365 Vállalati prémium verzióra, a kezdőlapon megjelenik a beállítási varázsló, és a [telepítővarázsló lépéseiben a Microsoft 365 Business Premium beállítása](set-up.md) a telepítővarázsló lépéseit követve megvédheti a fájlokat és a mobileszközöket.

Ezeket a lépéseket az Eszközök lapon is elvégezheti:
  
1. A felügyeleti központban a bal oldali navigációs sávon nyissa meg az **Eszközök** \> **házirendje it.**
    
2. Az **Eszközházirendek** lapon válassza a **Hozzáadás gombot.**
    
3. A **Házirend hozzáadása** ablaktáblán adjon nevet a házirendnek, majd válasszon egy **házirendtípust** a legördülő menüből. 
    
     Beállíthat alkalmazásházirendeket az Android és iPhone eszközökön, valamint a Windows 10-en lévő fájlok védelmére, és eszközkonfigurációs házirendeket állíthat be a vállalat tulajdonában lévő Windows 10-es eszközökhöz. A részleteket az alábbi linkeken találja:
    
  - [Appvédelmi beállítások megadása androidos vagy iOS-es eszközökhöz](app-protection-settings-for-android-and-ios.md)
    
  - [Alkalmazásvédelmi beállítások megadása Windows 10-es eszközökhöz](protection-settings-for-windows-10-devices.md)
    
  - [A Windows 10 rendszerű számítógépek eszközvédelmi beállításainak megadása](protection-settings-for-windows-10-pcs.md)
  
4. A házirendek beállítása után Ön és az alkalmazottak beállíthatják az eszközöket:
    
  - A [Windows-eszközök beállítása A Microsoft 365 Business Premium-felhasználók számára](set-up-windows-devices.md) a Windows-eszközökhöz szükséges lépéseket lásd. 
    
  - Az Android-telefonokra és iPhone-okra vonatkozó lépésekért olvassa el [A mobileszközök beállítása Microsoft 365 Business Premium-felhasználók számára.](set-up-mobile-devices.md) 

### <a name="threat-protection"></a>Veszélyforrások elleni védelem

Miután áttelepítette a Microsoft 365 Vállalati Prémium verzióra, office 365 ATP-vel rendelkezik. Az [Office 365 ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) című témakörben olvashat. A beállításról az [ATP-biztonságos hivatkozások beállítása](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [az ATP-biztonságos mellékletek beállítása](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)és az [ATP adathalászat elleni beállítása.](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)

### <a name="sensitivity-labels"></a>Érzékenységi címkék

Az érzékenységi címkék használatának megkezdéséhez olvassa [el az érzékenységi címkék áttekintése,](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) valamint [az érzékenységi címkék létrehozása és kezelése](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) című videót.

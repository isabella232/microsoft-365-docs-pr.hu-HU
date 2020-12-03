---
title: Áttérés a Microsoft 365 Business verzióra az Office 365 E3 csomagból
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
description: Megtudhatja, hogy miként helyezheti át vállalkozását a Microsoft 365 vállalati prémium verzióba az Office 365 E3 csomagból.
ms.openlocfilehash: eebf78c24ed4bfd1a4fc2d843f37aebbe3d35e31
ms.sourcegitcommit: c1dd5be42fe0c5dcc7c05817c941edd9076febf8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/02/2020
ms.locfileid: "49558258"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>Áttérés az Office 365 E3 csomagról Microsoft 365 Business Premium rendszerre 

A Microsoft 365 vállalati prémium verzióban mindent meg kell tennie a kisvállalati verzióhoz, amely a legalkalmasabb felhőalapú hatékonyságnövelő alkalmazásokat ötvözi egyszerű eszközkezelés és-biztonság segítségével. Ha jelenleg Office 365 E3-előfizetése van, de több mint 300 alkalmazottja van, érdemes áttérnie a Microsoft 365 vállalati prémium verzióra a további biztonsági funkciókhoz.

A Migrálás egyszerű: először a licencek váltása, valamint a jelenlegi előfizetésben lévő összes adat és felhasználói adat megmarad. Az áttelepítés után be kell állítania a Microsoft 365 vállalati prémium verzióban hozzáadott funkciókat.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>Az Office 365 E3 és a Microsoft 365 Business prémium verzió közötti különbségek

Ez a táblázat a Microsoft 365 Business Premium és az Office 365 E3 közötti különbségeket mutatja be.

| Funkció    | Támogatás a Microsoft 365 vállalati prémium verzióban    | Támogatás az Office 365 E3 csomaghoz | 
|:-------|:-----|:-----|
| **Helyszíni**        | | | 
| Office-alkalmazások<sup>1</sup>    | Microsoft 365-alkalmazások vállalati verzió    | Nagyvállalati Microsoft 365-alkalmazások | 
| **Felhőbeli hatékonyságnövelő alkalmazások**        | | | 
| Exchange Online és Outlook    | 50 GB tárolási korlát egy postaládában és korlátlan Exchange Online archiválás    | 100 GB tárolási korlát egy postaládában és korlátlan Exchange Online archiválás | 
| Teams    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![Az Office 365 E3 csomag része](../media/check-mark.png) | 
| OneDrive Vállalati verzió    | 1 TB tárterület felhasználónként    | Korlátlan | 
| Yammer, SharePoint Online, Planner, Stream    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![Az Office 365 E3 csomag része](../media/check-mark.png) | 
| StaffHub    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![Az Office 365 E3 csomag része](../media/check-mark.png) | 
| Outlook Customer Manager, MileIQ    | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | | 
| **Veszélyforrások elleni védelem**        | | | 
| Defender for Office 365-es csomag 1 | ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | Nem szerepelnek, de hozzáadhatók | 
| **Személyazonosság-kezelés**        | | | 
| Önkiszolgáló jelszó-visszaállítás a hibrid Azure Active Directory-fiókokhoz, Azure ad multi-Factor Authentication (MFA), feltételes hozzáférés, jelszó-és writeback a helyszíni identitásokhoz|     ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    |  | 
| **Eszközök és alkalmazások kezelése**        | | |
| Microsoft Intune, Windows Autopilot|     ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    |  |
| Megosztott számítógép aktiválása|     ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    | ![Az Office 365 E3 csomag része](../media/check-mark.png)| 
| A Windows 10 Pro rendszerre való frissítés jogosultsága a Win 7/8.1 Pro licenccel|     ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)    || 
| **Adatvédelem**        | | |
|Az Office 365 adatvesztés-megelőzése|    ![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)|![Az Office 365 E3 csomag része](../media/check-mark.png)|
|Azure Information Protection Plan 1, BitLocker-kényszerítés|![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)||
|Azure Information Protection Plan 1, érzékenységi Címkék|![A Microsoft 365 vállalati prémium verzió része](../media/check-mark.png)||
|**Ügyfél-hozzáférési licenc (CAL-jogok)**|||
|Nagyvállalati CAL Suite (Exchange, SharePoint, Skype)||![Az Office 365 E3 csomag része](../media/check-mark.png)|

<sup>1</sup> az Office-alkalmazások Microsoft 365 vállalati prémium verziója nem tartalmaz mennyiségi aktiválást a csoportházirend, az App-telemetriai, a frissítési vezérlőelemek, a számolótábla-összehasonlítás és a felmérés vagy az üzleti intelligencia között.

## <a name="migration"></a>Áttelepítési

Az előfizetés áttelepítéséről a [csomagok manuális módosítása](../commerce/subscriptions/change-plans-manually.md) című témakörben tájékozódhat, ha csak néhány személyt szeretne áthelyezni a Microsoft 365 vállalati prémium verzióba. A [mindenkit automatikusan frissítheti](../commerce/subscriptions/upgrade-to-different-plan.md), vagy egy partnerrel áthelyezheti az E3-előfizetést és a licenceket egy Microsoft 365 vállalati prémium verziós előfizetésbe.
Az alábbi szakaszok leírják azokat a módosításokat, amelyeket az áttelepítés után el kell végeznie, és hogy mit tehet.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Office 365 E3-előfizetés konfigurációja és adatainak
Az áttelepítés előtt semmilyen módosítást nem kell végrehajtania az aktuális előfizetésben vagy az adatokban, beleértve az alábbiakat:

- Az előfizetés konfigurációja, például a DNS-rekordok és a tartománynevek.
- Felhasználók és csoportok fiókjai és hitelesítési beállításai, például többtényezős hitelesítés vagy feltételes hozzáférésű házirendek.
- A hatékonyságnövelő szolgáltatások konfigurációi és adatai, többek között a Teams, az Exchange Online-postaládák, a SharePoint Online-webhelyek, a OneDrive vállalati verziós mappák és a OneNote-jegyzetfüzetek.
- Az Office-alkalmazások automatikusan méretarányba kerülnek. Az Office 365 modern licencelése 72 óránként ellenőrzi a felhasználó licenc-hozzárendelését, és átalakítja az Office-alkalmazásokat a felhasználó előfizetéséhez illő verzióra.

### <a name="windows-10"></a>Windows 10

Ha Windows Pro Creator-frissítésben még nem szerepelnek a Windowsban, [frissítse őket a Windows Pro alkotói frissítésére](upgrade-to-windows-pro-creators-update.md).

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>Házirendek beállítása a felhasználói eszközök és fájlok védelmére

> [!NOTE]
> Ha beállítja az Office 365 MDM irányelveit és eszközeit, ezek az eszközök a Microsoft 365 felügyeleti központ **eszközök** lapján jelennek meg. A beállított házirendek megjelennek az [Intune portál](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)klasszikus házirendek listájában.

Miután kiosztotta a licenceket a Microsoft 365 vállalati prémium verzióra, megkezdheti a felhasználók eszközeinek és fájljainak védelmét.

Ha a szervezet minden tagját frissítette a Microsoft 365 vállalati prémium verzióra, akkor a kezdőlapon megjelenik a beállítási varázsló, és a [microsoft 365 vállalati prémium verzió beállítása a beállítási varázslóban](set-up.md) a fájlok és mobileszközök védelméhez című témakörben található.

Ezeket a lépéseket az eszközök lapon is elvégezheti:
  
1. A felügyeleti központ bal oldali navigációs sávján kattintson az **eszközök** \> **házirendek** elemre.
    
2. Az **eszközök házirendjei** lapon válassza a **Hozzáadás** lehetőséget.
    
3. A házirend **hozzáadása** ablaktáblában adjon nevet a házirendnek, majd válasszon egy **házirend-típust** a legördülő listából. 
    
     Az Android-és iPhone-eszközökön, valamint a Windows 10-on található fájlok védelmére szolgáló alkalmazás-házirendeket, valamint a Windows 10 rendszerű eszközökön beállíthatja az eszköz-konfigurációs házirendeket. További információt az alábbi hivatkozásokra kattintva talál:
    
  - [Appvédelmi beállítások megadása androidos vagy iOS-es eszközökhöz](app-protection-settings-for-android-and-ios.md)
    
  - [Alkalmazásvédelmi beállítások megadása Windows 10-es eszközökhöz](protection-settings-for-windows-10-devices.md)
    
  - [Az eszközbeállítások beállításainak megadása Windows 10 rendszerű PC-ken](protection-settings-for-windows-10-pcs.md)
  
4. Miután beállította a házirendeket, az alkalmazottak a következő eszközökön állíthatják be az eszközöket:
    
  - Lásd: [Windows-eszközök beállítása a Microsoft 365 vállalati prémium verzió felhasználóinak](set-up-windows-devices.md) a Windows-eszközökhöz. 
    
  - Lásd: [mobileszközök beállítása a Microsoft 365 vállalati prémium verzió felhasználóinak](set-up-mobile-devices.md) az Android-telefonokhoz és-iPhone-hoz szükséges lépésekhez. 
  
### <a name="mailbox-size"></a>Postaláda mérete

A Microsoft 365 vállalati prémium verzió 50 GB tárterületet tartalmaz az Exchange Online 1-es verziójának használati határidejeként. A Microsoft 365 vállalati prémium verzióra való áttéréskor, ha egy felhasználója túllépi a 50 GB-ot a postaládában, javasoljuk, hogy rendelje hozzá az Exchange Online 2-es verziós csomagját, és távolítsa el az Exchange Online-csomagot, mert az nem kivitelezhető.


### <a name="threat-protection"></a>Veszélyforrások elleni védelem

A Microsoft 365 vállalati prémium verzióra való áttérés után az Office 365-nek van Defender-je. Áttekintésért olvassa el a [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) című témakört. A beállításról a [biztonságos hivatkozások beállítása](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), a [biztonságos mellékletek](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)beállítása és az [adathalászat beállítása az Office 365-ban](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)című témakörben olvashat.

### <a name="sensitivity-labels"></a>Érzékenységi címkék

A tartalmi címkék használatáról a tartalmi címkék [áttekintése](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) és a [tartalmi Címkék létrehozása és kezelése](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) című témakörben tájékozódhat.

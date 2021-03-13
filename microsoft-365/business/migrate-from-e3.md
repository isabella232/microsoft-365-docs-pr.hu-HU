---
title: Áttelepítés a Microsoft 365 Vállalati verzióba az Office 365 E3-ból
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
description: Megtudhatja, hogy miként helyezze át vállalatát a Microsoft 365 Vállalati prémium verzióba az Office 365 E3 csomagból.
ms.openlocfilehash: eebf78c24ed4bfd1a4fc2d843f37aebbe3d35e31
ms.sourcegitcommit: c1dd5be42fe0c5dcc7c05817c941edd9076febf8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/02/2020
ms.locfileid: "49558258"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>Áttelepítés az Office 365 E3 csomagról a Microsoft 365 Vállalati prémium verzióra 

A Microsoft 365 Vállalati prémium verzió mindennel rendelkezik, ami a kisvállalati verzióhoz szükséges, a kategóriában legjobb felhőalapú hatékonyságnövelő alkalmazásokat egyszerű eszközkezeléssel és biztonsággal kombinálva. Ha jelenleg Office 365 E3-előfizetéssel rendelkezik, de nem rendelkezik több mint 300 alkalmazottal, érdemes a Microsoft 365 Vállalati prémium verzióra váltani a további biztonsági funkciókért.

Az áttelepítés egyszerű: Először váltson a licencek között, és az aktuális előfizetésében lévő összes adata és felhasználói adata megmarad. Az áttelepítés után be kell állítania a Microsoft 365 Vállalati prémium verzióban hozzáadott funkciókat.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>Az Office 365 E3 és a Microsoft 365 Vállalati prémium verzió közötti különbségek

Az alábbi táblázatban a Microsoft 365 Vállalati prémium verzió és az Office 365 E3 csomag közötti különbségeket mutatjuk be.

| Funkció    | Támogatás a Microsoft 365 Vállalati prémium verzióban    | Támogatás az Office 365 E3-ban | 
|:-------|:-----|:-----|
| **Helyszíni**        | | | 
| Office-appok<sup>1</sup>    | Microsoft 365-alkalmazások vállalati verzióhoz    | Nagyvállalati Microsoft 365-alkalmazások | 
| **Felhőbeli hatékonyságnövelő alkalmazások**        | | | 
| Exchange Online és Outlook    | Postaládánként 50 GB tárterületkorlát és korlátlan Exchange Online-archiválás    | Postaládánként 100 GB tárterületkorlát és korlátlan Exchange Online-archiválás | 
| Teams    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![Az Office 365 E3 része](../media/check-mark.png) | 
| OneDrive Vállalati verzió    | Felhasználónként 1 TB tárterületkorlát    | Korlátlan | 
| Yammer, SharePoint Online, Planner, Stream    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![Az Office 365 E3 része](../media/check-mark.png) | 
| StaffHub    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![Az Office 365 E3 része](../media/check-mark.png) | 
| Outlook Customer Manager, MileIQ    | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | | 
| **Veszélyforrások elleni védelem**        | | | 
| Defender az Office 365 1. csomaghoz | ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | Nem tartalmazza, de a következőn használhatja: | 
| **Identitáskezelés**        | | | 
| Önkiszolgáló jelszó-visszaállítás hibrid Azure Active Directory-(Azure AD-) fiókokban, Azure AD többtényezős hitelesítés (MFA), feltételes hozzáférés, jelszóvisszaírás a helyszíni identitásokhoz|     ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    |  | 
| **Eszköz- és alkalmazáskezelés**        | | |
| Microsoft Intune, Windows AutoPilot|     ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    |  |
| Megosztott számítógép aktiválása|     ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    | ![Az Office 365 E3 része](../media/check-mark.png)| 
| A Windows 10 Pro verzióra vonatkozó frissítési jogok a Win 7/8.1 Pro verziós licencekről|     ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)    || 
| **Információvédelem**        | | |
|Office 365 Adatveszteség-megelőzés|    ![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)|![Az Office 365 E3 része](../media/check-mark.png)|
|Azure Information Protection Plan 1, Bitlocker enforcement|![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)||
|Azure Information Protection Plan 1, Bizalmasság-címkék|![A Microsoft 365 Vállalati prémium verzió része](../media/check-mark.png)||
|**Ügyfélelérési licenc (CAL-jogok)**|||
|Nagyvállalati CAL csomag (Exchange, SharePoint, Skype)||![Az Office 365 E3 része](../media/check-mark.png)|

<sup>1</sup> Az Office-appok Microsoft 365 Business Premium verziója nem tartalmazza a mennyiségi aktiválást csoportházirenden, alkalmazás telemetrián, frissítési vezérlőn, számolótábla-összehasonlításon és -lekérdezésen keresztül, illetve az üzleti intelligencia segítségével.

## <a name="migration"></a>Áttelepítés

Ha csak néhány embert [](../commerce/subscriptions/change-plans-manually.md) szeretne áthelyezni a Microsoft 365 Vállalati prémium verzióba, az előfizetés áttelepítéséhez olvassa el a Csomagváltás manuálisan lehetőséget. Automatikusan [frissíthet](../commerce/subscriptions/upgrade-to-different-plan.md)mindenkit , vagy egy partnerrel együtt áthelyezheti az E3-előfizetését és -licenceit egy Microsoft 365 Vállalati prémium verziós előfizetésbe.
Az alábbi szakaszok ismertetik az esetlegesen szükséges módosításokat, valamint azt, hogy mit lehet tenni az áttelepítés után.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Az Office 365 E3 előfizetés konfigurációja és adatai
Az áttelepítés előtt semmit sem kell változtatnia az aktuális előfizetésen vagy az adatain, beleértve az alábbi adatokat:

- Előfizetés-konfiguráció, például DNS-rekordok és tartománynevek.
- Felhasználói és csoportfiókok, valamint hitelesítési beállítások, például többtényezős hitelesítés vagy feltételes hozzáférési házirendek.
- Hatékonyságnövelő szolgáltatáskonfigurációk és adataik, például Teams, Exchange Online-postaládák, SharePoint Online-webhelyek, OneDrive Vállalati verziós mappák és OneNote-jegyzetfüzetek.
- Az Office-alkalmazások mérete automatikusan megtörténik. Az Office 365 modern licencelése 72 óránként ellenőrzi a felhasználó licenc-hozzárendelését, és átalakítja az Office-alkalmazásokat a felhasználói előfizetésnek megfelelő verzióra.

### <a name="windows-10"></a>Windows 10

Ha még nem frissítette a Windows Pro alkotói frissítését a Windows Pro alkotói frissítésére, frissítse őket a [Windows Pro alkotói frissítésére.](upgrade-to-windows-pro-creators-update.md)

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>Házirendek beállítása a felhasználói eszközök és fájlok védelméhez

> [!NOTE]
> Ha Office 365-ös MDM-házirendeket és -eszközöket  ad meg, ezek az eszközök a Microsoft 365 Felügyeleti központ Eszközök lapján lesznek felsorolva. Az Ön által beállított házirendek az Intune portál klasszikus házirendek [listájában megjelenik.](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)

Miután hozzárendelte a licenceket a Microsoft 365 Vállalati prémium verzióhoz, elkezdheti megvédeni a felhasználók eszközeit és fájljait.

Ha szervezetében mindenkit frissített a Microsoft 365 Vállalati prémium verzióra, a kezdőlapon használhatja a beállítási varázslót, és A [Microsoft 365 Vállalati](set-up.md) prémium verzió beállítása varázsló lépéseit követve védheti a fájlokat és a mobileszközeket.

Az Eszközök lapon az alábbi lépéseket is végre tudja tenni:
  
1. A felügyeleti központ bal oldali navigációs  sávjában menjen az Eszköz \> **házirendek lapra.**
    
2. Az Eszköz **házirendek lapon** válassza a Hozzáadás **lehetőséget.**
    
3. A Házirend **hozzáadása ablaktáblában** nevezze el a házirendet, majd válasszon **egy** Házirendtípust a legördülő menüből. 
    
     Alkalmazás-konfigurációs házirendeket állíthat be a fájlok védelméhez Android- és iPhone-eszközökön, valamint Windows 10-es eszközökön, valamint eszközkonfigurációs házirendeket is állíthat be a vállalati tulajdonú Windows 10-es eszközökön. A részleteket az alábbi hivatkozásokra kattintva olvashatja el:
    
  - [Appvédelmi beállítások megadása androidos vagy iOS-es eszközökhöz](app-protection-settings-for-android-and-ios.md)
    
  - [Alkalmazásvédelmi beállítások megadása Windows 10-es eszközökhöz](protection-settings-for-windows-10-devices.md)
    
  - [Eszközvédelmi beállítások megadása Windows 10-es PC-khez](protection-settings-for-windows-10-pcs.md)
  
4. A házirendek beállítása után Ön és alkalmazottai eszközeiket is beállíthatja:
    
  - A Windows rendszerű eszközökhöz a Windows-eszközök beállítása a [Microsoft 365 Vállalati prémium](set-up-windows-devices.md) verzió felhasználóinak lépéseit mutatja be. 
    
  - Az Android-telefonok és iPhone-ok használatának lépéseit a Mobileszközök beállítása [a Microsoft 365 Business Premium](set-up-mobile-devices.md) felhasználói számára. 
  
### <a name="mailbox-size"></a>Postaláda mérete

A Microsoft 365 Vállalati prémium verzió 50 GB-os tárterületkorlátot használ, mivel az Exchange Online 1. csomagját használja. Ha a Microsoft 365 Vállalati prémium verzióra való áttelepítés során bármelyik felhasználó meghaladja az 50 GB-os postaláda-tárterületet, javasoljuk, hogy rendeljen a felhasználóhoz egy Exchange Online 2. csomaggal, és távolítsa el az Exchange Online 1. csomagját, mivel mindkettőt nem lehet hozzárendelni.


### <a name="threat-protection"></a>Veszélyforrások elleni védelem

Miután áttért a Microsoft 365 Vállalati prémium verzióra, az Office 365-nek már van Defendere. További [áttekintést a Microsoft Defender az Office 365-hez](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) témakörben talál. A beállításról további tudnivalókat a Biztonságos hivatkozások [beállítása,](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)a Biztonságos mellékletek beállítása [és](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)az Adathalászat elleni védelem beállítása az [Office 365 Defenderben témakörben található.](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)

### <a name="sensitivity-labels"></a>Érzékenységi címkék

A bizalmasság-címkék használatának elkezdését a Bizalmasság-címkék áttekintése és a bizalmasság-címkék létrehozása és [kezelése videóban](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) olvashatja. [](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)

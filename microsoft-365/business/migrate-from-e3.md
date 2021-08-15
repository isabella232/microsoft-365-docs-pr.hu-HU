---
title: Áttelepítés Microsoft 365 Vállalati verzióba Office 365 E3 csomag
f1.keywords:
- NOCSH
ms.author: cmcatee
author: cmcatee-MSFT
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
- AdminTemplateSet
search.appverid:
- BCS160
- MET150
description: Ha van előfizetése Office 365 E3 csomag, de nincs több mint 300 alkalmazottja, fontolja meg a váltást a Microsoft 365 Vállalati prémium verzió.
ms.openlocfilehash: 89bf493b39250d88fcb47585d71e7dadd6600c4c3fff0658bb72e51b9ff386c5
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53837663"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>Áttelepítés Office 365 E3 csomag Microsoft 365 Vállalati prémium verzió

Microsoft 365 Vállalati prémium verzió rendelkezik mindennel, ami a kisvállalata számára szükséges, a legjobb, felhőalapú hatékonyságnövelő appokat egyszerű eszközkezeléssel és biztonsággal kombinálva. Ha jelenleg Office 365 E3 csomag rendelkezik, de nincs több mint 300 alkalmazottja, fontolja meg a Microsoft 365 Vállalati prémium verzió-re való váltást a további biztonsági funkciókért.

Az áttelepítés egyszerű: Először váltson a licencek között, és az aktuális előfizetésében lévő összes adata és felhasználói adata megmarad. Az áttelepítés után be kell állítania a Microsoft 365 Vállalati prémium verzió.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>Különbségek a Office 365 E3 csomag és a Microsoft 365 Vállalati prémium verzió

Az alábbi táblázat a két táblázatban Microsoft 365 Vállalati prémium verzió és a Office 365 E3 csomag.

| Funkció    | Támogatás a Microsoft 365 Vállalati prémium verzió    | Támogatás a Office 365 E3 csomag |
|:-------|:-----|:-----|
| **Helyszíni**        | | |
| Office alkalmazások<sup>1</sup>    | Üzleti Microsoft 365-alkalmazások    | Microsoft 365 Vállalati alkalmazások |
| **Felhőbeli hatékonyságnövelő alkalmazások**        | | |
| Exchange Online és Outlook    | Postaládánként 50 GB tárterületkorlát és korlátlan Exchange Online Archiválás    | Postaládánként 100 GB tárterületkorlát és korlátlan Exchange Online Archiválás |
| Teams    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![Az Office 365 E3 csomag](../media/check-mark.png) | 
| OneDrive Vállalati verzió    | Felhasználónként 1 TB tárterületkorlát    | Korlátlan | 
| Yammer, SharePoint, Planner, Stream    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![Az Office 365 E3 csomag](../media/check-mark.png) | 
| StaffHub    | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![Az Office 365 E3 csomag](../media/check-mark.png) |
| **Veszélyforrások elleni védelem**        | | |
| Defender a Office 365 1. csomaghoz | ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | Nem tartalmazza, de a következőn használhatja: |
| **Identitáskezelés**        | | |
| Önkiszolgáló jelszó-visszaállítás hibrid Azure Active Directory -fiókokhoz (Azure AD-fiókokhoz), Azure AD többtényezős hitelesítés (MFA), feltételes hozzáférés, jelszóvisszaírás a helyszíni identitásokhoz|     ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    |  |
| **Eszköz- és alkalmazáskezelés**        | | |
| Microsoft Intune, Windows AutoPilot|     ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    |  |
| Megosztott számítógép aktiválása|     ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    | ![Az Office 365 E3 csomag](../media/check-mark.png)| 
| Frissítési jogok Windows 10 Pro Windows 7/8.1 verziós Pro verzióról|     ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)    ||
| **Információvédelem**        | | |
|Office 365 Adatveszteség-megelőzés|    ![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)|![Az Office 365 E3 csomag](../media/check-mark.png)|
|Azure Information Protection Plan 1, BitLocker enforcement|![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)||
|Azure Information Protection Plan 1, Bizalmasság-címkék|![Az Microsoft 365 Vállalati prémium verzió](../media/check-mark.png)||
|**Ügyfélelérési licenc (CAL-jogok)**|||
|Nagyvállalati CAL csomag (Exchange, SharePoint, Skype)||![Az Office 365 E3 csomag](../media/check-mark.png)|

<sup>1</sup> A Microsoft 365 Vállalati prémium verzió appok Office nem tartalmazza a mennyiségi aktiválást csoportházirenden, alkalmazás telemetrián, frissítési vezérlőn, számolótábla-összehasonlításon és -lekérdezésen keresztül, illetve az üzleti intelligencia segítségével.

## <a name="migration"></a>Áttelepítés

Ha csak néhány embert [](../commerce/subscriptions/change-plans-manually.md) szeretne áthelyezni a csomagváltásba, az előfizetés áttelepítéséhez olvassa el a Csomagváltás manuálisan Microsoft 365 Vállalati prémium verzió. Automatikusan is [frissíthet](../commerce/subscriptions/upgrade-to-different-plan.md)mindenkit , vagy egy partnerrel együtt áthelyezheti az E3-előfizetését és -licenceit egy Microsoft 365 Vállalati prémium verzió előfizetésbe.
Az alábbi szakaszok ismertetik az esetlegesen szükséges módosításokat, valamint azt, hogy mit lehet tenni az áttelepítés után.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Office 365 E3 csomag-előfizetés beállítása és adatai
Az áttelepítés előtt semmit sem kell változtatnia az aktuális előfizetésen vagy az adatain, beleértve az alábbi adatokat:

- Előfizetés-konfiguráció, például DNS-rekordok és tartománynevek.
- Felhasználói és csoportfiókok, valamint hitelesítési beállítások, például többtényezős hitelesítés vagy feltételes hozzáférési házirendek.
- Hatékonyságnövelő szolgáltatáskonfigurációk és adataik , például Teams, Exchange Online-postaládák, SharePoint Online webhelyek, OneDrive Vállalati verzió mappák és OneNote jegyzetfüzetek.
- Office alkalmazások méretezése automatikusan megtörténik. Office 365 a modern licencelés 72 óránként ellenőrzi a felhasználó licenc-hozzárendelését, és a Office-alkalmazásokat a felhasználói előfizetésnek megfelelő verzióra konvertálja.

### <a name="windows-10"></a>Windows 10 rendszer esetén

Ha a Windows még nem frissítette a Windows Pro alkotói frissítést, frissítse őket [a Windows Pro alkotói frissítésre.](upgrade-to-windows-pro-creators-update.md)

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>Házirendek beállítása a felhasználói eszközök és fájlok védelméhez

> [!NOTE]
> Ha több MDM Office 365-házirendet és -eszközt is beállított,  ezek az eszközök az Eszközök lapon fognak Microsoft 365 Felügyeleti központ. Az Ön által beállított házirendek az Intune portál klasszikus házirendek [listájában megjelenik.](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)

Miután hozzárendelt licenceket a Microsoft 365 Vállalati prémium verzió, elkezdheti védeni a felhasználók eszközeit és fájljait.

Ha szervezetében mindenkit frissített a Microsoft 365 Vállalati prémium verzió-frissítésre, a kezdőlapon használhatja a beállítási varázslót, és a telepítővarázsló lépéseit követve védheti a fájlokat és a mobileszközeket a [Microsoft 365 Vállalati prémium verzió](set-up.md) beállítási varázslóban.

Az Eszközök lapon az alábbi lépéseket is végre tudja tenni:
  
1. A felügyeleti központ bal oldali navigációs  sávjában menjen az Eszköz \> **házirendek lapra.**

2. Az Eszköz **házirendek lapon** válassza a Hozzáadás **lehetőséget.**

3. A Házirend **hozzáadása ablaktáblában** nevezze el a házirendet, majd válasszon **egy** Házirendtípust a legördülő menüből.

     Alkalmazás-konfigurációs házirendeket állíthat be az Android- és iPhone-eszközökön, valamint az Windows 10-ban lévő fájlok védelmére, valamint eszközkonfigurációs házirendeket állíthat be a vállalati tulajdonú Windows 10 eszközökön. A részleteket az alábbi hivatkozásokra kattintva olvashatja el:

  - [Appvédelmi beállítások megadása androidos vagy iOS-es eszközökhöz](app-protection-settings-for-android-and-ios.md)

  - [Alkalmazásvédelmi beállítások megadása Windows 10-es eszközökhöz](protection-settings-for-windows-10-devices.md)

  - [Eszközvédelmi beállítások megadása Windows 10 PC-khez](protection-settings-for-windows-10-pcs.md)
  
4. A házirendek beállítása után Ön és alkalmazottai eszközeiket is beállíthatja:

  - Az [eszköz Windows beállítása Microsoft 365 Vállalati prémium verzió felhasználók](set-up-windows-devices.md) számára Windows lépéseket. 

  - Az [Android-telefonok és](set-up-mobile-devices.md) iPhone-ok használatának Microsoft 365 Vállalati prémium verzió beállítása a mobileszközök számára. 
  
### <a name="mailbox-size"></a>Postaláda mérete

Microsoft 365 Vállalati prémium verzió 50 GB-os tárterületkorlátot használ az 1. Exchange Online használ. Az Microsoft 365 Vállalati prémium verzió-re való áttelepítés során, ha a felhasználók bármelyike meghaladja az 50 GB-os postaláda-tárterületet, javasoljuk, hogy rendeljen a felhasználóhoz egy Exchange Online 2. csomaggal, és távolítsa el az Exchange Online 1. csomagját, mivel mindkettőt nem lehet hozzárendelni.

### <a name="threat-protection"></a>Veszélyforrások elleni védelem

Az áttelepítés után Microsoft 365 Vállalati prémium verzió Defender Office 365. További [áttekintést a Microsoft Defender Office 365](../security/office-365-security/defender-for-office-365.md) talál. A beállításról [](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)további Széf, a mellékletek Széf [és](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)az Adathalászat elleni védelem beállítása a [Defenderben a](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)Office 365.

### <a name="sensitivity-labels"></a>Érzékenységi címkék

A bizalmasság-címkék használatának elkezdését a Bizalmasság-címkék áttekintése és a bizalmasság-címkék létrehozása és [kezelése videóban](../business-video/create-sensitivity-labels.md) olvashatja. [](../compliance/sensitivity-labels.md)

## <a name="related-content"></a>Kapcsolódó tartalom

[Csomagváltás kézzel](../commerce/subscriptions/change-plans-manually.md) (cikk)\
[Az Windows-eszközök frissítése Windows 10 Pro](upgrade-to-windows-pro-creators-update.md) (videó)\
[Appvédelmi beállítások megadása Android- és iOS-eszközökön](app-protection-settings-for-android-and-ios.md) (cikk)\
[Alkalmazásvédelmi beállítások](protection-settings-for-windows-10-devices.md) megadása és szerkesztése Windows 10 eszközökön (cikk)\
[]


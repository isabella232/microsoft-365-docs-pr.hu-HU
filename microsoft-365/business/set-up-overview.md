---
title: A beállítás áttekintése
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Ismerje meg a Microsoft 365 vállalati prémium verzió telepítési lépéseit, a feliratkozást, a tartomány és a felhasználók hozzáadását, illetve a biztonsági házirendek beállítását.
ms.openlocfilehash: fa9c02fa9546437c83b9cc6c1f1e6e0d723ec868
ms.sourcegitcommit: 555d756c69ac9031d1fb928f2e1f9750beede066
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/29/2020
ms.locfileid: "47306469"
---
# <a name="overview-of-setup"></a>A beállítás áttekintése

Tekintsen meg egy rövid videót a Microsoft 365 vállalati prémium verzió telepítéséről.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Ha hasznosnak találta ezt a videót, tekintse meg a [teljes tanfolyamok kisvállalatoknak és Microsoft 365-újoncoknak](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) című cikket.

A beállítási lépések többsége a beállítási varázslóban végezhető el, de az egyéb beállítások is szerepelnek a listában.

## <a name="step-1-add-your-domain-and-users"></a>Első lépés: a tartomány és a felhasználók felvétele

   - **[Tartomány felvétele](set-up.md#add-your-domain-to-personalize-sign-in)** (ha a [regisztráció](sign-up.md)során vásárolta meg a tartományt, ez a lépés már elkészült.)

   - **Felhasználók hozzáadása** A felhasználók a következő három módon adhatók hozzá:
        - A [varázslóban](set-up.md#add-users-in-the-wizard).
        - A címtár-szinkronizálás segítségével [felhasználókat vehet fel az Azure ad Connect segítségével](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) , ha helyszíni Active Directoryval rendelkezik.
        - A felügyeleti központban [később is hozzáadhat felhasználókat](add-users-m365b.md) .
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>2. lépés: biztonsági házirendek beállítása és eszközök beállítása 

  - Az eszköz-házirendek beállításához használja a [beállítási varázslót](set-up.md#protect-your-organization) . 
  - Később a [felügyeleti központban](view-policies-and-devices.md) és az [Intune portálon](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)is hozzáadhat további vagy szerkesztheti őket.
  - A beállítási varázsló a fenyegetések elleni védelem és az adatvesztés megelőzésére szolgáló beállításokat is megadhatja.
  
  A beállítási varázsló biztonsági beállításain kívül az alábbi beállítások megadásával növelheti a biztonságot:

- **E-mailes kártevők elleni védelem**
- **ATP-adathalászat**
- **Exchange Online Archiválás**
- **Azure Information Protection (Plan1**)

A kezdéshez lásd: a [fenyegetések elleni védelem növelése](increase-threat-protection.md) és a [megfelelőségi funkciók beállítása](set-up-compliance.md).

Lásd még az [első 10 módszer a Microsoft 365 vállalati prémium verzió biztonságossá](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) tételéhez a legjobb biztonsági gyakorlatokra vonatkozó ütemtervet.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>3. lépés: a Windows 10-es eszközök beállítása és kezelése

A beállítás varázsló futtatása után a szervezet minden Windwos 10 számítógépét proctect.
  
- A Windows 10 Pro a Microsoft 365 vállalati prémium verzió [előfeltétele](pre-requisites-for-data-protection.md) , de ha Windows 7 Pro, Windows 8 Pro vagy Windows 8,1 Pro verziót futtat, az előfizetése feljogosítja a [Windows 10 Pro rendszerre való frissítésre](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
- Kövesse a [Windows 10 rendszerű PC-k biztonsága](secure-win-10-pcs.md) című témakör lépéseit a Windows 10-es eszközök házirendjeinek beállításához.

Amikor Windows 10-es eszközre csatlakozik az Azure AD-hoz, a rendszer a Windows 10 rendszerű számítógépekre beállított házirendeket alkalmazza. További információt a Windows- [eszközök beállítása a Microsoft 365-felhasználók](set-up-windows-devices.md)számára című témakörben talál.

## <a name="step-4-install-microsoft-365-apps-for-business"></a>4. lépés: a Microsoft 365-alkalmazások vállalati verzió telepítése
- A [beállítási varázsló](set-up.md#deploy-office-365-client-apps)segítségével automatikusan telepítheti az Office-t a Windows-eszközökön.
- Az [Office-alkalmazások telepítése](https://docs.microsoft.com/office365/admin/setup/install-applications) Windows rendszerre és eszközökre
     
## <a name="advanced"></a>Speciális
- **Új eszközök beállítása az Autopilot használatával**
            
     A [Windows Autopilot](add-autopilot-devices-and-profile.md) segítségével automatikusan megadhatja az **új** Windows 10-es eszközöket a felhasználóknak, de egyszerűbb lehet egy olyan [partner](https://www.microsoft.com/solution-providers/search) beszerzése, aki ezt elvégezheti. A [Microsoft áruházat](https://go.microsoft.com/fwlink/?linkid=874598)is elérheti, és megkérheti a felhőalapú technológiai szakértőt, hogy állítsa be a megvásárolt új eszközöket.

- **Hozzáférés helyszíni erőforrásokhoz**

     - Ha a szervezete a Windows Server Active Directoryt használja helyszíniként, beállíthatja a Microsoft 365 vállalati prémium verziót a Windows 10-es eszközök védelmére, miközben továbbra is megőrizheti a helyi hitelesítéshez szükséges helyszíni erőforrásokhoz való hozzáférést. Kövesse a [tartományhoz csatlakoztatott Windows 10-es eszközök kezelésének engedélyezése a Microsoft 365 vállalati prémium](manage-windows-devices.md) verzióban című témakör lépéseit. Ez a preferált módszer, és az ebben az állapotban lévő eszközök neve hibrid Azure AD összekapcsolt eszközök.

    - Ha a vállalkozása rendelkezik helyi Active Directory-címtárral, amely egy helyszíni erőforrásokat (például fájlmegosztás és nyomtató) tartalmaz, az alábbi lépésekkel érheti el az Azure AD-csatlakozású eszközök elérését az alábbi lépésekkel: a [helyszíni erőforrások elérése a Microsoft 365 Business Premium rendszer Azure ad-eszközéről](access-resources.md).

## <a name="see-also"></a>Lásd még

[Microsoft 365 vállalati verziós képzési videók](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)

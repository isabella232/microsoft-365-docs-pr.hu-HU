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
description: Ismerje meg a Microsoft 365 Vállalati prémium verzió beállítási lépéseit, az előfizetéstől az előfizetésen át a tartományok és felhasználók hozzáadásán át a biztonsági házirendek beállításán át a biztonsági házirendek beállításához stb.
ms.openlocfilehash: 9d92aefb3b5666bb7c2fd2e13c9a00f074f107a7
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912490"
---
# <a name="overview-of-setup"></a>A beállítás áttekintése

Tekintsen meg egy rövid videót a Microsoft 365 Vállalati prémium verzió beállításról.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Ha hasznosnak találta ezt a videót, tekintse meg a [teljes tanfolyamok kisvállalatoknak és Microsoft 365-újoncoknak](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) című cikket.

A beállítási lépések nagy része az irányított telepítés során megjelenik, de a többi lehetőség is szerepel a listában.

## <a name="step-1-add-your-domain-and-users"></a>1. lépés: A tartomány és a felhasználók hozzáadása

   - **[Tartomány hozzáadása](set-up.md#add-your-domain-to-personalize-sign-in)** (ha a regisztráció során megvásárolta a tartományt, [](sign-up.md)ez a lépés már megtörtént.)

   - **Felhasználók hozzáadása gombra.** A felhasználókat a következő három módszer bármelyikében felveheti:
        - Az irányított [beállításban](set-up.md#add-users-in-the-wizard).
        - Ha helyszíni Active Directoryval rendelkezik, a címtár-szinkronizálással felhasználókat adhat hozzá az [Azure AD Connect](../enterprise/set-up-directory-synchronization.md) használatával.
        - A felhasználókat [később is hozzáadhatja a](../admin/add-users/add-users.md) Felügyeleti központban.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>2. lépés: Biztonsági házirendek beállítása és eszközök beállítása 

  - Az eszköz [házirendek konfigurálása az](set-up.md#protect-your-organization) interaktív beállítással. 
  - További funkciókat is felvehet vagy szerkeszthet később a felügyeleti [központban](view-policies-and-devices.md) és az [Intune portálon.](/intune/tutorial-walkthrough-intune-portal)
  - A beállítási varázsló alapszintű veszélyforrás-védelmi és adatveszteség-megelőzési beállításokat is beállít.
  
  A beállítási varázsló biztonsági beállításain kívül az alábbi beállítások megadásával növelheti a biztonságot:

- **Kártevők elleni védelem az e-mailekben**
- **Adathalászat elleni védelem az Office 365 Defenderben**
- **Exchange Online Archiválás**
- **Azure Information Protection (1. csomag)**

Első lépések: A veszélyforrások [elleni védelem](increase-threat-protection.md) növelése és megfelelőségi [funkciók beállítása.](set-up-compliance.md)

A 10 legjobb módszer a [Microsoft 365 Vállalati prémium](/office365/admin/security-and-compliance/secure-your-business-data) verzió biztonságának biztonságára vonatkozó gyakorlati tanácsokért tekintse meg az utcatérképet.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>3. lépés: Windows 10-es eszközök beállítása és kezelése

Az irányított beállítás befejezése után meg kell védenie a szervezet összes Windows 10-es számítógépét.
  
- A Windows 10 Pro előfeltétele [a](pre-requisites-for-data-protection.md) Microsoft 365 Business Premium terméknek, ha azonban Windows 7 Pro, Windows 8 Pro vagy Windows 8.1 Pro rendszerrel rendelkezik, előfizetése feljogosítja a Windows 10 Pro verzióra [való frissítésre.](./upgrade-to-windows-pro-creators-update.md)
- Kövesse a [biztonságos Windows 10-es PC-k](secure-win-10-pcs.md) lépéseit a Windows 10-es eszközökhöz beállított házirendek beállításához.

Amikor egy Windows 10-es eszközhöz csatlakozik az Azure AD-hez, a Windows 10-es számítógépeken beállított házirendek érvényesek rá. További információt a Windows-eszközök beállítása [a Microsoft 365 felhasználóinak.](set-up-windows-devices.md)

## <a name="step-4-install-microsoft-365-apps-for-business"></a>4. lépés: A Microsoft 365 Vállalati verziós alkalmazások telepítése
- Az Office-t automatikusan telepítheti a Windows-eszközökre a [beállítási varázslóval.](set-up.md#deploy-office-365-client-apps)
- A felhasználók [telepíthetinek Office-appokat](/office365/admin/setup/install-applications) Windowsra és eszközökre.
     
## <a name="advanced"></a>Speciális
- **Új eszközök beállítása az Autopilottal**
            
     A [Windows Autopilottal](add-autopilot-devices-and-profile.md) automatikusan előre konfigurálhatja az új **Windows** 10-es eszközöket [](https://www.microsoft.com/solution-providers/search) a felhasználóknak, de egyszerűbb lehet egy partnert kihozni, aki ezt meg tudja tenni Önért. A Microsoft [Store](https://go.microsoft.com/fwlink/?linkid=874598)áruházban meg is kérhet egy felhőtechnológia-szakértőt, hogy állítsa be a megvásárolt új eszközöket.

- **Helyszíni erőforrások elérése**

     - Ha szervezete helyszíni Windows Server Active Directoryt használ, beállíthatja a Microsoft 365 Business Premiumt a Windows 10-es eszközök védelme érdekében úgy, hogy közben továbbra is hozzáférjen a helyi hitelesítést igénylő helyszíni erőforrásokhoz. A beállítás beállításához kövesse A tartományhoz csatlakozott [Windows 10-es eszközök microsoft 365 Vállalati prémium](manage-windows-devices.md) verzió által történő kezelése. Ez az előnyben részesített módszer, az ebben az állapotban használt eszközök pedig hibrid Azure AD-hez csatlakozott eszközök.

    - Ha vállalata helyi Active Directory-címtárral rendelkezik, amely helyszíni erőforrásokat (például fájlmegosztásokat és nyomtatókat) tartalmaz, az alábbi lépéseket követve hozzáférést adhat Azure AD-hez eszközének ezekhez az erőforrásokhoz: Hozzáférés helyszíni erőforrásokhoz egy Azure AD-hez csatlakozott eszközről a [Microsoft 365 Vállalati prémium verzióban.](access-resources.md)

## <a name="see-also"></a>Lásd még

[Microsoft 365 Vállalati verzió – oktatóvideók](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
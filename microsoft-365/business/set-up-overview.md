---
title: A beállítás áttekintése
f1.keywords:
- NOCSH
ms.author: kwekua
author: kwekua
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
description: Megtudhatja, hogy hogyan Microsoft 365 Vállalati prémium verzió, az előfizetéstől a tartományok és felhasználók felvételén át a biztonsági házirendek beállításán át a biztonsági házirendek beállításához.
ms.openlocfilehash: 008a5c51698589667acc0d01649f67dab33b4c58
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52245064"
---
# <a name="overview-of-setup"></a>A beállítás áttekintése

Tekintsen meg egy rövid videót a Microsoft 365 Vállalati prémium verzió beállításról.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Ha hasznosnak találta ezt a videót, tekintse meg a [teljes tanfolyamok kisvállalatoknak és Microsoft 365-újoncoknak](../business-video/index.yml) című cikket.

A beállítási lépések nagy része az irányított telepítés során megjelenik, de a többi lehetőség is szerepel a listában.

## <a name="step-1-add-your-domain-and-users"></a>1. lépés: A tartomány és a felhasználók hozzáadása

   - **[Tartomány hozzáadása](set-up.md#add-your-domain-to-personalize-sign-in)** (ha a regisztráció során megvásárolta a tartományt, [](sign-up.md)ez a lépés már megtörtént.)

   - **Felhasználók hozzáadása gombra.** A felhasználókat a következő három módszer bármelyikében felveheti:
        - Az irányított [beállításban](set-up.md#add-users-in-the-wizard).
        - A címtár-szinkronizálással felhasználókat adhat hozzá az [Azure AD](../enterprise/set-up-directory-synchronization.md) Csatlakozás használatával, ha helyszíni Active Directoryval rendelkezik.
        - A felhasználókat [később is hozzáadhatja a](../admin/add-users/add-users.md) Felügyeleti központban.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>2. lépés: Biztonsági házirendek beállítása és eszközök beállítása 

  - Az eszköz [házirendek konfigurálása az](set-up.md#protect-your-organization) interaktív beállítással. 
  - További funkciókat is felvehet vagy szerkeszthet később a felügyeleti [központban](view-policies-and-devices.md) és az [Intune portálon.](/intune/tutorial-walkthrough-intune-portal)
  - A beállítási varázsló alapszintű veszélyforrás-védelmi és adatveszteség-megelőzési beállításokat is beállít.
  
  A beállítási varázsló biztonsági beállításain kívül az alábbi beállítások megadásával növelheti a biztonságot:

- **Kártevők elleni védelem az e-mailekben**
- **Adathalászat elleni védelem a Defender Office 365**
- **Exchange Online Archiválás**
- **Azure Information Protection (1. csomag)**

Első lépések: A veszélyforrások [elleni védelem](increase-threat-protection.md) növelése és megfelelőségi [funkciók beállítása.](set-up-compliance.md)

Az ajánlott biztonsági eljárásokról a [10](/office365/admin/security-and-compliance/secure-your-business-data) legjobb Microsoft 365 Vállalati prémium verzió kínálunk.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>3. lépés: A mobileszközök Windows 10 kezelése

Az irányított beállítás befejezése után meg kell védenie a Windows 10 összes számítógépét.
  
- Windows 10 Pro a Microsoft 365 Vállalati prémium verzió [](pre-requisites-for-data-protection.md) előfeltétele, de ha Windows 7 Pro, Windows 8 Pro vagy Windows 8.1 Pro verzióval rendelkezik, előfizetése feljogosítja a Windows 10 Pro. [](./upgrade-to-windows-pro-creators-update.md)
- A pc-k biztonságos Windows 10 [a](secure-win-10-pcs.md) házirendek beállításához Windows 10 eszközökre.

Amikor egy Windows 10 eszközhöz csatlakozik az Azure AD-hez, a számítógéphez Windows 10 házirendeket alkalmazza a rendszer. További információt A mobileszközök beállítása [Windows felhasználóknak Microsoft 365.](set-up-windows-devices.md)

## <a name="step-4-install-microsoft-365-apps-for-business"></a>4. lépés: A Üzleti Microsoft 365-alkalmazások
- A telepítővarázsló Office automatikusan telepítheti Windows eszközén. [](set-up.md#deploy-office-365-client-apps)
- A felhasználók [telepíthet Office appokat](/office365/admin/setup/install-applications) a Windows eszközökhöz.
     
## <a name="advanced"></a>Speciális
- **Új eszközök beállítása az Autopilottal**
            
     A Windows [Autopilottal](add-autopilot-devices-and-profile.md) automatikusan előre konfigurálhatja  az új Windows 10-eszközöket a felhasználók számára, de [](https://www.microsoft.com/solution-providers/search) egyszerűbb, ha egy olyan partnert szerez be, aki ezt meg tudja tenni Önért. Azt is beállíthatja, hogy [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), és kérje meg egy felhőtechnológiát szakértőt, hogy állítsa be a megvásárolt új eszközöket.

- **Helyszíni erőforrások elérése**

     - Ha szervezete helyszíni Windows Server Active Directoryt használ, beállíthatja a Microsoft 365 Vállalati prémium verzió-t az Windows 10-eszközök védelmére, miközben továbbra is hozzáfér a helyi hitelesítést igénylő helyszíni erőforrásokhoz. A beállításhoz kövesse A tartományhoz Windows 10 eszközök felhasználói [Microsoft 365 Vállalati prémium verzió](manage-windows-devices.md) beállításának lépéseit. Ez az előnyben részesített módszer, az ebben az állapotban használt eszközök pedig hibrid Azure AD-hez csatlakozott eszközök.

    - Ha vállalata rendelkezik olyan helyi Active Directory-címtárral, amely helyszíni erőforrásokat (például fájlmegosztásokat és nyomtatókat) tartalmaz, az alábbi lépéseket követve hozzáférést adhat Azure AD-hez eszközének az erőforrásokhoz: Hozzáférés helyszíni erőforrásokhoz [egy Azure AD-hez](access-resources.md)csatlakozott eszközről a Microsoft 365 Vállalati prémium verzió-ban.

## <a name="related-content"></a>Kapcsolódó tartalom

[Microsoft 365 vállalati verziós oktatóvideók](../business-video/index.yml) (hivatkozáslap)
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
description: Ismerje meg a Microsoft 365 Vállalati prémium verzió beállítási lépéseit, az előfizetéstől, a tartományok és felhasználók hozzáadásától a biztonsági házirendek beállításán át stb.
ms.openlocfilehash: 46370166a9d5e8c9308b8947513e631c159f0b86
ms.sourcegitcommit: 815229e39a0f905d9f06717f00dc82e2a028fa7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48842130"
---
# <a name="overview-of-setup"></a>A beállítás áttekintése

Nézze meg a Microsoft 365 Vállalati prémium verzió beállítását bemutató rövid videót.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Ha hasznosnak találta ezt a videót, tekintse meg a [teljes tanfolyamok kisvállalatoknak és Microsoft 365-újoncoknak](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) című cikket.

A beállítási lépések nagy része az irányított beállításban is el lehet végezve, de a többi beállítás is szerepel a listában.

## <a name="step-1-add-your-domain-and-users"></a>1. lépés: A tartomány és a felhasználók hozzáadása

   - **[Tartomány hozzáadása](set-up.md#add-your-domain-to-personalize-sign-in)** (ha a regisztráció során vásárolta meg a tartományt, [](sign-up.md)ez a lépés már megtörtént.)

   - **Felhasználók hozzáadása** A felhasználókat a következő három módon adhat hozzá:
        - Az interaktív [beállításban.](set-up.md#add-users-in-the-wizard)
        - Ha helyszíni Active Directoryval rendelkezik, akkor címtár-szinkronizálással adhat hozzá felhasználókat az [Azure AD Connect](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) használatával.
        - A felügyeleti [központban később is](add-users-m365b.md) felvehet felhasználókat.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>2. lépés: Biztonsági házirendek és eszközök beállítása 

  - Az interaktív [beállítással konfigurálhatja](set-up.md#protect-your-organization) az eszköz-házirendeket. 
  - A felügyeleti központban és az [](view-policies-and-devices.md) Intune portálon is felvehet további funkciókat, illetve szerkesztheti [őket.](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)
  - A beállítási varázsló a veszélyforrások elleni védelem és az adatveszteség-megelőzés alapvető beállításait is be fogja állítani.
  
  A beállítási varázsló biztonsági beállításain kívül az alábbi beállítások felvételével növelheti a biztonságot:

- **E-mail kártevők elleni védelem**
- **Adathalászat elleni védelem az Office 365- ös Defenderben**
- **Exchange Online Archiválás**
- **Azure Information Protection (1. csomag)**

Első lépések a veszélyforrások [elleni védelem](increase-threat-protection.md) növelése és a megfelelőségi [funkciók beállítása.](set-up-compliance.md)

A [microsoftos 365 Vállalati prémium](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) verzió biztonságossá 10 legjobb módjait is bevetve útitérképet láthat az ajánlott biztonsági eljárásokról.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>3. lépés: Windows 10-es eszközök beállítása és kezelése

Az irányított beállítás befejezése után meg kell védenie a szervezet összes Windows 10-es számítógépét.
  
- A Windows 10 [](pre-requisites-for-data-protection.md) Pro a Microsoft 365 Vállalati prémium verzió előfeltétele, ha azonban Windows 7 Pro, Windows 8 Pro vagy Windows 8.1 Pro rendszert rendelkezik, előfizetése feljogosítja a [Windows 10 Pro frissítésre.](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update)
- A Windows [10-es](secure-win-10-pcs.md) eszközökre vonatkozó házirendek beállításához kövesse a Biztonságos Windows 10-es PC-k lépéseit.

Amikor egy Windows 10-es eszközhöz csatlakozik az Azure AD-hez, a Windows 10-es számítógépekhez beállított házirendek vonatkoznak rá. További információt a [Windows-eszközök beállítása a Microsoft 365 felhasználóinak.](set-up-windows-devices.md)

## <a name="step-4-install-microsoft-365-apps-for-business"></a>4. lépés: A Microsoft 365 Vállalati verziós alkalmazások telepítése
- A beállítási varázslóval automatikusan telepítheti az Office-t a [Windows-eszközökre.](set-up.md#deploy-office-365-client-apps)
- A felhasználók [telepíthetik a Windowsra](https://docs.microsoft.com/office365/admin/setup/install-applications) és az eszközökre telepített Office-alkalmazásokat.
     
## <a name="advanced"></a>Speciális
- **Új eszközök beállítása az Autopilottal**
            
     A [Windows Autopilottal](add-autopilot-devices-and-profile.md) automatikusan előre konfigurálhatja az új **Windows** 10-es eszközöket [](https://www.microsoft.com/solution-providers/search) a felhasználóknak, de egyszerűbb lehet egy olyan partnert szerezni, aki ezt meg tudja tenni Önért. A Microsoft [Store-ban](https://go.microsoft.com/fwlink/?linkid=874598)is megkérhet egy felhőalapú technológiai szakértőt, hogy állítsa be a megvásárolt új eszközöket.

- **Helyszíni erőforrások elérése**

     - Ha szervezete helyszíni Windows Server Active Directoryt használ, beállíthatja a Microsoft 365 Vállalati prémium verzióban a Windows 10-es eszközök védelmét, miközben továbbra is hozzáférhet a helyi hitelesítést igénylő helyszíni erőforrásokhoz. A beállítás beállításához kövesse az [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) (Tartományhoz csatlakozott Windows 10-es eszközök engedélyezése) beállítás lépéseit. Ez az előnyben részesített módszer, és az ebben az állapotban használt eszközöket hibrid Azure AD-hez csatlakozott eszközöknek nevezzük.

    - Ha vállalata rendelkezik helyi Active Directory-címtárral, amely helyszíni erőforrásokat (például fájlmegosztásokat és nyomtatókat) tartalmaz, az alábbi lépéseket követve hozzáférést adhat az Azure AD-hez csatlakozott eszközöknek: A [Microsoft 365](access-resources.md)Vállalati prémium verzió Azure AD-hez csatlakozott eszközén helyszíni erőforrásokhoz férhet hozzá.

## <a name="see-also"></a>Lásd még

[Microsoft 365 Vállalati verziós oktatóvideók](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)

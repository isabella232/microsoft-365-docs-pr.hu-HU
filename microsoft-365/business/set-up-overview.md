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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Ismerje meg a Microsoft 365 Business beállítási lépéseit, az előfizetéstől kezdve a tartomány és a felhasználók hozzáadásán át a biztonsági házirendek beállításáig stb.
ms.openlocfilehash: 4c9c3ee4c45625cebe5d19eb03fcb6d90eb9243e
ms.sourcegitcommit: ab916c216053999c9c4ef4838217e82cd861f23f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2020
ms.locfileid: "42415565"
---
# <a name="overview-of-setup"></a>A beállítás áttekintése

Nézzen meg egy rövid videót a Microsoft 365 Vállalati verzió beállításáról.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Ha hasznosnak találta ezt a videót, tekintse meg a [teljes tanfolyamok kisvállalatoknak és Microsoft 365-újoncoknak](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) című témakört.

A beállítási lépések többsége elvégezhető a telepítővarázslóban, de a többi beállítás is megjelenik a listában.

## <a name="step-1-add-your-domain-and-users"></a>1. lépés: Tartomány és felhasználók hozzáadása

   - **[Adja hozzá a tartományt](set-up.md#add-your-domain-to-personalize-sign-in)** (ha [a regisztráció](sign-up.md)során vásárolta meg a tartományt, ez a lépés már megtörtént.)

    - **Felhasználók hozzáadása**. A felhasználókat a következő három módszer közül választhatja ki:
        - A [varázslóban.](set-up.md#add-users-in-the-wizard)
        - A címtár-szinkronizálás használatával [felhasználókat vehet fel az Azure AD Connect használatával,](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) ha helyszíni Active directoryval rendelkezik.
        - [Később is hozzáadhat felhasználókat](add-users-m365b.md) a felügyeleti központban.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>2. lépés: Biztonsági házirendek beállítása és eszközök konfigurálása 

  - Az eszközházirendek konfigurálása a [Telepítő varázslóval.](set-up.md#protect-your-organization) 
  - Később további vagy szerkesztheti őket a [felügyeleti központban](view-policies-and-devices.md) és az [Intune-portálon.](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)
  - A telepítővarázsló beállítja az alapvető veszélyforrások elleni védelem és az adatvesztés-megelőzési beállításokat is.
  
  A telepítővarázsló biztonsági beállításai mellett a következő beállítások hozzáadásával növelheti a biztonságot:

- **Rosszindulatú programok elleni védelem e-mailben**
- **ATP adathalászat elleni**
- **Exchange Online Archiválás**
- **Azure Information Protection (1. terv**)

Első lépésekhez olvassa el a [fenyegetésvédelem növelése](increase-threat-protection.md) és [a megfelelőségi funkciók beállítása](set-up-compliance.md)című témakört.

Tekintse meg a [Microsoft 365 Business 10 legfontosabb módját](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) a legjobb biztonsági eljárások ütemtervéhez.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>3. lépés: Windows 10-es eszközök beállítása és kezelése

A beállítási varázsló futtatása után érdemes ellátni a szervezet összes Windwos 10 számítógépét.
  
- A Windows 10 Pro a Microsoft 365 Business [előfeltétele,](pre-requisites-for-data-protection.md) de ha Windows 7 Pro, Windows 8 Pro vagy Windows 8.1 Pro rendszert használ, az előfizetés feljogosítja Önt a [Windows 10 Pro rendszerre való frissítésre.](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update)
- A Windows [10 rendszerű számítógépek biztonságos](secure-win-10-pcs.md) védelmében a Windows 10-es eszközökre vonatkozó házirendek beállításához kövesse a lépéseket.

Amikor windows 10-es eszközt csatlakoztat az Azure AD-hez, a Windows 10-es számítógépekre beállított szabályzatok vonatkoznak rá. További információt [a Windows-eszközök beállítása a Microsoft 365 Vállalati verzió felhasználói számára](set-up-windows-devices.md)című témakörben talál.

## <a name="step-4-install-office-365-business"></a>4. lépés: Az Office 365 Vállalati verzió telepítése
- Az Office automatikusan telepíthető a Windows-eszközökre a [telepítővarázsló segítségével.](set-up.md#deploy-office-365-client-apps)
- Lehetővé teszi a felhasználók számára a Windows-alapú [Office-alkalmazások](https://docs.microsoft.com/office365/admin/setup/install-applications) és -eszközök telepítését.
     
## <a name="advanced"></a>Speciális
- **Új eszközök beállítása az Autopilot segítségével**
            
     A [Windows Autopilot](add-autopilot-devices-and-profile.md) segítségével automatikusan előre konfigurálhatja az **új** Windows 10-es eszközöket a felhasználó számára, de egyszerűbb lehet olyan [partnert](https://www.microsoft.com/solution-providers/search) szerezni, aki ezt megteheti Ön számára. A [Microsoft Store-ban](https://go.microsoft.com/fwlink/?linkid=874598)is megkérhet egy felhőtechnológiai szakértőt, hogy állítson be új, megvásárolt eszközöket.

- **Helyszíni erőforrások elérése**

     - Ha szervezete a helyszínen használja a Windows Server Active Directoryt, beállíthatja a Microsoft 365 Business alkalmazást a Windows 10-es eszközök védelmére, miközben továbbra is hozzáférhet a helyi hitelesítést igénylő helyszíni erőforrásokhoz. Kövesse a [Microsoft 365 Business által felügyelt tartományhoz csatlakozó Windows 10-eszközök engedélyezése](manage-windows-devices.md) című részt. Ez az előnyben részesített módszer, és az ebben az állapotban lévő eszközöket hibrid Azure AD-csatlakozású eszközöknek nevezzük.

    - Ha a vállalkozás a helyi Active Directory, amely tartalmaz néhány helyszíni erőforrások (például a fájlmegosztások és nyomtatók), adhat az Azure AD-csatlakozású eszközök hozzáférését ezekhez az erőforrásokhoz az alábbi lépéseket: Hozzáférés a helyszíni erőforrások egy [Azure AD-csatlakozású eszköz a Microsoft 365 Business.](access-resources.md)

## <a name="see-also"></a>Lásd még

[Microsoft 365 Vállalati verziós oktatóvideók](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)

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
description: Ismerje meg a Microsoft 365 Business Premium beállítási lépéseit, az előfizetéstől a tartomány és felhasználók hozzáadásáig, a biztonsági házirendek beállításáig és egyebekig.
ms.openlocfilehash: 80243fac6ca2efcfca030b6ee1c1113c026a80ce
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44402978"
---
# <a name="overview-of-setup"></a>A beállítás áttekintése

Tekintse meg a Microsoft 365 Business Premium beállításáról szóló rövid videót.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Ha hasznosnak találta ezt a videót, tekintse meg a [teljes tanfolyamok kisvállalatoknak és Microsoft 365-újoncoknak](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) című cikket.

A beállítási lépések többsége elvégezhető a telepítővarázslóban, de a többi lehetőség is szerepel a listában.

## <a name="step-1-add-your-domain-and-users"></a>1. lépés: Tartomány és felhasználók hozzáadása

   - **[Adja hozzá a tartományt](set-up.md#add-your-domain-to-personalize-sign-in)** (ha a regisztráció során vásárolta meg a [tartományt,](sign-up.md)ez a lépés már megtörtént.)

    - **Felhasználók hozzáadása**. A felhasználókat a következő három módon veheti fel:
        - A [varázslóban.](set-up.md#add-users-in-the-wizard)
        - A címtár-szinkronizálás használatával [felhasználókat adhat hozzá az Azure AD Connect használatával,](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) ha rendelkezik egy helyszíni Active directory használatával.
        - Később a felügyeleti központban is [hozzáadhat felhasználókat.](add-users-m365b.md)
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>2. lépés: Biztonsági házirendek beállítása és eszközök konfigurálása 

  - Az eszközházirendek konfigurálásához használja a [Telepítő varázslót.](set-up.md#protect-your-organization) 
  - A [felügyeleti központban](view-policies-and-devices.md) és az [Intune-portálon](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)később is hozzáadhat vagy szerkesztheti őket.
  - A telepítővarázsló alapszintű veszélyforrások elleni védelmet és adatveszteség-megelőzési beállításokat is beállít.
  
  A beállítási varázsló biztonsági beállításai mellett a következő beállítások hozzáadásával növelheti a biztonságot:

- **E-mail malware védelem**
- **ATP adathalászat elleni**
- **Exchange Online Archiválás**
- **Azure Information Protection (1. terv)**

Első lépésekhez olvassa el a [veszélyforrások elleni védelem növelése](increase-threat-protection.md) és a megfelelőségi funkciók beállítása című [témakört.](set-up-compliance.md)

A legjobb biztonsági gyakorlatok megvalósítását a [Microsoft 365 Business Premium szolgáltatás védelmének első 10 témakörében](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) is megtekintheti.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>3. lépés: Windows 10-es eszközök beállítása és kezelése

A beállítási varázsló futtatása után a szervezet összes Windwos 10 számítógépét meg kell vásárolnia.
  
- A Windows 10 Pro a Microsoft 365 Business Premium [előfeltétele,](pre-requisites-for-data-protection.md) de ha Windows 7 Pro, Windows 8 Pro vagy Windows 8.1 Pro rendszerrel rendelkezik, előfizetése feljogosítja Önt a [Windows 10 Pro frissítésére.](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update)
- Kövesse a [windows 10-es számítógépek biztonságos](secure-win-10-pcs.md) beállításának lépéseit a Windows 10-es eszközökházirendjeinek beállításához.

Amikor csatlakozik egy Windows 10-es eszközhöz az Azure AD-hez, a Windows 10-es számítógépekhez beállított házirendek lesznek alkalmazva. További információt a [Windows-eszközök beállítása Microsoft 365-felhasználók számára](set-up-windows-devices.md)című témakörben talál.

## <a name="step-4-install-microsoft-365-apps-for-business"></a>4. lépés: Microsoft 365 vállalati alkalmazások telepítése
- A [telepítővarázslóval](set-up.md#deploy-office-365-client-apps)automatikusan telepítheti az Office-t a Windows-eszközökre.
- A felhasználók telepíthetik a Windows és az eszközök [Office-alkalmazásait.](https://docs.microsoft.com/office365/admin/setup/install-applications)
     
## <a name="advanced"></a>Speciális
- **Új eszközök beállítása az Autopilot segítségével**
            
     A [Windows Autopilot](add-autopilot-devices-and-profile.md) segítségével automatikusan előre konfigurálhatja az **új** Windows 10-es eszközöket egy felhasználó számára, de egyszerűbb lehet olyan [partnert](https://www.microsoft.com/solution-providers/search) szerezni, aki ezt megteheti Ön számára. A [Microsoft Store-ban](https://go.microsoft.com/fwlink/?linkid=874598)is megnyithatja a Microsoft Store-t, és megkérhet egy felhőtechnológiai szakértőt, hogy állítson be új eszközöket.

- **Helyszíni erőforrások elérése**

     - Ha a szervezet a helyszíni Windows Server Active Directoryt használja, beállíthatja a Microsoft 365 Business Premium rendszert a Windows 10-es eszközök védelmére, miközben továbbra is hozzáférhet a helyi hitelesítést igénylő helyszíni erőforrásokhoz. A beállításhoz kövesse a [Tartományhoz csatlakozó Windows 10-eszközök Microsoft 365 Business Premium által idomainak engedélyezéséhez](manage-windows-devices.md) szükséges lépéseket. Ez az előnyben részesített módszer, és az ilyen állapotban lévő eszközöket hibrid Azure AD-hez csatlakozó eszközöknek nevezzük.

    - Ha a vállalkozás rendelkezik egy helyi Active Directoryval, amely néhány helyszíni erőforrást (például fájlmegosztásokat és nyomtatókat) tartalmaz, az Azure AD-hez csatlakoztatt eszközöknek hozzáférést adhat ezekhez az erőforrásokhoz az alábbi lépések végrehajtásával: [Helyszíni erőforrások elérése a Microsoft 365 Business Premium szolgáltatásban egy Azure AD-hez csatlakozott eszközről.](access-resources.md)

## <a name="see-also"></a>Lásd még

[Microsoft 365 üzleti oktatóvideók](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)

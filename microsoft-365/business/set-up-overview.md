---
title: A beállítás áttekintése
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
description: A Microsoft 365 Business telepítési lépéseinek áttekintése.
ms.openlocfilehash: 4aca617015cceb85ca35c8d8ada7b83d1416d959
ms.sourcegitcommit: 178ecb21cacdeaf440f3df2fe6e539e9127fcf15
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/23/2019
ms.locfileid: "40850804"
---
# <a name="overview-of-setup"></a>A beállítás áttekintése

Nézzen meg egy rövid videót a Microsoft 365 Business beállításról.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Ha Ön alapít ez video segíteni kész, kijelenti magát a [kiegészít képzés sor részére kicsi teendő és azok új-hoz mikroszkóp 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

A telepítési lépések többsége elvégezhető a telepítővarázslóban, de a többi beállítás is listázható.

## <a name="step-1-add-your-domain-and-users"></a>1. lépés: a tartomány és a felhasználók hozzáadása

   - **[Add hozzá a domain](set-up.md#add-your-domain-to-personalize-sign-in)** (ha vásárolta a domain [regisztráció](sign-up.md)során, ez a lépés már megtörtént.)

    - **Hozzáadhatnak felhasználókat**. A felhasználókat háromféle módon adhatja hozzá a felhasználókhoz:
        - A [varázslóban](set-up.md#add-users-in-the-wizard).
        - Ha intézményi Active Directory címtárral rendelkezik, a címtár-szinkronizálás segítségével [felhasználókat adhat hozzá az azúrkék ad Connect alkalmazással](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) .
        - Később az admin központban is [hozzáadhat felhasználókat](add-users-m365b.md) .
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>2. lépés: biztonsági házirendek beállítása és eszközök konfigurálása 

  - Az eszközházirendek konfigurálásához használja a [telepítővarázslót](set-up.md#protect-your-organization) . 
  - Később az [Admin központban](view-policies-and-devices.md) és az [Intune portálon](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)is hozzáadhat további, vagy szerkesztheti azokat.
  - A telepítő varázsló emellett alapvető fenyegetettséget és adatvesztés-megelőzési beállításokat is beállít.
  
  A Beállításvarázsló biztonsági beállításai mellett a következő beállítások hozzáadásával növelheti biztonságát:

- **E-mail malware-védelem**
- **ATP anti-phishing**
- **Exchange Online Archiválás**
- **Azure információvédelem (Plan1**)

A kezdéshez tekintse [meg a speciális biztonsági házirendek beállítása](set-up-advanced-security.md)című témakört.

Lásd még a [10 legjobb módja a Microsoft 365 Business biztonságának](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) a legjobb biztonsági gyakorlatok útitervében való biztonságossá tétele érdekében.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>3. lépés: a Windows 10-eszközök beállítása és kezelése

A varázsló futtatása után a szervezet összes Windwos 10 számítógépét be szeretné szerezni.
  
- Windows 10 Profi van egy [előfeltétel](pre-requisites-for-data-protection.md) részére Mikroszkóp 365 teendő, de ha önnek van Windows 7 profi, Windows 8 profi, vagy Windows 8,1 Profi,-a aláírás feljogosítja ön-hoz egy [feljavít-hoz Windows 10 profi](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
- Kövesse a [Windows 10 PC](secure-win-10-pcs.md) -k biztonságának lépéseit a Windows 10 eszközök házirendjeinek beállításához.

Amikor csatlakozunk egy Windows 10 készüléket Azure AD-hez, a Windows 10 számítógépeire beállított házirendek kerülnek alkalmazásra. További információ: a [Windows-eszközök beállítása a Microsoft 365 üzleti felhasználók](set-up-windows-devices.md)számára.

## <a name="step-4-install-office-365-business"></a>4. lépés: telepítse az Office 365 Business
- Az Office-eszközöket a [telepítővarázslóval](set-up.md#deploy-office-365-client-apps)automatikusan is telepítheti a Windows-eszközökön.
- A felhasználók [telepíthetik az Office-alkalmazásokat](https://docs.microsoft.com/office365/admin/setup/install-applications) a Windows és az eszközök számára.
     
## <a name="advanced"></a>Speciális
- **A robotpilóta használata új eszközök beállításához**
            
     A [Windows automatikus vezérlőt](add-autopilot-devices-and-profile.md) használhatja a felhasználó számára az **új** Windows 10 eszköz automatikus konfigurálására, de egyszerűbb lehet olyan [partnert](https://www.microsoft.com/solution-providers/search) kérni, aki ezt megteheti. Tudod is megy [Mikroszkóp készlet](https://go.microsoft.com/fwlink/?linkid=874598), és kérdez egy felhő technológia szakértő-hoz felállít új berendezés amit ön megvásárol.

- **Az intézményi erőforrások elérése**

     - Ha a szervezet helyi Windows Server Active Directoryt használ, beállíthatja a Microsoft 365 Business rendszert, hogy védje a Windows 10 eszközeit, miközben továbbra is fenntartja az intézményi erőforrásokhoz való hozzáférést, amelyekhez szükség van lokális hitelesítésre. Hajtsa végre a [Microsoft 365 Business által felügyelt, tartományhoz csatlakoztatott Windows 10 eszközök engedélyezésére](manage-windows-devices.md) vonatkozó lépéseket. Ez az előnyben részesített módszer, és az ebben az állapotban lévő eszközök elnevezése Hybrid Azure hirdetési egyesített eszközök.

    - Ha vállalkozása olyan helyi Active Directoryval rendelkezik, amely intézményi erőforrásokat (például fájlmegosztásokat és nyomtatókat) is tartalmaz, akkor az Azure-alapú AD-összekapcsolt eszközök számára hozzáférést biztosít ezekhez az erőforrásokhoz az alábbi lépések végrehajtásával: [a Microsoft 365 Business egy Azure rendszerű ad-illesztett eszközből származó intézményi erőforrások elérése](access-resources.md).

## <a name="see-also"></a>See also

[Microsoft 365 üzleti képzési videók](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)

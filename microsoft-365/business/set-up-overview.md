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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: A Microsoft 365 Business által létrehozott lépések áttekintése.
ms.openlocfilehash: 4be0a8aa1b050ee3e20a045eb2c07666765118ed
ms.sourcegitcommit: cbf117a4cd92a907115c9f10752f3c557361e586
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/10/2019
ms.locfileid: "37440537"
---
# <a name="overview-of-setup"></a>A beállítás áttekintése

A legtöbb beállítási lépés elvégezhető a telepítővarázslóban, de a többi beállítás is listázható.


## <a name="step-1-add-your-domain-and-users"></a>1. lépés: a tartomány és a felhasználók hozzáadása

   - **[Add hozzá a domain](set-up.md#add-your-domain-to-personalize-sign-in)** (ha vásárolta a domain [regisztráció](sign-up.md)során, ez a lépés már megtörtént.)

    - **Hozzáadhatnak felhasználókat**. Ezt megteheti a következő három módon:
        - A [varázslóban](set-up.md#add-users-in-the-wizard).
        - Ha intézményi Active Directory címtárral rendelkezik, a címtár-szinkronizálás segítségével [felhasználókat adhat hozzá az azúrkék ad Connect alkalmazással](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) .
        - Később az admin központban is [hozzáadhat felhasználókat](add-users-m365b.md) .
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>2. lépés: biztonsági házirendek beállítása és eszközök konfigurálása 

  - Az eszköz-és biztonsági házirendek konfigurálásához használja a [telepítővarázslót](set-up.md#protect-data-and-devices) . 
  - Később az [Admin központban](view-policies-and-devices.md) és az [Intune portálon](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)is hozzáadhat további, vagy szerkesztheti azokat.
  - A Beállításvarázsló biztonsági beállításai mellett a következő beállítások hozzáadásával növelheti biztonságát:

      - **E-mail malware-védelem**
      - **Speciális Veszélyvédelmi (ATP) hivatkozások**
      - **ATP-biztos mellékletek**
      - **ATP anti-phishing**
      - **Exchange Online Archiválás**
      - **Adatvesztés megelőzése (DLP)**
      - **Azure információvédelem (Plan1**)

          A kezdéshez tekintse [meg a speciális biztonsági házirendeket](set-up-advanced-security.md).

        Lásd még a [10 legjobb módja a Microsoft 365 Business biztonságának](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) a legjobb biztonsági gyakorlatok útitervében való biztonságossá tétele érdekében.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>3. lépés: a Windows 10-eszközök beállítása és kezelése

   Amikor csatlakozunk egy Windows 10 készüléket Azure AD-hez, a [2](#step-2-set-up-security-policies-and-configure-devices) .

   - Windows 10 Profi van egy [előtti-követelmény](pre-requisites-for-data-protection.md) részére Mikroszkóp 365 teendő, de ha önnek van Windows 7 profi, Windows 8 profi, vagy Windows 8,1 Profi,-a aláírás feljogosítja ön-hoz egy [feljavít-hoz Windows 10 profi](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
    - A Windows 10 eszközök házirendjeinek konfigurálásához használja a [telepítővarázslót](set-up.md#protect-data-and-devices) .

## <a name="stes-4-install-office-365-business"></a>Stes 4: telepítse az Office 365 Business
- Az Office-eszközöket a [telepítővarázslóval](set-up.md#deploy-office-365-client-apps)automatikusan is telepítheti a Windows-eszközökön.
- Gépiesen [felszerel hivatal](auto-install-or-uninstall-office.md) -ból admin központ.
- A felhasználók [telepíthetik az Office-alkalmazásokat](https://docs.microsoft.com/office365/admin/setup/install-applications) a Windows és az eszközök számára.
     
## <a name="advanced"></a>Speciális
- **A robotpilóta használata új eszközök beállításához**
            
     A [Windows automatikus vezérlőt](add-autopilot-devices-and-profile.md) használhatja a felhasználó számára az **új** Windows 10 eszköz automatikus konfigurálására, de egyszerűbb lehet olyan [partnert](https://www.microsoft.com/solution-providers/search) kérni, aki ezt megteheti. Ön is látogasson el a [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) , és kérje a felhő-technológiai szakértő létrehozott új eszközöket vásárol az Ön számára.

- **Az intézményi erőforrások elérése**

     - Ha a szervezet helyi Windows Server Active Directoryt használ, beállíthatja a Microsoft 365 Business rendszert, hogy védje a Windows 10 eszközeit, miközben továbbra is fenntartja az intézményi erőforrásokhoz való hozzáférést, amelyekhez szükség van lokális hitelesítésre. Hajtsa végre a [Microsoft 365 Business által felügyelt, tartományhoz csatlakoztatott Windows 10 eszközök engedélyezésére](manage-windows-devices.md) vonatkozó lépéseket. Ez az adott állapotú módszer és eszközök a hibrid Azure rendszerű hirdetési eszközök.

    - Ha vállalkozása olyan helyi Active Directoryval rendelkezik, amely intézményi erőforrásokat (például fájlmegosztásokat vagy nyomtatókat) tartalmaz, akkor az azúrkék AD-illesztett eszközök ezekhez az erőforrásokhoz való hozzáférését az alábbi lépések végrehajtásával adhatja meg: az [intézményi erőforrások elérése egy Azúrkék hirdetés-összekapcsolt berendezés-ban Mikroszkóp 365 teendő](access-resources.md).

  
---
title: Beállítása – áttekintés
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: A Microsoft 365 üzleti lépések létrehozott áttekintése.
ms.openlocfilehash: ae7ed0aab36a6e759e0f0c1fbc3d3183273a284e
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/15/2019
ms.locfileid: "35086340"
---
# <a name="overview-of-setup"></a>A telepítő áttekintése

Lépéseket beállítása a legtöbb elvégezhető a telepítő varázsló, de az egyéb beállítások is szerepelnek.


## <a name="step-1-add-your-domain-and-users"></a>1. lépés: A tartomány és a felhasználó hozzáadása

   - **[A tartomány hozzáadása](set-up.md#add-your-domain-to-personalize-sign-in)** (a domain [regisztráció](sign-up.md)során vásárolt, ha ez a lépés már megtörtént.)

    - **Felhasználók hozzáadása**. Ez a három módokon teheti meg:
        - A [varázsló](set-up.md#add-users-in-the-wizard).
        - Ha a helyszíni Active directory [Azure AD csatlakozás segítségével a felhasználók](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) hozzáadása a címtárszinkronizálás használata
        - Is [újabb felhasználók hozzáadása](add-users-m365b.md) a felügyeleti központban.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>2. lépés: Állítsa be a biztonsági házirendek és eszközök konfigurálása 

  - A [telepítő varázsló](set-up.md#set-up-security-policies-and-device-configurations) segítségével konfigurálhatja az eszköz és a biztonsági házirendek. 
  - Több hozzáadása vagy később a [felügyeleti központ](view-policies-and-devices.md) és az [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)szerkeszthetők is.
  - A telepítő varázsló a biztonsági beállítások mellett az alábbi beállítások hozzáadásával növelheti a biztonsági:

      - **E-mail rosszindulatú programok elleni védekezés**
      - **Speciális veszély védelmi (ATP) biztonságos kapcsolatok**
      - **ATP biztonságos mellékletek**
      - **ATP-adathalászat**
      - **Exchange Online Archiválás**
      - **Adatvesztés megelőzése (DLP)**
      - **Borzas információk védelméről (Plan1**)

          Get elindítani a [Speciális biztonsági házirendek beállítása](set-up-advanced-security.md)című témakörben talál.

        Lásd még: [365 a Microsoft üzleti biztonságos felső 10 mód](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) a legjobb biztonsági gyakorlatok ütemterv.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>3. lépés: Állítsa be, és a Windows 10 eszközök kezelése

   Ha eszköz Windows 10 Azure ad, a házirendek beállítása a [2](#step-2-set-up-security-policies-and-configure-devices) a rendszer alkalmazza azt.

   - Windows 10 Pro egy [előfeltételként](pre-requisites-for-data-protection.md) Microsoft 365 üzleti, de ha Windows 7 Pro, Windows 8 Pro vagy Pro Windows 8.1-, az előfizetés feljogosítja a, hogy [frissítsen a Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
    - A [telepítő varázsló](set-up.md#set-up-security-policies-and-device-configurations) segítségével konfigurálja a Windows 10 eszközök.

## <a name="stes-4-install-office-365-business"></a>Stes 4: Telepítse az Office 365 üzleti
- A [telepítő varázsló](set-up.md#deploy-office-365-client-apps)segítségével a Windows-eszközök automatikusan telepíthető Office.
- Automatikusan [az Office telepítése](auto-install-or-uninstall-office.md) az admin center.
- Lehetővé teszik a felhasználók [Office alkalmazások telepítése](https://docs.microsoft.com/office365/admin/setup/install-applications) a Windows és az eszközök.
     
## <a name="advanced"></a>Speciális
- **Automata segítségével állítsa be az új eszközök**
            
     [Windows automata](add-autopilot-devices-and-profile.md) segítségével automatikusan előre konfigurálja egy felhasználó **Új** Windows 10 eszközök, de lehet egyszerűbben, egy [partner](https://www.microsoft.com/solution-providers/search) , aki teheti meg. Ugrás a [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) is, és kérje meg a felhő technológia szakértői vásárol meg az új eszközök beállítása.

- **Helyi erőforrások eléréséhez.**

     - Ha a szervezet használja a Windows Server Active Directory helyszíni, állíthat be Microsoft 365 üzleti védelme érdekében a Windows 10 eszközök továbbra is fenntartva helyi hitelesítést igénylő helyszíni erőforrásokhoz való hozzáférést. Kövesse a [Microsoft 365 üzleti által kezelt tartományhoz tartozó Windows 10 eszközök engedélyezése](manage-windows-devices.md) meg. Ez a javasolt módszer és eszközök ebben az állapotban úgynevezett hibrid Azure AD eszközöket csatlakozott.

    - Ha a vállalatnál a helyi Active Directory, amely tartalmazza az egyes helyi erőforrásokat (például fájlmegosztásokat és nyomtatókat), a Borzas AD csatlakoztatott eszközök hozzáférést biztosíthat a forrásokhoz való lépések itt: [Access helyszíni erőforrásokat egy 365 üzleti Microsoft Azure AD csatlakozott eszköz](access-resources.md).

  
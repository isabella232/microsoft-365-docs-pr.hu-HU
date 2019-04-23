---
title: AutoPilot-profilok létrehozása és szerkesztése
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: 'Ismerje meg, hogyan létrehozása, szerkesztése, törlése vagy automata profilok eltávolítása. '
ms.openlocfilehash: 85fc897b2f428afae8d55feeb577021adaa30f72
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32277121"
---
# <a name="create-and-edit-autopilot-profiles"></a>AutoPilot-profilok létrehozása és szerkesztése

## <a name="create-a-profile"></a>Profil létrehozása

A profil egy eszközre vagy eszközök csoportjára vonatkozik.
  
1. A Microsoft 365 üzleti rendszergazdai központban válassza az **eszközök** \> **automata**.
  
2. Az **automata** lapon válassza ki **a profilt** \> **profil létrehozása**.
    
3. A **Profil létrehozása** lapon írjon be egy azonosítást segítő nevet a profilhoz, például Marketing, kapcsolja be a kívánt beállítást (további információ: [Az AutoPilot-profil beállításai](autopilot-profile-settings.md)), és válassza a **Mentés** gombot.
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a>Profil alkalmazása eszközre

A profil létrehozása után alkalmazhatja azt egy eszközre vagy eszközcsoportra. Kiválaszthat egy meglévő profilt a [részletes útmutatóban](add-autopilot-devices-and-profile.md), és alkalmazhatja azt új eszközökre, vagy lecserélheti egy eszköz vagy eszközcsoport meglévő profilját. 
  
1. **A Windows előkészítése** lapon válassza az **Eszközök** fület. 
    
2. Click the check-box next to a device name and in the **Device** panel, choose a profile from the **Assigned profile** drop-down \> **Save**.
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a>Profil szerkesztése, törlése vagy eltávolítása

Miután hozzárendelt egy profilt egy eszközhöz, frissítheti azt még akkor is, ha már odaadta az eszközt egy felhasználónak. Amikor az eszköz csatlakozik az internethez, a beállítási folyamat során letölti a profil legújabb verzióját. Ha a felhasználó visszaállítja az eszköz gyári alapértelmezett beállításait, az eszköz ismét le fogja tölteni a profil legújabb frissítéseit. 
  
### <a name="edit-a-profile"></a>Profil szerkesztése

1. **A Windows előkészítése** lapon válassza a **Profilok** fület. 
    
2. Click the check-box next to a device name and in the **Profile** panel update any of the available settings \> **Save**.
    
    Ha ezt azelőtt végzi el, hogy a felhasználó csatlakoztatná az eszközt az internetre, akkor a profilt a rendszer alkalmazza a beállítási folyamatra.
    
### <a name="delete-a-profile"></a>Profil törlése

1. **A Windows előkészítése** lapon válassza a **Profilok** fület. 
    
2. Jelölje be az egyik eszköz neve melletti jelölőnégyzetet, és a **Profil** panelen kattintson a **Profil törlése** \> **Mentés** elemre.
    
    A törléssel a profilt eltávolítja arról az eszközről vagy abból az eszközcsoportból, amelyhez hozzá volt rendelve.
    
### <a name="remove-a-profile"></a>Profil eltávolítása

1. **A Windows előkészítése** lapon válassza az **Eszközök** fület. 
    
2. Click the check-box next to a device name and in the **Device** panel, choose a **None** from the **Assigned profile** drop-down \> **Save**.
    

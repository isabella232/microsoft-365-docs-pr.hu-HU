---
title: AutoPilot-profilok létrehozása és szerkesztése
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: 'Ismerkedjen meg a robotpilóta-profilok létrehozásával, szerkesztésével, törlésével vagy eltávolításával. '
ms.openlocfilehash: 8fae8af5e7aa7b866745d0b34a4fe11862de6e9d
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "37287775"
---
# <a name="create-and-edit-autopilot-profiles"></a>AutoPilot-profilok létrehozása és szerkesztése

## <a name="create-a-profile"></a>Profil létrehozása

A profil egy eszközre vagy eszközök csoportjára vonatkozik.
  
1. -Ban Mikroszkóp 365 teendő admin központ, választ **berendezés** \> **robotpilóta**.
  
2. A **robotpilóta** oldalon válassza a profil lap **** \> **létrehozása profilt**.
    
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
    

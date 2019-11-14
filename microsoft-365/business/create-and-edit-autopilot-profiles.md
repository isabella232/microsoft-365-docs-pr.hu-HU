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
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: Ismerkedjen meg a robotpilóta-profilok létrehozásával, szerkesztésével, törlésével vagy eltávolításával.
ms.openlocfilehash: f7fdc2632e93c48e043fe158842f8395d6a89e14
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/14/2019
ms.locfileid: "38320238"
---
# <a name="create-and-edit-autopilot-profiles"></a>AutoPilot-profilok létrehozása és szerkesztése

## <a name="create-a-profile"></a>Profil létrehozása

A profil egy eszközre vagy eszközök csoportjára vonatkozik.
  
1. -Ban Mikroszkóp 365 teendő admin központ, választ **berendezés** \> **robotpilóta**.
  
2. A **robotpilóta** oldalon válassza a profil lap **** \> **létrehozása profilt**.
    
3. A **profil létrehozása** lapon adjon nevet a profilnak, amely segít azonosítani, például marketing. Kapcsolja be a kívánt beállítást, majd kattintson a **Mentés**gombra. A robotpilóta profilbeállításaival kapcsolatos további tudnivalókért tanulmányozza az [robotpilóta-profil beállításai](autopilot-profile-settings.md)című témakört.
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a>Profil alkalmazása eszközre

A profil létrehozása után alkalmazhatja azt egy eszközre vagy eszközcsoportra. A [Részletes útmutató](add-autopilot-devices-and-profile.md) segítségével egy meglévő profilt választhat ki, és alkalmazhatja azt az új eszközökre, vagy kicserélheti egy eszköz vagy eszközcsoport meglévő profilját. 
  
1. **A Windows előkészítése** lapon válassza az **Eszközök** fület. 
    
2. Jelölje be az eszköznév melletti jelölőnégyzetet, majd az **eszközpanelen** válasszon egy profilt a **hozzárendelt profil** \> **legördülő listáról.**
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a>Profil szerkesztése, törlése vagy eltávolítása

Miután hozzárendelt egy profilt egy eszközhöz, frissítheti azt még akkor is, ha már odaadta az eszközt egy felhasználónak. Amikor az eszköz csatlakozik az internethez, a beállítási folyamat során letölti a profil legújabb verzióját. Ha a felhasználó visszaállítja az eszköz gyári alapértelmezett beállításait, az eszköz ismét le fogja tölteni a profil legújabb frissítéseit. 
  
### <a name="edit-a-profile"></a>Profil szerkesztése

1. **A Windows előkészítése** lapon válassza a **Profilok** fület. 
    
2. Jelölje be az eszköz neve melletti jelölőnégyzetet, és a **profil** panelen frissítse az elérhető beállítások \> **mentését**.
    
    Ha ezt azelőtt végzi el, hogy a felhasználó csatlakoztatná az eszközt az internetre, akkor a profilt a rendszer alkalmazza a beállítási folyamatra.
    
### <a name="delete-a-profile"></a>Profil törlése

1. **A Windows előkészítése** lapon válassza a **Profilok** fület. 
    
2. Jelölje be az eszköznév melletti jelölőnégyzetet, majd a **profil** panelen jelölje be a **profilmentés** \> **** törlése négyzetet.
    
    A törléssel a profilt eltávolítja arról az eszközről vagy abból az eszközcsoportból, amelyhez hozzá volt rendelve.
    
### <a name="remove-a-profile"></a>Profil eltávolítása

1. **A Windows előkészítése** lapon válassza az **Eszközök** fület. 
    
2. Jelölje be az eszköznév melletti jelölőnégyzetet, az **eszközpanelen** pedig válassza a **nincs** beállítást a **hozzárendelt profil** legördülő \> **listából.**
    

---
title: AutoPilot-profilok létrehozása és szerkesztése
f1.keywords:
- NOCSH
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
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: Ismerje meg, hogyan hozhat létre AutoPilot-profilt, és alkalmazhatja azt egy eszközre, valamint szerkesztsen vagy töröljön egy profilt, illetve távolítson el egy profilt az eszközről.
ms.openlocfilehash: 58c16b68c66dce7541a02ecd0d2466babe8cc338
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/07/2020
ms.locfileid: "42560720"
---
# <a name="create-and-edit-autopilot-profiles"></a>AutoPilot-profilok létrehozása és szerkesztése

## <a name="create-a-profile"></a>Profil létrehozása

A profil egy eszközre vagy eszközök csoportjára vonatkozik.
  
1. A Microsoft 365 Vállalati felügyeleti központban válassza az **Eszközök** \> **AutoPilot**lehetőséget.
  
2. Az **AutoPilot** lapon válassza **** a \> Profilok lapot **Profil létrehozása**.
    
3. A **Profil létrehozása** lapon adja meg a profil nevét, amely segít azonosítani azt, például a Marketing. Kapcsolja be a kívánt beállítást, majd kattintson a **Mentés gombra.** Az AutoPilot profilbeállításairól további információt [az AutoPilot-profil beállításairól című témakörben](autopilot-profile-settings.md)talál.
    
    ![Enter name and turn on settings in the Create profile panel.](../media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a>Profil alkalmazása eszközre

Miután létrehozott egy profilt, alkalmazhatja azt egy eszközre vagy eszközcsoportra. A [részletes útmutatóban](add-autopilot-devices-and-profile.md) kiválaszthatja a meglévő profilt, és alkalmazhatja azt új eszközökre, vagy lecserélhet egy meglévő profilt egy eszközre vagy eszközcsoportra. 
  
1. **A Windows előkészítése** lapon válassza az **Eszközök** fület. 
    
2. Jelölje be az eszköznév melletti jelölőnégyzetet, és az **Eszköz** panelen válasszon egy profilt a **Hozzárendelt profil** legördülő \> **listából Mentés**.
    
    ![In the Device panel, select an Assigned profile to apply it.](../media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a>Profil szerkesztése, törlése vagy eltávolítása

Miután hozzárendelt egy profilt egy eszközhöz, frissítheti azt még akkor is, ha már odaadta az eszközt egy felhasználónak. Amikor az eszköz csatlakozik az internethez, a beállítási folyamat során letölti a profil legújabb verzióját. Ha a felhasználó visszaállítja az eszköz gyári alapértelmezett beállításait, az eszköz ismét le fogja tölteni a profil legújabb frissítéseit. 
  
### <a name="edit-a-profile"></a>Profil szerkesztése

1. **A Windows előkészítése** lapon válassza a **Profilok** fület. 
    
2. Jelölje be az eszközneve melletti jelölőnégyzetet, és a **Profil** panelen frissítse a rendelkezésre álló beállítások \> bármelyikét **Mentés**.
    
    Ha ezt azelőtt végzi el, hogy a felhasználó csatlakoztatná az eszközt az internetre, akkor a profilt a rendszer alkalmazza a beállítási folyamatra.
    
### <a name="delete-a-profile"></a>Profil törlése

1. **A Windows előkészítése** lapon válassza a **Profilok** fület. 
    
2. Jelölje be az eszközneve melletti jelölőnégyzetet, majd a **Profil panelen** válassza a \> Profil **mentése** **törlése lehetőséget.**
    
    A törléssel a profilt eltávolítja arról az eszközről vagy abból az eszközcsoportból, amelyhez hozzá volt rendelve.
    
### <a name="remove-a-profile"></a>Profil eltávolítása

1. **A Windows előkészítése** lapon válassza az **Eszközök** fület. 
    
2. Jelölje be az eszköznév melletti jelölőnégyzetet, és az **Eszköz** panelen válassza a \> **Hozzárendelési profil** mentés i. listájának Nincs **elemét.** ****
    

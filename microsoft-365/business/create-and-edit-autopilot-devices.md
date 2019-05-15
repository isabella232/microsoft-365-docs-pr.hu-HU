---
title: AutoPilot-eszközök létrehozása és szerkesztése
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Útmutató a Microsoft 365 üzleti automata használó eszközök feltölteni. A profil hozzárendelése egy eszköz vagy eszközök egy csoportjához.
ms.openlocfilehash: dee77a014ef519f3487a082edc3cf81058ec1c00
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/15/2019
ms.locfileid: "34071640"
---
# <a name="create-and-edit-autopilot-devices"></a>AutoPilot-eszközök létrehozása és szerkesztése

## <a name="upload-a-list-of-devices"></a>Eszközlista feltöltése

A [lépésenkénti hozzáadási folyamat](add-autopilot-devices-and-profile.md) mellett az **Eszközök** lapon is tölthet fel eszközöket. 
  
Az eszközöknek meg kell felelniük az alábbi követelményeknek:
  
- A Windows 10 rendszer 1703-as vagy újabb verzióját kell futtatniuk.
    
- Olyan új eszközöknek kell lenniük, amelyeken még nem használták a Windowst.

1. A Microsoft 365 üzleti rendszergazdai központban válassza az **eszközök** \> **automata**.
  
2. Az **automata** lapon válassza ki **az eszközök** lapon \> **eszközök hozzáadása**.
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. Készített [eszköz lista CSV-fájl](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) **hozzáadása eszközök** panelen keresse \> **Mentés** \> **bezárása**.
    
    Ezeket az adatokat beszerezheti a hardvergyártójától, vagy használhatja a [Get-WindowsAutoPilotInfo PowerShell-parancsfájlt](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), amely elkészíti a CSV-fájlt. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Profil társítása egy eszközhöz vagy az eszközök egy csoportjához

1. **A Windows előkészítése** lapon válassza az **Eszközök** fület, majd jelölje be egy vagy több eszköz jelölőnégyzetét. 
    
2. Az **Eszköz** panelen válasszon egy profilt a **Hozzárendelt profil** legördülő listából. 
    
    Ha egyetlen profilja sincs még, utasításokért olvassa el az [AutoPilot-profilok létrehozása és szerkesztése](create-and-edit-autopilot-profiles.md) című témakört. 
    

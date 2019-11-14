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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Megtanulják, hogyan kell feltölteni eszközök segítségével AutoPilot a Microsoft 365 Business. Profilt hozzárendelhet egy eszközhöz vagy eszközcsoporthoz.
ms.openlocfilehash: 1dd6b1a574166379e29465bf3699e47e3b155e0b
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/14/2019
ms.locfileid: "38320258"
---
# <a name="create-and-edit-autopilot-devices"></a>AutoPilot-eszközök létrehozása és szerkesztése

## <a name="upload-a-list-of-devices"></a>Eszközlista feltöltése

Az eszközök feltöltéséhez használja a [részletes útmutatót](add-autopilot-devices-and-profile.md) , de az **Eszközök lapon is** tölthet fel eszközöket. 
  
Az eszközöknek meg kell felelniük ezeknek a követelményeknek:
  
- Windows 10, 1703-es vagy újabb verzió
    
- Új berendezés amit kikötő ' átmenő Windows ki--ból-doboz tapasztalat

1. -Ban Mikroszkóp 365 teendő admin központ, választ **berendezés** \> **robotpilóta**.
  
2. A **robotpilóta** oldalán válassza ki az eszközök **fület.** \> ****
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. Az **eszközök hozzáadása** panelen tallózással keresse meg a **mentett** \> [eszközlistát tartalmazó CSV-fájlt](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) . **** \>
    
    Ezt az információt a hardver forgalmazójától kaphatja meg, vagy a [Get-WindowsAutoPilotInfo PowerShell parancsfájl](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) segítségével hozhat létre CSV-fájlt. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Profil társítása egy eszközhöz vagy az eszközök egy csoportjához

1. A **Windows előkészítése** lapon válassza az **eszközök** fület, és jelölje be az eszközök melletti jelölőnégyzetet. 
    
2. Az **Eszköz** panelen válasszon egy profilt a **Hozzárendelt profil** legördülő listából. 
    
    Ha egyetlen profilja sincs még, utasításokért olvassa el az [AutoPilot-profilok létrehozása és szerkesztése](create-and-edit-autopilot-profiles.md) című témakört. 
    

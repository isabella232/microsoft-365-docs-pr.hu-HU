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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Megtanulják, hogyan kell feltölteni eszközök segítségével AutoPilot a Microsoft 365 Business. Profilt hozzárendelhet egy eszközhöz vagy eszközcsoporthoz.
ms.openlocfilehash: 9ae94266f5a41d8d115fc92f0f080a6fdbdc9f15
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288015"
---
# <a name="create-and-edit-autopilot-devices"></a>AutoPilot-eszközök létrehozása és szerkesztése

## <a name="upload-a-list-of-devices"></a>Eszközlista feltöltése

A [lépésenkénti hozzáadási folyamat](add-autopilot-devices-and-profile.md) mellett az **Eszközök** lapon is tölthet fel eszközöket. 
  
Az eszközöknek meg kell felelniük az alábbi követelményeknek:
  
- A Windows 10 rendszer 1703-as vagy újabb verzióját kell futtatniuk.
    
- Olyan új eszközöknek kell lenniük, amelyeken még nem használták a Windowst.

1. -Ban Mikroszkóp 365 teendő admin központ, választ **berendezés** \> **robotpilóta**.
  
2. A **robotpilóta** oldalán válassza ki az eszközök **fület.** \> ****
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. Az **eszközök hozzáadása** panelen tallózással keresse meg az előkészített [](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) \> CSV-fájlt, amely **bezárva** **menti** \> az eszközt.
    
    Ezeket az adatokat beszerezheti a hardvergyártójától, vagy használhatja a [Get-WindowsAutoPilotInfo PowerShell-parancsfájlt](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), amely elkészíti a CSV-fájlt. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Profil társítása egy eszközhöz vagy az eszközök egy csoportjához

1. **A Windows előkészítése** lapon válassza az **Eszközök** fület, majd jelölje be egy vagy több eszköz jelölőnégyzetét. 
    
2. Az **Eszköz** panelen válasszon egy profilt a **Hozzárendelt profil** legördülő listából. 
    
    Ha egyetlen profilja sincs még, utasításokért olvassa el az [AutoPilot-profilok létrehozása és szerkesztése](create-and-edit-autopilot-profiles.md) című témakört. 
    

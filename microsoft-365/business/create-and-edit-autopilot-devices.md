---
title: AutoPilot-eszközök létrehozása és szerkesztése
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Megtudhatja, hogy miként tölthet fel eszközöket az AutoPilottal a Microsoft 365 Vállalati prémium verzió. A profilokat hozzárendelheti egy eszközhöz vagy eszközcsoporthoz.
ms.openlocfilehash: ae3a760db4b94aac50301685a0c4f468e46ec8e9aa907a1b6fb35e03a9e541f0
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53867039"
---
# <a name="create-and-edit-autopilot-devices"></a>AutoPilot-eszközök létrehozása és szerkesztése

## <a name="upload-a-list-of-devices"></a>Eszközlista feltöltése

Az eszközök [](add-autopilot-devices-and-profile.md) feltöltéséhez használhatja a részletes útmutatót, de az Eszközök lapon is **feltölthet** eszközöket. 
  
Az eszközöknek meg kell felelnie az alábbi követelményeknek:
  
- Windows 10 1703-as vagy újabb verzió
    
- Új eszközök, amelyeken még nem Windows nem voltak bevetve

1. Az eszköz Microsoft 365 Felügyeleti központ az **Eszközök** \> **AutoPilot lehetőséget.**
  
2. Az **AutoPilot lapon** válassza  az Eszközök lap \> **Eszközök hozzáadása lapját.**
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. Az Eszközök **hozzáadása panelen** tallózással keresse meg a Save Close (Bezárás mentése) eszközlista [CSV-fájlját.](../admin/misc/device-list.md) \>  \> 
    
    Ezeket az információkat a hardvergyártójától kaphatja meg, vagy a [Get-WindowsAutoPilotInfo PowerShell-parancsprogrammal](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) létrehozhat egy CSV-fájlt. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Profil társítása egy eszközhöz vagy az eszközök egy csoportjához

1. Az Előkészítés **Windows** kattintson az Eszközök  fülre, és jelölje be egy vagy több eszköz jelölőnégyzetét. 
    
2. Az **Eszköz** panelen válasszon egy profilt a **Hozzárendelt profil** legördülő listából. 
    
    Ha egyetlen profilja sincs még, utasításokért olvassa el az [AutoPilot-profilok létrehozása és szerkesztése](create-and-edit-autopilot-profiles.md) című témakört. 

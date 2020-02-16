---
title: AutoPilot-eszközök létrehozása és szerkesztése
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Megtudhatja, hogy miként tölthet fel eszközöket az AutoPilot használatával a Microsoft 365 Business programban. Profilt rendelhet egy eszközhöz vagy eszközcsoporthoz.
ms.openlocfilehash: 640e4af7cccde83c87d90a875c1d44dead7255ca
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/15/2020
ms.locfileid: "42065982"
---
# <a name="create-and-edit-autopilot-devices"></a>AutoPilot-eszközök létrehozása és szerkesztése

## <a name="upload-a-list-of-devices"></a>Eszközlista feltöltése

A részletes [útmutatósegítségével](add-autopilot-devices-and-profile.md) eszközöket tölthet fel, de az **Eszközök** lapon is feltöltheti az eszközöket. 
  
Az eszközöknek meg kell felelniük ezeknek a követelményeknek:
  
- Windows 10, 1703-as vagy újabb verzió
    
- Új eszközök, amelyek nem voltak a Windows beépített élményén

1. A Microsoft 365 Vállalati felügyeleti központban válassza az **Eszközök** \> **AutoPilot**lehetőséget.
  
2. Az **AutoPilot** lapon válassza **** az \> Eszközök lapot **Eszközök hozzáadása**.
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. Az **Eszközök hozzáadása** panelen keresse meg a **Bezárás** **mentése** \> című eszközlistát tartalmazó [CSV-fájlt.](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) \>
    
    Ezeket az információkat a hardver gyártójától szerezheti be, vagy a [Get-WindowsAutoPilotInfo PowerShell parancsfájl](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) segítségével CSV-fájlt hozhat létre. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Profil társítása egy eszközhöz vagy az eszközök egy csoportjához

1. A **Windows előkészítése** lapon válassza az **Eszközök** lapot, és jelölje be az egy vagy több eszköz melletti jelölőnégyzetet. 
    
2. Az **Eszköz** panelen válasszon egy profilt a **Hozzárendelt profil** legördülő listából. 
    
    Ha egyetlen profilja sincs még, utasításokért olvassa el az [AutoPilot-profilok létrehozása és szerkesztése](create-and-edit-autopilot-profiles.md) című témakört. 
    

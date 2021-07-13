---
title: Autopilot-eszközök és -profilok hozzáadása a lépésenkénti útmutatóval
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection:
- M365-subscription-management
- M365-identity-device-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
- AdminTemplateSet
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Ebből a cikkből megtudhatja, Windows AutoPilot használatával hogyan állíthat be új Windows 10 eszközét a vállalata számára, hogy azok készen állnak az alkalmazottak használatára.
ms.openlocfilehash: f160ddcd1e41bd44c908ecc8bbd30a9819f76902
ms.sourcegitcommit: 00f001019c653269d85718d410f970887d904304
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/12/2021
ms.locfileid: "53393439"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Autopilot-eszközök és -profilok hozzáadása a lépésenkénti útmutatóval

Az AutoPilot Windows használatával új  Windows 10 állíthat be a vállalata számára, így azok készen állnak a használatra, amikor az alkalmazottaknak adja őket.
  
## <a name="device-requirements"></a>Eszközkövetelmények

Az eszközöknek meg kell felelnie az alábbi követelményeknek:
  
- Windows 10 1703-as vagy újabb verzió
    
- Új eszközök, amelyeken még nem Windows nem voltak bevetve
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Eszközök és profilok létrehozása a beállítási útmutató használatával

Ha még nem hozott létre eszközcsoportokat vagy -profilokat, a legjobb, ha a részletes útmutatót használja. Az útmutató [használata](create-and-edit-autopilot-devices.md) [](create-and-edit-autopilot-profiles.md) nélkül is felvehet eszközöket, és profilokat rendelhet hozzájuk. 
  
1. A felügyeleti központ megnyitásához: <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .

2. A bal oldali navigációs ablakban válassza az **Eszközök** \> **AutoPilot lehetőséget.**

    ![A Felügyeleti központban válassza az eszközök, majd az AutoPilot lehetőséget.](../media/AutoPilot.png)
  
2. Az **AutoPilot lapon** kattintson vagy koppintson az Útmutató **kezdése elemre.**
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. Az **Eszközlista .csv** fájl feltöltése lapon tallózással keresse meg azt a helyet, ahol  az előkészített fájl .CSV, majd a Tovább \> **gombra.** A fájlnak három fejléccel kell lennie:
    
    - A oszlop: Eszköz sorozatszáma
    
    - B oszlop: Windows-termékazonosító
    
    - C oszlop: Hardverkivonat
    
    Ezeket az információkat a hardvergyártójától kaphatja meg, vagy a [Get-WindowsAutoPilotInfo PowerShell-parancsprogrammal](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) létrehozhat egy CSV-fájlt. 
    
    További információ: [Eszközlistát tartalmazó CSV-fájl](../admin/misc/device-list.md). Az **Eszközlistát tartalmazó CSV-fájl feltöltése** lapon egy mintafájlt is letölthet. 
    
> [!NOTE]
> Ez a parancsprogram WMI segítségével beolvassa az autopilottal regisztrált eszközöknek az Windows tulajdonságait. Felhívjuk a figyelmét arra, hogy az eredményül kapott CSV-fájlban nem kell egy Windows-termékazonosító (PKID) értéket gyűjteni, mivel ez nem szükséges egy eszköz regisztrálásához, és a PKID NULL érték a kimeneti CSV-fájlban teljesen rendben van. A rendszer csak a sorozatszámot és a hardver kivonatát tölti ki.
    
4. A Profil **hozzárendelése lapon** kiválaszthat egy meglévő profilt, vagy létrehozhat egy újat. Ha még nincs ilyen fiókja, a rendszer kérni fogja, hogy hozzon létre egyet. 
    
    A profil azoknak a beállításoknak a gyűjteménye, amelyek egyetlen eszközre vagy eszközök csoportjára lehet alkalmazni.
    
    Az alapértelmezett funkciók kötelezők, és automatikusan vannak beállítva. Az alapértelmezett funkciók az alábbiak:
    
    - Kihagyhatja Cortana, a OneDrive és az OEM-regisztrációt.
    
    - Bejelentkezés céges márkával.
    
    - Csatlakozás az eszközeit a Azure Active Directory fiókokhoz, és automatikusan regisztrálja őket a Microsoft 365 Vállalati prémium verzió.
    
    További információ: [Az AutoPilot-profil beállításai.](autopilot-profile-settings.md) 
    
5. A további beállítások: **Adatvédelmi beállítások kihagyása** és **Nem léptethető elő a felhasználó a helyi rendszergazdává**. Mindkettő értéke alapértelmezés szerint **Kikapcsolva**. 
    
    Válassza a **Tovább** gombot.
    
6. **Ha végzett,** az azt jelenti, hogy a létrehozott (vagy kiválasztott) profilt a rendszer az eszközlista feltöltésével létrehozott eszközcsoportra alkalmazza. A beállítások akkor lépnek életbe, amikor az eszköz felhasználói legközelebb bejelentkeznek. Válassza a **Bezárás** gombot.

## <a name="related-content"></a>Kapcsolódó tartalom

[Az AutoPilot-profil beállításai](autopilot-profile-settings.md) (cikk)\
[Az eszközök és az alkalmazásadatok védelmére vonatkozó](../admin/devices/choose-device-security.md) beállítások (cikk)

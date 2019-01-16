---
title: Autopilot-eszközök és -profilok hozzáadása a lépésenkénti útmutatóval
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Útmutató a Windows automata segítségével állítsa be az új Windows 10 eszközök a vállalkozás számára.
ms.openlocfilehash: 56225424125e9eed9f46867837c564aa5d1c4adc
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982165"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Autopilot-eszközök és -profilok hozzáadása a lépésenkénti útmutatóval

A Windows AutoPilot segítségével előkészítheti cégének új Windows 10-es eszközeit, így az alkalmazottak azonnal hatékonyan munkához láthatnak, amint megkapják az eszközüket.
  
## <a name="device-requirements"></a>Eszközkövetelmények

Az eszközöknek meg kell felelniük az alábbi követelményeknek:
  
- A Windows 10 rendszer 1703-as vagy újabb verzióját kell futtatniuk.
    
- Olyan új eszközöknek kell lenniük, amelyeken még nem használták a Windowst.
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Eszközök és profilok létrehozása a beállítási útmutató használatával

Ha még nem hozott létre eszközcsoportokat vagy profilokat, a legjobb, ha azzal kezdi, hogy elolvassa a részletes útmutatót, de azt is megteheti, hogy az útmutató nélkül [vesz fel eszközöket](create-and-edit-autopilot-devices.md) és [rendel hozzájuk profilokat](create-and-edit-autopilot-profiles.md). 
  
1. A Microsoft 365 Business Felügyeleti központban keresse meg az **Eszközműveletek** kártyát, és válassza **A Windows üzembe helyezése az Autopilottal** lehetőséget.
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. **A Windows előkészítése** lapon kattintson vagy koppintson az **Útmutató indítása** elemre.
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. Az **Eszközlistát tartalmazó CSV-fájl feltöltése** lapon tallózással keresse meg az előkészített CSV-fájlt, és válassza a **Megnyitás** \> **Tovább** lehetőséget. A fájlnak három fejlécet kell tartalmaznia:
    
  - A oszlop: Eszköz sorozatszáma
    
  - B oszlop: Windows-termékazonosító
    
  - C oszlop: Hardverkivonat
    
    Ezeket az adatokat beszerezheti a hardvergyártójától, vagy használhatja a [Get-WindowsAutoPilotInfo PowerShell-parancsfájlt](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), amely elkészíti a CSV-fájlt. 
    
    További információ: [Eszközlistát tartalmazó CSV-fájl](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Az **Eszközlistát tartalmazó CSV-fájl feltöltése** lapon egy mintafájlt is letölthet. 
    
4. A **Profil hozzárendelése** lapon kiválaszthat egy meglévő profilt, vagy létrehozhat egy újat. Ha még nincs profilja, a rendszer új profil létrehozására fogja kérni. 
    
    A profil azoknak a beállításoknak a gyűjteménye, amelyek egyetlen eszközre vagy eszközök csoportjára lehet alkalmazni.
    
    Az alapértelmezett funkciók kötelezők, és beállításuk automatikusan megtörténik. Az alapértelmezett funkciók az alábbiak:
    
  - A Cortana, a OneDrive és a számítógépgyártók regisztrációja kihagyva.
    
  - Bejelentkezés céges márkával.
    
  - Az eszközöket ezzel csatlakoztatja az Azure Active Directory-fiókokhoz, és automatikusan regisztrálja őket a Microsoft 365 Business általi kezelésre.
    
    További információ:
    
    [Az AutoPilot-profil beállításai](autopilot-profile-settings.md) . 
    
5. A további beállítások: **Adatvédelmi beállítások kihagyása** és **Nem léptethető elő a felhasználó a helyi rendszergazdává**. Mindkettő értéke alapértelmezés szerint **Kikapcsolva**. 
    
    Válassza a **Tovább** gombot.
    
6. Az **Elkészült!** lap megjelenése jelzi, hogy a rendszer a létrehozott (vagy kiválasztott) profilt alkalmazza arra az eszközcsoportra, amelyet Ön az eszközlista feltöltésével létrehozott. Ezek a beállítások lesznek érvényben legközelebb, amikor az eszköz felhasználói bejelentkeznek. Válassza a **Bezárás** gombot.
    
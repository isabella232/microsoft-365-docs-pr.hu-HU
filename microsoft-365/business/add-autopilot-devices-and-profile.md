---
title: Autopilot-eszközök és -profilok hozzáadása a lépésenkénti útmutatóval
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: A Windows AutoPilot használata új Windows 10 eszközök beállítására a vállalat számára.
ms.openlocfilehash: d028ea3e902965d55c445dc3b3a02aa315201b25
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/17/2019
ms.locfileid: "37574788"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Autopilot-eszközök és -profilok hozzáadása a lépésenkénti útmutatóval

Használhatja a Windows AutoPilot, hogy hozzanak létre **új** Windows 10 eszközök a vállalkozás számára, így azok készen állnak a hatékony használatra, amint megadja nekik az alkalmazottak.
  
## <a name="device-requirements"></a>Eszközkövetelmények

Az eszközöknek meg kell felelniük az alábbi követelményeknek:
  
- A Windows 10 rendszer 1703-as vagy újabb verzióját kell futtatniuk.
    
- Olyan új eszközöknek kell lenniük, amelyeken még nem használták a Windowst.
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Eszközök és profilok létrehozása a beállítási útmutató használatával

[![Label, hogy tudd, az admin központ változik, és találsz további részleteket a aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Ha még nem hozott létre eszközcsoportokat vagy profilokat, a legjobb, ha azzal kezdi, hogy elolvassa a részletes útmutatót, de azt is megteheti, hogy az útmutató nélkül [vesz fel eszközöket](create-and-edit-autopilot-devices.md) és [rendel hozzájuk profilokat](create-and-edit-autopilot-profiles.md). 
  
1. Menj az admin központba <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.

2. A bal oldali NAV válasszon **eszközök** \> **robotpilóta**.

    ![Az Admin Center válasszon eszközöket, majd robotpilóta.](media/AutoPilot.png)
  
2. A **robotpilóta** oldalon kattintson vagy koppintson a **Start Guide**elemre.
    
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
    
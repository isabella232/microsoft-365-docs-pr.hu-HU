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
ms.openlocfilehash: 5f40dac57285b83da57d4506bac58e562475522c
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/14/2019
ms.locfileid: "38323095"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Autopilot-eszközök és -profilok hozzáadása a lépésenkénti útmutatóval

Használhatja a Windows AutoPilot, hogy hozzanak létre **új** Windows 10 eszközök a vállalkozás számára, így ők készen áll, amikor megadja nekik az alkalmazottak.
  
## <a name="device-requirements"></a>Eszközkövetelmények

Az eszközöknek meg kell felelniük ezeknek a követelményeknek:
  
- Windows 10, 1703-es vagy újabb verzió
    
- Új berendezés amit kikötő ' átmenő Windows ki--ból-doboz tapasztalat
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Eszközök és profilok létrehozása a beállítási útmutató használatával

[![A megjelenő címke figyelmeztet a felügyeleti központ változásaira, további részleteket itt talál: aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Ha még nem hozott létre eszközcsoportokat vagy profilokat, a legjobb módszer a részletes útmutató használatával a kezdéshez. A segédvonal használata nélkül is [hozzáadhat eszközöket](create-and-edit-autopilot-devices.md) , és [profilokat rendelhet](create-and-edit-autopilot-profiles.md) hozzájuk. 
  
1. Menj az admin központba <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.

2. A bal oldali navigációs ablaktáblán kattintson az **eszközök** \> **robotpilóta**parancsra.

    ![Az admin központban, válasszon eszközöket, majd robotpilóta.](media/AutoPilot.png)
  
2. A **robotpilóta** oldalon kattintson vagy koppintson a **Start Guide**elemre.
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. A **upload. csv fájlban az eszközök listáját tartalmazó** lapon keresse meg azt a helyet, ahol az előkészített. CSV fájlt, majd **nyissa meg** \> a **Next**. A fájlnak három fejlécet kell tartalmaznia:
    
    - A oszlop: Eszköz sorozatszáma
    
    - B oszlop: Windows-termékazonosító
    
    - C oszlop: Hardverkivonat
    
    Ezt az információt a hardver forgalmazójától kaphatja meg, vagy a [Get-WindowsAutoPilotInfo PowerShell parancsfájl](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) segítségével hozhat létre CSV-fájlt. 
    
    További információ: [Eszközlistát tartalmazó CSV-fájl](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Az **Eszközlistát tartalmazó CSV-fájl feltöltése** lapon egy mintafájlt is letölthet. 
    
4. A **profil hozzárendelése** lapon választhat egy meglévő profilt, vagy létrehozhat egy újat. Ha még nincs ilyen, akkor a program kérni fogja, hogy hozzon létre egyet. 
    
    A profil azoknak a beállításoknak a gyűjteménye, amelyek egyetlen eszközre vagy eszközök csoportjára lehet alkalmazni.
    
    Az alapértelmezett szolgáltatások szükségesek, és automatikusan beállnak. Az alapértelmezett funkciók az alábbiak:
    
    - Ugrál Cortana, OneDrive, és OEM beírás.
    
    - Bejelentkezés céges márkával.
    
    - Csatlakoztassa a készülékeket az Azure Active Directory fiókokhoz, és automatikusan igényelje őket a Microsoft 365 Business általi kezelésükhöz.
    
    További információ: [a robotpilóta-profil beállításai](autopilot-profile-settings.md). 
    
5. A további beállítások: **Adatvédelmi beállítások kihagyása** és **Nem léptethető elő a felhasználó a helyi rendszergazdává**. Mindkettő értéke alapértelmezés szerint **Kikapcsolva**. 
    
    Válassza a **Tovább** gombot.
    
6. **Elkészült** , azt jelzi, hogy a létrehozott (vagy választott) profilt a program az eszközök listájának feltöltésével létrehozott eszközcsoportra alkalmazza. A beállítások akkor lesznek érvényben, amikor az eszköz felhasználói bejelentkeznek. Válassza a **Bezárás** gombot.
    
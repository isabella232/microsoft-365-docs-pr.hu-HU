---
title: Autopilot-eszközök és -profilok hozzáadása a lépésenkénti útmutatóval
f1.keywords:
- NOCSH
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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Megtudhatja, hogy a Windows AutoPilot segítségével hogyan állíthatja be az új Windows 10-es eszközöket a vállalkozása számára, hogy készen álljanak az alkalmazottak használatára.
ms.openlocfilehash: 8449d5a3672a20b0cd1ba61bbda863073138c04c
ms.sourcegitcommit: 26e4d5091583765257b7533b5156daa373cd19fe
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/06/2020
ms.locfileid: "42550387"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Autopilot-eszközök és -profilok hozzáadása a lépésenkénti útmutatóval

A Windows AutoPilot segítségével **új** Windows 10-es eszközöket állíthat be a vállalkozása számára, hogy azok készen álljanak a használatra, amikor átadja azokat az alkalmazottaknak.
  
## <a name="device-requirements"></a>Eszközkövetelmények

Az eszközöknek meg kell felelniük ezeknek a követelményeknek:
  
- Windows 10, 1703-as vagy újabb verzió
    
- Új eszközök, amelyek nem voltak a Windows beépített élményén
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Eszközök és profilok létrehozása a beállítási útmutató használatával

[![A megjelenő címke figyelmeztet a felügyeleti központ változásaira, további részleteket itt talál: aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Ha még nem hozott létre eszközcsoportokat vagy profilokat, a legjobb módja az első lépéseknek a részletes útmutató használatával. Eszközöket is [hozzáadhat,](create-and-edit-autopilot-devices.md) és [profilokat rendelhet](create-and-edit-autopilot-profiles.md) hozzájuk az útmutató használata nélkül. 
  
1. Nyissa meg a <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>felügyeleti központot a .

2. A bal oldali navigációs ablakban válassza az **Eszközök** \> **AutoPilot**lehetőséget.

    ![A felügyeleti központban válassza az eszközök, majd az AutoPilot lehetőséget.](../media/AutoPilot.png)
  
2. Az **AutoPilot** lapon kattintson vagy koppintson az **Útmutató indítása**elemre.
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. A **Feltöltés .csv fájl eszközök listájával** lapon keresse meg azt a helyet, ahol előkészítette a fájlt. CSV fájlt, majd **nyissa meg** \> **a Tovább**. A fájlnak három fejlécből kell rendelkeznie:
    
    - A oszlop: Eszköz sorozatszáma
    
    - B oszlop: Windows-termékazonosító
    
    - C oszlop: Hardverkivonat
    
    Ezeket az információkat a hardver gyártójától szerezheti be, vagy a [Get-WindowsAutoPilotInfo PowerShell parancsfájl](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) segítségével CSV-fájlt hozhat létre. 
    
    További információ: [Eszközlistát tartalmazó CSV-fájl](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Az **Eszközlistát tartalmazó CSV-fájl feltöltése** lapon egy mintafájlt is letölthet. 
    
4. A **Profil hozzárendelése** lapon választhat egy meglévő profilt, vagy létrehozhat egy újat. Ha még nem rendelkezik ilyenvel, a rendszer kérni fogja, hogy hozzon létre egyet. 
    
    A profil azoknak a beállításoknak a gyűjteménye, amelyek egyetlen eszközre vagy eszközök csoportjára lehet alkalmazni.
    
    Az alapértelmezett funkciók szükségesek, és automatikusan be vannak állítva. Az alapértelmezett funkciók az alábbiak:
    
    - Cortana, OneDrive és OEM regisztráció kihagyása.
    
    - Bejelentkezés céges márkával.
    
    - Csatlakoztassa eszközeit az Azure Active Directory-fiókokhoz, és automatikusan regisztrálhatja őket a Microsoft 365 Business általi felügyelthez.
    
    További információt [az AutoPilot-profil beállításairól című témakörben](autopilot-profile-settings.md)talál. 
    
5. A további beállítások: **Adatvédelmi beállítások kihagyása** és **Nem léptethető elő a felhasználó a helyi rendszergazdává**. Mindkettő értéke alapértelmezés szerint **Kikapcsolva**. 
    
    Válassza a **Tovább** gombot.
    
6. **A kész azt** jelzi, hogy a létrehozott (vagy kiválasztott) profil az eszközök listájának feltöltésével létrehozott eszközcsoportra lesz alkalmazva. A beállítások akkor lépnek érvénybe, amikor az eszköz felhasználók bejelentkeznek legközelebb. Válassza a **Bezárás** gombot.
    

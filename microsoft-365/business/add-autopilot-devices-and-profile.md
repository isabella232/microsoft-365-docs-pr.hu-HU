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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Megtudhatja, hogy a Windows AutoPilot segítségével hogyan állíthatja be az új Windows 10-es eszközöket a vállalkozása számára, hogy azok készen álljanak az alkalmazottak használatára.
ms.openlocfilehash: efcb5442b34d2d42275cedc30e71ac98c7ea1266
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44401094"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Autopilot-eszközök és -profilok hozzáadása a lépésenkénti útmutatóval

A Windows AutoPilot segítségével **új** Windows 10-es eszközöket állíthat be a vállalkozása számára, hogy azok készen álljanak a használatra, amikor átadja azokat az alkalmazottaknak.
  
## <a name="device-requirements"></a>Eszközkövetelmények

Az eszközöknek meg kell felelniük az alábbi követelményeknek:
  
- Windows 10, 1703-as vagy újabb verzió
    
- Új eszközök, amelyek nem mentették át a Windows beépített élményét
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Eszközök és profilok létrehozása a beállítási útmutató használatával

[![A megjelenő címke figyelmeztet a felügyeleti központ változásaira, további részleteket itt talál: aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Ha még nem hozott létre eszközcsoportokat vagy profilokat, a legjobb módszer az első lépések rebája segítségével. Az útmutató használata nélkül is [hozzáadhat eszközöket](create-and-edit-autopilot-devices.md) és [rendelhet hozzájuk profilokat.](create-and-edit-autopilot-profiles.md) 
  
1. Nyissa meg a felügyeleti központot a <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> alkalmazásban.

2. A bal oldali navigációs ablakban válassza az **Eszközök** \> **autokísérleti**lehetőséget.

    ![A felügyeleti központban válassza az eszközöket, majd az AutoPilot lehetőséget.](../media/AutoPilot.png)
  
2. Az **AutoPilot** lapon kattintson vagy koppintson a **Start útmutató gombra.**
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. Az **Eszközök listájával rendelkező .csv fájl feltöltése** lapon keresse meg azt a helyet, ahol a program előkészítette a programot. CSV-fájlt, majd **nyissa meg a** Tovább \> **gombot.** A fájlnak három fejlécből kell rendelkeznie:
    
    - A oszlop: Eszköz sorozatszáma
    
    - B oszlop: Windows-termékazonosító
    
    - C oszlop: Hardverkivonat
    
    Ezeket az információkat beszerezheti a hardver forgalmazójától, vagy használhatja a [Get-WindowsAutoPilotInfo PowerShell parancsfájlt CSV-fájl](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) létrehozásához. 
    
    További információ: [Eszközlistát tartalmazó CSV-fájl](https://docs.microsoft.com/microsoft-365/admin/misc/device-list). Az **Eszközlistát tartalmazó CSV-fájl feltöltése** lapon egy mintafájlt is letölthet. 
    
4. A **Profil hozzárendelése** lapon választhat egy meglévő profilt, vagy létrehozhat egy újat. Ha még nem rendelkezik ilyen, a rendszer kéri, hogy hozzon létre egyet. 
    
    A profil azoknak a beállításoknak a gyűjteménye, amelyek egyetlen eszközre vagy eszközök csoportjára lehet alkalmazni.
    
    Az alapértelmezett szolgáltatások szükségesek, és automatikusan be vannak állítva. Az alapértelmezett funkciók az alábbiak:
    
    - Hagyja ki a Cortanát, a OneDrive-ot és az OEM-regisztrációt.
    
    - Bejelentkezés céges márkával.
    
    - Csatlakoztassa eszközeit az Azure Active Directory-fiókokhoz, és automatikusan regisztrálja őket a Microsoft 365 Business Premium által kezelendő szolgáltatásokhoz.
    
    További információt az [AutoPilot-profil beállításai című témakörben](autopilot-profile-settings.md)talál. 
    
5. A további beállítások: **Adatvédelmi beállítások kihagyása** és **Nem léptethető elő a felhasználó a helyi rendszergazdává**. Mindkettő értéke alapértelmezés szerint **Kikapcsolva**. 
    
    Válassza a **Tovább** gombot.
    
6. **A kész eszközazt** jelzi, hogy a létrehozott (vagy választott) profil az eszközök listájának feltöltésével létrehozott eszközcsoportra lesz alkalmazva. A beállítások akkor lépnek érvénybe, amikor a felhasználók legközelebb bejelentkeznek. Válassza a **Bezárás** gombot.
    

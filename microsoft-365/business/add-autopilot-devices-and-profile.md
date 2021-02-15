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
description: Megtudhatja, hogy a Windows AutoPilot használatával hogyan állíthat be új Windows 10-es eszközöket a vállalata számára, hogy készen álljanak az alkalmazottak használatára.
ms.openlocfilehash: f263cc90656ae5e7be1a89e3c7f56bfb2d0e3651
ms.sourcegitcommit: 3b369a44b71540c8b8214ce588a7aa6f47c3bb1e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/04/2021
ms.locfileid: "50099750"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Autopilot-eszközök és -profilok hozzáadása a lépésenkénti útmutatóval

A Windows AutoPilot segítségével új **Windows** 10-es eszközöket állíthat be a vállalata számára, így azok készen állnak a használatra, amikor átadjuk őket az alkalmazottainak.
  
## <a name="device-requirements"></a>Eszközkövetelmények

Az eszközöknek meg kell felelnie az alábbi követelményeknek:
  
- Windows 10 1703-as vagy újabb verzió
    
- Új eszközök, amelyek még nem voltak használhatók a Windows rendszerben
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Eszközök és profilok létrehozása a beállítási útmutató használatával

[![A megjelenő címke figyelmeztet a felügyeleti központ változásaira, további részleteket itt talál: aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Ha még nem hozott létre eszközcsoportokat vagy -profilokat, a legjobb, ha a lépésenként végigvezeti az első lépéseken. Az útmutató használata [](create-and-edit-autopilot-profiles.md) [nélkül](create-and-edit-autopilot-devices.md) is felvehet eszközöket, és profilokat rendelhet hozzájuk. 
  
1. A felügyeleti központ megnyitásához: <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .

2. A bal oldali navigációs ablakban válassza az **Eszközök** \> **AutoPilot lehetőséget.**

    ![A Felügyeleti központban válassza ki az eszközöket, majd az AutoPilotot.](../media/AutoPilot.png)
  
2. Az **AutoPilot lapon** kattintson vagy koppintson az útmutató **indítási parancsára.**
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. A **.csv** fájl feltöltése az eszközök listájával lapon tallózással keresse meg azt a helyet, ahol előkészítette. CSV-fájl, majd **a Tovább megnyitása** \> **gombra.** A fájlnak három fejlécet kell lennie:
    
    - A oszlop: Eszköz sorozatszáma
    
    - B oszlop: Windows-termékazonosító
    
    - C oszlop: Hardverkivonat
    
    Ezeket az információkat a hardvergyártótól kaphatja meg, vagy a [Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) PowerShell-parancsprogrammal létrehozhat egy CSV-fájlt. 
    
    További információ: [Eszközlistát tartalmazó CSV-fájl](https://docs.microsoft.com/microsoft-365/admin/misc/device-list). Az **Eszközlistát tartalmazó CSV-fájl feltöltése** lapon egy mintafájlt is letölthet. 
    
> [!NOTE]
> Ez a parancsprogram WMI segítségével olvassa be az ügyfélnek az eszköz Windows Autopilottal való regisztráláshoz szükséges tulajdonságait. Vegye figyelembe, hogy az eredményül kapott CSV-fájl nem gyűjti össze a Windows-termékazonosító (PKID) értékét, mivel ez nem szükséges az eszközök regisztrálásához, és a PKID null érték a kimeneti CSV-fájlban teljesen rendben van. Csak a sorozatszámot és a hardveres kivonatot tölti ki a rendszer.
    
4. A Profil **hozzárendelése lapon** választhat egy meglévő profilt, vagy létrehozhat egy újat. Ha még nincs ilyen üzenete, a rendszer kérni fogja, hogy hozzon létre egyet. 
    
    A profil azoknak a beállításoknak a gyűjteménye, amelyek egyetlen eszközre vagy eszközök csoportjára lehet alkalmazni.
    
    Az alapértelmezett funkciók kötelezők, és automatikusan be vannak állítva. Az alapértelmezett funkciók az alábbiak:
    
    - Kihagyhatja Cortanát, a OneDrive-ot és az OEM-regisztrációt.
    
    - Bejelentkezés céges márkával.
    
    - Csatlakoztassa az eszközeit az Azure Active Directory-fiókokhoz, és automatikusan regisztrálja őket a Microsoft 365 Business Premium által kezelt fiókokra.
    
    További információ: [Az AutoPilot-profil beállításai.](autopilot-profile-settings.md) 
    
5. A további beállítások: **Adatvédelmi beállítások kihagyása** és **Nem léptethető elő a felhasználó a helyi rendszergazdává**. Mindkettő értéke alapértelmezés szerint **Kikapcsolva**. 
    
    Válassza a **Tovább** gombot.
    
6. **Ha végzett,** az azt jelenti, hogy a létrehozott (vagy kiválasztott) profilt a rendszer az eszközlista feltöltésével létrehozott eszközcsoportra alkalmazza. A beállítások akkor lépnek életbe, amikor az eszköz felhasználói legközelebb bejelentkeznek. Válassza a **Bezárás** gombot.
    

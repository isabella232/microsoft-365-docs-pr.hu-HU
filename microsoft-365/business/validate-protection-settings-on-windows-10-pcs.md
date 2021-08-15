---
title: Appvédelmi beállítások érvényességének ellenőrzése Windows 10-es PC-ken
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Érvényesítse Microsoft 365 Vállalati prémium verzió appvédelmi beállításokat Windows 10 eszközökön, és ellenőrizze, hogy a felhasználók nem másolnak-e céges adatokat személyes fájlokba vagy nem felügyelt alkalmazásokba.
ms.openlocfilehash: ab084ded5ef052a7b85839f0debb96eb1bc5bdf332230293613396825c7263f0
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53861718"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Appvédelmi beállítások érvényességének ellenőrzése Windows 10-es PC-ken

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Meggyőződés arról, hogy a felhasználók nem tudnak céges adatokat másolni a vállalati eszközökön megtalálható személyes fájlokba

Miután [beállította az appvédelmi házirendeket](protection-settings-for-windows-10-devices.md), néhány óra is eltelhet, amíg a szabályzatok érvénybe lépnek a felhasználók eszközein. Ha be  van kapcsolva A felhasználók nem másolhat céges adatokat személyes fájlokba, és kényszerítheti őket **arra,** hogy munkahelyi fájlokat mentsenek egy vállalati tulajdonú eszközökre vonatkozó beállításba, ezt OneDrive Vállalati verzió felhasználó eszközén ellenőrizheti, miután csatlakoztak az Azure AD-hez, és bejelentkeztek. 
  
 **A kapcsolat beállításainak ellenőrzése**
  
1. Miután bejelentkezett az Microsoft 365 Vállalati prémium verzió-hitelesítő adataival, és csatlakozott az Azure AD-hez az Windows-eszközök beállítása Microsoft 365 Vállalati prémium verzió-felhasználók számára leírásának leírtak [szerint,](set-up-windows-devices.md)lépjen a **Windows Gépház-fiókok** elérése munkahelyi vagy iskolai \>  \> **környezetbe.** Válassza **a Csatlakoztatva \<tenant name\> az Azure AD-hez ,** majd az Információ **lehetőséget.**
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. A **Kezeltek lapon** láthatja azokat a kapcsolati adatokat, amelyek tartalmaznak egy Felügyeleti kiszolgáló címét, az alábbi \<tenant name\> ábrán láthatóhoz hasonló módon.   
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Annak ellenőrzése, hogy nem lehet-e beilleszteni céges adatokat egy nem felügyelt appba**
  
1. Nyissa Outlook 2016 telepített Microsoft 365 Vállalati prémium verzió.
    
2. Nyisson meg egy e-mailt, és másoljon belőle tartalmat a vágólapra.
    
    Nyissa meg a Jegyzettömböt, és kísérelje meg beilleszteni a vágólapra másolt tartalmat.
    
    Hibaüzenet jelenik meg, amely szerint az app nem tud hozzáférni a tartalomhoz.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    A Word 2016-ba azonban beillesztheti a szóban forgó tartalmat.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Meggyőződés arról, hogy a felhasználók nem tudnak céges adatokat másolni a személyes eszközökön megtalálható személyes fájlokba

 **A kapcsolat beállításainak ellenőrzése**
  
1. A Windows 10 eszközén, amelybe helyi felhasználóként van bejelentkezve, válassza a **Windows Gépház**, majd  kattintson vagy koppintson a Fiókok hozzáférése munkahelyi vagy iskolai \> **fiókhoz elemre.**
    
2. A **Hozzáférés munkahelyi vagy iskolai rendszerhez** csoportban válassza a **Csatlakozás** elemet.
    
3. Adja meg Microsoft 365 Vállalati prémium verzió hitelesítő adatait a Munkahelyi vagy iskolai fiók **beállítása** \> **párbeszédpanelEn jelentkezzen be.**
    
4. A **Munkahelyi vagy iskolai hozzáférés** lapon válassza a **Munkahelyi vagy iskolai fiók** lehetőséget, majd az **Információ** elemet.
    
    ![Kattintson vagy koppintson az Információ elemre a Munkahelyi vagy iskolai fiók párbeszédpanelen.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. A **Munkahelyi vagy** iskolai hozzáférés lapon  láthatja **a** Kapcsolati adatok lapot, amely tartalmazza a felügyeleti kiszolgáló címét az alábbi ábrán látható módon, és tartalmazza a *wip* és *a mam* szót is. 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Annak ellenőrzése, hogy nem lehet-e beilleszteni céges adatokat egy nem felügyelt appba**
  
1. Nyissa Outlook 2016 a Microsoft 365 Vállalati prémium verzió, vegye fel a Microsoft 365 Vállalati prémium verzió fiókját, és jelentkezzen be a Microsoft 365 Vállalati prémium verzió hitelesítő adataival.
    
2. Nyisson meg egy e-mailt, és másoljon belőle tartalmat a vágólapra.
    
    Nyissa meg a Jegyzettömböt, és kísérelje meg beilleszteni a vágólapra másolt tartalmat.
    
    Hibaüzenet jelenik meg, amely szerint az app nem tud hozzáférni a tartalomhoz.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    A Word 2016-ba azonban beillesztheti a szóban forgó tartalmat.
    


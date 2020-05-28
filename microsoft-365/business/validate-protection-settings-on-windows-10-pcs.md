---
title: Appvédelmi beállítások érvényességének ellenőrzése Windows 10-es PC-ken
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
description: Ellenőrizze a Microsoft 365 Business Premium alkalmazásvédelmi beállításait Windows 10-es eszközökön, és ellenőrizze, hogy a felhasználók nem másolhatnak-e vállalati adatokat személyes fájlokba vagy nem felügyelt alkalmazásokba.
ms.openlocfilehash: 589d2fc25cc1425a775523595881660cc03e152e
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403390"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Appvédelmi beállítások érvényességének ellenőrzése Windows 10-es PC-ken

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Meggyőződés arról, hogy a felhasználók nem tudnak céges adatokat másolni a vállalati eszközökön megtalálható személyes fájlokba

Miután [beállította az appvédelmi házirendeket](protection-settings-for-windows-10-devices.md), néhány óra is eltelhet, amíg a szabályzatok érvénybe lépnek a felhasználók eszközein. Ha bekapcsolta **a** **Felhasználók személyes fájlokba másolásának megakadályozása, és kényszeríti őket arra, hogy munkafájlokat mentsenek** a vállalati tulajdonú eszközök OneDrive Vállalati verzióbeállítására, ezt ellenőrizheti a felhasználó eszközén, miután csatlakozott az Azure AD-hez, és bejelentkezett. 
  
 **A kapcsolat beállításainak ellenőrzése**
  
1. Miután bejelentkezett a Microsoft 365 Business Premium hitelesítő adatokkal, és csatlakozott az Azure AD-hez a [Windows-eszközök beállítása Microsoft 365 Business Premium-felhasználók számára című](set-up-windows-devices.md)részben leírtak szerint, nyissa meg a **Windows Beállítások** \> **fiókok** \> **elérése munkahelyi vagy iskolai verziót.** Válassza **a Connected to Azure AD (Csatlakozás az Azure \<tenant name\> AD-hez**) lehetőséget, majd az **Információ**lehetőséget.
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. A **Felügyelt kezelés** \<tenant name\> lapon az alábbi ábrán **láthatóhoz** hasonló felügyeleti kiszolgálócímet tartalmazó **kapcsolati adatok** láthatók. 
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Annak ellenőrzése, hogy nem lehet-e vállalati adatokat beilleszteni egy nem felügyelt alkalmazásba**
  
1. Nyissa meg a Microsoft 365 Business Premium által telepített Outlook 2016-ot.
    
2. Nyisson meg egy e-mailt, és másoljon belőle tartalmat a vágólapra.
    
    Nyissa meg a Jegyzettömböt, és kísérelje meg beilleszteni a vágólapra másolt tartalmat.
    
    Hibaüzenet et fog kapni, amely szerint az alkalmazás nem tud hozzáférni a tartalomhoz.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    A Word 2016-ba azonban beillesztheti a szóban forgó tartalmat.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Meggyőződés arról, hogy a felhasználók nem tudnak céges adatokat másolni a személyes eszközökön megtalálható személyes fájlokba

 **A kapcsolat beállításainak ellenőrzése**
  
1. A Windows 10-es személyes eszközén, ahol helyi felhasználóként van bejelentkezve, nyissa meg a **Windows beállításai**lehetőséget, és koppintson a **Fiókok** elérése munkahelyi \> **vagy iskolai**elemre.
    
2. A **Hozzáférés munkahelyi vagy iskolai rendszerhez** csoportban válassza a **Csatlakozás** elemet.
    
3. Adja meg a Microsoft 365 Vállalati Prémium verzió hitelesítő adatait a **Munkahelyi vagy iskolai fiók beállítása** \> **párbeszédpanelen Jelentkezzen be.**
    
4. A **Munkahelyi vagy iskolai hozzáférés** lapon válassza a **Munkahelyi vagy iskolai fiók** lehetőséget, majd az **Információ** elemet.
    
    ![Kattintson vagy koppintson az Információ elemre a Munkahelyi vagy iskolai fiók párbeszédpanelen.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. Az **Access munkahelyi vagy iskolai** lapján láthatja a **Kapcsolat adatait,** amely tartalmazza a **felügyeleti kiszolgáló címét,** mint az alábbi ábrán látható címet, és magában foglalja a *wip* és *az mam* szavakat. 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Annak ellenőrzése, hogy nem lehet-e vállalati adatokat beilleszteni egy nem felügyelt alkalmazásba**
  
1. Nyissa meg az Outlook 2016-ot, és szükség esetén adja hozzá Microsoft 365 Vállalati Prémium verziós fiókját, és jelentkezzen be microsoft 365 Vállalati prémium szintű hitelesítő adataival.
    
2. Nyisson meg egy e-mailt, és másoljon belőle tartalmat a vágólapra.
    
    Nyissa meg a Jegyzettömböt, és kísérelje meg beilleszteni a vágólapra másolt tartalmat.
    
    Hibaüzenet jelenik meg, amely szerint az alkalmazás nem tud hozzáférni a tartalomhoz.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    A Word 2016-ba azonban beillesztheti a szóban forgó tartalmat.
    


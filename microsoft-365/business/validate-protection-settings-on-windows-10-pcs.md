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
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Megtudhatja, hogy miként ellenőrizheti a Microsoft 365 Vállalati alkalmazásvédelmi beállításait A Windows 10-es eszközökön.
ms.openlocfilehash: 577921f7f33eafbbe652dcf825a145d89f1ff556
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/15/2020
ms.locfileid: "42057261"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Appvédelmi beállítások érvényességének ellenőrzése Windows 10-es PC-ken

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Meggyőződés arról, hogy a felhasználók nem tudnak céges adatokat másolni a vállalati eszközökön megtalálható személyes fájlokba

Miután [beállította az appvédelmi házirendeket](protection-settings-for-windows-10-devices.md), néhány óra is eltelhet, amíg a szabályzatok érvénybe lépnek a felhasználók eszközein. Ha bekapcsolta **a** **Vállalati adatok személyes fájlokba másolásának megakadályozása beállítást, és arra kényszeríti őket, hogy munkahelyi fájlokat mentsenek** a OneDrive Vállalati verzióba vállalati tulajdonú eszközökhöz, ezt ellenőrizheti a felhasználó eszközén, miután csatlakoztak az Azure AD-hez, és bejelentkeztek. 
  
 **A kapcsolat beállításainak ellenőrzése**
  
1. After you sign in with Microsoft 365 Business credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**. Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. A **Bérlő által** \<\> kezelt név lapon láthatja a **Kapcsolat adatait,** amely az alábbi ábrán láthatóhoz hasonló **felügyeleti kiszolgálócímet** tartalmaz. 
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Annak ellenőrzése, hogy nem tud-e vállalati adatokat beilleszteni egy nem felügyelt alkalmazásban**
  
1. Nyissa meg a Microsoft 365 Business által telepített Outlook 2016-ot.
    
2. Nyisson meg egy e-mailt, és másoljon belőle tartalmat a vágólapra.
    
    Nyissa meg a Jegyzettömböt, és kísérelje meg beilleszteni a vágólapra másolt tartalmat.
    
    Hibaüzenet jelenik meg, amely szerint az alkalmazás nem tud hozzáférni a tartalomhoz.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    A Word 2016-ba azonban beillesztheti a szóban forgó tartalmat.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Meggyőződés arról, hogy a felhasználók nem tudnak céges adatokat másolni a személyes eszközökön megtalálható személyes fájlokba

 **A kapcsolat beállításainak ellenőrzése**
  
1. A Windows 10-es személyes eszközén, ahol helyi felhasználóként van bejelentkezve, nyissa meg a **Windows-beállítások**lapot, és koppintson vagy koppintson vagy koppintson a **Fiókok** \> **elérése munkahelyi vagy iskolai elemre.**
    
2. A **Hozzáférés munkahelyi vagy iskolai rendszerhez** csoportban válassza a **Csatlakozás** elemet.
    
3. Írja be a Microsoft 365 Business hitelesítő adatait a **Munkahelyi vagy iskolai fiók beállítása** \> **Bejelentkezés** lehetőséget választva.
    
4. A **Munkahelyi vagy iskolai hozzáférés** lapon válassza a **Munkahelyi vagy iskolai fiók** lehetőséget, majd az **Információ** elemet.
    
    ![Kattintson vagy koppintson az Információ elemre a Munkahelyi vagy iskolai fiók párbeszédpanelen.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. Az **Access munka vagy iskola** lapon megtekintheti a **Kapcsolat adatait,** amely az alábbi ábrán láthatóhoz hasonló **felügyeleti kiszolgálócímet** tartalmaz, és tartalmazza a *wip* és *a mam* szavakat. 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Annak ellenőrzése, hogy nem tud-e vállalati adatokat beilleszteni egy nem felügyelt alkalmazásban**
  
1. Nyissa meg az Outlook 2016-ot, szükség esetén vegye fel Microsoft 365 Business-fiókját, és jelentkezzen be a Microsoft 365 Business hitelesítő adataival.
    
2. Nyisson meg egy e-mailt, és másoljon belőle tartalmat a vágólapra.
    
    Nyissa meg a Jegyzettömböt, és kísérelje meg beilleszteni a vágólapra másolt tartalmat.
    
    Hibaüzenet jelenik meg, amely szerint az Alkalmazás nem fér hozzá a tartalomhoz.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    A Word 2016-ba azonban beillesztheti a szóban forgó tartalmat.
    


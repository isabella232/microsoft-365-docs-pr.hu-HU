---
title: Appvédelmi beállítások érvényességének ellenőrzése Windows 10-es PC-ken
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
description: Útmutató a Microsoft 365 üzleti alkalmazás beállításai Windows 10 eszközök ellenőrzése.
ms.openlocfilehash: 4f1f0993dff0ef8d3f6858a3749e063c7b5579c7
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32279976"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Appvédelmi beállítások érvényességének ellenőrzése Windows 10-es PC-ken

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Meggyőződés arról, hogy a felhasználók nem tudnak céges adatokat másolni a vállalati eszközökön megtalálható személyes fájlokba

Miután [beállította az appvédelmi házirendeket](protection-settings-for-windows-10-devices.md), néhány óra is eltelhet, amíg a szabályzatok érvénybe lépnek a felhasználók eszközein. Ha **A felhasználók nem másolhatnak céges adatokat saját fájljaikba, a munkahelyi fájlokat pedig csak a OneDrive Vállalati verzióba menthetik** beállítát **Be** értékre állította a cég tulajdonában álló eszközökhöz, a beállítást ellenőrizheti a felhasználó eszközén, miután az illető csatlakozott az Azure AD szolgáltatáshoz, és bejelentkezett. 
  
 **A kapcsolat beállításainak ellenőrzése**
  
1. After you sign in with Microsoft 365 Business credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**. Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.
    
    ![Click or tap Info on the Connected to Azure AD dialog.](media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. A **Kezeli:** \<bérlő neve\> lapon láthatja a **Kapcsolatadatok** csoportot, amelyben, az alábbi ábrán látható módon megjelenik a **Felügyeleti kiszolgáló címe**. 
    
    ![Managed by page shows connection info of the device manager URL.](media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Meggyőződés arról, hogy nem lehet beilleszteni céges adatokat a nem kezelt appokba**
  
1. Nyissa meg a Microsoft 365 Business által telepített Outlook 2016-ot.
    
2. Nyisson meg egy e-mailt, és másoljon belőle tartalmat a vágólapra.
    
    Nyissa meg a Jegyzettömböt, és kísérelje meg beilleszteni a vágólapra másolt tartalmat.
    
    Ekkor egy hibaüzenet jelenik meg, amely szerint az app nem tud hozzáférni a tartalomhoz.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    A Word 2016-ba azonban beillesztheti a szóban forgó tartalmat.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Meggyőződés arról, hogy a felhasználók nem tudnak céges adatokat másolni a személyes eszközökön megtalálható személyes fájlokba

 **A kapcsolat beállításainak ellenőrzése**
  
1. On your Windows 10 personal device where you are logged in as a local user, go to **Windows Settings** and click or tap **Accounts** \> **Access work or school**.
    
2. A **Hozzáférés munkahelyi vagy iskolai rendszerhez** csoportban válassza a **Csatlakozás** elemet.
    
3. Írja be a Microsoft 365 Business hitelesítő adatait a **Munkahelyi vagy iskolai fiók beállítása** \> **Bejelentkezés** lehetőséget választva.
    
4. A **Munkahelyi vagy iskolai hozzáférés** lapon válassza a **Munkahelyi vagy iskolai fiók** lehetőséget, majd az **Információ** elemet.
    
    ![Click or tap Info on the Work or school account dalog.](media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. A **Hozzáférés munkahelyi vagy iskolai rendszerhez** lapon láthatja a **Kapcsolatadatok** csoportot, amelyben, az alábbi ábrán látható módon megjelenik a **Felügyeleti kiszolgáló címe**, és a címben szerepel a  *wip*  és a  *mam*  szó. 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Meggyőződés arról, hogy nem lehet beilleszteni céges adatokat a nem kezelt appokba**
  
1. Nyissa meg az Outlook 2016-ot, szükség esetén vegye fel Microsoft 365 Business-fiókját, és jelentkezzen be a Microsoft 365 Business hitelesítő adataival.
    
2. Nyisson meg egy e-mailt, és másoljon belőle tartalmat a vágólapra.
    
    Nyissa meg a Jegyzettömböt, és kísérelje meg beilleszteni a vágólapra másolt tartalmat.
    
    Ekkor egy hibaüzenet jelenik meg, amely szerint az app nem tud hozzáférni a tartalomhoz.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    A Word 2016-ba azonban beillesztheti a szóban forgó tartalmat.
    


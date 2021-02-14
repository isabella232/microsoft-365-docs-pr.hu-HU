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
description: Érvényesítse a Microsoft 365 Vállalati prémium verzió appvédelmi beállításait Windows 10-es eszközökön, és ellenőrizze, hogy a felhasználók nem másolnak-e céges adatokat személyes fájlokba vagy nem felügyelt alkalmazásokba.
ms.openlocfilehash: 589d2fc25cc1425a775523595881660cc03e152e
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403390"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Appvédelmi beállítások érvényességének ellenőrzése Windows 10-es PC-ken

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Meggyőződés arról, hogy a felhasználók nem tudnak céges adatokat másolni a vállalati eszközökön megtalálható személyes fájlokba

Miután [beállította az appvédelmi házirendeket](protection-settings-for-windows-10-devices.md), néhány óra is eltelhet, amíg a szabályzatok érvénybe lépnek a felhasználók eszközein. Ha bekapcsolta a "Felhasználók megakadályozása abban, hogy a céges adatokat személyes fájlokba másolják, és kényszerítsék őket arra, hogy a munkahelyi fájlokat a **OneDrive** Vállalati verzióba mentsék a vállalati tulajdonú eszközökre" beállítást, ezt a felhasználó eszközén ellenőrizheti, miután csatlakoztak az Azure AD-hez, és bejelentkeztek.  
  
 **A kapcsolat beállításainak ellenőrzése**
  
1. Miután bejelentkezett a Microsoft 365 Vállalati prémium verzió hitelesítő adataival, és csatlakozott az Azure AD-hez a [Windows-eszközök beállítása a Microsoft 365 Vállalati prémium](set-up-windows-devices.md)verzió felhasználóinak leírásának leírásával, lépjen a **Windows** Settings Accounts Access munkahelyi vagy iskolai \>  \> lapra. Válassza **a Csatlakoztatva \<tenant name\> az Azure AD-hez** lehetőséget, majd az **Információ lehetőséget.**
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. A **Kezeltek lapon** láthatja azokat a kapcsolati adatokat, amelyek egy felügyeleti kiszolgáló címét tartalmazzák, az alábbi \<tenant name\> ábrán láthatóhoz hasonló módon.   
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Annak ellenőrzése, hogy nem lehet-e vállalati adatokat beilleszteni egy nem felügyelt appba**
  
1. Nyissa meg a Microsoft 365 Vállalati prémium verzió által telepített Outlook 2016-ot.
    
2. Nyisson meg egy e-mailt, és másoljon belőle tartalmat a vágólapra.
    
    Nyissa meg a Jegyzettömböt, és kísérelje meg beilleszteni a vágólapra másolt tartalmat.
    
    Hibaüzenet jelenik meg, amely szerint az alkalmazás nem tud hozzáférni a tartalmakhoz.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    A Word 2016-ba azonban beillesztheti a szóban forgó tartalmat.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Meggyőződés arról, hogy a felhasználók nem tudnak céges adatokat másolni a személyes eszközökön megtalálható személyes fájlokba

 **A kapcsolat beállításainak ellenőrzése**
  
1. A Windows 10-es személyes eszközén, amelybe helyi felhasználóként van bejelentkezve,  válassza a **Windows** beállításai lehetőséget, és kattintson vagy koppintson a Fiókok hozzáférése munkahelyi vagy iskolai \> **fiókra.**
    
2. A **Hozzáférés munkahelyi vagy iskolai rendszerhez** csoportban válassza a **Csatlakozás** elemet.
    
3. Adja meg a Microsoft 365 Vállalati prémium verziós hitelesítő adatait **a** Munkahelyi vagy iskolai fiók beállítása \> **párbeszédpanelen.**
    
4. A **Munkahelyi vagy iskolai hozzáférés** lapon válassza a **Munkahelyi vagy iskolai fiók** lehetőséget, majd az **Információ** elemet.
    
    ![Kattintson vagy koppintson a Munkahelyi vagy iskolai fiók párbeszédpanel Információ gombjára.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. Az **Access** munkahelyi vagy iskolai lapján  láthatja **azokat** a kapcsolati adatokat, amelyek tartalmaznak egy felügyeleti kiszolgáló címét, az alábbi ábrán láthatóhoz hasonlót, valamint a *wip* és *a mam* szót. 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Annak ellenőrzése, hogy nem lehet-e vállalati adatokat beilleszteni egy nem felügyelt appba**
  
1. Nyissa meg az Outlook 2016-ot, és szükség esetén vegye fel a Microsoft 365 Vállalati prémium verziós fiókját, és jelentkezzen be a Microsoft 365 Vállalati prémium verziós hitelesítő adataival.
    
2. Nyisson meg egy e-mailt, és másoljon belőle tartalmat a vágólapra.
    
    Nyissa meg a Jegyzettömböt, és kísérelje meg beilleszteni a vágólapra másolt tartalmat.
    
    Hibaüzenet jelenik meg, amely szerint az app nem tud hozzáférni a tartalomhoz.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    A Word 2016-ba azonban beillesztheti a szóban forgó tartalmat.
    


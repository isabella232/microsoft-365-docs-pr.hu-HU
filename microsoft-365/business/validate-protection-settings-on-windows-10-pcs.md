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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Ellenőrizze a Microsoft 365 Vállalati alkalmazásvédelmi beállításokat Windows 10-es eszközökön, és ellenőrizze, hogy a felhasználók nem másolhatnak vállalati adatokat személyes fájlokba vagy nem felügyelt alkalmazásokba.
ms.openlocfilehash: 4d3d7e950311ac32606e700ebb35bf026ae091cc
ms.sourcegitcommit: 26e4d5091583765257b7533b5156daa373cd19fe
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/06/2020
ms.locfileid: "42549997"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="ac608-103">Appvédelmi beállítások érvényességének ellenőrzése Windows 10-es PC-ken</span><span class="sxs-lookup"><span data-stu-id="ac608-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="ac608-104">Meggyőződés arról, hogy a felhasználók nem tudnak céges adatokat másolni a vállalati eszközökön megtalálható személyes fájlokba</span><span class="sxs-lookup"><span data-stu-id="ac608-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="ac608-105">Miután [beállította az appvédelmi házirendeket](protection-settings-for-windows-10-devices.md), néhány óra is eltelhet, amíg a szabályzatok érvénybe lépnek a felhasználók eszközein.</span><span class="sxs-lookup"><span data-stu-id="ac608-105">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="ac608-106">Ha bekapcsolta **a** **Vállalati adatok személyes fájlokba másolásának megakadályozása beállítást, és arra kényszeríti őket, hogy munkahelyi fájlokat mentsenek** a OneDrive Vállalati verzióba vállalati tulajdonú eszközökhöz, ezt ellenőrizheti a felhasználó eszközén, miután csatlakoztak az Azure AD-hez, és bejelentkeztek.</span><span class="sxs-lookup"><span data-stu-id="ac608-106">If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they've connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="ac608-107">**A kapcsolat beállításainak ellenőrzése**</span><span class="sxs-lookup"><span data-stu-id="ac608-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="ac608-p102">After you sign in with Microsoft 365 Business credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**. Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span><span class="sxs-lookup"><span data-stu-id="ac608-p102">After you sign in with Microsoft 365 Business credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**. Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="ac608-111">A **Bérlő által** \<\> kezelt név lapon láthatja a **Kapcsolat adatait,** amely az alábbi ábrán láthatóhoz hasonló **felügyeleti kiszolgálócímet** tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="ac608-111">On the **Managed by** \<tenant name\> page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="ac608-113">**Annak ellenőrzése, hogy nem tud-e vállalati adatokat beilleszteni egy nem felügyelt alkalmazásban**</span><span class="sxs-lookup"><span data-stu-id="ac608-113">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="ac608-114">Nyissa meg a Microsoft 365 Business által telepített Outlook 2016-ot.</span><span class="sxs-lookup"><span data-stu-id="ac608-114">Open Outlook 2016 that was installed by Microsoft 365 Business.</span></span>
    
2. <span data-ttu-id="ac608-115">Nyisson meg egy e-mailt, és másoljon belőle tartalmat a vágólapra.</span><span class="sxs-lookup"><span data-stu-id="ac608-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="ac608-116">Nyissa meg a Jegyzettömböt, és kísérelje meg beilleszteni a vágólapra másolt tartalmat.</span><span class="sxs-lookup"><span data-stu-id="ac608-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="ac608-117">Hibaüzenet jelenik meg, amely szerint az alkalmazás nem tud hozzáférni a tartalomhoz.</span><span class="sxs-lookup"><span data-stu-id="ac608-117">You'll receive an error that states the app can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="ac608-119">A Word 2016-ba azonban beillesztheti a szóban forgó tartalmat.</span><span class="sxs-lookup"><span data-stu-id="ac608-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="ac608-120">Meggyőződés arról, hogy a felhasználók nem tudnak céges adatokat másolni a személyes eszközökön megtalálható személyes fájlokba</span><span class="sxs-lookup"><span data-stu-id="ac608-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="ac608-121">**A kapcsolat beállításainak ellenőrzése**</span><span class="sxs-lookup"><span data-stu-id="ac608-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="ac608-122">A Windows 10-es személyes eszközén, ahol helyi felhasználóként van bejelentkezve, nyissa meg a **Windows-beállítások**lapot, és koppintson vagy koppintson vagy koppintson a **Fiókok** \> **elérése munkahelyi vagy iskolai elemre.**</span><span class="sxs-lookup"><span data-stu-id="ac608-122">On your Windows 10 personal device where you're logged in as a local user, go to **Windows Settings**, and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="ac608-123">A **Hozzáférés munkahelyi vagy iskolai rendszerhez** csoportban válassza a **Csatlakozás** elemet.</span><span class="sxs-lookup"><span data-stu-id="ac608-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="ac608-124">Írja be a Microsoft 365 Business hitelesítő adatait a **Munkahelyi vagy iskolai fiók beállítása** \> **Bejelentkezés** lehetőséget választva.</span><span class="sxs-lookup"><span data-stu-id="ac608-124">Enter your Microsoft 365 Business credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="ac608-125">A **Munkahelyi vagy iskolai hozzáférés** lapon válassza a **Munkahelyi vagy iskolai fiók** lehetőséget, majd az **Információ** elemet.</span><span class="sxs-lookup"><span data-stu-id="ac608-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![Kattintson vagy koppintson az Információ elemre a Munkahelyi vagy iskolai fiók párbeszédpanelen.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="ac608-127">Az **Access munka vagy iskola** lapon megtekintheti a **Kapcsolat adatait,** amely az alábbi ábrán láthatóhoz hasonló **felügyeleti kiszolgálócímet** tartalmaz, és tartalmazza a *wip* és *a mam* szavakat.</span><span class="sxs-lookup"><span data-stu-id="ac608-127">On the **Access work or school** page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="ac608-129">**Annak ellenőrzése, hogy nem tud-e vállalati adatokat beilleszteni egy nem felügyelt alkalmazásban**</span><span class="sxs-lookup"><span data-stu-id="ac608-129">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="ac608-130">Nyissa meg az Outlook 2016-ot, szükség esetén vegye fel Microsoft 365 Business-fiókját, és jelentkezzen be a Microsoft 365 Business hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="ac608-130">Open Outlook 2016 and add your Microsoft 365 Business account if necessary and sign in with your Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="ac608-131">Nyisson meg egy e-mailt, és másoljon belőle tartalmat a vágólapra.</span><span class="sxs-lookup"><span data-stu-id="ac608-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="ac608-132">Nyissa meg a Jegyzettömböt, és kísérelje meg beilleszteni a vágólapra másolt tartalmat.</span><span class="sxs-lookup"><span data-stu-id="ac608-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="ac608-133">Hibaüzenet jelenik meg, amely szerint az Alkalmazás nem fér hozzá a tartalomhoz.</span><span class="sxs-lookup"><span data-stu-id="ac608-133">You'll receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="ac608-135">A Word 2016-ba azonban beillesztheti a szóban forgó tartalmat.</span><span class="sxs-lookup"><span data-stu-id="ac608-135">You can, however, paste the same content into Word 2016.</span></span>
    


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
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="6da0b-103">Appvédelmi beállítások érvényességének ellenőrzése Windows 10-es PC-ken</span><span class="sxs-lookup"><span data-stu-id="6da0b-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="6da0b-104">Meggyőződés arról, hogy a felhasználók nem tudnak céges adatokat másolni a vállalati eszközökön megtalálható személyes fájlokba</span><span class="sxs-lookup"><span data-stu-id="6da0b-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="6da0b-p101">Miután [beállította az appvédelmi házirendeket](protection-settings-for-windows-10-devices.md), néhány óra is eltelhet, amíg a szabályzatok érvénybe lépnek a felhasználók eszközein. Ha **A felhasználók nem másolhatnak céges adatokat saját fájljaikba, a munkahelyi fájlokat pedig csak a OneDrive Vállalati verzióba menthetik** beállítát **Be** értékre állította a cég tulajdonában álló eszközökhöz, a beállítást ellenőrizheti a felhasználó eszközén, miután az illető csatlakozott az Azure AD szolgáltatáshoz, és bejelentkezett.</span><span class="sxs-lookup"><span data-stu-id="6da0b-p101">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices. If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they have connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="6da0b-107">**A kapcsolat beállításainak ellenőrzése**</span><span class="sxs-lookup"><span data-stu-id="6da0b-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="6da0b-p102">After you sign in with Microsoft 365 Business credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**. Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span><span class="sxs-lookup"><span data-stu-id="6da0b-p102">After you sign in with Microsoft 365 Business credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**. Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="6da0b-111">A **Kezeli:** \<bérlő neve\> lapon láthatja a **Kapcsolatadatok** csoportot, amelyben, az alábbi ábrán látható módon megjelenik a **Felügyeleti kiszolgáló címe**.</span><span class="sxs-lookup"><span data-stu-id="6da0b-111">On the **Managed by** \<tenant name\> page you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="6da0b-113">**Meggyőződés arról, hogy nem lehet beilleszteni céges adatokat a nem kezelt appokba**</span><span class="sxs-lookup"><span data-stu-id="6da0b-113">**Verify that you cannot paste company data to a non-managed app**</span></span>
  
1. <span data-ttu-id="6da0b-114">Nyissa meg a Microsoft 365 Business által telepített Outlook 2016-ot.</span><span class="sxs-lookup"><span data-stu-id="6da0b-114">Open Outlook 2016 that was installed by Microsoft 365 Business.</span></span>
    
2. <span data-ttu-id="6da0b-115">Nyisson meg egy e-mailt, és másoljon belőle tartalmat a vágólapra.</span><span class="sxs-lookup"><span data-stu-id="6da0b-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="6da0b-116">Nyissa meg a Jegyzettömböt, és kísérelje meg beilleszteni a vágólapra másolt tartalmat.</span><span class="sxs-lookup"><span data-stu-id="6da0b-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="6da0b-117">Ekkor egy hibaüzenet jelenik meg, amely szerint az app nem tud hozzáférni a tartalomhoz.</span><span class="sxs-lookup"><span data-stu-id="6da0b-117">You will receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="6da0b-119">A Word 2016-ba azonban beillesztheti a szóban forgó tartalmat.</span><span class="sxs-lookup"><span data-stu-id="6da0b-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="6da0b-120">Meggyőződés arról, hogy a felhasználók nem tudnak céges adatokat másolni a személyes eszközökön megtalálható személyes fájlokba</span><span class="sxs-lookup"><span data-stu-id="6da0b-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="6da0b-121">**A kapcsolat beállításainak ellenőrzése**</span><span class="sxs-lookup"><span data-stu-id="6da0b-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="6da0b-122">On your Windows 10 personal device where you are logged in as a local user, go to **Windows Settings** and click or tap **Accounts** \> **Access work or school**.</span><span class="sxs-lookup"><span data-stu-id="6da0b-122">On your Windows 10 personal device where you are logged in as a local user, go to **Windows Settings** and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="6da0b-123">A **Hozzáférés munkahelyi vagy iskolai rendszerhez** csoportban válassza a **Csatlakozás** elemet.</span><span class="sxs-lookup"><span data-stu-id="6da0b-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="6da0b-124">Írja be a Microsoft 365 Business hitelesítő adatait a **Munkahelyi vagy iskolai fiók beállítása** \> **Bejelentkezés** lehetőséget választva.</span><span class="sxs-lookup"><span data-stu-id="6da0b-124">Enter your Microsoft 365 Business credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="6da0b-125">A **Munkahelyi vagy iskolai hozzáférés** lapon válassza a **Munkahelyi vagy iskolai fiók** lehetőséget, majd az **Információ** elemet.</span><span class="sxs-lookup"><span data-stu-id="6da0b-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Work or school account dalog.](media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="6da0b-127">A **Hozzáférés munkahelyi vagy iskolai rendszerhez** lapon láthatja a **Kapcsolatadatok** csoportot, amelyben, az alábbi ábrán látható módon megjelenik a **Felügyeleti kiszolgáló címe**, és a címben szerepel a  *wip*  és a  *mam*  szó.</span><span class="sxs-lookup"><span data-stu-id="6da0b-127">On the **Access work or school** page you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="6da0b-129">**Meggyőződés arról, hogy nem lehet beilleszteni céges adatokat a nem kezelt appokba**</span><span class="sxs-lookup"><span data-stu-id="6da0b-129">**Verify that you cannot paste company data to a non-managed app**</span></span>
  
1. <span data-ttu-id="6da0b-130">Nyissa meg az Outlook 2016-ot, szükség esetén vegye fel Microsoft 365 Business-fiókját, és jelentkezzen be a Microsoft 365 Business hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="6da0b-130">Open Outlook 2016 and add your Microsoft 365 Business account if necessary and sign in with your Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="6da0b-131">Nyisson meg egy e-mailt, és másoljon belőle tartalmat a vágólapra.</span><span class="sxs-lookup"><span data-stu-id="6da0b-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="6da0b-132">Nyissa meg a Jegyzettömböt, és kísérelje meg beilleszteni a vágólapra másolt tartalmat.</span><span class="sxs-lookup"><span data-stu-id="6da0b-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="6da0b-133">Ekkor egy hibaüzenet jelenik meg, amely szerint az app nem tud hozzáférni a tartalomhoz.</span><span class="sxs-lookup"><span data-stu-id="6da0b-133">You will receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="6da0b-135">A Word 2016-ba azonban beillesztheti a szóban forgó tartalmat.</span><span class="sxs-lookup"><span data-stu-id="6da0b-135">You can, however, paste the same content into Word 2016.</span></span>
    


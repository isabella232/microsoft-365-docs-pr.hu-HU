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
description: Ellenőrizze a Microsoft 365 Vállalati prémium verzió appvédelmi beállításait Windows 10-es eszközökön, és ellenőrizze, hogy a felhasználók nem másolnak-e céges adatokat személyes fájlokba vagy nem felügyelt alkalmazásokba.
ms.openlocfilehash: e319ffa5149f055b5de45078facc8899acffc223
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579862"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="21bd5-103">Appvédelmi beállítások érvényességének ellenőrzése Windows 10-es PC-ken</span><span class="sxs-lookup"><span data-stu-id="21bd5-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="21bd5-104">Meggyőződés arról, hogy a felhasználók nem tudnak céges adatokat másolni a vállalati eszközökön megtalálható személyes fájlokba</span><span class="sxs-lookup"><span data-stu-id="21bd5-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="21bd5-105">Miután [beállította az appvédelmi házirendeket](protection-settings-for-windows-10-devices.md), néhány óra is eltelhet, amíg a szabályzatok érvénybe lépnek a felhasználók eszközein.</span><span class="sxs-lookup"><span data-stu-id="21bd5-105">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="21bd5-106">Ha be  van kapcsolva A felhasználók nem másolhat céges adatokat személyes fájlokba, és kényszerítheti őket arra, hogy a munkahelyi fájlokat a **OneDrive** Vállalati verzióba mentsék a cég tulajdonában álló eszközökre beállítást, akkor ezt ellenőrizheti a felhasználó eszközén, miután csatlakoztak az Azure AD-hez, és bejelentkeztek.</span><span class="sxs-lookup"><span data-stu-id="21bd5-106">If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they've connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="21bd5-107">**A kapcsolat beállításainak ellenőrzése**</span><span class="sxs-lookup"><span data-stu-id="21bd5-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="21bd5-108">Miután bejelentkezett a Microsoft 365 Vállalati prémium verzió hitelesítő adataival, és csatlakozott az Azure AD-hez a Windows-eszközök beállítása [a Microsoft 365 Vállalati prémium](set-up-windows-devices.md)verzió felhasználóinak leírásában leírtak szerint, lépjen a Windows **Settings** Accounts Access munkahelyi vagy iskolai \>  \> webhelyre.</span><span class="sxs-lookup"><span data-stu-id="21bd5-108">After you sign in with Microsoft 365 Business Premium credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**.</span></span> <span data-ttu-id="21bd5-109">Válassza **a Csatlakoztatva \<tenant name\> az Azure AD-hez ,** majd az Információ **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="21bd5-109">Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="21bd5-111">A **Kezeltek lapon** láthatja azokat a kapcsolati adatokat, amelyek tartalmaznak egy Felügyeleti kiszolgáló címét, az alábbi \<tenant name\> ábrán láthatóhoz hasonló módon.  </span><span class="sxs-lookup"><span data-stu-id="21bd5-111">On the **Managed by** \<tenant name\> page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="21bd5-113">**Annak ellenőrzése, hogy nem lehet-e beilleszteni céges adatokat egy nem felügyelt appba**</span><span class="sxs-lookup"><span data-stu-id="21bd5-113">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="21bd5-114">Nyissa meg a Microsoft 365 Vállalati prémium verzió által telepített Outlook 2016-ot.</span><span class="sxs-lookup"><span data-stu-id="21bd5-114">Open Outlook 2016 that was installed by Microsoft 365 Business Premium.</span></span>
    
2. <span data-ttu-id="21bd5-115">Nyisson meg egy e-mailt, és másoljon belőle tartalmat a vágólapra.</span><span class="sxs-lookup"><span data-stu-id="21bd5-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="21bd5-116">Nyissa meg a Jegyzettömböt, és kísérelje meg beilleszteni a vágólapra másolt tartalmat.</span><span class="sxs-lookup"><span data-stu-id="21bd5-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="21bd5-117">Hibaüzenet jelenik meg, amely szerint az app nem tud hozzáférni a tartalomhoz.</span><span class="sxs-lookup"><span data-stu-id="21bd5-117">You'll receive an error that states the app can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="21bd5-119">A Word 2016-ba azonban beillesztheti a szóban forgó tartalmat.</span><span class="sxs-lookup"><span data-stu-id="21bd5-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="21bd5-120">Meggyőződés arról, hogy a felhasználók nem tudnak céges adatokat másolni a személyes eszközökön megtalálható személyes fájlokba</span><span class="sxs-lookup"><span data-stu-id="21bd5-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="21bd5-121">**A kapcsolat beállításainak ellenőrzése**</span><span class="sxs-lookup"><span data-stu-id="21bd5-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="21bd5-122">A Windows 10-es személyes eszközén, amelybe helyi felhasználóként van bejelentkezve,  válassza a **Windows-beállítások** lehetőséget, és kattintson vagy koppintson a Fiókok elérése munkahelyi vagy iskolai \> **fiókra elemre.**</span><span class="sxs-lookup"><span data-stu-id="21bd5-122">On your Windows 10 personal device where you're logged in as a local user, go to **Windows Settings**, and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="21bd5-123">A **Hozzáférés munkahelyi vagy iskolai rendszerhez** csoportban válassza a **Csatlakozás** elemet.</span><span class="sxs-lookup"><span data-stu-id="21bd5-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="21bd5-124">Adja meg Microsoft 365 Vállalati prémium verziós hitelesítő adatait a Munkahelyi vagy iskolai fiók **beállítása** \> **párbeszédpanelEn jelentkezzen be.**</span><span class="sxs-lookup"><span data-stu-id="21bd5-124">Enter your Microsoft 365 Business Premium credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="21bd5-125">A **Munkahelyi vagy iskolai hozzáférés** lapon válassza a **Munkahelyi vagy iskolai fiók** lehetőséget, majd az **Információ** elemet.</span><span class="sxs-lookup"><span data-stu-id="21bd5-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![Kattintson vagy koppintson az Információ elemre a Munkahelyi vagy iskolai fiók párbeszédpanelen.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="21bd5-127">A **Munkahelyi vagy** iskolai hozzáférés lapon  láthatja **a** Kapcsolati adatok lapot, amely tartalmazza a felügyeleti kiszolgáló címét az alábbi ábrán látható módon, és tartalmazza a *wip* és *a mam* szót is.</span><span class="sxs-lookup"><span data-stu-id="21bd5-127">On the **Access work or school** page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="21bd5-129">**Annak ellenőrzése, hogy nem lehet-e beilleszteni céges adatokat egy nem felügyelt appba**</span><span class="sxs-lookup"><span data-stu-id="21bd5-129">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="21bd5-130">Nyissa meg az Outlook 2016-ot, és szükség esetén vegye fel a Microsoft 365 Vállalati prémium verziós fiókját, és jelentkezzen be a Microsoft 365 Vállalati prémium verziós hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="21bd5-130">Open Outlook 2016 and add your Microsoft 365 Business Premium account if necessary and sign in with your Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="21bd5-131">Nyisson meg egy e-mailt, és másoljon belőle tartalmat a vágólapra.</span><span class="sxs-lookup"><span data-stu-id="21bd5-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="21bd5-132">Nyissa meg a Jegyzettömböt, és kísérelje meg beilleszteni a vágólapra másolt tartalmat.</span><span class="sxs-lookup"><span data-stu-id="21bd5-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="21bd5-133">Hibaüzenet jelenik meg, amely szerint az app nem tud hozzáférni a tartalomhoz.</span><span class="sxs-lookup"><span data-stu-id="21bd5-133">You'll receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="21bd5-135">A Word 2016-ba azonban beillesztheti a szóban forgó tartalmat.</span><span class="sxs-lookup"><span data-stu-id="21bd5-135">You can, however, paste the same content into Word 2016.</span></span>
    


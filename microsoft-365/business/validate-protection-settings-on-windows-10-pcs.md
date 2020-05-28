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
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="cef26-103">Appvédelmi beállítások érvényességének ellenőrzése Windows 10-es PC-ken</span><span class="sxs-lookup"><span data-stu-id="cef26-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="cef26-104">Meggyőződés arról, hogy a felhasználók nem tudnak céges adatokat másolni a vállalati eszközökön megtalálható személyes fájlokba</span><span class="sxs-lookup"><span data-stu-id="cef26-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="cef26-105">Miután [beállította az appvédelmi házirendeket](protection-settings-for-windows-10-devices.md), néhány óra is eltelhet, amíg a szabályzatok érvénybe lépnek a felhasználók eszközein.</span><span class="sxs-lookup"><span data-stu-id="cef26-105">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="cef26-106">Ha bekapcsolta **a** **Felhasználók személyes fájlokba másolásának megakadályozása, és kényszeríti őket arra, hogy munkafájlokat mentsenek** a vállalati tulajdonú eszközök OneDrive Vállalati verzióbeállítására, ezt ellenőrizheti a felhasználó eszközén, miután csatlakozott az Azure AD-hez, és bejelentkezett.</span><span class="sxs-lookup"><span data-stu-id="cef26-106">If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they've connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="cef26-107">**A kapcsolat beállításainak ellenőrzése**</span><span class="sxs-lookup"><span data-stu-id="cef26-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="cef26-108">Miután bejelentkezett a Microsoft 365 Business Premium hitelesítő adatokkal, és csatlakozott az Azure AD-hez a [Windows-eszközök beállítása Microsoft 365 Business Premium-felhasználók számára című](set-up-windows-devices.md)részben leírtak szerint, nyissa meg a **Windows Beállítások** \> **fiókok** \> **elérése munkahelyi vagy iskolai verziót.**</span><span class="sxs-lookup"><span data-stu-id="cef26-108">After you sign in with Microsoft 365 Business Premium credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**.</span></span> <span data-ttu-id="cef26-109">Válassza **a Connected to Azure AD (Csatlakozás az Azure \<tenant name\> AD-hez**) lehetőséget, majd az **Információ**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="cef26-109">Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="cef26-111">A **Felügyelt kezelés** \<tenant name\> lapon az alábbi ábrán **láthatóhoz** hasonló felügyeleti kiszolgálócímet tartalmazó **kapcsolati adatok** láthatók.</span><span class="sxs-lookup"><span data-stu-id="cef26-111">On the **Managed by** \<tenant name\> page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="cef26-113">**Annak ellenőrzése, hogy nem lehet-e vállalati adatokat beilleszteni egy nem felügyelt alkalmazásba**</span><span class="sxs-lookup"><span data-stu-id="cef26-113">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="cef26-114">Nyissa meg a Microsoft 365 Business Premium által telepített Outlook 2016-ot.</span><span class="sxs-lookup"><span data-stu-id="cef26-114">Open Outlook 2016 that was installed by Microsoft 365 Business Premium.</span></span>
    
2. <span data-ttu-id="cef26-115">Nyisson meg egy e-mailt, és másoljon belőle tartalmat a vágólapra.</span><span class="sxs-lookup"><span data-stu-id="cef26-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="cef26-116">Nyissa meg a Jegyzettömböt, és kísérelje meg beilleszteni a vágólapra másolt tartalmat.</span><span class="sxs-lookup"><span data-stu-id="cef26-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="cef26-117">Hibaüzenet et fog kapni, amely szerint az alkalmazás nem tud hozzáférni a tartalomhoz.</span><span class="sxs-lookup"><span data-stu-id="cef26-117">You'll receive an error that states the app can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="cef26-119">A Word 2016-ba azonban beillesztheti a szóban forgó tartalmat.</span><span class="sxs-lookup"><span data-stu-id="cef26-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="cef26-120">Meggyőződés arról, hogy a felhasználók nem tudnak céges adatokat másolni a személyes eszközökön megtalálható személyes fájlokba</span><span class="sxs-lookup"><span data-stu-id="cef26-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="cef26-121">**A kapcsolat beállításainak ellenőrzése**</span><span class="sxs-lookup"><span data-stu-id="cef26-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="cef26-122">A Windows 10-es személyes eszközén, ahol helyi felhasználóként van bejelentkezve, nyissa meg a **Windows beállításai**lehetőséget, és koppintson a **Fiókok** elérése munkahelyi \> **vagy iskolai**elemre.</span><span class="sxs-lookup"><span data-stu-id="cef26-122">On your Windows 10 personal device where you're logged in as a local user, go to **Windows Settings**, and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="cef26-123">A **Hozzáférés munkahelyi vagy iskolai rendszerhez** csoportban válassza a **Csatlakozás** elemet.</span><span class="sxs-lookup"><span data-stu-id="cef26-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="cef26-124">Adja meg a Microsoft 365 Vállalati Prémium verzió hitelesítő adatait a **Munkahelyi vagy iskolai fiók beállítása** \> **párbeszédpanelen Jelentkezzen be.**</span><span class="sxs-lookup"><span data-stu-id="cef26-124">Enter your Microsoft 365 Business Premium credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="cef26-125">A **Munkahelyi vagy iskolai hozzáférés** lapon válassza a **Munkahelyi vagy iskolai fiók** lehetőséget, majd az **Információ** elemet.</span><span class="sxs-lookup"><span data-stu-id="cef26-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![Kattintson vagy koppintson az Információ elemre a Munkahelyi vagy iskolai fiók párbeszédpanelen.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="cef26-127">Az **Access munkahelyi vagy iskolai** lapján láthatja a **Kapcsolat adatait,** amely tartalmazza a **felügyeleti kiszolgáló címét,** mint az alábbi ábrán látható címet, és magában foglalja a *wip* és *az mam* szavakat.</span><span class="sxs-lookup"><span data-stu-id="cef26-127">On the **Access work or school** page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="cef26-129">**Annak ellenőrzése, hogy nem lehet-e vállalati adatokat beilleszteni egy nem felügyelt alkalmazásba**</span><span class="sxs-lookup"><span data-stu-id="cef26-129">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="cef26-130">Nyissa meg az Outlook 2016-ot, és szükség esetén adja hozzá Microsoft 365 Vállalati Prémium verziós fiókját, és jelentkezzen be microsoft 365 Vállalati prémium szintű hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="cef26-130">Open Outlook 2016 and add your Microsoft 365 Business Premium account if necessary and sign in with your Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="cef26-131">Nyisson meg egy e-mailt, és másoljon belőle tartalmat a vágólapra.</span><span class="sxs-lookup"><span data-stu-id="cef26-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="cef26-132">Nyissa meg a Jegyzettömböt, és kísérelje meg beilleszteni a vágólapra másolt tartalmat.</span><span class="sxs-lookup"><span data-stu-id="cef26-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="cef26-133">Hibaüzenet jelenik meg, amely szerint az alkalmazás nem tud hozzáférni a tartalomhoz.</span><span class="sxs-lookup"><span data-stu-id="cef26-133">You'll receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="cef26-135">A Word 2016-ba azonban beillesztheti a szóban forgó tartalmat.</span><span class="sxs-lookup"><span data-stu-id="cef26-135">You can, however, paste the same content into Word 2016.</span></span>
    


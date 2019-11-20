---
title: Appvédelmi beállítások érvényességének ellenőrzése Windows 10-es PC-ken
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
description: Útmutató a Microsoft 365 Business app védelmi beállításainak érvényesítéséhez Windows 10 eszközökön.
ms.openlocfilehash: c54b053c1f6efbca8fd02431c416793a044c6821
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38721860"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="ffe05-103">Appvédelmi beállítások érvényességének ellenőrzése Windows 10-es PC-ken</span><span class="sxs-lookup"><span data-stu-id="ffe05-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="ffe05-104">Meggyőződés arról, hogy a felhasználók nem tudnak céges adatokat másolni a vállalati eszközökön megtalálható személyes fájlokba</span><span class="sxs-lookup"><span data-stu-id="ffe05-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="ffe05-105">Miután [beállította az appvédelmi házirendeket](protection-settings-for-windows-10-devices.md), néhány óra is eltelhet, amíg a szabályzatok érvénybe lépnek a felhasználók eszközein.</span><span class="sxs-lookup"><span data-stu-id="ffe05-105">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="ffe05-106">Ha **be van kapcsolva** a **megakadályoz használók-ból másolás társaság adat-hoz személyes fájlokat és kényszerít őket-hoz megment dolgozik fájlokat-hoz Onedrive részére teendő** elintézés részére társaság birtokolt berendezés, tudod ellenőriz ez-on használók ' berendezés után ők ' összekapcsolt-hoz azúrkék hirdetés és aláíró-ban.</span><span class="sxs-lookup"><span data-stu-id="ffe05-106">If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they've connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="ffe05-107">**A kapcsolat beállításainak ellenőrzése**</span><span class="sxs-lookup"><span data-stu-id="ffe05-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="ffe05-p102">After you sign in with Microsoft 365 Business credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**. Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span><span class="sxs-lookup"><span data-stu-id="ffe05-p102">After you sign in with Microsoft 365 Business credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**. Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="ffe05-111">A bérlő **által** \<kezelt név\> lapon megtekintheti a **kapcsolatinformációt** , amely tartalmazza a következő ábrán látható **kezelési kiszolgálócímet** .</span><span class="sxs-lookup"><span data-stu-id="ffe05-111">On the **Managed by** \<tenant name\> page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="ffe05-113">**Annak ellenőrzése, hogy nem lehet beilleszteni vállalati adatokat nem felügyelt alkalmazásba**</span><span class="sxs-lookup"><span data-stu-id="ffe05-113">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="ffe05-114">Nyissa meg a Microsoft 365 Business által telepített Outlook 2016-ot.</span><span class="sxs-lookup"><span data-stu-id="ffe05-114">Open Outlook 2016 that was installed by Microsoft 365 Business.</span></span>
    
2. <span data-ttu-id="ffe05-115">Nyisson meg egy e-mailt, és másoljon belőle tartalmat a vágólapra.</span><span class="sxs-lookup"><span data-stu-id="ffe05-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="ffe05-116">Nyissa meg a Jegyzettömböt, és kísérelje meg beilleszteni a vágólapra másolt tartalmat.</span><span class="sxs-lookup"><span data-stu-id="ffe05-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="ffe05-117">Youll ' kap egy hiba amit Államok a app vidám ' belépés elégedett.</span><span class="sxs-lookup"><span data-stu-id="ffe05-117">You'll receive an error that states the app can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="ffe05-119">A Word 2016-ba azonban beillesztheti a szóban forgó tartalmat.</span><span class="sxs-lookup"><span data-stu-id="ffe05-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="ffe05-120">Meggyőződés arról, hogy a felhasználók nem tudnak céges adatokat másolni a személyes eszközökön megtalálható személyes fájlokba</span><span class="sxs-lookup"><span data-stu-id="ffe05-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="ffe05-121">**A kapcsolat beállításainak ellenőrzése**</span><span class="sxs-lookup"><span data-stu-id="ffe05-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="ffe05-122">A Windows 10 személyes eszközén, ahol helyi felhasználóként jelentkezett be, nyissa meg a **Windows beállításait**, és kattintson vagy koppintson a **fiókokhoz** \> **való hozzáférés vagy az iskola**elemre.</span><span class="sxs-lookup"><span data-stu-id="ffe05-122">On your Windows 10 personal device where you're logged in as a local user, go to **Windows Settings**, and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="ffe05-123">A **Hozzáférés munkahelyi vagy iskolai rendszerhez** csoportban válassza a **Csatlakozás** elemet.</span><span class="sxs-lookup"><span data-stu-id="ffe05-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="ffe05-124">Írja be a Microsoft 365 Business hitelesítő adatait a **Munkahelyi vagy iskolai fiók beállítása** \> **Bejelentkezés** lehetőséget választva.</span><span class="sxs-lookup"><span data-stu-id="ffe05-124">Enter your Microsoft 365 Business credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="ffe05-125">A **Munkahelyi vagy iskolai hozzáférés** lapon válassza a **Munkahelyi vagy iskolai fiók** lehetőséget, majd az **Információ** elemet.</span><span class="sxs-lookup"><span data-stu-id="ffe05-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![Kattintson vagy koppintson a munka vagy az iskolai fiók párbeszédpanelre vonatkozó információk parancsra.](media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="ffe05-127">Az **Access munka-vagy iskolai** oldalon az alábbi ábrán látható, a **kezelési kiszolgálócímet** tartalmazó **kapcsolati adatokat** tekintheti meg, beleértve a *befejezetlen termelés* és a *MAM* szavakat is.</span><span class="sxs-lookup"><span data-stu-id="ffe05-127">On the **Access work or school** page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="ffe05-129">**Annak ellenőrzése, hogy nem lehet beilleszteni vállalati adatokat nem felügyelt alkalmazásba**</span><span class="sxs-lookup"><span data-stu-id="ffe05-129">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="ffe05-130">Nyissa meg az Outlook 2016-ot, szükség esetén vegye fel Microsoft 365 Business-fiókját, és jelentkezzen be a Microsoft 365 Business hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="ffe05-130">Open Outlook 2016 and add your Microsoft 365 Business account if necessary and sign in with your Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="ffe05-131">Nyisson meg egy e-mailt, és másoljon belőle tartalmat a vágólapra.</span><span class="sxs-lookup"><span data-stu-id="ffe05-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="ffe05-132">Nyissa meg a Jegyzettömböt, és kísérelje meg beilleszteni a vágólapra másolt tartalmat.</span><span class="sxs-lookup"><span data-stu-id="ffe05-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="ffe05-133">Hibaüzenetet kap, amely kimondja, hogy az alkalmazás nem fér hozzá a tartalomhoz.</span><span class="sxs-lookup"><span data-stu-id="ffe05-133">You'll receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="ffe05-135">A Word 2016-ba azonban beillesztheti a szóban forgó tartalmat.</span><span class="sxs-lookup"><span data-stu-id="ffe05-135">You can, however, paste the same content into Word 2016.</span></span>
    


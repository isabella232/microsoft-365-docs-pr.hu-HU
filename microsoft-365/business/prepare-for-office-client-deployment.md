---
title: Felkészülés a Microsoft 365 vállalati verzió statisztulásának Office-ügyféltelepítésére
f1.keywords:
- CSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 10/31/2017
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Megtudhatja, hogy miként telepítheti automatikusan a 32 bites Office-alkalmazásokat Windows 10 rendszerű számítógépekre, és hogyan őrizheti meg azokat.
ms.openlocfilehash: b5f01bc9bb10765929f3c6bdd5908e8b48a51a11
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/21/2020
ms.locfileid: "43633099"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a><span data-ttu-id="fe1df-103">Felkészülés a Microsoft 365 vállalati verzió statisztulásának Office-ügyféltelepítésére</span><span class="sxs-lookup"><span data-stu-id="fe1df-103">Prepare for Office client deployment by Microsoft 365 for business</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="fe1df-104">Felkészülés az Office-appok ügyfélszámítógépekre történő automatikus telepítésére</span><span class="sxs-lookup"><span data-stu-id="fe1df-104">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="fe1df-105">A Microsoft 365 vállalati verzióval automatikusan telepítheti a 32 bites Office-alkalmazásokat Windows 10 rendszerű számítógépekre, és naprakészen tarthatja őket a frissítésekkel kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="fe1df-105">You can use Microsoft 365 for business to automatically install the 32-bit Office apps on Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="fe1df-106">Az automatikus telepítés akkor működik a legjobban, ha a végfelhasználó számítógépe Windows 10 Business rendszeren van, és:</span><span class="sxs-lookup"><span data-stu-id="fe1df-106">Automatic installation works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="fe1df-107">Nincsenek telepített asztali Office-appjai (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access és OneDrive).</span><span class="sxs-lookup"><span data-stu-id="fe1df-107">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="fe1df-108">vagy</span><span class="sxs-lookup"><span data-stu-id="fe1df-108">or</span></span>
    
- <span data-ttu-id="fe1df-109">Telepítve van egy Office Kattintásra verzió.</span><span class="sxs-lookup"><span data-stu-id="fe1df-109">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="fe1df-110">Ha ki szeretné deríteni, hogy az Office Office Kattintásra verziójával rendelkezik-e, egy tetszőleges Office-appban válassza a **Fájl** \> **Fiók** (az Outlookban **Office-fiók**) lehetőséget).</span><span class="sxs-lookup"><span data-stu-id="fe1df-110">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook).</span></span> <span data-ttu-id="fe1df-111">Ha az **Office-frissítések** az alábbi ábrán látható módon jelenik meg, akkor a telepítés az Office-hoz kattintással történt.</span><span class="sxs-lookup"><span data-stu-id="fe1df-111">If you see **Office Updates** as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="fe1df-113">**Ki élvezi ezt a funkciót?**</span><span class="sxs-lookup"><span data-stu-id="fe1df-113">**Who benefits from having this feature**</span></span>
  
<span data-ttu-id="fe1df-114">Annak a végfelhasználónak, akinek a PC-jén:</span><span class="sxs-lookup"><span data-stu-id="fe1df-114">The end user whose PC:</span></span>
  
- <span data-ttu-id="fe1df-115">**Windows** 10 Business felhasználói licenccel, aktív Microsoft 365 vállalati licenccel, Windows 10 Alkotók frissítésével rendelkezik, és csatlakozik az Azure Active Directoryhoz.</span><span class="sxs-lookup"><span data-stu-id="fe1df-115">**Has**  a Windows 10 Business user license, an active Microsoft 365 for business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="fe1df-116">**Nem rendelkezik** 64 bites Office-alkalmazásokkal (például Word, Excel, PowerPoint).</span><span class="sxs-lookup"><span data-stu-id="fe1df-116">**Doesn't have** 64-bit Office apps (example: Word, Excel, PowerPoint).</span></span> <span data-ttu-id="fe1df-117">Ha 64 bites Office-alkalmazásokra van szükség, akkor ez a funkció nem megfelelő, mert nem támogatja az Office 64 bites Office Kattintásra verziójának elindítását a Microsoft 365 vállalati verziós felügyeleti konzolról.</span><span class="sxs-lookup"><span data-stu-id="fe1df-117">If 64-bit Office apps are required, then this feature isn't a good fit because there's no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 for business admin console.</span></span> 
    
- <span data-ttu-id="fe1df-118">**Nem található meg** egy Windows Installer (MSI) technológiával telepített különálló 2016-os app sem (például Visio vagy Project).</span><span class="sxs-lookup"><span data-stu-id="fe1df-118">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project).</span></span> <span data-ttu-id="fe1df-119">A Microsoft 365 vállalati verzió frissíti az Office-t az Office 2016 Office 2016 Kattintásra verziója szolgáltatásra, és ez nem működik az Office 2016 MSI önálló alkalmazásaival.</span><span class="sxs-lookup"><span data-stu-id="fe1df-119">Microsoft 365 for business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="fe1df-120">Az alábbi táblázat bemutatja, hogy a végfelhasználóknak/rendszergazdáknak a kezdeti állapotuktól függően milyen műveletet kell végrehajtaniuk ahhoz, hogy a Microsoft 365 vállalati verziós felügyeleti konzolon az Office-telepítés sikeres, Kattintásra alkalmazásra készült verziója meglegyen.</span><span class="sxs-lookup"><span data-stu-id="fe1df-120">The following table shows what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 for business admin console.</span></span>
  
|<span data-ttu-id="fe1df-121">**Az Office telepítésének kezdő állapota**</span><span class="sxs-lookup"><span data-stu-id="fe1df-121">**Starting Office install status**</span></span>|<span data-ttu-id="fe1df-122">**Végrehajtandó művelet a Microsoft 365 vállalati verzió Office-telepítése előtt**</span><span class="sxs-lookup"><span data-stu-id="fe1df-122">**Action to take before Microsoft 365 for business Office install**</span></span>|<span data-ttu-id="fe1df-123">**Záró állapot**</span><span class="sxs-lookup"><span data-stu-id="fe1df-123">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="fe1df-124">Nincs telepítve Office programcsomag</span><span class="sxs-lookup"><span data-stu-id="fe1df-124">No Office suite installed</span></span>  <br/> |<span data-ttu-id="fe1df-125">Egyikre sem.</span><span class="sxs-lookup"><span data-stu-id="fe1df-125">None</span></span>  <br/> |<span data-ttu-id="fe1df-126">Az Office 2016 32 bites telepítése az Office Kattintásra alkalmazással történik</span><span class="sxs-lookup"><span data-stu-id="fe1df-126">Office 2016 32-bit is installed by using Click-to-Run</span></span>  <br/> |
|<span data-ttu-id="fe1df-127">Az Office Kattintásra technológiával telepített Office 32 bites verziója (2016-os vagy korábbi verzió), különálló appok nélkül</span><span class="sxs-lookup"><span data-stu-id="fe1df-127">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="fe1df-128">Egyikre sem.</span><span class="sxs-lookup"><span data-stu-id="fe1df-128">None</span></span>  <br/> |<span data-ttu-id="fe1df-129">Frissítve az Office 2016 legújabb 32 bites, Office Kattintásra verziójára, szükség szerint **\***</span><span class="sxs-lookup"><span data-stu-id="fe1df-129">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="fe1df-130">Az Office meglévő Kattintásra 32 bites verziója és az Office Kattintásra 32 bites vagy 64 bites önálló Office-alkalmazások (például Visio, Project)</span><span class="sxs-lookup"><span data-stu-id="fe1df-130">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32-bit or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="fe1df-131">Egyikre sem.</span><span class="sxs-lookup"><span data-stu-id="fe1df-131">None</span></span>  <br/> |<span data-ttu-id="fe1df-132">Az önálló alkalmazásokat ez nem érinti.</span><span class="sxs-lookup"><span data-stu-id="fe1df-132">Standalone apps aren't affected.</span></span> <span data-ttu-id="fe1df-133">A programcsomag frissül az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára</span><span class="sxs-lookup"><span data-stu-id="fe1df-133">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="fe1df-134">Az Office Kattintásra technológiával telepített Office 32 bites verziója és bármely 32 vagy 64 bites (a 2016-os verzió kivételével), MSI technológiával telepített különálló Office-app</span><span class="sxs-lookup"><span data-stu-id="fe1df-134">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="fe1df-135">Egyikre sem.</span><span class="sxs-lookup"><span data-stu-id="fe1df-135">None</span></span>  <br/> |<span data-ttu-id="fe1df-136">Az önálló alkalmazásokat ez nem érinti.</span><span class="sxs-lookup"><span data-stu-id="fe1df-136">Standalone apps aren't affected.</span></span> <span data-ttu-id="fe1df-137">A programcsomag frissül az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára</span><span class="sxs-lookup"><span data-stu-id="fe1df-137">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="fe1df-138">Az Office Kattintásra technológiával telepített Office bármely meglévő, 64 bites verziója</span><span class="sxs-lookup"><span data-stu-id="fe1df-138">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="fe1df-139">A 64 bites Office-alkalmazások eltávolítása, ha nem baj, ha 32 bites Office-appokkal helyettesíti őket</span><span class="sxs-lookup"><span data-stu-id="fe1df-139">Uninstall the 64-bit Office apps, if it's OK to replace them with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="fe1df-140">Ha eltávolítja a 64 bites Office-appokat, az Office Kattintásra technológiával telepített Office 2016 32 bites verziója települ</span><span class="sxs-lookup"><span data-stu-id="fe1df-140">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="fe1df-141">Az Office 2016 meglévő, MSI technológiával telepített példánya különálló appokkal vagy anélkül</span><span class="sxs-lookup"><span data-stu-id="fe1df-141">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="fe1df-142">Az MSI technológiával telepített Office 2016 eltávolítása</span><span class="sxs-lookup"><span data-stu-id="fe1df-142">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="fe1df-p106">Telepítve van az Office Kattintásra technológiával telepített Office 2016 32 bites verziója. A különálló appokat nem érinti semmilyen változás.</span><span class="sxs-lookup"><span data-stu-id="fe1df-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="fe1df-145">Az Office 2013 és/vagy különálló Office-appok meglévő, MSI technológiával telepített példánya</span><span class="sxs-lookup"><span data-stu-id="fe1df-145">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="fe1df-146">Nincs</span><span class="sxs-lookup"><span data-stu-id="fe1df-146">None</span></span>  <br/> |<span data-ttu-id="fe1df-147">Az Office Kattintásra technológiával telepített Office 2016 32 bites verziója, amely együtt létezik a korábbról meglévő, MSI technológiával telepített Office-példánnyal (és különálló appokkal)</span><span class="sxs-lookup"><span data-stu-id="fe1df-147">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="fe1df-148">**(\*) Megjegyzés:** Egy ismert hiba miatt nem történik meg az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára való frissítés.</span><span class="sxs-lookup"><span data-stu-id="fe1df-148">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug.</span></span> <span data-ttu-id="fe1df-149">A javítás folyamatban van.</span><span class="sxs-lookup"><span data-stu-id="fe1df-149">A fix is in progress.</span></span> 
  

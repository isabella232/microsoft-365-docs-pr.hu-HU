---
title: Felkészülés Office-ügyfél központi telepítésére a Microsoft 365 Vállalati verzióban
f1.keywords:
- CSH
ms.author: efrene
author: efrene
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Megtudhatja, hogy miként telepítheti automatikusan a 32 bites Office-appokat Windows 10-es számítógépekre, és hogyan tarthatja őket naprakészen.
ms.openlocfilehash: 868d06fadfef0f55b41131b7fdfbb368b9128405
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580054"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a><span data-ttu-id="1e5cc-103">Felkészülés Office-ügyfél központi telepítésére a Microsoft 365 Vállalati verzióban</span><span class="sxs-lookup"><span data-stu-id="1e5cc-103">Prepare for Office client deployment by Microsoft 365 for business</span></span>

<span data-ttu-id="1e5cc-104">Ez a cikk a Microsoft 365 Vállalati prémium verzióra vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="1e5cc-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="1e5cc-105">Felkészülés az Office-appok ügyfélszámítógépekre történő automatikus telepítésére</span><span class="sxs-lookup"><span data-stu-id="1e5cc-105">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="1e5cc-106">A Microsoft 365 Vállalati prémium verzióval automatikusan telepítheti a 32 bites Office-appokat Windows 10-es számítógépekre, és folyamatosan frissülhet a frissítésekkel.</span><span class="sxs-lookup"><span data-stu-id="1e5cc-106">You can use Microsoft 365 Business Premium to automatically install the 32-bit Office apps on Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="1e5cc-107">Az automatikus telepítés akkor működik a legjobban, ha a végfelhasználó számítógépe a Windows 10 Business rendszert használja, és:</span><span class="sxs-lookup"><span data-stu-id="1e5cc-107">Automatic installation works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="1e5cc-108">Nincsenek telepített asztali Office-appjai (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access és OneDrive).</span><span class="sxs-lookup"><span data-stu-id="1e5cc-108">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="1e5cc-109">vagy</span><span class="sxs-lookup"><span data-stu-id="1e5cc-109">or</span></span>
    
- <span data-ttu-id="1e5cc-110">Telepítve van egy Office Kattintásra verzió.</span><span class="sxs-lookup"><span data-stu-id="1e5cc-110">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="1e5cc-111">Ha ki szeretné deríteni, hogy az Office Office Kattintásra verziójával rendelkezik-e, egy tetszőleges Office-appban válassza a **Fájl** \> **Fiók** (az Outlookban **Office-fiók**) lehetőséget).</span><span class="sxs-lookup"><span data-stu-id="1e5cc-111">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook).</span></span> <span data-ttu-id="1e5cc-112">Ha az **Office-frissítések az** alábbi ábrán látható módon jelennek meg, akkor a telepítés az Office Kattintásra használatával történt.</span><span class="sxs-lookup"><span data-stu-id="1e5cc-112">If you see **Office Updates** as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="1e5cc-114">**Kik számára előnyös ez a funkció?**</span><span class="sxs-lookup"><span data-stu-id="1e5cc-114">**Who benefits from having this feature**</span></span>
  
<span data-ttu-id="1e5cc-115">Annak a végfelhasználónak, akinek a PC-jén:</span><span class="sxs-lookup"><span data-stu-id="1e5cc-115">The end user whose PC:</span></span>
  
- <span data-ttu-id="1e5cc-116">**Windows**  10 Business felhasználói licenccel, aktív Microsoft 365 Vállalati verziós licenccel és a Windows 10 alkotói frissítéssel rendelkezik, és csatlakozik az Azure Active Directoryhoz.</span><span class="sxs-lookup"><span data-stu-id="1e5cc-116">**Has**  a Windows 10 Business user license, an active Microsoft 365 for business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="1e5cc-117">**Nincs 64** bites Office-appja (például: Word, Excel, PowerPoint).</span><span class="sxs-lookup"><span data-stu-id="1e5cc-117">**Doesn't have** 64-bit Office apps (example: Word, Excel, PowerPoint).</span></span> <span data-ttu-id="1e5cc-118">Ha 64 bites Office-appokra van szükség, akkor ez a funkció nem jó hely, mert az Office 2016 64 bites, Office Kattintásra verziójának a Microsoft 365 Vállalati verzió felügyeleti konzolról való kiváltása nem támogatott.</span><span class="sxs-lookup"><span data-stu-id="1e5cc-118">If 64-bit Office apps are required, then this feature isn't a good fit because there's no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 for business admin console.</span></span> 
    
- <span data-ttu-id="1e5cc-119">**Nem található meg** egy Windows Installer (MSI) technológiával telepített különálló 2016-os app sem (például Visio vagy Project).</span><span class="sxs-lookup"><span data-stu-id="1e5cc-119">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project).</span></span> <span data-ttu-id="1e5cc-120">A Microsoft 365 vállalati verzió az Office-t az Office 2016 Office Kattintásra verziójára frissíti, és nem működik együtt az MSI különálló Office 2016-appokkal.</span><span class="sxs-lookup"><span data-stu-id="1e5cc-120">Microsoft 365 for business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="1e5cc-121">Az alábbi táblázatban látható, hogy a felhasználóknak/rendszergazdáknak milyen műveletet kell követniük a kezdő állapotuktól függően ahhoz, hogy az Office 365 Vállalati verzió felügyeleti konzolján az Office 32 bites, Office Kattintásra típusú verzióját futtatják.</span><span class="sxs-lookup"><span data-stu-id="1e5cc-121">The following table shows what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 for business admin console.</span></span>
  
|<span data-ttu-id="1e5cc-122">**Az Office telepítésének kezdő állapota**</span><span class="sxs-lookup"><span data-stu-id="1e5cc-122">**Starting Office install status**</span></span>|<span data-ttu-id="1e5cc-123">**A Microsoft 365 Vállalati verzió telepítése előtt szükséges teendők**</span><span class="sxs-lookup"><span data-stu-id="1e5cc-123">**Action to take before Microsoft 365 for business Office install**</span></span>|<span data-ttu-id="1e5cc-124">**Záró állapot**</span><span class="sxs-lookup"><span data-stu-id="1e5cc-124">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1e5cc-125">Nincs telepítve Office programcsomag</span><span class="sxs-lookup"><span data-stu-id="1e5cc-125">No Office suite installed</span></span>  <br/> |<span data-ttu-id="1e5cc-126">Nincs</span><span class="sxs-lookup"><span data-stu-id="1e5cc-126">None</span></span>  <br/> |<span data-ttu-id="1e5cc-127">Az Office 2016 32 bites telepítése az Office Kattintásra használatával</span><span class="sxs-lookup"><span data-stu-id="1e5cc-127">Office 2016 32-bit is installed by using Click-to-Run</span></span>  <br/> |
|<span data-ttu-id="1e5cc-128">Az Office Kattintásra technológiával telepített Office 32 bites verziója (2016-os vagy korábbi verzió), különálló appok nélkül</span><span class="sxs-lookup"><span data-stu-id="1e5cc-128">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="1e5cc-129">Nincs</span><span class="sxs-lookup"><span data-stu-id="1e5cc-129">None</span></span>  <br/> |<span data-ttu-id="1e5cc-130">Frissítve az Office 2016 legújabb 32 bites, Office Kattintásra verziójára, szükség szerint **\***</span><span class="sxs-lookup"><span data-stu-id="1e5cc-130">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="1e5cc-131">Az Office Kattintásra szolgáltatás meglévő, 32 bites verziója és 32 bites vagy 64 bites különálló Office-appok (például Visio, Project)</span><span class="sxs-lookup"><span data-stu-id="1e5cc-131">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32-bit or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="1e5cc-132">Egyikre sem.</span><span class="sxs-lookup"><span data-stu-id="1e5cc-132">None</span></span>  <br/> |<span data-ttu-id="1e5cc-133">A különálló appok nem érintettek.</span><span class="sxs-lookup"><span data-stu-id="1e5cc-133">Standalone apps aren't affected.</span></span> <span data-ttu-id="1e5cc-134">A programcsomag frissül az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára</span><span class="sxs-lookup"><span data-stu-id="1e5cc-134">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="1e5cc-135">Az Office Kattintásra technológiával telepített Office 32 bites verziója és bármely 32 vagy 64 bites (a 2016-os verzió kivételével), MSI technológiával telepített különálló Office-app</span><span class="sxs-lookup"><span data-stu-id="1e5cc-135">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="1e5cc-136">Nincs</span><span class="sxs-lookup"><span data-stu-id="1e5cc-136">None</span></span>  <br/> |<span data-ttu-id="1e5cc-137">A különálló appok nem érintettek.</span><span class="sxs-lookup"><span data-stu-id="1e5cc-137">Standalone apps aren't affected.</span></span> <span data-ttu-id="1e5cc-138">A programcsomag frissül az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára</span><span class="sxs-lookup"><span data-stu-id="1e5cc-138">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="1e5cc-139">Az Office Kattintásra technológiával telepített Office bármely meglévő, 64 bites verziója</span><span class="sxs-lookup"><span data-stu-id="1e5cc-139">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="1e5cc-140">Távolítsa el a 64 bites Office-appokat, ha nem gond, hogy lecserélje őket a 32 bites Office-appokkal</span><span class="sxs-lookup"><span data-stu-id="1e5cc-140">Uninstall the 64-bit Office apps, if it's OK to replace them with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="1e5cc-141">Ha eltávolítja a 64 bites Office-appokat, az Office Kattintásra technológiával telepített Office 2016 32 bites verziója települ</span><span class="sxs-lookup"><span data-stu-id="1e5cc-141">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="1e5cc-142">Az Office 2016 meglévő, MSI technológiával telepített példánya különálló appokkal vagy anélkül</span><span class="sxs-lookup"><span data-stu-id="1e5cc-142">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="1e5cc-143">Az MSI technológiával telepített Office 2016 eltávolítása</span><span class="sxs-lookup"><span data-stu-id="1e5cc-143">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="1e5cc-p106">Telepítve van az Office Kattintásra technológiával telepített Office 2016 32 bites verziója. A különálló appokat nem érinti semmilyen változás.</span><span class="sxs-lookup"><span data-stu-id="1e5cc-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="1e5cc-146">Az Office 2013 és/vagy különálló Office-appok meglévő, MSI technológiával telepített példánya</span><span class="sxs-lookup"><span data-stu-id="1e5cc-146">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="1e5cc-147">Nincs</span><span class="sxs-lookup"><span data-stu-id="1e5cc-147">None</span></span>  <br/> |<span data-ttu-id="1e5cc-148">Az Office Kattintásra technológiával telepített Office 2016 32 bites verziója, amely együtt létezik a korábbról meglévő, MSI technológiával telepített Office-példánnyal (és különálló appokkal)</span><span class="sxs-lookup"><span data-stu-id="1e5cc-148">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="1e5cc-149">**(\*) Megjegyzés:** Egy ismert hiba miatt nem történik meg az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára való frissítés.</span><span class="sxs-lookup"><span data-stu-id="1e5cc-149">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug.</span></span> <span data-ttu-id="1e5cc-150">Már folyamatban van a javítás.</span><span class="sxs-lookup"><span data-stu-id="1e5cc-150">A fix is in progress.</span></span> 
  

---
title: Felkészülés Office-ügyfél központi telepítésére a Microsoft 365 Business segítségével
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
description: Megtudhatja, hogy miként telepítheti automatikusan a 32 bites Office-alkalmazásokat Windows 10-es számítógépekre, és hogyan tarthatja őket naprakészen.
ms.openlocfilehash: 0f8cd7df49ad627b190fad6737ec95a6d64d99d0
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/15/2020
ms.locfileid: "42065106"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a><span data-ttu-id="bafa0-103">Felkészülés Office-ügyfél központi telepítésére a Microsoft 365 Business segítségével</span><span class="sxs-lookup"><span data-stu-id="bafa0-103">Prepare for Office client deployment by Microsoft 365 Business</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="bafa0-104">Felkészülés az Office-appok ügyfélszámítógépekre történő automatikus telepítésére</span><span class="sxs-lookup"><span data-stu-id="bafa0-104">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="bafa0-105">A Microsoft 365 Vállalati verzió segítségével automatikusan telepítheti a 32 bites Office-alkalmazásokat Windows 10-es számítógépekre, és naprakészen tarthatja őket a frissítésekkel.</span><span class="sxs-lookup"><span data-stu-id="bafa0-105">You can use Microsoft 365 Business to automatically install the 32-bit Office apps on Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="bafa0-106">Az automatikus telepítés akkor működik a legjobban, ha a végfelhasználó számítógépe Windows 10 Business rendszeren van, és:</span><span class="sxs-lookup"><span data-stu-id="bafa0-106">Automatic installation works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="bafa0-107">Nincsenek telepített asztali Office-appjai (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access és OneDrive).</span><span class="sxs-lookup"><span data-stu-id="bafa0-107">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="bafa0-108">vagy</span><span class="sxs-lookup"><span data-stu-id="bafa0-108">or</span></span>
    
- <span data-ttu-id="bafa0-109">Telepítve van egy Office Kattintásra verzió.</span><span class="sxs-lookup"><span data-stu-id="bafa0-109">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="bafa0-110">Ha ki szeretné deríteni, hogy az Office Office Kattintásra verziójával rendelkezik-e, egy tetszőleges Office-appban válassza a **Fájl** \> **Fiók** (az Outlookban **Office-fiók**) lehetőséget).</span><span class="sxs-lookup"><span data-stu-id="bafa0-110">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook).</span></span> <span data-ttu-id="bafa0-111">Ha az **Office-frissítések** az alábbi ábrán látható módon jelenik meg, akkor a telepítés a Kattintásra szolgáltatás sal történt.</span><span class="sxs-lookup"><span data-stu-id="bafa0-111">If you see **Office Updates** as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="bafa0-113">**Kinek származik előnye ennek a funkciónak a birtoklásából?**</span><span class="sxs-lookup"><span data-stu-id="bafa0-113">**Who benefits from having this feature**</span></span>
  
<span data-ttu-id="bafa0-114">Annak a végfelhasználónak, akinek a PC-jén:</span><span class="sxs-lookup"><span data-stu-id="bafa0-114">The end user whose PC:</span></span>
  
- <span data-ttu-id="bafa0-115">**Megtalálható** egy Windows 10 Business verzióhoz való felhasználói licenc, egy aktív Microsoft 365 Business-licenc és a Windows 10 alkotói frissítés, illetve akinek a PC-je csatlakoztatva van az Azure Active Directoryhoz.</span><span class="sxs-lookup"><span data-stu-id="bafa0-115">**Has**  a Windows 10 Business user license, an active Microsoft 365 Business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="bafa0-116">**Nincs** 64 bites Office-alkalmazás (például Word, Excel, PowerPoint).</span><span class="sxs-lookup"><span data-stu-id="bafa0-116">**Doesn't have** 64-bit Office apps (example: Word, Excel, PowerPoint).</span></span> <span data-ttu-id="bafa0-117">Ha 64 bites Office-alkalmazásokra van szükség, akkor ez a funkció nem megfelelő, mert nem támogatja az Office 64 bites, kattintásra futó verziójának aktiválását a Microsoft 365 Vállalati verzió felügyeleti konzoljáról.</span><span class="sxs-lookup"><span data-stu-id="bafa0-117">If 64-bit Office apps are required, then this feature isn't a good fit because there's no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 Business admin console.</span></span> 
    
- <span data-ttu-id="bafa0-118">**Nem található meg** egy Windows Installer (MSI) technológiával telepített különálló 2016-os app sem (például Visio vagy Project).</span><span class="sxs-lookup"><span data-stu-id="bafa0-118">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project).</span></span> <span data-ttu-id="bafa0-119">A Microsoft 365 Vállalati verzió az Office-t az Office 2016 Office Kattintásra verziójára frissíti, és ez nem működik az Office 2016-os MSI önálló alkalmazásokkal.</span><span class="sxs-lookup"><span data-stu-id="bafa0-119">Microsoft 365 Business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="bafa0-120">Az alábbi táblázat bemutatja, hogy a végfelhasználóknak/rendszergazdáknak milyen lépéseket kell tenniük a kezdeti állapotuktól függően ahhoz, hogy az Office központi telepítésének sikeres 32 bites Office-telepítést a Microsoft 365 Vállalati verzió felügyeleti konzoljáról történő futtatásához.</span><span class="sxs-lookup"><span data-stu-id="bafa0-120">The following table shows what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 Business admin console.</span></span>
  
|<span data-ttu-id="bafa0-121">**Az Office telepítésének kezdő állapota**</span><span class="sxs-lookup"><span data-stu-id="bafa0-121">**Starting Office install status**</span></span>|<span data-ttu-id="bafa0-122">**Az Office Microsoft 365 Business-szel való telepítése előtt szükséges művelet**</span><span class="sxs-lookup"><span data-stu-id="bafa0-122">**Action to take before Microsoft 365 Business Office install**</span></span>|<span data-ttu-id="bafa0-123">**Záró állapot**</span><span class="sxs-lookup"><span data-stu-id="bafa0-123">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="bafa0-124">Nincs telepítve Office programcsomag</span><span class="sxs-lookup"><span data-stu-id="bafa0-124">No Office suite installed</span></span>  <br/> |<span data-ttu-id="bafa0-125">Egyikre sem.</span><span class="sxs-lookup"><span data-stu-id="bafa0-125">None</span></span>  <br/> |<span data-ttu-id="bafa0-126">Az Office 2016 32 bites telepítése kattintásra</span><span class="sxs-lookup"><span data-stu-id="bafa0-126">Office 2016 32-bit is installed by using Click-to-Run</span></span>  <br/> |
|<span data-ttu-id="bafa0-127">Az Office Kattintásra technológiával telepített Office 32 bites verziója (2016-os vagy korábbi verzió), különálló appok nélkül</span><span class="sxs-lookup"><span data-stu-id="bafa0-127">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="bafa0-128">Egyikre sem.</span><span class="sxs-lookup"><span data-stu-id="bafa0-128">None</span></span>  <br/> |<span data-ttu-id="bafa0-129">Frissítve az Office 2016 legújabb 32 bites, Office Kattintásra verziójára, szükség szerint **\***</span><span class="sxs-lookup"><span data-stu-id="bafa0-129">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="bafa0-130">Az Office és a Kattintásra 32 bites vagy a 64 bites önálló Office-alkalmazások (például Visio, Project) meglévő, Kattintásra 32 bites verziója</span><span class="sxs-lookup"><span data-stu-id="bafa0-130">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32-bit or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="bafa0-131">Egyikre sem.</span><span class="sxs-lookup"><span data-stu-id="bafa0-131">None</span></span>  <br/> |<span data-ttu-id="bafa0-132">Az önálló alkalmazásokat ez nem érinti.</span><span class="sxs-lookup"><span data-stu-id="bafa0-132">Standalone apps aren't affected.</span></span> <span data-ttu-id="bafa0-133">A programcsomag frissül az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára</span><span class="sxs-lookup"><span data-stu-id="bafa0-133">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="bafa0-134">Az Office Kattintásra technológiával telepített Office 32 bites verziója és bármely 32 vagy 64 bites (a 2016-os verzió kivételével), MSI technológiával telepített különálló Office-app</span><span class="sxs-lookup"><span data-stu-id="bafa0-134">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="bafa0-135">Egyikre sem.</span><span class="sxs-lookup"><span data-stu-id="bafa0-135">None</span></span>  <br/> |<span data-ttu-id="bafa0-136">Az önálló alkalmazásokat ez nem érinti.</span><span class="sxs-lookup"><span data-stu-id="bafa0-136">Standalone apps aren't affected.</span></span> <span data-ttu-id="bafa0-137">A programcsomag frissül az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára</span><span class="sxs-lookup"><span data-stu-id="bafa0-137">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="bafa0-138">Az Office Kattintásra technológiával telepített Office bármely meglévő, 64 bites verziója</span><span class="sxs-lookup"><span data-stu-id="bafa0-138">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="bafa0-139">Távolítsa el a 64 bites Office-alkalmazásokat, ha nem baj, ha 32 bites Office-appokra cseréli őket</span><span class="sxs-lookup"><span data-stu-id="bafa0-139">Uninstall the 64-bit Office apps, if it's OK to replace them with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="bafa0-140">Ha eltávolítja a 64 bites Office-appokat, az Office Kattintásra technológiával telepített Office 2016 32 bites verziója települ</span><span class="sxs-lookup"><span data-stu-id="bafa0-140">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="bafa0-141">Az Office 2016 meglévő, MSI technológiával telepített példánya különálló appokkal vagy anélkül</span><span class="sxs-lookup"><span data-stu-id="bafa0-141">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="bafa0-142">Az MSI technológiával telepített Office 2016 eltávolítása</span><span class="sxs-lookup"><span data-stu-id="bafa0-142">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="bafa0-p106">Telepítve van az Office Kattintásra technológiával telepített Office 2016 32 bites verziója. A különálló appokat nem érinti semmilyen változás.</span><span class="sxs-lookup"><span data-stu-id="bafa0-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="bafa0-145">Az Office 2013 és/vagy különálló Office-appok meglévő, MSI technológiával telepített példánya</span><span class="sxs-lookup"><span data-stu-id="bafa0-145">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="bafa0-146">Nincs</span><span class="sxs-lookup"><span data-stu-id="bafa0-146">None</span></span>  <br/> |<span data-ttu-id="bafa0-147">Az Office Kattintásra technológiával telepített Office 2016 32 bites verziója, amely együtt létezik a korábbról meglévő, MSI technológiával telepített Office-példánnyal (és különálló appokkal)</span><span class="sxs-lookup"><span data-stu-id="bafa0-147">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="bafa0-148">**(\*) Megjegyzés:** Egy ismert hiba miatt nem történik meg az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára való frissítés.</span><span class="sxs-lookup"><span data-stu-id="bafa0-148">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug.</span></span> <span data-ttu-id="bafa0-149">A javítás folyamatban van.</span><span class="sxs-lookup"><span data-stu-id="bafa0-149">A fix is in progress.</span></span> 
  

---
title: Felkészülés Office-ügyfél központi telepítésére a Microsoft 365 Business segítségével
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
description: Útmutató a 32 bites Office-alkalmazások Windows 10 számítógépre való automatikus telepítéséhez és naprakészen tartásáról.
ms.openlocfilehash: 5b28c1e62d813c52b41ce8e7619c865cdf7690e2
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575818"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a><span data-ttu-id="7270d-103">Felkészülés Office-ügyfél központi telepítésére a Microsoft 365 Business segítségével</span><span class="sxs-lookup"><span data-stu-id="7270d-103">Prepare for Office client deployment by Microsoft 365 Business</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="7270d-104">Felkészülés az Office-appok ügyfélszámítógépekre történő automatikus telepítésére</span><span class="sxs-lookup"><span data-stu-id="7270d-104">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="7270d-105">A Microsoft 365 Business használatával automatikusan telepítheti az Office-appok 32 bites verzióját a Windows 10-es számítógépekre, és frissítésekkel naprakészen tarthatja őket.</span><span class="sxs-lookup"><span data-stu-id="7270d-105">You can use Microsoft 365 Business to automatically install the 32-bit Office apps to Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="7270d-106">Ez akkor működik a legjobban, ha a végfelhasználó számítógépén Windows 10 Business fut, és:</span><span class="sxs-lookup"><span data-stu-id="7270d-106">This works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="7270d-107">Nincsenek telepített asztali Office-appjai (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access és OneDrive).</span><span class="sxs-lookup"><span data-stu-id="7270d-107">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="7270d-108">vagy</span><span class="sxs-lookup"><span data-stu-id="7270d-108">or</span></span>
    
- <span data-ttu-id="7270d-109">Telepítve van egy Office Kattintásra verzió.</span><span class="sxs-lookup"><span data-stu-id="7270d-109">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="7270d-p101">Ha ki szeretné deríteni, hogy az Office Office Kattintásra verziójával rendelkezik-e, egy tetszőleges Office-appban válassza a **Fájl** \> **Fiók** (az Outlookban **Office-fiók**) lehetőséget). Ha ekkor megjelennek az Office-frissítések az alábbi ábrán látható módon, akkor a telepített példány Office Kattintásra verziójú.</span><span class="sxs-lookup"><span data-stu-id="7270d-p101">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook). If you see Office Updates as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="7270d-113">**Kinek származik előnye a funkcióból?**</span><span class="sxs-lookup"><span data-stu-id="7270d-113">**Who will benefit from having this feature**</span></span>
  
<span data-ttu-id="7270d-114">Annak a végfelhasználónak, akinek a PC-jén:</span><span class="sxs-lookup"><span data-stu-id="7270d-114">The end user whose PC:</span></span>
  
- <span data-ttu-id="7270d-115">**Megtalálható** egy Windows 10 Business verzióhoz való felhasználói licenc, egy aktív Microsoft 365 Business-licenc és a Windows 10 alkotói frissítés, illetve akinek a PC-je csatlakoztatva van az Azure Active Directoryhoz.</span><span class="sxs-lookup"><span data-stu-id="7270d-115">**Has**  a Windows 10 Business user license, an active Microsoft 365 Business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="7270d-p102">**Nem található meg** az Office-appok 64 bites verziója (például: Word, Excel, Powerpoint). Ha az Office-appok 64 bites verzióját kell használnia, akkor ez a funkció nem jó választás, mivel az Office 2016 64 bites, Office Kattintásra verziójának elindítása a Microsoft 365 Business felügyeleti konzoljából nem támogatott.</span><span class="sxs-lookup"><span data-stu-id="7270d-p102">**Doesn't have** 64-bit Office apps (example: Word, Excel, Powerpoint). If 64-bit Office apps are required, then this feature is not a good fit because there is no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 Business admin console.</span></span> 
    
- <span data-ttu-id="7270d-p103">**Nem található meg** egy Windows Installer (MSI) technológiával telepített különálló 2016-os app sem (például Visio vagy Project). A Microsoft 365 Business az Office-t az Office 2016 Office Kattintásra verziójára frissíti, amely nem működik együtt az MSI telepítésű különálló Office 2016-appokkal.</span><span class="sxs-lookup"><span data-stu-id="7270d-p103">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project). Microsoft 365 Business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="7270d-120">Az alábbi táblázat azt részletezi, hogy a kezdő állapotuktól függően a végfelhasználóknak/rendszergazdáknak milyen műveleteket kell végrehajtaniuk a Microsoft 365 Business felügyeleti konzoljában ahhoz, hogy megfelelően működjön az Office 32 bites, Office Kattintásra verziója.</span><span class="sxs-lookup"><span data-stu-id="7270d-120">The following table details what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 Business admin console.</span></span>
  
|<span data-ttu-id="7270d-121">**Az Office telepítésének kezdő állapota**</span><span class="sxs-lookup"><span data-stu-id="7270d-121">**Starting Office install status**</span></span>|<span data-ttu-id="7270d-122">**Az Office Microsoft 365 Business-szel való telepítése előtt szükséges művelet**</span><span class="sxs-lookup"><span data-stu-id="7270d-122">**Action to take before Microsoft 365 Business Office install**</span></span>|<span data-ttu-id="7270d-123">**Záró állapot**</span><span class="sxs-lookup"><span data-stu-id="7270d-123">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7270d-124">Nincs telepítve Office programcsomag</span><span class="sxs-lookup"><span data-stu-id="7270d-124">No Office suite installed</span></span>  <br/> |<span data-ttu-id="7270d-125">Egyikre sem.</span><span class="sxs-lookup"><span data-stu-id="7270d-125">None</span></span>  <br/> |<span data-ttu-id="7270d-126">Az Office Kattintásra technológiával telepített Office 2016 32 bites verziója</span><span class="sxs-lookup"><span data-stu-id="7270d-126">Office 2016 32-bit is installed by using click-to-run</span></span>  <br/> |
|<span data-ttu-id="7270d-127">Az Office Kattintásra technológiával telepített Office 32 bites verziója (2016-os vagy korábbi verzió), különálló appok nélkül</span><span class="sxs-lookup"><span data-stu-id="7270d-127">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="7270d-128">Egyikre sem.</span><span class="sxs-lookup"><span data-stu-id="7270d-128">None</span></span>  <br/> |<span data-ttu-id="7270d-129">Frissítve az Office 2016 legújabb 32 bites, Office Kattintásra verziójára, szükség szerint **\***</span><span class="sxs-lookup"><span data-stu-id="7270d-129">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="7270d-130">Az Office Kattintásra technológiával telepített Office 32 bites verziója és Office Kattintásra technológiával telepített 32 vagy 64 bites különálló Office-appok (például Visio, Project)</span><span class="sxs-lookup"><span data-stu-id="7270d-130">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32- or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="7270d-131">Egyikre sem.</span><span class="sxs-lookup"><span data-stu-id="7270d-131">None</span></span>  <br/> |<span data-ttu-id="7270d-p104">A különálló appok nem érintettek. A programcsomag frissül az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára</span><span class="sxs-lookup"><span data-stu-id="7270d-p104">Standalone apps are not affected. Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="7270d-134">Az Office Kattintásra technológiával telepített Office 32 bites verziója és bármely 32 vagy 64 bites (a 2016-os verzió kivételével), MSI technológiával telepített különálló Office-app</span><span class="sxs-lookup"><span data-stu-id="7270d-134">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="7270d-135">Egyikre sem.</span><span class="sxs-lookup"><span data-stu-id="7270d-135">None</span></span>  <br/> |<span data-ttu-id="7270d-p105">A különálló appok nem érintettek. A programcsomag frissül az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára</span><span class="sxs-lookup"><span data-stu-id="7270d-p105">Standalone apps are not affected. Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="7270d-138">Az Office Kattintásra technológiával telepített Office bármely meglévő, 64 bites verziója</span><span class="sxs-lookup"><span data-stu-id="7270d-138">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="7270d-139">Az Office-appok 64 bites verziójának eltávolítása, ha az lecserélhető az Office-appok 32 bites verziójára</span><span class="sxs-lookup"><span data-stu-id="7270d-139">Uninstall the 64-bit Office apps, if it is OK to replace it with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="7270d-140">Ha eltávolítja a 64 bites Office-appokat, az Office Kattintásra technológiával telepített Office 2016 32 bites verziója települ</span><span class="sxs-lookup"><span data-stu-id="7270d-140">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="7270d-141">Az Office 2016 meglévő, MSI technológiával telepített példánya különálló appokkal vagy anélkül</span><span class="sxs-lookup"><span data-stu-id="7270d-141">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="7270d-142">Az MSI technológiával telepített Office 2016 eltávolítása</span><span class="sxs-lookup"><span data-stu-id="7270d-142">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="7270d-p106">Telepítve van az Office Kattintásra technológiával telepített Office 2016 32 bites verziója. A különálló appokat nem érinti semmilyen változás.</span><span class="sxs-lookup"><span data-stu-id="7270d-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="7270d-145">Az Office 2013 és/vagy különálló Office-appok meglévő, MSI technológiával telepített példánya</span><span class="sxs-lookup"><span data-stu-id="7270d-145">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="7270d-146">Nincs</span><span class="sxs-lookup"><span data-stu-id="7270d-146">None</span></span>  <br/> |<span data-ttu-id="7270d-147">Az Office Kattintásra technológiával telepített Office 2016 32 bites verziója, amely együtt létezik a korábbról meglévő, MSI technológiával telepített Office-példánnyal (és különálló appokkal)</span><span class="sxs-lookup"><span data-stu-id="7270d-147">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="7270d-p107">**(\*) Megjegyzés:** Egy ismert hiba miatt nem történik meg az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára való frissítés. A javítás folyamatban van.</span><span class="sxs-lookup"><span data-stu-id="7270d-p107">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug. Fix is in progress.</span></span> 
  



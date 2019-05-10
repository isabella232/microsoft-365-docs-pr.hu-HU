---
title: AutoPilot-eszközök létrehozása és szerkesztése
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Útmutató a Microsoft 365 üzleti automata használó eszközök feltölteni. A profil hozzárendelése egy eszköz vagy eszközök egy csoportjához.
ms.openlocfilehash: 6492f1469a1ac9ea67750e9ffa071d19c88c743f
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660404"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="d5c76-104">AutoPilot-eszközök létrehozása és szerkesztése</span><span class="sxs-lookup"><span data-stu-id="d5c76-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="d5c76-105">Eszközlista feltöltése</span><span class="sxs-lookup"><span data-stu-id="d5c76-105">Upload a list of devices</span></span>

<span data-ttu-id="d5c76-106">A [lépésenkénti hozzáadási folyamat](add-autopilot-devices-and-profile.md) mellett az **Eszközök** lapon is tölthet fel eszközöket.</span><span class="sxs-lookup"><span data-stu-id="d5c76-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload the in the **Devices** tab.</span></span> 
  
<span data-ttu-id="d5c76-107">Az eszközöknek meg kell felelniük az alábbi követelményeknek:</span><span class="sxs-lookup"><span data-stu-id="d5c76-107">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="d5c76-108">A Windows 10 rendszer 1703-as vagy újabb verzióját kell futtatniuk.</span><span class="sxs-lookup"><span data-stu-id="d5c76-108">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="d5c76-109">Olyan új eszközöknek kell lenniük, amelyeken még nem használták a Windowst.</span><span class="sxs-lookup"><span data-stu-id="d5c76-109">New devices that have not been through Windows out-of-box experience.</span></span>

1. <span data-ttu-id="d5c76-110">A Microsoft 365 üzleti rendszergazdai központban válassza az **eszközök** \> **automata**.</span><span class="sxs-lookup"><span data-stu-id="d5c76-110">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="d5c76-111">Az **automata** lapon válassza ki **az eszközök** lapon \> **eszközök hozzáadása**.</span><span class="sxs-lookup"><span data-stu-id="d5c76-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="d5c76-113">Készített [eszköz lista CSV-fájl](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) **hozzáadása eszközök** panelen keresse \> **Mentés** \> **bezárása**.</span><span class="sxs-lookup"><span data-stu-id="d5c76-113">On the **Add devices** panel, browse to a [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) that you have prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="d5c76-114">Ezeket az adatokat beszerezheti a hardvergyártójától, vagy használhatja a [Get-WindowsAutoPilotInfo PowerShell-parancsfájlt](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), amely elkészíti a CSV-fájlt.</span><span class="sxs-lookup"><span data-stu-id="d5c76-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a csv file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="d5c76-115">Profil társítása egy eszközhöz vagy az eszközök egy csoportjához</span><span class="sxs-lookup"><span data-stu-id="d5c76-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="d5c76-116">**A Windows előkészítése** lapon válassza az **Eszközök** fület, majd jelölje be egy vagy több eszköz jelölőnégyzetét.</span><span class="sxs-lookup"><span data-stu-id="d5c76-116">On the **Prepare Windows** page, choose the **Devices** tab and check the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="d5c76-117">Az **Eszköz** panelen válasszon egy profilt a **Hozzárendelt profil** legördülő listából.</span><span class="sxs-lookup"><span data-stu-id="d5c76-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="d5c76-118">Ha egyetlen profilja sincs még, utasításokért olvassa el az [AutoPilot-profilok létrehozása és szerkesztése](create-and-edit-autopilot-profiles.md) című témakört.</span><span class="sxs-lookup"><span data-stu-id="d5c76-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    

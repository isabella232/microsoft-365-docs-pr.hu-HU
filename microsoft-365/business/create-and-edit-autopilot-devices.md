---
title: AutoPilot-eszközök létrehozása és szerkesztése
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Megtanulják, hogyan kell feltölteni eszközök segítségével AutoPilot a Microsoft 365 Business. Profilt hozzárendelhet egy eszközhöz vagy eszközcsoporthoz.
ms.openlocfilehash: 1dd6b1a574166379e29465bf3699e47e3b155e0b
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/14/2019
ms.locfileid: "38320258"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="68ecf-104">AutoPilot-eszközök létrehozása és szerkesztése</span><span class="sxs-lookup"><span data-stu-id="68ecf-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="68ecf-105">Eszközlista feltöltése</span><span class="sxs-lookup"><span data-stu-id="68ecf-105">Upload a list of devices</span></span>

<span data-ttu-id="68ecf-106">Az eszközök feltöltéséhez használja a [részletes útmutatót](add-autopilot-devices-and-profile.md) , de az **Eszközök lapon is** tölthet fel eszközöket.</span><span class="sxs-lookup"><span data-stu-id="68ecf-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload devices in the **Devices** tab.</span></span> 
  
<span data-ttu-id="68ecf-107">Az eszközöknek meg kell felelniük ezeknek a követelményeknek:</span><span class="sxs-lookup"><span data-stu-id="68ecf-107">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="68ecf-108">Windows 10, 1703-es vagy újabb verzió</span><span class="sxs-lookup"><span data-stu-id="68ecf-108">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="68ecf-109">Új berendezés amit kikötő ' átmenő Windows ki--ból-doboz tapasztalat</span><span class="sxs-lookup"><span data-stu-id="68ecf-109">New devices that haven't been through Windows out-of-box experience</span></span>

1. <span data-ttu-id="68ecf-110">-Ban Mikroszkóp 365 teendő admin központ, választ **berendezés** \> **robotpilóta**.</span><span class="sxs-lookup"><span data-stu-id="68ecf-110">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="68ecf-111">A **robotpilóta** oldalán válassza ki az eszközök **fület.** \> \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="68ecf-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="68ecf-113">Az **eszközök hozzáadása** panelen tallózással keresse meg a **mentett** \> [eszközlistát tartalmazó CSV-fájlt](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) . \*\*\*\* \></span><span class="sxs-lookup"><span data-stu-id="68ecf-113">On the **Add devices** panel, browse to a [Device list CSV file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) that you prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="68ecf-114">Ezt az információt a hardver forgalmazójától kaphatja meg, vagy a [Get-WindowsAutoPilotInfo PowerShell parancsfájl](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) segítségével hozhat létre CSV-fájlt.</span><span class="sxs-lookup"><span data-stu-id="68ecf-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="68ecf-115">Profil társítása egy eszközhöz vagy az eszközök egy csoportjához</span><span class="sxs-lookup"><span data-stu-id="68ecf-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="68ecf-116">A **Windows előkészítése** lapon válassza az **eszközök** fület, és jelölje be az eszközök melletti jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="68ecf-116">On the **Prepare Windows** page, choose the **Devices** tab, and select the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="68ecf-117">Az **Eszköz** panelen válasszon egy profilt a **Hozzárendelt profil** legördülő listából.</span><span class="sxs-lookup"><span data-stu-id="68ecf-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="68ecf-118">Ha egyetlen profilja sincs még, utasításokért olvassa el az [AutoPilot-profilok létrehozása és szerkesztése](create-and-edit-autopilot-profiles.md) című témakört.</span><span class="sxs-lookup"><span data-stu-id="68ecf-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    

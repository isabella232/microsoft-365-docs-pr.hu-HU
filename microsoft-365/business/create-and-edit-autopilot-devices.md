---
title: AutoPilot-eszközök létrehozása és szerkesztése
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
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Megtudhatja, hogy miként tölthet fel eszközöket az AutoPilot segítségével a Microsoft 365 Business Premium szolgáltatásban. Profilt hozzárendelhet egy eszközhöz vagy eszközcsoporthoz.
ms.openlocfilehash: 8c3d029d682ae30444bdc7d30a4790a8f982e0e0
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44400994"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="6555d-104">AutoPilot-eszközök létrehozása és szerkesztése</span><span class="sxs-lookup"><span data-stu-id="6555d-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="6555d-105">Eszközlista feltöltése</span><span class="sxs-lookup"><span data-stu-id="6555d-105">Upload a list of devices</span></span>

<span data-ttu-id="6555d-106">A részletes [útmutató](add-autopilot-devices-and-profile.md) segítségével feltöltheti az eszközöket, de az **Eszközök** lapon is feltölthet eszközöket.</span><span class="sxs-lookup"><span data-stu-id="6555d-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload devices in the **Devices** tab.</span></span> 
  
<span data-ttu-id="6555d-107">Az eszközöknek meg kell felelniük az alábbi követelményeknek:</span><span class="sxs-lookup"><span data-stu-id="6555d-107">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="6555d-108">Windows 10, 1703-as vagy újabb verzió</span><span class="sxs-lookup"><span data-stu-id="6555d-108">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="6555d-109">Új eszközök, amelyek nem mentették át a Windows beépített élményét</span><span class="sxs-lookup"><span data-stu-id="6555d-109">New devices that haven't been through Windows out-of-box experience</span></span>

1. <span data-ttu-id="6555d-110">A Microsoft 365 Felügyeleti központban válassza az **Eszközök** \> **Autokísérleti**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="6555d-110">In the Microsoft 365 admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="6555d-111">Az **AutoPilot** lapon válassza az **Eszközök** lap \> **Eszközök hozzáadása**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="6555d-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="6555d-113">Az **Eszközök hozzáadása** panelen keresse meg a Bezárás mentése segédprogramot elkészített [Eszközlista CSV-fájlját.](https://docs.microsoft.com/microsoft-365/admin/misc/device-list) \> **Save** \> **Close**</span><span class="sxs-lookup"><span data-stu-id="6555d-113">On the **Add devices** panel, browse to a [Device list CSV file](https://docs.microsoft.com/microsoft-365/admin/misc/device-list) that you prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="6555d-114">Ezeket az információkat beszerezheti a hardver forgalmazójától, vagy használhatja a [Get-WindowsAutoPilotInfo PowerShell parancsfájlt CSV-fájl](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="6555d-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="6555d-115">Profil társítása egy eszközhöz vagy az eszközök egy csoportjához</span><span class="sxs-lookup"><span data-stu-id="6555d-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="6555d-116">A **Windows előkészítése** lapon válassza az **Eszközök** lapot, és jelölje be az egy vagy több eszköz melletti jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="6555d-116">On the **Prepare Windows** page, choose the **Devices** tab, and select the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="6555d-117">Az **Eszköz** panelen válasszon egy profilt a **Hozzárendelt profil** legördülő listából.</span><span class="sxs-lookup"><span data-stu-id="6555d-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="6555d-118">Ha egyetlen profilja sincs még, utasításokért olvassa el az [AutoPilot-profilok létrehozása és szerkesztése](create-and-edit-autopilot-profiles.md) című témakört.</span><span class="sxs-lookup"><span data-stu-id="6555d-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    

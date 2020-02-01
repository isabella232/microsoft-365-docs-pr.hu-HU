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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Megtudhatja, hogy miként tölthet fel eszközöket az AutoPilot használatával a Microsoft 365 Business programban. Profilt rendelhet egy eszközhöz vagy eszközcsoporthoz.
ms.openlocfilehash: 5a99f691b0325f511f34e3a6c3a20f08ee8d909f
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/29/2020
ms.locfileid: "41594011"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="59e63-104">AutoPilot-eszközök létrehozása és szerkesztése</span><span class="sxs-lookup"><span data-stu-id="59e63-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="59e63-105">Eszközlista feltöltése</span><span class="sxs-lookup"><span data-stu-id="59e63-105">Upload a list of devices</span></span>

<span data-ttu-id="59e63-106">A részletes [útmutatósegítségével](add-autopilot-devices-and-profile.md) eszközöket tölthet fel, de az **Eszközök** lapon is feltöltheti az eszközöket.</span><span class="sxs-lookup"><span data-stu-id="59e63-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload devices in the **Devices** tab.</span></span> 
  
<span data-ttu-id="59e63-107">Az eszközöknek meg kell felelniük ezeknek a követelményeknek:</span><span class="sxs-lookup"><span data-stu-id="59e63-107">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="59e63-108">Windows 10, 1703-as vagy újabb verzió</span><span class="sxs-lookup"><span data-stu-id="59e63-108">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="59e63-109">Új eszközök, amelyek nem voltak a Windows beépített élményén</span><span class="sxs-lookup"><span data-stu-id="59e63-109">New devices that haven't been through Windows out-of-box experience</span></span>

1. <span data-ttu-id="59e63-110">A Microsoft 365 Vállalati felügyeleti központban válassza az **Eszközök** \> **AutoPilot**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="59e63-110">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="59e63-111">Az **AutoPilot** lapon válassza \*\*\*\* az \> Eszközök lapot **Eszközök hozzáadása**.</span><span class="sxs-lookup"><span data-stu-id="59e63-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="59e63-113">Az **Eszközök hozzáadása** panelen keresse meg a **Bezárás** **mentése** \> című eszközlistát tartalmazó [CSV-fájlt.](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) \></span><span class="sxs-lookup"><span data-stu-id="59e63-113">On the **Add devices** panel, browse to a [Device list CSV file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) that you prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="59e63-114">Ezeket az információkat a hardver gyártójától szerezheti be, vagy a [Get-WindowsAutoPilotInfo PowerShell parancsfájl](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) segítségével CSV-fájlt hozhat létre.</span><span class="sxs-lookup"><span data-stu-id="59e63-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="59e63-115">Profil társítása egy eszközhöz vagy az eszközök egy csoportjához</span><span class="sxs-lookup"><span data-stu-id="59e63-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="59e63-116">A **Windows előkészítése** lapon válassza az **Eszközök** lapot, és jelölje be az egy vagy több eszköz melletti jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="59e63-116">On the **Prepare Windows** page, choose the **Devices** tab, and select the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="59e63-117">Az **Eszköz** panelen válasszon egy profilt a **Hozzárendelt profil** legördülő listából.</span><span class="sxs-lookup"><span data-stu-id="59e63-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="59e63-118">Ha egyetlen profilja sincs még, utasításokért olvassa el az [AutoPilot-profilok létrehozása és szerkesztése](create-and-edit-autopilot-profiles.md) című témakört.</span><span class="sxs-lookup"><span data-stu-id="59e63-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    

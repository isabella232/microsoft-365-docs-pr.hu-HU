---
title: AutoPilot-profilok létrehozása és szerkesztése
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
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: Ismerje meg, hogyan hozhat létre AutoPilot-profilt, és alkalmazhatja azt egy eszközre, valamint szerkesztheti vagy törölheti a profilt, illetve távolíthat el egy profilt az eszközről.
ms.openlocfilehash: a6e02ab56faeb08718a9831657b55cff0356a4ec
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/21/2020
ms.locfileid: "43627374"
---
# <a name="create-and-edit-autopilot-profiles"></a><span data-ttu-id="c92f0-103">AutoPilot-profilok létrehozása és szerkesztése</span><span class="sxs-lookup"><span data-stu-id="c92f0-103">Create and edit AutoPilot profiles</span></span>

## <a name="create-a-profile"></a><span data-ttu-id="c92f0-104">Profil létrehozása</span><span class="sxs-lookup"><span data-stu-id="c92f0-104">Create a profile</span></span>

<span data-ttu-id="c92f0-105">A profil egy eszközre vagy eszközök csoportjára vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="c92f0-105">A profile applies to a device, or a group of devices,</span></span>
  
1. <span data-ttu-id="c92f0-106">A Microsoft 365 Felügyeleti központban válassza az **Eszközök** \> **Autokísérleti**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c92f0-106">In the Microsoft 365 admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="c92f0-107">Az **AutoPilot** lapon válassza **Profiles** a \> Profilok lap **Profil létrehozása**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c92f0-107">On the **AutoPilot** page, choose the **Profiles** tab \> **Create profile**.</span></span>
    
3. <span data-ttu-id="c92f0-108">A **Profil létrehozása** lapon adja meg a profil nevét, amely segít az azonosításában, például marketing.</span><span class="sxs-lookup"><span data-stu-id="c92f0-108">On the **Create profile** page, enter a name for the profile that helps you identify it, for example Marketing.</span></span> <span data-ttu-id="c92f0-109">Kapcsolja be a kívánt beállítást, majd válassza a **Mentés gombot.**</span><span class="sxs-lookup"><span data-stu-id="c92f0-109">Turn on the setting you want, and then choose **Save**.</span></span> <span data-ttu-id="c92f0-110">Az AutoPilot profilbeállításairól az [AutoPilot-profil beállításai című témakörben](autopilot-profile-settings.md)olvashat bővebben.</span><span class="sxs-lookup"><span data-stu-id="c92f0-110">For more information about AutoPilot profile settings, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span>
    
    ![Enter name and turn on settings in the Create profile panel.](../media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a><span data-ttu-id="c92f0-112">Profil alkalmazása eszközre</span><span class="sxs-lookup"><span data-stu-id="c92f0-112">Apply profile to a device</span></span>

<span data-ttu-id="c92f0-113">Miután létrehozott egy profilt, alkalmazhatja azt egy eszközre vagy eszközök egy csoportjára.</span><span class="sxs-lookup"><span data-stu-id="c92f0-113">After you create a profile, you can apply it to a device or a group of devices.</span></span> <span data-ttu-id="c92f0-114">Kiválaszthat egy meglévő profilt a [részletes útmutatóban,](add-autopilot-devices-and-profile.md) és alkalmazhatja azt új eszközökre, vagy lecserélhet egy meglévő profilt egy eszközre vagy eszközcsoportra.</span><span class="sxs-lookup"><span data-stu-id="c92f0-114">You can pick an existing profile in the [step-by-step guide](add-autopilot-devices-and-profile.md) and apply it to new devices, or replace an existing profile for a device or group of devices.</span></span> 
  
1. <span data-ttu-id="c92f0-115">**A Windows előkészítése** lapon válassza az **Eszközök** fület.</span><span class="sxs-lookup"><span data-stu-id="c92f0-115">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="c92f0-116">Jelölje be az eszköz neve melletti jelölőnégyzetet, és az **Eszköz** panelen válasszon egy profilt a **Hozzárendelt profil** \> **legördülő listából Mentés**.</span><span class="sxs-lookup"><span data-stu-id="c92f0-116">Select the check box next to a device name, and in the **Device** panel, choose a profile from the **Assigned profile** drop-down list \> **Save**.</span></span>
    
    ![In the Device panel, select an Assigned profile to apply it.](../media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a><span data-ttu-id="c92f0-118">Profil szerkesztése, törlése vagy eltávolítása</span><span class="sxs-lookup"><span data-stu-id="c92f0-118">Edit, delete, or remove a profile</span></span>

<span data-ttu-id="c92f0-p103">Miután hozzárendelt egy profilt egy eszközhöz, frissítheti azt még akkor is, ha már odaadta az eszközt egy felhasználónak. Amikor az eszköz csatlakozik az internethez, a beállítási folyamat során letölti a profil legújabb verzióját. Ha a felhasználó visszaállítja az eszköz gyári alapértelmezett beállításait, az eszköz ismét le fogja tölteni a profil legújabb frissítéseit.</span><span class="sxs-lookup"><span data-stu-id="c92f0-p103">Once you've assigned a profile to a device, you can update it, even if you've already given the device to a user. When the device connects to the internet, it downloads the latest version of your profile during the setup process. If the user restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 
  
### <a name="edit-a-profile"></a><span data-ttu-id="c92f0-122">Profil szerkesztése</span><span class="sxs-lookup"><span data-stu-id="c92f0-122">Edit a profile</span></span>

1. <span data-ttu-id="c92f0-123">**A Windows előkészítése** lapon válassza a **Profilok** fület.</span><span class="sxs-lookup"><span data-stu-id="c92f0-123">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="c92f0-124">Jelölje be az eszköz neve melletti jelölőnégyzetet, és a **Profil** \> panelen frissítse a **rendelkezésre**álló Mentés beállítást.</span><span class="sxs-lookup"><span data-stu-id="c92f0-124">Select the check box next to a device name, and in the **Profile** panel, update any of the available settings \> **Save**.</span></span>
    
    <span data-ttu-id="c92f0-125">Ha ezt azelőtt végzi el, hogy a felhasználó csatlakoztatná az eszközt az internetre, akkor a profilt a rendszer alkalmazza a beállítási folyamatra.</span><span class="sxs-lookup"><span data-stu-id="c92f0-125">If you do this before a user connects the device to the internet, then the profile gets applied to the setup process.</span></span>
    
### <a name="delete-a-profile"></a><span data-ttu-id="c92f0-126">Profil törlése</span><span class="sxs-lookup"><span data-stu-id="c92f0-126">Delete a profile</span></span>

1. <span data-ttu-id="c92f0-127">**A Windows előkészítése** lapon válassza a **Profilok** fület.</span><span class="sxs-lookup"><span data-stu-id="c92f0-127">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="c92f0-128">Jelölje be az eszköz neve melletti jelölőnégyzetet, és a **Profil** panelen válassza a **Profil** \> **mentése törlése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="c92f0-128">Select the check box next to a device name, and in the **Profile** panel, select **Delete profile** \> **Save**.</span></span>
    
    <span data-ttu-id="c92f0-129">A törléssel a profilt eltávolítja arról az eszközről vagy abból az eszközcsoportból, amelyhez hozzá volt rendelve.</span><span class="sxs-lookup"><span data-stu-id="c92f0-129">When you delete a profile, it gets removed from a device or a group of devices it was assigned to.</span></span>
    
### <a name="remove-a-profile"></a><span data-ttu-id="c92f0-130">Profil eltávolítása</span><span class="sxs-lookup"><span data-stu-id="c92f0-130">Remove a profile</span></span>

1. <span data-ttu-id="c92f0-131">**A Windows előkészítése** lapon válassza az **Eszközök** fület.</span><span class="sxs-lookup"><span data-stu-id="c92f0-131">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="c92f0-132">Jelölje be az eszköz neve melletti jelölőnégyzetet, és az **Eszköz** panelen válassza a **Nincs** lehetőséget a **Hozzárendelt profil** legördülő \> **lista Mentés listájában.**</span><span class="sxs-lookup"><span data-stu-id="c92f0-132">Select the check box next to a device name, and in the **Device** panel, choose **None** from the **Assigned profile** drop-down list \> **Save**.</span></span>
    

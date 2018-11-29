---
title: AutoPilot-profilok létrehozása és szerkesztése
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: 'Ismerje meg, hogyan létrehozása, szerkesztése, törlése vagy automata profilok eltávolítása. '
ms.openlocfilehash: 4658a27e5f2c64a52f8a7d08b3fc13df5e239dc3
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983135"
---
# <a name="create-and-edit-autopilot-profiles"></a><span data-ttu-id="f0366-103">AutoPilot-profilok létrehozása és szerkesztése</span><span class="sxs-lookup"><span data-stu-id="f0366-103">Create and edit AutoPilot profiles</span></span>

## <a name="create-a-profile"></a><span data-ttu-id="f0366-104">Profil létrehozása</span><span class="sxs-lookup"><span data-stu-id="f0366-104">Create a profile</span></span>

<span data-ttu-id="f0366-105">A profil egy eszközre vagy eszközök csoportjára vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="f0366-105">A profile applies to a device, or a group of devices,</span></span>
  
1. <span data-ttu-id="f0366-106">A Microsoft 365 Business Felügyeleti központban válassza **A Windows üzembe helyezése az AutoPilottal** lehetőséget az **Eszközműveletek** kártyán.</span><span class="sxs-lookup"><span data-stu-id="f0366-106">In the Microsoft 365 Business Admin center, choose **Deploy Windows with AutoPilot** on the **Device actions** card.</span></span> 
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. <span data-ttu-id="f0366-108">**A Windows előkészítése** lapon válassza a **Profilok** \> **Profil létrehozása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f0366-108">On the **Prepare Windows** page, choose the **Profiles** tab \> **Create profile**.</span></span>
    
3. <span data-ttu-id="f0366-109">A **Profil létrehozása** lapon írjon be egy azonosítást segítő nevet a profilhoz, például Marketing, kapcsolja be a kívánt beállítást (további információ: [Az AutoPilot-profil beállításai](autopilot-profile-settings.md)), és válassza a **Mentés** gombot.</span><span class="sxs-lookup"><span data-stu-id="f0366-109">On the **Create profile** page, enter a name for the profile that helps you identify it, for example Marketing, turn on the setting you want (see [About AutoPilot Profile settings](autopilot-profile-settings.md) for more information), and choose **Save**.</span></span>
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a><span data-ttu-id="f0366-111">Profil alkalmazása eszközre</span><span class="sxs-lookup"><span data-stu-id="f0366-111">Apply profile to a device</span></span>

<span data-ttu-id="f0366-p101">A profil létrehozása után alkalmazhatja azt egy eszközre vagy eszközcsoportra. Kiválaszthat egy meglévő profilt a [részletes útmutatóban](add-autopilot-devices-and-profile.md), és alkalmazhatja azt új eszközökre, vagy lecserélheti egy eszköz vagy eszközcsoport meglévő profilját.</span><span class="sxs-lookup"><span data-stu-id="f0366-p101">After you create a profile you can apply it to a device or a group of devices. You can pick an existing profile in the [step-by-step guide](add-autopilot-devices-and-profile.md), you can apply it to new devices, or you can replace an existing profile for a device or group of devices.</span></span> 
  
1. <span data-ttu-id="f0366-114">**A Windows előkészítése** lapon válassza az **Eszközök** fület.</span><span class="sxs-lookup"><span data-stu-id="f0366-114">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="f0366-115">A jelölőnégyzetet egy eszköz neve mellett, és az **eszközök** panelen kattintson a, válasszon egy profilt a **hozzárendelt profil** legördülő \> **mentése**.</span><span class="sxs-lookup"><span data-stu-id="f0366-115">Click the check-box next to a device name and in the **Device** panel, choose a profile from the **Assigned profile** drop-down \> **Save**.</span></span>
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a><span data-ttu-id="f0366-117">Profil szerkesztése, törlése vagy eltávolítása</span><span class="sxs-lookup"><span data-stu-id="f0366-117">Edit, delete, or remove a profile</span></span>

<span data-ttu-id="f0366-p102">Miután hozzárendelt egy profilt egy eszközhöz, frissítheti azt még akkor is, ha már odaadta az eszközt egy felhasználónak. Amikor az eszköz csatlakozik az internethez, a beállítási folyamat során letölti a profil legújabb verzióját. Ha a felhasználó visszaállítja az eszköz gyári alapértelmezett beállításait, az eszköz ismét le fogja tölteni a profil legújabb frissítéseit.</span><span class="sxs-lookup"><span data-stu-id="f0366-p102">Once you've assigned a profile to a device, you can update it, even if you've already given the device to a user. When the device connects to the internet, it downloads the latest version of your profile during the setup process. If the user restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 
  
### <a name="edit-a-profile"></a><span data-ttu-id="f0366-121">Profil szerkesztése</span><span class="sxs-lookup"><span data-stu-id="f0366-121">Edit a profile</span></span>

1. <span data-ttu-id="f0366-122">**A Windows előkészítése** lapon válassza a **Profilok** fület.</span><span class="sxs-lookup"><span data-stu-id="f0366-122">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="f0366-123">Kattintson az eszköz neve melletti jelölőnégyzetet, és a **profil** panel frissíti a rendelkezésre álló beállítások \> **mentése**.</span><span class="sxs-lookup"><span data-stu-id="f0366-123">Click the check-box next to a device name and in the **Profile** panel update any of the available settings \> **Save**.</span></span>
    
    <span data-ttu-id="f0366-124">Ha ezt azelőtt végzi el, hogy a felhasználó csatlakoztatná az eszközt az internetre, akkor a profilt a rendszer alkalmazza a beállítási folyamatra.</span><span class="sxs-lookup"><span data-stu-id="f0366-124">If you do this before a user connects the device to the internet, then the profile gets applied to the setup process.</span></span>
    
### <a name="delete-a-profile"></a><span data-ttu-id="f0366-125">Profil törlése</span><span class="sxs-lookup"><span data-stu-id="f0366-125">Delete a profile</span></span>

1. <span data-ttu-id="f0366-126">**A Windows előkészítése** lapon válassza a **Profilok** fület.</span><span class="sxs-lookup"><span data-stu-id="f0366-126">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="f0366-127">Jelölje be az egyik eszköz neve melletti jelölőnégyzetet, és a **Profil** panelen kattintson a **Profil törlése** \> **Mentés** elemre.</span><span class="sxs-lookup"><span data-stu-id="f0366-127">Click the check-box next to a device name and in the **Profile** panel click **Delete profile** \> **Save**.</span></span>
    
    <span data-ttu-id="f0366-128">A törléssel a profilt eltávolítja arról az eszközről vagy abból az eszközcsoportból, amelyhez hozzá volt rendelve.</span><span class="sxs-lookup"><span data-stu-id="f0366-128">When you delete a profile, it gets removed from a device or a group of devices it was assigned to.</span></span>
    
### <a name="remove-a-profile"></a><span data-ttu-id="f0366-129">Profil eltávolítása</span><span class="sxs-lookup"><span data-stu-id="f0366-129">Remove a profile</span></span>

1. <span data-ttu-id="f0366-130">**A Windows előkészítése** lapon válassza az **Eszközök** fület.</span><span class="sxs-lookup"><span data-stu-id="f0366-130">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="f0366-131">Jelölje be a jelölőnégyzetet-egy eszköz neve mellett, és az **eszközök** panelen, válassza a **nincs** **hozzárendelt profil** legördülő \> **mentése**.</span><span class="sxs-lookup"><span data-stu-id="f0366-131">Click the check-box next to a device name and in the **Device** panel, choose a **None** from the **Assigned profile** drop-down \> **Save**.</span></span>
    

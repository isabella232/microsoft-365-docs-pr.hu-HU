---
title: AutoPilot-profilok létrehozása és szerkesztése
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
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: Ismerkedjen meg a robotpilóta-profilok létrehozásával, szerkesztésével, törlésével vagy eltávolításával.
ms.openlocfilehash: f7fdc2632e93c48e043fe158842f8395d6a89e14
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/14/2019
ms.locfileid: "38320238"
---
# <a name="create-and-edit-autopilot-profiles"></a><span data-ttu-id="9e848-103">AutoPilot-profilok létrehozása és szerkesztése</span><span class="sxs-lookup"><span data-stu-id="9e848-103">Create and edit AutoPilot profiles</span></span>

## <a name="create-a-profile"></a><span data-ttu-id="9e848-104">Profil létrehozása</span><span class="sxs-lookup"><span data-stu-id="9e848-104">Create a profile</span></span>

<span data-ttu-id="9e848-105">A profil egy eszközre vagy eszközök csoportjára vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="9e848-105">A profile applies to a device, or a group of devices,</span></span>
  
1. <span data-ttu-id="9e848-106">-Ban Mikroszkóp 365 teendő admin központ, választ **berendezés** \> **robotpilóta**.</span><span class="sxs-lookup"><span data-stu-id="9e848-106">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="9e848-107">A **robotpilóta** oldalon válassza a profil lap \*\*\*\* \> **létrehozása profilt**.</span><span class="sxs-lookup"><span data-stu-id="9e848-107">On the **AutoPilot** page, choose the **Profiles** tab \> **Create profile**.</span></span>
    
3. <span data-ttu-id="9e848-108">A **profil létrehozása** lapon adjon nevet a profilnak, amely segít azonosítani, például marketing.</span><span class="sxs-lookup"><span data-stu-id="9e848-108">On the **Create profile** page, enter a name for the profile that helps you identify it, for example Marketing.</span></span> <span data-ttu-id="9e848-109">Kapcsolja be a kívánt beállítást, majd kattintson a **Mentés**gombra.</span><span class="sxs-lookup"><span data-stu-id="9e848-109">Turn on the setting you want, and then choose **Save**.</span></span> <span data-ttu-id="9e848-110">A robotpilóta profilbeállításaival kapcsolatos további tudnivalókért tanulmányozza az [robotpilóta-profil beállításai](autopilot-profile-settings.md)című témakört.</span><span class="sxs-lookup"><span data-stu-id="9e848-110">For more information about AutoPilot profile settings, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span>
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a><span data-ttu-id="9e848-112">Profil alkalmazása eszközre</span><span class="sxs-lookup"><span data-stu-id="9e848-112">Apply profile to a device</span></span>

<span data-ttu-id="9e848-113">A profil létrehozása után alkalmazhatja azt egy eszközre vagy eszközcsoportra.</span><span class="sxs-lookup"><span data-stu-id="9e848-113">After you create a profile, you can apply it to a device or a group of devices.</span></span> <span data-ttu-id="9e848-114">A [Részletes útmutató](add-autopilot-devices-and-profile.md) segítségével egy meglévő profilt választhat ki, és alkalmazhatja azt az új eszközökre, vagy kicserélheti egy eszköz vagy eszközcsoport meglévő profilját.</span><span class="sxs-lookup"><span data-stu-id="9e848-114">You can pick an existing profile in the [step-by-step guide](add-autopilot-devices-and-profile.md) and apply it to new devices, or replace an existing profile for a device or group of devices.</span></span> 
  
1. <span data-ttu-id="9e848-115">**A Windows előkészítése** lapon válassza az **Eszközök** fület.</span><span class="sxs-lookup"><span data-stu-id="9e848-115">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="9e848-116">Jelölje be az eszköznév melletti jelölőnégyzetet, majd az **eszközpanelen** válasszon egy profilt a **hozzárendelt profil** \> **legördülő listáról.**</span><span class="sxs-lookup"><span data-stu-id="9e848-116">Select the check box next to a device name, and in the **Device** panel, choose a profile from the **Assigned profile** drop-down list \> **Save**.</span></span>
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a><span data-ttu-id="9e848-118">Profil szerkesztése, törlése vagy eltávolítása</span><span class="sxs-lookup"><span data-stu-id="9e848-118">Edit, delete, or remove a profile</span></span>

<span data-ttu-id="9e848-p103">Miután hozzárendelt egy profilt egy eszközhöz, frissítheti azt még akkor is, ha már odaadta az eszközt egy felhasználónak. Amikor az eszköz csatlakozik az internethez, a beállítási folyamat során letölti a profil legújabb verzióját. Ha a felhasználó visszaállítja az eszköz gyári alapértelmezett beállításait, az eszköz ismét le fogja tölteni a profil legújabb frissítéseit.</span><span class="sxs-lookup"><span data-stu-id="9e848-p103">Once you've assigned a profile to a device, you can update it, even if you've already given the device to a user. When the device connects to the internet, it downloads the latest version of your profile during the setup process. If the user restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 
  
### <a name="edit-a-profile"></a><span data-ttu-id="9e848-122">Profil szerkesztése</span><span class="sxs-lookup"><span data-stu-id="9e848-122">Edit a profile</span></span>

1. <span data-ttu-id="9e848-123">**A Windows előkészítése** lapon válassza a **Profilok** fület.</span><span class="sxs-lookup"><span data-stu-id="9e848-123">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="9e848-124">Jelölje be az eszköz neve melletti jelölőnégyzetet, és a **profil** panelen frissítse az elérhető beállítások \> **mentését**.</span><span class="sxs-lookup"><span data-stu-id="9e848-124">Select the check box next to a device name, and in the **Profile** panel, update any of the available settings \> **Save**.</span></span>
    
    <span data-ttu-id="9e848-125">Ha ezt azelőtt végzi el, hogy a felhasználó csatlakoztatná az eszközt az internetre, akkor a profilt a rendszer alkalmazza a beállítási folyamatra.</span><span class="sxs-lookup"><span data-stu-id="9e848-125">If you do this before a user connects the device to the internet, then the profile gets applied to the setup process.</span></span>
    
### <a name="delete-a-profile"></a><span data-ttu-id="9e848-126">Profil törlése</span><span class="sxs-lookup"><span data-stu-id="9e848-126">Delete a profile</span></span>

1. <span data-ttu-id="9e848-127">**A Windows előkészítése** lapon válassza a **Profilok** fület.</span><span class="sxs-lookup"><span data-stu-id="9e848-127">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="9e848-128">Jelölje be az eszköznév melletti jelölőnégyzetet, majd a **profil** panelen jelölje be a **profilmentés** \> \*\*\*\* törlése négyzetet.</span><span class="sxs-lookup"><span data-stu-id="9e848-128">Select the check box next to a device name, and in the **Profile** panel, select **Delete profile** \> **Save**.</span></span>
    
    <span data-ttu-id="9e848-129">A törléssel a profilt eltávolítja arról az eszközről vagy abból az eszközcsoportból, amelyhez hozzá volt rendelve.</span><span class="sxs-lookup"><span data-stu-id="9e848-129">When you delete a profile, it gets removed from a device or a group of devices it was assigned to.</span></span>
    
### <a name="remove-a-profile"></a><span data-ttu-id="9e848-130">Profil eltávolítása</span><span class="sxs-lookup"><span data-stu-id="9e848-130">Remove a profile</span></span>

1. <span data-ttu-id="9e848-131">**A Windows előkészítése** lapon válassza az **Eszközök** fület.</span><span class="sxs-lookup"><span data-stu-id="9e848-131">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="9e848-132">Jelölje be az eszköznév melletti jelölőnégyzetet, az **eszközpanelen** pedig válassza a **nincs** beállítást a **hozzárendelt profil** legördülő \> **listából.**</span><span class="sxs-lookup"><span data-stu-id="9e848-132">Select the check box next to a device name, and in the **Device** panel, choose **None** from the **Assigned profile** drop-down list \> **Save**.</span></span>
    

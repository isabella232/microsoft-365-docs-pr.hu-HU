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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: Ismerje meg, hogyan hozhat létre AutoPilot-profilt, és alkalmazhatja azt egy eszközre, valamint szerkesztsen vagy töröljön egy profilt, illetve távolítson el egy profilt az eszközről.
ms.openlocfilehash: 6a8057969242d839ebbb4cbef8d26dd3f1858c59
ms.sourcegitcommit: d6c871bf3f94d9299d22695f5dbaf25dc1bd6ff9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42417336"
---
# <a name="create-and-edit-autopilot-profiles"></a><span data-ttu-id="844ab-103">AutoPilot-profilok létrehozása és szerkesztése</span><span class="sxs-lookup"><span data-stu-id="844ab-103">Create and edit AutoPilot profiles</span></span>

## <a name="create-a-profile"></a><span data-ttu-id="844ab-104">Profil létrehozása</span><span class="sxs-lookup"><span data-stu-id="844ab-104">Create a profile</span></span>

<span data-ttu-id="844ab-105">A profil egy eszközre vagy eszközök csoportjára vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="844ab-105">A profile applies to a device, or a group of devices,</span></span>
  
1. <span data-ttu-id="844ab-106">A Microsoft 365 Vállalati felügyeleti központban válassza az **Eszközök** \> **AutoPilot**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="844ab-106">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="844ab-107">Az **AutoPilot** lapon válassza \*\*\*\* a \> Profilok lapot **Profil létrehozása**.</span><span class="sxs-lookup"><span data-stu-id="844ab-107">On the **AutoPilot** page, choose the **Profiles** tab \> **Create profile**.</span></span>
    
3. <span data-ttu-id="844ab-108">A **Profil létrehozása** lapon adja meg a profil nevét, amely segít azonosítani azt, például a Marketing.</span><span class="sxs-lookup"><span data-stu-id="844ab-108">On the **Create profile** page, enter a name for the profile that helps you identify it, for example Marketing.</span></span> <span data-ttu-id="844ab-109">Kapcsolja be a kívánt beállítást, majd kattintson a **Mentés gombra.**</span><span class="sxs-lookup"><span data-stu-id="844ab-109">Turn on the setting you want, and then choose **Save**.</span></span> <span data-ttu-id="844ab-110">Az AutoPilot profilbeállításairól további információt [az AutoPilot-profil beállításairól című témakörben](autopilot-profile-settings.md)talál.</span><span class="sxs-lookup"><span data-stu-id="844ab-110">For more information about AutoPilot profile settings, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span>
    
    ![Enter name and turn on settings in the Create profile panel.](../media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a><span data-ttu-id="844ab-112">Profil alkalmazása eszközre</span><span class="sxs-lookup"><span data-stu-id="844ab-112">Apply profile to a device</span></span>

<span data-ttu-id="844ab-113">Miután létrehozott egy profilt, alkalmazhatja azt egy eszközre vagy eszközcsoportra.</span><span class="sxs-lookup"><span data-stu-id="844ab-113">After you create a profile, you can apply it to a device or a group of devices.</span></span> <span data-ttu-id="844ab-114">A [részletes útmutatóban](add-autopilot-devices-and-profile.md) kiválaszthatja a meglévő profilt, és alkalmazhatja azt új eszközökre, vagy lecserélhet egy meglévő profilt egy eszközre vagy eszközcsoportra.</span><span class="sxs-lookup"><span data-stu-id="844ab-114">You can pick an existing profile in the [step-by-step guide](add-autopilot-devices-and-profile.md) and apply it to new devices, or replace an existing profile for a device or group of devices.</span></span> 
  
1. <span data-ttu-id="844ab-115">**A Windows előkészítése** lapon válassza az **Eszközök** fület.</span><span class="sxs-lookup"><span data-stu-id="844ab-115">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="844ab-116">Jelölje be az eszköznév melletti jelölőnégyzetet, és az **Eszköz** panelen válasszon egy profilt a **Hozzárendelt profil** legördülő \> **listából Mentés**.</span><span class="sxs-lookup"><span data-stu-id="844ab-116">Select the check box next to a device name, and in the **Device** panel, choose a profile from the **Assigned profile** drop-down list \> **Save**.</span></span>
    
    ![In the Device panel, select an Assigned profile to apply it.](../media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a><span data-ttu-id="844ab-118">Profil szerkesztése, törlése vagy eltávolítása</span><span class="sxs-lookup"><span data-stu-id="844ab-118">Edit, delete, or remove a profile</span></span>

<span data-ttu-id="844ab-p103">Miután hozzárendelt egy profilt egy eszközhöz, frissítheti azt még akkor is, ha már odaadta az eszközt egy felhasználónak. Amikor az eszköz csatlakozik az internethez, a beállítási folyamat során letölti a profil legújabb verzióját. Ha a felhasználó visszaállítja az eszköz gyári alapértelmezett beállításait, az eszköz ismét le fogja tölteni a profil legújabb frissítéseit.</span><span class="sxs-lookup"><span data-stu-id="844ab-p103">Once you've assigned a profile to a device, you can update it, even if you've already given the device to a user. When the device connects to the internet, it downloads the latest version of your profile during the setup process. If the user restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 
  
### <a name="edit-a-profile"></a><span data-ttu-id="844ab-122">Profil szerkesztése</span><span class="sxs-lookup"><span data-stu-id="844ab-122">Edit a profile</span></span>

1. <span data-ttu-id="844ab-123">**A Windows előkészítése** lapon válassza a **Profilok** fület.</span><span class="sxs-lookup"><span data-stu-id="844ab-123">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="844ab-124">Jelölje be az eszközneve melletti jelölőnégyzetet, és a **Profil** panelen frissítse a rendelkezésre álló beállítások \> bármelyikét **Mentés**.</span><span class="sxs-lookup"><span data-stu-id="844ab-124">Select the check box next to a device name, and in the **Profile** panel, update any of the available settings \> **Save**.</span></span>
    
    <span data-ttu-id="844ab-125">Ha ezt azelőtt végzi el, hogy a felhasználó csatlakoztatná az eszközt az internetre, akkor a profilt a rendszer alkalmazza a beállítási folyamatra.</span><span class="sxs-lookup"><span data-stu-id="844ab-125">If you do this before a user connects the device to the internet, then the profile gets applied to the setup process.</span></span>
    
### <a name="delete-a-profile"></a><span data-ttu-id="844ab-126">Profil törlése</span><span class="sxs-lookup"><span data-stu-id="844ab-126">Delete a profile</span></span>

1. <span data-ttu-id="844ab-127">**A Windows előkészítése** lapon válassza a **Profilok** fület.</span><span class="sxs-lookup"><span data-stu-id="844ab-127">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="844ab-128">Jelölje be az eszközneve melletti jelölőnégyzetet, majd a **Profil panelen** válassza a \> Profil **mentése** **törlése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="844ab-128">Select the check box next to a device name, and in the **Profile** panel, select **Delete profile** \> **Save**.</span></span>
    
    <span data-ttu-id="844ab-129">A törléssel a profilt eltávolítja arról az eszközről vagy abból az eszközcsoportból, amelyhez hozzá volt rendelve.</span><span class="sxs-lookup"><span data-stu-id="844ab-129">When you delete a profile, it gets removed from a device or a group of devices it was assigned to.</span></span>
    
### <a name="remove-a-profile"></a><span data-ttu-id="844ab-130">Profil eltávolítása</span><span class="sxs-lookup"><span data-stu-id="844ab-130">Remove a profile</span></span>

1. <span data-ttu-id="844ab-131">**A Windows előkészítése** lapon válassza az **Eszközök** fület.</span><span class="sxs-lookup"><span data-stu-id="844ab-131">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="844ab-132">Jelölje be az eszköznév melletti jelölőnégyzetet, és az **Eszköz** panelen válassza a \> **Hozzárendelési profil** mentés i. listájának Nincs **elemét.** \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="844ab-132">Select the check box next to a device name, and in the **Device** panel, choose **None** from the **Assigned profile** drop-down list \> **Save**.</span></span>
    

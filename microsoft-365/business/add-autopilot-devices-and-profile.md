---
title: Autopilot-eszközök és -profilok hozzáadása a lépésenkénti útmutatóval
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection:
- M365-subscription-management
- M365-identity-device-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Megtudhatja, hogy a Windows AutoPilot segítségével hogyan állíthatja be az új Windows 10-es eszközöket a vállalkozása számára, hogy készen álljanak az alkalmazottak használatára.
ms.openlocfilehash: 3b1cf297914862aaa74fdf9a8bb7290d00f73b1d
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/07/2020
ms.locfileid: "42561580"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="f90bd-103">Autopilot-eszközök és -profilok hozzáadása a lépésenkénti útmutatóval</span><span class="sxs-lookup"><span data-stu-id="f90bd-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="f90bd-104">A Windows AutoPilot segítségével **új** Windows 10-es eszközöket állíthat be a vállalkozása számára, hogy azok készen álljanak a használatra, amikor átadja azokat az alkalmazottaknak.</span><span class="sxs-lookup"><span data-stu-id="f90bd-104">You can use Windows AutoPilot to set up **new** Windows 10 devices for your business so they're ready for use when you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="f90bd-105">Eszközkövetelmények</span><span class="sxs-lookup"><span data-stu-id="f90bd-105">Device requirements</span></span>

<span data-ttu-id="f90bd-106">Az eszközöknek meg kell felelniük ezeknek a követelményeknek:</span><span class="sxs-lookup"><span data-stu-id="f90bd-106">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="f90bd-107">Windows 10, 1703-as vagy újabb verzió</span><span class="sxs-lookup"><span data-stu-id="f90bd-107">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="f90bd-108">Új eszközök, amelyek nem voltak a Windows beépített élményén</span><span class="sxs-lookup"><span data-stu-id="f90bd-108">New devices that haven't been through Windows out-of-box experience</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="f90bd-109">Eszközök és profilok létrehozása a beállítási útmutató használatával</span><span class="sxs-lookup"><span data-stu-id="f90bd-109">Use the setup guide to create devices and profiles</span></span>

<span data-ttu-id="f90bd-110">[![A megjelenő címke figyelmeztet a felügyeleti központ változásaira, további részleteket itt talál: aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="f90bd-110">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="f90bd-111">Ha még nem hozott létre eszközcsoportokat vagy profilokat, a legjobb módja az első lépéseknek a részletes útmutató használatával.</span><span class="sxs-lookup"><span data-stu-id="f90bd-111">If you haven't created device groups or profiles yet, the best way to get started is by using the step-by-step guide.</span></span> <span data-ttu-id="f90bd-112">Eszközöket is [hozzáadhat,](create-and-edit-autopilot-devices.md) és [profilokat rendelhet](create-and-edit-autopilot-profiles.md) hozzájuk az útmutató használata nélkül.</span><span class="sxs-lookup"><span data-stu-id="f90bd-112">You can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="f90bd-113">Nyissa meg a <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>felügyeleti központot a .</span><span class="sxs-lookup"><span data-stu-id="f90bd-113">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="f90bd-114">A bal oldali navigációs ablakban válassza az **Eszközök** \> **AutoPilot**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="f90bd-114">On the left navigation pane, choose **Devices** \> **AutoPilot**.</span></span>

    ![A felügyeleti központban válassza az eszközök, majd az AutoPilot lehetőséget.](../media/AutoPilot.png)
  
2. <span data-ttu-id="f90bd-116">Az **AutoPilot** lapon kattintson vagy koppintson az **Útmutató indítása**elemre.</span><span class="sxs-lookup"><span data-stu-id="f90bd-116">On the **AutoPilot** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="f90bd-118">A **Feltöltés .csv fájl eszközök listájával** lapon keresse meg azt a helyet, ahol előkészítette a fájlt. CSV fájlt, majd **nyissa meg** \> **a Tovább**.</span><span class="sxs-lookup"><span data-stu-id="f90bd-118">On the **Upload .csv file with list of devices** page, browse to a location where you have the prepared .CSV file, then **Open** \> **Next**.</span></span> <span data-ttu-id="f90bd-119">A fájlnak három fejlécből kell rendelkeznie:</span><span class="sxs-lookup"><span data-stu-id="f90bd-119">The file must have three headers:</span></span>
    
    - <span data-ttu-id="f90bd-120">A oszlop: Eszköz sorozatszáma</span><span class="sxs-lookup"><span data-stu-id="f90bd-120">Column A: Device Serial Number</span></span>
    
    - <span data-ttu-id="f90bd-121">B oszlop: Windows-termékazonosító</span><span class="sxs-lookup"><span data-stu-id="f90bd-121">Column B: Windows Product ID</span></span>
    
    - <span data-ttu-id="f90bd-122">C oszlop: Hardverkivonat</span><span class="sxs-lookup"><span data-stu-id="f90bd-122">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="f90bd-123">Ezeket az információkat a hardver gyártójától szerezheti be, vagy a [Get-WindowsAutoPilotInfo PowerShell parancsfájl](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) segítségével CSV-fájlt hozhat létre.</span><span class="sxs-lookup"><span data-stu-id="f90bd-123">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
    <span data-ttu-id="f90bd-p103">További információ: [Eszközlistát tartalmazó CSV-fájl](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Az **Eszközlistát tartalmazó CSV-fájl feltöltése** lapon egy mintafájlt is letölthet.</span><span class="sxs-lookup"><span data-stu-id="f90bd-p103">For more information, see [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
4. <span data-ttu-id="f90bd-126">A **Profil hozzárendelése** lapon választhat egy meglévő profilt, vagy létrehozhat egy újat.</span><span class="sxs-lookup"><span data-stu-id="f90bd-126">On the **Assign a profile** page, you can either pick an existing profile or create a new one.</span></span> <span data-ttu-id="f90bd-127">Ha még nem rendelkezik ilyenvel, a rendszer kérni fogja, hogy hozzon létre egyet.</span><span class="sxs-lookup"><span data-stu-id="f90bd-127">If you don't have one yet, you'll be prompted to create one.</span></span> 
    
    <span data-ttu-id="f90bd-128">A profil azoknak a beállításoknak a gyűjteménye, amelyek egyetlen eszközre vagy eszközök csoportjára lehet alkalmazni.</span><span class="sxs-lookup"><span data-stu-id="f90bd-128">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="f90bd-129">Az alapértelmezett funkciók szükségesek, és automatikusan be vannak állítva.</span><span class="sxs-lookup"><span data-stu-id="f90bd-129">The default features are required and are set automatically.</span></span> <span data-ttu-id="f90bd-130">Az alapértelmezett funkciók az alábbiak:</span><span class="sxs-lookup"><span data-stu-id="f90bd-130">The default features are:</span></span>
    
    - <span data-ttu-id="f90bd-131">Cortana, OneDrive és OEM regisztráció kihagyása.</span><span class="sxs-lookup"><span data-stu-id="f90bd-131">Skip Cortana, OneDrive, and OEM registration.</span></span>
    
    - <span data-ttu-id="f90bd-132">Bejelentkezés céges márkával.</span><span class="sxs-lookup"><span data-stu-id="f90bd-132">Create sign-in experience with your company brand.</span></span>
    
    - <span data-ttu-id="f90bd-133">Csatlakoztassa eszközeit az Azure Active Directory-fiókokhoz, és automatikusan regisztrálhatja őket a Microsoft 365 Business általi felügyelthez.</span><span class="sxs-lookup"><span data-stu-id="f90bd-133">Connect your devices to Azure Active Directory accounts, and automatically enroll them to be managed by Microsoft 365 Business.</span></span>
    
    <span data-ttu-id="f90bd-134">További információt [az AutoPilot-profil beállításairól című témakörben](autopilot-profile-settings.md)talál.</span><span class="sxs-lookup"><span data-stu-id="f90bd-134">For more information, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span> 
    
5. <span data-ttu-id="f90bd-135">A további beállítások: **Adatvédelmi beállítások kihagyása** és **Nem léptethető elő a felhasználó a helyi rendszergazdává**. Mindkettő értéke alapértelmezés szerint **Kikapcsolva**.</span><span class="sxs-lookup"><span data-stu-id="f90bd-135">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="f90bd-136">Válassza a **Tovább** gombot.</span><span class="sxs-lookup"><span data-stu-id="f90bd-136">Choose **Next**.</span></span>
    
6. <span data-ttu-id="f90bd-137">**A kész azt** jelzi, hogy a létrehozott (vagy kiválasztott) profil az eszközök listájának feltöltésével létrehozott eszközcsoportra lesz alkalmazva.</span><span class="sxs-lookup"><span data-stu-id="f90bd-137">**You're done** indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices.</span></span> <span data-ttu-id="f90bd-138">A beállítások akkor lépnek érvénybe, amikor az eszköz felhasználók bejelentkeznek legközelebb.</span><span class="sxs-lookup"><span data-stu-id="f90bd-138">The settings will be in effect when the device users sign in next.</span></span> <span data-ttu-id="f90bd-139">Válassza a **Bezárás** gombot.</span><span class="sxs-lookup"><span data-stu-id="f90bd-139">Choose **Close**.</span></span>
    

---
title: Autopilot-eszközök és -profilok hozzáadása a lépésenkénti útmutatóval
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: A Windows AutoPilot használata új Windows 10 eszközök beállítására a vállalat számára.
ms.openlocfilehash: 5f40dac57285b83da57d4506bac58e562475522c
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/14/2019
ms.locfileid: "38323095"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="850dc-103">Autopilot-eszközök és -profilok hozzáadása a lépésenkénti útmutatóval</span><span class="sxs-lookup"><span data-stu-id="850dc-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="850dc-104">Használhatja a Windows AutoPilot, hogy hozzanak létre **új** Windows 10 eszközök a vállalkozás számára, így ők készen áll, amikor megadja nekik az alkalmazottak.</span><span class="sxs-lookup"><span data-stu-id="850dc-104">You can use Windows AutoPilot to set up **new** Windows 10 devices for your business so they're ready for use when you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="850dc-105">Eszközkövetelmények</span><span class="sxs-lookup"><span data-stu-id="850dc-105">Device requirements</span></span>

<span data-ttu-id="850dc-106">Az eszközöknek meg kell felelniük ezeknek a követelményeknek:</span><span class="sxs-lookup"><span data-stu-id="850dc-106">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="850dc-107">Windows 10, 1703-es vagy újabb verzió</span><span class="sxs-lookup"><span data-stu-id="850dc-107">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="850dc-108">Új berendezés amit kikötő ' átmenő Windows ki--ból-doboz tapasztalat</span><span class="sxs-lookup"><span data-stu-id="850dc-108">New devices that haven't been through Windows out-of-box experience</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="850dc-109">Eszközök és profilok létrehozása a beállítási útmutató használatával</span><span class="sxs-lookup"><span data-stu-id="850dc-109">Use the setup guide to create devices and profiles</span></span>

<span data-ttu-id="850dc-110">[![A megjelenő címke figyelmeztet a felügyeleti központ változásaira, további részleteket itt talál: aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="850dc-110">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="850dc-111">Ha még nem hozott létre eszközcsoportokat vagy profilokat, a legjobb módszer a részletes útmutató használatával a kezdéshez.</span><span class="sxs-lookup"><span data-stu-id="850dc-111">If you haven't created device groups or profiles yet, the best way to get started is by using the step-by-step guide.</span></span> <span data-ttu-id="850dc-112">A segédvonal használata nélkül is [hozzáadhat eszközöket](create-and-edit-autopilot-devices.md) , és [profilokat rendelhet](create-and-edit-autopilot-profiles.md) hozzájuk.</span><span class="sxs-lookup"><span data-stu-id="850dc-112">You can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="850dc-113">Menj az admin központba <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span><span class="sxs-lookup"><span data-stu-id="850dc-113">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="850dc-114">A bal oldali navigációs ablaktáblán kattintson az **eszközök** \> **robotpilóta**parancsra.</span><span class="sxs-lookup"><span data-stu-id="850dc-114">On the left navigation pane, choose **Devices** \> **AutoPilot**.</span></span>

    ![Az admin központban, válasszon eszközöket, majd robotpilóta.](media/AutoPilot.png)
  
2. <span data-ttu-id="850dc-116">A **robotpilóta** oldalon kattintson vagy koppintson a **Start Guide**elemre.</span><span class="sxs-lookup"><span data-stu-id="850dc-116">On the **AutoPilot** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="850dc-118">A **upload. csv fájlban az eszközök listáját tartalmazó** lapon keresse meg azt a helyet, ahol az előkészített. CSV fájlt, majd **nyissa meg** \> a **Next**.</span><span class="sxs-lookup"><span data-stu-id="850dc-118">On the **Upload .csv file with list of devices** page, browse to a location where you have the prepared .CSV file, then **Open** \> **Next**.</span></span> <span data-ttu-id="850dc-119">A fájlnak három fejlécet kell tartalmaznia:</span><span class="sxs-lookup"><span data-stu-id="850dc-119">The file must have three headers:</span></span>
    
    - <span data-ttu-id="850dc-120">A oszlop: Eszköz sorozatszáma</span><span class="sxs-lookup"><span data-stu-id="850dc-120">Column A: Device Serial Number</span></span>
    
    - <span data-ttu-id="850dc-121">B oszlop: Windows-termékazonosító</span><span class="sxs-lookup"><span data-stu-id="850dc-121">Column B: Windows Product ID</span></span>
    
    - <span data-ttu-id="850dc-122">C oszlop: Hardverkivonat</span><span class="sxs-lookup"><span data-stu-id="850dc-122">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="850dc-123">Ezt az információt a hardver forgalmazójától kaphatja meg, vagy a [Get-WindowsAutoPilotInfo PowerShell parancsfájl](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) segítségével hozhat létre CSV-fájlt.</span><span class="sxs-lookup"><span data-stu-id="850dc-123">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
    <span data-ttu-id="850dc-p103">További információ: [Eszközlistát tartalmazó CSV-fájl](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Az **Eszközlistát tartalmazó CSV-fájl feltöltése** lapon egy mintafájlt is letölthet.</span><span class="sxs-lookup"><span data-stu-id="850dc-p103">For more information, see [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
4. <span data-ttu-id="850dc-126">A **profil hozzárendelése** lapon választhat egy meglévő profilt, vagy létrehozhat egy újat.</span><span class="sxs-lookup"><span data-stu-id="850dc-126">On the **Assign a profile** page, you can either pick an existing profile or create a new one.</span></span> <span data-ttu-id="850dc-127">Ha még nincs ilyen, akkor a program kérni fogja, hogy hozzon létre egyet.</span><span class="sxs-lookup"><span data-stu-id="850dc-127">If you don't have one yet, you'll be prompted to create one.</span></span> 
    
    <span data-ttu-id="850dc-128">A profil azoknak a beállításoknak a gyűjteménye, amelyek egyetlen eszközre vagy eszközök csoportjára lehet alkalmazni.</span><span class="sxs-lookup"><span data-stu-id="850dc-128">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="850dc-129">Az alapértelmezett szolgáltatások szükségesek, és automatikusan beállnak.</span><span class="sxs-lookup"><span data-stu-id="850dc-129">The default features are required and are set automatically.</span></span> <span data-ttu-id="850dc-130">Az alapértelmezett funkciók az alábbiak:</span><span class="sxs-lookup"><span data-stu-id="850dc-130">The default features are:</span></span>
    
    - <span data-ttu-id="850dc-131">Ugrál Cortana, OneDrive, és OEM beírás.</span><span class="sxs-lookup"><span data-stu-id="850dc-131">Skip Cortana, OneDrive, and OEM registration.</span></span>
    
    - <span data-ttu-id="850dc-132">Bejelentkezés céges márkával.</span><span class="sxs-lookup"><span data-stu-id="850dc-132">Create sign-in experience with your company brand.</span></span>
    
    - <span data-ttu-id="850dc-133">Csatlakoztassa a készülékeket az Azure Active Directory fiókokhoz, és automatikusan igényelje őket a Microsoft 365 Business általi kezelésükhöz.</span><span class="sxs-lookup"><span data-stu-id="850dc-133">Connect your devices to Azure Active Directory accounts, and automatically enroll them to be managed by Microsoft 365 Business.</span></span>
    
    <span data-ttu-id="850dc-134">További információ: [a robotpilóta-profil beállításai](autopilot-profile-settings.md).</span><span class="sxs-lookup"><span data-stu-id="850dc-134">For more information, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span> 
    
5. <span data-ttu-id="850dc-135">A további beállítások: **Adatvédelmi beállítások kihagyása** és **Nem léptethető elő a felhasználó a helyi rendszergazdává**. Mindkettő értéke alapértelmezés szerint **Kikapcsolva**.</span><span class="sxs-lookup"><span data-stu-id="850dc-135">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="850dc-136">Válassza a **Tovább** gombot.</span><span class="sxs-lookup"><span data-stu-id="850dc-136">Choose **Next**.</span></span>
    
6. <span data-ttu-id="850dc-137">**Elkészült** , azt jelzi, hogy a létrehozott (vagy választott) profilt a program az eszközök listájának feltöltésével létrehozott eszközcsoportra alkalmazza.</span><span class="sxs-lookup"><span data-stu-id="850dc-137">**You're done** indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices.</span></span> <span data-ttu-id="850dc-138">A beállítások akkor lesznek érvényben, amikor az eszköz felhasználói bejelentkeznek.</span><span class="sxs-lookup"><span data-stu-id="850dc-138">The settings will be in effect when the device users sign in next.</span></span> <span data-ttu-id="850dc-139">Válassza a **Bezárás** gombot.</span><span class="sxs-lookup"><span data-stu-id="850dc-139">Choose **Close**.</span></span>
    
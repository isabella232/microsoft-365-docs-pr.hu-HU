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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Megtudhatja, hogy a Windows AutoPilot segítségével hogyan állíthat be új Windows 10-es eszközöket a vállalata számára, hogy azok készen állnak az alkalmazottak használatára.
ms.openlocfilehash: 75cc51b889f8673de8dba2357c777de47fd0d296
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913502"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="889fd-103">Autopilot-eszközök és -profilok hozzáadása a lépésenkénti útmutatóval</span><span class="sxs-lookup"><span data-stu-id="889fd-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="889fd-104">A Windows AutoPilot segítségével új **Windows** 10-es eszközöket állíthat be a vállalata számára, így azok készen állnak a használatra, amikor átadjuk őket az alkalmazottainak.</span><span class="sxs-lookup"><span data-stu-id="889fd-104">You can use Windows AutoPilot to set up **new** Windows 10 devices for your business so they're ready for use when you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="889fd-105">Eszközkövetelmények</span><span class="sxs-lookup"><span data-stu-id="889fd-105">Device requirements</span></span>

<span data-ttu-id="889fd-106">Az eszközöknek meg kell felelnie az alábbi követelményeknek:</span><span class="sxs-lookup"><span data-stu-id="889fd-106">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="889fd-107">Windows 10, 1703-as vagy újabb verzió</span><span class="sxs-lookup"><span data-stu-id="889fd-107">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="889fd-108">Új eszközök, amelyek még nem voltak használhatók a Windowsban</span><span class="sxs-lookup"><span data-stu-id="889fd-108">New devices that haven't been through Windows out-of-box experience</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="889fd-109">Eszközök és profilok létrehozása a beállítási útmutató használatával</span><span class="sxs-lookup"><span data-stu-id="889fd-109">Use the setup guide to create devices and profiles</span></span>

<span data-ttu-id="889fd-110">[![A megjelenő címke figyelmeztet a felügyeleti központ változásaira, további részleteket itt talál: aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="889fd-110">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="889fd-111">Ha még nem hozott létre eszközcsoportokat vagy -profilokat, a legjobb, ha a részletes útmutatót használja.</span><span class="sxs-lookup"><span data-stu-id="889fd-111">If you haven't created device groups or profiles yet, the best way to get started is by using the step-by-step guide.</span></span> <span data-ttu-id="889fd-112">Az útmutató [használata](create-and-edit-autopilot-devices.md) [](create-and-edit-autopilot-profiles.md) nélkül is felvehet eszközöket, és profilokat rendelhet hozzájuk.</span><span class="sxs-lookup"><span data-stu-id="889fd-112">You can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="889fd-113">A felügyeleti központ megnyitásához: <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="889fd-113">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="889fd-114">A bal oldali navigációs ablakban válassza az **Eszközök** \> **AutoPilot lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="889fd-114">On the left navigation pane, choose **Devices** \> **AutoPilot**.</span></span>

    ![A Felügyeleti központban válassza az eszközök, majd az AutoPilot lehetőséget.](../media/AutoPilot.png)
  
2. <span data-ttu-id="889fd-116">Az **AutoPilot lapon** kattintson vagy koppintson az Útmutató **kezdése elemre.**</span><span class="sxs-lookup"><span data-stu-id="889fd-116">On the **AutoPilot** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="889fd-118">Az **Eszközlistát** is tartalmazza .csv fájl feltöltése lapon tallózással keresse meg azt a helyet, ahol előkészítette az eszközt. CSV-fájl, majd **a Következő megnyitása** \> **gombra.**</span><span class="sxs-lookup"><span data-stu-id="889fd-118">On the **Upload .csv file with list of devices** page, browse to a location where you have the prepared .CSV file, then **Open** \> **Next**.</span></span> <span data-ttu-id="889fd-119">A fájlnak három fejléccel kell lennie:</span><span class="sxs-lookup"><span data-stu-id="889fd-119">The file must have three headers:</span></span>
    
    - <span data-ttu-id="889fd-120">A oszlop: Eszköz sorozatszáma</span><span class="sxs-lookup"><span data-stu-id="889fd-120">Column A: Device Serial Number</span></span>
    
    - <span data-ttu-id="889fd-121">B oszlop: Windows-termékazonosító</span><span class="sxs-lookup"><span data-stu-id="889fd-121">Column B: Windows Product ID</span></span>
    
    - <span data-ttu-id="889fd-122">C oszlop: Hardverkivonat</span><span class="sxs-lookup"><span data-stu-id="889fd-122">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="889fd-123">Ezeket az információkat a hardvergyártójától kaphatja meg, vagy a [Get-WindowsAutoPilotInfo PowerShell-parancsprogrammal](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) létrehozhat egy CSV-fájlt.</span><span class="sxs-lookup"><span data-stu-id="889fd-123">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
    <span data-ttu-id="889fd-p103">További információ: [Eszközlistát tartalmazó CSV-fájl](../admin/misc/device-list.md). Az **Eszközlistát tartalmazó CSV-fájl feltöltése** lapon egy mintafájlt is letölthet.</span><span class="sxs-lookup"><span data-stu-id="889fd-p103">For more information, see [Device list CSV-file](../admin/misc/device-list.md). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="889fd-126">Ez a parancsfájl WMI segítségével beolvassa az eszközök Windows Autopilottal való regisztrálása esetén szükséges tulajdonságokat.</span><span class="sxs-lookup"><span data-stu-id="889fd-126">This script uses WMI to retrieve properties needed for a customer to register a device with Windows Autopilot.</span></span> <span data-ttu-id="889fd-127">Vegye figyelembe, hogy az eredményül kapott CSV-fájlban nem kell Windows-termékazonosító (PKID) értéket gyűjteni, mivel ez nem szükséges egy eszköz regisztrálásához, és a PKID NULL érték a kimeneti CSV-fájlban teljesen rendben van.</span><span class="sxs-lookup"><span data-stu-id="889fd-127">Note that it is normal for the resulting CSV file to not collect a Windows Product ID (PKID) value since this is not required to register a device and PKID being NULL in the output CSV is totally fine.</span></span> <span data-ttu-id="889fd-128">A rendszer csak a sorozatszámot és a hardver kivonatát tölti ki.</span><span class="sxs-lookup"><span data-stu-id="889fd-128">Only the serial number and hardware hash will be populated.</span></span>
    
4. <span data-ttu-id="889fd-129">A Profil **hozzárendelése lapon** kiválaszthat egy meglévő profilt, vagy létrehozhat egy újat.</span><span class="sxs-lookup"><span data-stu-id="889fd-129">On the **Assign a profile** page, you can either pick an existing profile or create a new one.</span></span> <span data-ttu-id="889fd-130">Ha még nincs ilyen fiókja, a rendszer kérni fogja, hogy hozzon létre egyet.</span><span class="sxs-lookup"><span data-stu-id="889fd-130">If you don't have one yet, you'll be prompted to create one.</span></span> 
    
    <span data-ttu-id="889fd-131">A profil azoknak a beállításoknak a gyűjteménye, amelyek egyetlen eszközre vagy eszközök csoportjára lehet alkalmazni.</span><span class="sxs-lookup"><span data-stu-id="889fd-131">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="889fd-132">Az alapértelmezett funkciók kötelezők, és automatikusan vannak beállítva.</span><span class="sxs-lookup"><span data-stu-id="889fd-132">The default features are required and are set automatically.</span></span> <span data-ttu-id="889fd-133">Az alapértelmezett funkciók az alábbiak:</span><span class="sxs-lookup"><span data-stu-id="889fd-133">The default features are:</span></span>
    
    - <span data-ttu-id="889fd-134">Kihagyhatja Cortanát, a OneDrive-ot és az OEM-regisztrációt.</span><span class="sxs-lookup"><span data-stu-id="889fd-134">Skip Cortana, OneDrive, and OEM registration.</span></span>
    
    - <span data-ttu-id="889fd-135">Bejelentkezés céges márkával.</span><span class="sxs-lookup"><span data-stu-id="889fd-135">Create sign-in experience with your company brand.</span></span>
    
    - <span data-ttu-id="889fd-136">Csatlakoztassa az eszközeit az Azure Active Directory-fiókokhoz, és automatikusan regisztrálja őket a Microsoft 365 Business Premiumval való használatra.</span><span class="sxs-lookup"><span data-stu-id="889fd-136">Connect your devices to Azure Active Directory accounts, and automatically enroll them to be managed by Microsoft 365 Business Premium.</span></span>
    
    <span data-ttu-id="889fd-137">További információ: [Az AutoPilot-profil beállításai.](autopilot-profile-settings.md)</span><span class="sxs-lookup"><span data-stu-id="889fd-137">For more information, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span> 
    
5. <span data-ttu-id="889fd-138">A további beállítások: **Adatvédelmi beállítások kihagyása** és **Nem léptethető elő a felhasználó a helyi rendszergazdává**. Mindkettő értéke alapértelmezés szerint **Kikapcsolva**.</span><span class="sxs-lookup"><span data-stu-id="889fd-138">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="889fd-139">Válassza a **Tovább** gombot.</span><span class="sxs-lookup"><span data-stu-id="889fd-139">Choose **Next**.</span></span>
    
6. <span data-ttu-id="889fd-140">**Ha végzett,** az azt jelenti, hogy a létrehozott (vagy kiválasztott) profilt a rendszer az eszközlista feltöltésével létrehozott eszközcsoportra alkalmazza.</span><span class="sxs-lookup"><span data-stu-id="889fd-140">**You're done** indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices.</span></span> <span data-ttu-id="889fd-141">A beállítások akkor lépnek életbe, amikor az eszköz felhasználói legközelebb bejelentkeznek.</span><span class="sxs-lookup"><span data-stu-id="889fd-141">The settings will be in effect when the device users sign in next.</span></span> <span data-ttu-id="889fd-142">Válassza a **Bezárás** gombot.</span><span class="sxs-lookup"><span data-stu-id="889fd-142">Choose **Close**.</span></span>

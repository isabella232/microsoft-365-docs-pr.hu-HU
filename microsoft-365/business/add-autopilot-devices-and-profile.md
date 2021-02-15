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
description: Megtudhatja, hogy a Windows AutoPilot használatával hogyan állíthat be új Windows 10-es eszközöket a vállalata számára, hogy készen álljanak az alkalmazottak használatára.
ms.openlocfilehash: f263cc90656ae5e7be1a89e3c7f56bfb2d0e3651
ms.sourcegitcommit: 3b369a44b71540c8b8214ce588a7aa6f47c3bb1e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/04/2021
ms.locfileid: "50099750"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="a37a7-103">Autopilot-eszközök és -profilok hozzáadása a lépésenkénti útmutatóval</span><span class="sxs-lookup"><span data-stu-id="a37a7-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="a37a7-104">A Windows AutoPilot segítségével új **Windows** 10-es eszközöket állíthat be a vállalata számára, így azok készen állnak a használatra, amikor átadjuk őket az alkalmazottainak.</span><span class="sxs-lookup"><span data-stu-id="a37a7-104">You can use Windows AutoPilot to set up **new** Windows 10 devices for your business so they're ready for use when you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="a37a7-105">Eszközkövetelmények</span><span class="sxs-lookup"><span data-stu-id="a37a7-105">Device requirements</span></span>

<span data-ttu-id="a37a7-106">Az eszközöknek meg kell felelnie az alábbi követelményeknek:</span><span class="sxs-lookup"><span data-stu-id="a37a7-106">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="a37a7-107">Windows 10 1703-as vagy újabb verzió</span><span class="sxs-lookup"><span data-stu-id="a37a7-107">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="a37a7-108">Új eszközök, amelyek még nem voltak használhatók a Windows rendszerben</span><span class="sxs-lookup"><span data-stu-id="a37a7-108">New devices that haven't been through Windows out-of-box experience</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="a37a7-109">Eszközök és profilok létrehozása a beállítási útmutató használatával</span><span class="sxs-lookup"><span data-stu-id="a37a7-109">Use the setup guide to create devices and profiles</span></span>

<span data-ttu-id="a37a7-110">[![A megjelenő címke figyelmeztet a felügyeleti központ változásaira, további részleteket itt talál: aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="a37a7-110">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="a37a7-111">Ha még nem hozott létre eszközcsoportokat vagy -profilokat, a legjobb, ha a lépésenként végigvezeti az első lépéseken.</span><span class="sxs-lookup"><span data-stu-id="a37a7-111">If you haven't created device groups or profiles yet, the best way to get started is by using the step-by-step guide.</span></span> <span data-ttu-id="a37a7-112">Az útmutató használata [](create-and-edit-autopilot-profiles.md) [nélkül](create-and-edit-autopilot-devices.md) is felvehet eszközöket, és profilokat rendelhet hozzájuk.</span><span class="sxs-lookup"><span data-stu-id="a37a7-112">You can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="a37a7-113">A felügyeleti központ megnyitásához: <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="a37a7-113">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="a37a7-114">A bal oldali navigációs ablakban válassza az **Eszközök** \> **AutoPilot lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="a37a7-114">On the left navigation pane, choose **Devices** \> **AutoPilot**.</span></span>

    ![A Felügyeleti központban válassza ki az eszközöket, majd az AutoPilotot.](../media/AutoPilot.png)
  
2. <span data-ttu-id="a37a7-116">Az **AutoPilot lapon** kattintson vagy koppintson az útmutató **indítási parancsára.**</span><span class="sxs-lookup"><span data-stu-id="a37a7-116">On the **AutoPilot** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="a37a7-118">A **.csv** fájl feltöltése az eszközök listájával lapon tallózással keresse meg azt a helyet, ahol előkészítette. CSV-fájl, majd **a Tovább megnyitása** \> **gombra.**</span><span class="sxs-lookup"><span data-stu-id="a37a7-118">On the **Upload .csv file with list of devices** page, browse to a location where you have the prepared .CSV file, then **Open** \> **Next**.</span></span> <span data-ttu-id="a37a7-119">A fájlnak három fejlécet kell lennie:</span><span class="sxs-lookup"><span data-stu-id="a37a7-119">The file must have three headers:</span></span>
    
    - <span data-ttu-id="a37a7-120">A oszlop: Eszköz sorozatszáma</span><span class="sxs-lookup"><span data-stu-id="a37a7-120">Column A: Device Serial Number</span></span>
    
    - <span data-ttu-id="a37a7-121">B oszlop: Windows-termékazonosító</span><span class="sxs-lookup"><span data-stu-id="a37a7-121">Column B: Windows Product ID</span></span>
    
    - <span data-ttu-id="a37a7-122">C oszlop: Hardverkivonat</span><span class="sxs-lookup"><span data-stu-id="a37a7-122">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="a37a7-123">Ezeket az információkat a hardvergyártótól kaphatja meg, vagy a [Get-WindowsAutoPilotInfo](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) PowerShell-parancsprogrammal létrehozhat egy CSV-fájlt.</span><span class="sxs-lookup"><span data-stu-id="a37a7-123">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
    <span data-ttu-id="a37a7-p103">További információ: [Eszközlistát tartalmazó CSV-fájl](https://docs.microsoft.com/microsoft-365/admin/misc/device-list). Az **Eszközlistát tartalmazó CSV-fájl feltöltése** lapon egy mintafájlt is letölthet.</span><span class="sxs-lookup"><span data-stu-id="a37a7-p103">For more information, see [Device list CSV-file](https://docs.microsoft.com/microsoft-365/admin/misc/device-list). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="a37a7-126">Ez a parancsprogram WMI segítségével olvassa be az ügyfélnek az eszköz Windows Autopilottal való regisztráláshoz szükséges tulajdonságait.</span><span class="sxs-lookup"><span data-stu-id="a37a7-126">This script uses WMI to retrieve properties needed for a customer to register a device with Windows Autopilot.</span></span> <span data-ttu-id="a37a7-127">Vegye figyelembe, hogy az eredményül kapott CSV-fájl nem gyűjti össze a Windows-termékazonosító (PKID) értékét, mivel ez nem szükséges az eszközök regisztrálásához, és a PKID null érték a kimeneti CSV-fájlban teljesen rendben van.</span><span class="sxs-lookup"><span data-stu-id="a37a7-127">Note that it is normal for the resulting CSV file to not collect a Windows Product ID (PKID) value since this is not required to register a device and PKID being NULL in the output CSV is totally fine.</span></span> <span data-ttu-id="a37a7-128">Csak a sorozatszámot és a hardveres kivonatot tölti ki a rendszer.</span><span class="sxs-lookup"><span data-stu-id="a37a7-128">Only the serial number and hardware hash will be populated.</span></span>
    
4. <span data-ttu-id="a37a7-129">A Profil **hozzárendelése lapon** választhat egy meglévő profilt, vagy létrehozhat egy újat.</span><span class="sxs-lookup"><span data-stu-id="a37a7-129">On the **Assign a profile** page, you can either pick an existing profile or create a new one.</span></span> <span data-ttu-id="a37a7-130">Ha még nincs ilyen üzenete, a rendszer kérni fogja, hogy hozzon létre egyet.</span><span class="sxs-lookup"><span data-stu-id="a37a7-130">If you don't have one yet, you'll be prompted to create one.</span></span> 
    
    <span data-ttu-id="a37a7-131">A profil azoknak a beállításoknak a gyűjteménye, amelyek egyetlen eszközre vagy eszközök csoportjára lehet alkalmazni.</span><span class="sxs-lookup"><span data-stu-id="a37a7-131">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="a37a7-132">Az alapértelmezett funkciók kötelezők, és automatikusan be vannak állítva.</span><span class="sxs-lookup"><span data-stu-id="a37a7-132">The default features are required and are set automatically.</span></span> <span data-ttu-id="a37a7-133">Az alapértelmezett funkciók az alábbiak:</span><span class="sxs-lookup"><span data-stu-id="a37a7-133">The default features are:</span></span>
    
    - <span data-ttu-id="a37a7-134">Kihagyhatja Cortanát, a OneDrive-ot és az OEM-regisztrációt.</span><span class="sxs-lookup"><span data-stu-id="a37a7-134">Skip Cortana, OneDrive, and OEM registration.</span></span>
    
    - <span data-ttu-id="a37a7-135">Bejelentkezés céges márkával.</span><span class="sxs-lookup"><span data-stu-id="a37a7-135">Create sign-in experience with your company brand.</span></span>
    
    - <span data-ttu-id="a37a7-136">Csatlakoztassa az eszközeit az Azure Active Directory-fiókokhoz, és automatikusan regisztrálja őket a Microsoft 365 Business Premium által kezelt fiókokra.</span><span class="sxs-lookup"><span data-stu-id="a37a7-136">Connect your devices to Azure Active Directory accounts, and automatically enroll them to be managed by Microsoft 365 Business Premium.</span></span>
    
    <span data-ttu-id="a37a7-137">További információ: [Az AutoPilot-profil beállításai.](autopilot-profile-settings.md)</span><span class="sxs-lookup"><span data-stu-id="a37a7-137">For more information, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span> 
    
5. <span data-ttu-id="a37a7-138">A további beállítások: **Adatvédelmi beállítások kihagyása** és **Nem léptethető elő a felhasználó a helyi rendszergazdává**. Mindkettő értéke alapértelmezés szerint **Kikapcsolva**.</span><span class="sxs-lookup"><span data-stu-id="a37a7-138">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="a37a7-139">Válassza a **Tovább** gombot.</span><span class="sxs-lookup"><span data-stu-id="a37a7-139">Choose **Next**.</span></span>
    
6. <span data-ttu-id="a37a7-140">**Ha végzett,** az azt jelenti, hogy a létrehozott (vagy kiválasztott) profilt a rendszer az eszközlista feltöltésével létrehozott eszközcsoportra alkalmazza.</span><span class="sxs-lookup"><span data-stu-id="a37a7-140">**You're done** indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices.</span></span> <span data-ttu-id="a37a7-141">A beállítások akkor lépnek életbe, amikor az eszköz felhasználói legközelebb bejelentkeznek.</span><span class="sxs-lookup"><span data-stu-id="a37a7-141">The settings will be in effect when the device users sign in next.</span></span> <span data-ttu-id="a37a7-142">Válassza a **Bezárás** gombot.</span><span class="sxs-lookup"><span data-stu-id="a37a7-142">Choose **Close**.</span></span>
    

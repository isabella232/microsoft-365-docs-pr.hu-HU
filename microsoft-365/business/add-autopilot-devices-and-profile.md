---
title: Autopilot-eszközök és -profilok hozzáadása a lépésenkénti útmutatóval
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
- AdminTemplateSet
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Ebből a cikkből megtudhatja, Windows AutoPilot használatával hogyan állíthat be új Windows 10 eszközét a vállalata számára, hogy azok készen állnak az alkalmazottak használatára.
ms.openlocfilehash: f160ddcd1e41bd44c908ecc8bbd30a9819f76902
ms.sourcegitcommit: 00f001019c653269d85718d410f970887d904304
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/12/2021
ms.locfileid: "53393439"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="aaefa-103">Autopilot-eszközök és -profilok hozzáadása a lépésenkénti útmutatóval</span><span class="sxs-lookup"><span data-stu-id="aaefa-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="aaefa-104">Az AutoPilot Windows használatával új  Windows 10 állíthat be a vállalata számára, így azok készen állnak a használatra, amikor az alkalmazottaknak adja őket.</span><span class="sxs-lookup"><span data-stu-id="aaefa-104">You can use Windows AutoPilot to set up **new** Windows 10 devices for your business so they're ready for use when you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="aaefa-105">Eszközkövetelmények</span><span class="sxs-lookup"><span data-stu-id="aaefa-105">Device requirements</span></span>

<span data-ttu-id="aaefa-106">Az eszközöknek meg kell felelnie az alábbi követelményeknek:</span><span class="sxs-lookup"><span data-stu-id="aaefa-106">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="aaefa-107">Windows 10 1703-as vagy újabb verzió</span><span class="sxs-lookup"><span data-stu-id="aaefa-107">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="aaefa-108">Új eszközök, amelyeken még nem Windows nem voltak bevetve</span><span class="sxs-lookup"><span data-stu-id="aaefa-108">New devices that haven't been through Windows out-of-box experience</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="aaefa-109">Eszközök és profilok létrehozása a beállítási útmutató használatával</span><span class="sxs-lookup"><span data-stu-id="aaefa-109">Use the setup guide to create devices and profiles</span></span>

<span data-ttu-id="aaefa-110">Ha még nem hozott létre eszközcsoportokat vagy -profilokat, a legjobb, ha a részletes útmutatót használja.</span><span class="sxs-lookup"><span data-stu-id="aaefa-110">If you haven't created device groups or profiles yet, the best way to get started is by using the step-by-step guide.</span></span> <span data-ttu-id="aaefa-111">Az útmutató [használata](create-and-edit-autopilot-devices.md) [](create-and-edit-autopilot-profiles.md) nélkül is felvehet eszközöket, és profilokat rendelhet hozzájuk.</span><span class="sxs-lookup"><span data-stu-id="aaefa-111">You can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="aaefa-112">A felügyeleti központ megnyitásához: <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="aaefa-112">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="aaefa-113">A bal oldali navigációs ablakban válassza az **Eszközök** \> **AutoPilot lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="aaefa-113">On the left navigation pane, choose **Devices** \> **AutoPilot**.</span></span>

    ![A Felügyeleti központban válassza az eszközök, majd az AutoPilot lehetőséget.](../media/AutoPilot.png)
  
2. <span data-ttu-id="aaefa-115">Az **AutoPilot lapon** kattintson vagy koppintson az Útmutató **kezdése elemre.**</span><span class="sxs-lookup"><span data-stu-id="aaefa-115">On the **AutoPilot** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="aaefa-117">Az **Eszközlista .csv** fájl feltöltése lapon tallózással keresse meg azt a helyet, ahol  az előkészített fájl .CSV, majd a Tovább \> **gombra.**</span><span class="sxs-lookup"><span data-stu-id="aaefa-117">On the **Upload .csv file with list of devices** page, browse to a location where you have the prepared .CSV file, then **Open** \> **Next**.</span></span> <span data-ttu-id="aaefa-118">A fájlnak három fejléccel kell lennie:</span><span class="sxs-lookup"><span data-stu-id="aaefa-118">The file must have three headers:</span></span>
    
    - <span data-ttu-id="aaefa-119">A oszlop: Eszköz sorozatszáma</span><span class="sxs-lookup"><span data-stu-id="aaefa-119">Column A: Device Serial Number</span></span>
    
    - <span data-ttu-id="aaefa-120">B oszlop: Windows-termékazonosító</span><span class="sxs-lookup"><span data-stu-id="aaefa-120">Column B: Windows Product ID</span></span>
    
    - <span data-ttu-id="aaefa-121">C oszlop: Hardverkivonat</span><span class="sxs-lookup"><span data-stu-id="aaefa-121">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="aaefa-122">Ezeket az információkat a hardvergyártójától kaphatja meg, vagy a [Get-WindowsAutoPilotInfo PowerShell-parancsprogrammal](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) létrehozhat egy CSV-fájlt.</span><span class="sxs-lookup"><span data-stu-id="aaefa-122">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
    <span data-ttu-id="aaefa-p103">További információ: [Eszközlistát tartalmazó CSV-fájl](../admin/misc/device-list.md). Az **Eszközlistát tartalmazó CSV-fájl feltöltése** lapon egy mintafájlt is letölthet.</span><span class="sxs-lookup"><span data-stu-id="aaefa-p103">For more information, see [Device list CSV-file](../admin/misc/device-list.md). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="aaefa-125">Ez a parancsprogram WMI segítségével beolvassa az autopilottal regisztrált eszközöknek az Windows tulajdonságait.</span><span class="sxs-lookup"><span data-stu-id="aaefa-125">This script uses WMI to retrieve properties needed for a customer to register a device with Windows Autopilot.</span></span> <span data-ttu-id="aaefa-126">Felhívjuk a figyelmét arra, hogy az eredményül kapott CSV-fájlban nem kell egy Windows-termékazonosító (PKID) értéket gyűjteni, mivel ez nem szükséges egy eszköz regisztrálásához, és a PKID NULL érték a kimeneti CSV-fájlban teljesen rendben van.</span><span class="sxs-lookup"><span data-stu-id="aaefa-126">Note that it is normal for the resulting CSV file to not collect a Windows Product ID (PKID) value since this is not required to register a device and PKID being NULL in the output CSV is totally fine.</span></span> <span data-ttu-id="aaefa-127">A rendszer csak a sorozatszámot és a hardver kivonatát tölti ki.</span><span class="sxs-lookup"><span data-stu-id="aaefa-127">Only the serial number and hardware hash will be populated.</span></span>
    
4. <span data-ttu-id="aaefa-128">A Profil **hozzárendelése lapon** kiválaszthat egy meglévő profilt, vagy létrehozhat egy újat.</span><span class="sxs-lookup"><span data-stu-id="aaefa-128">On the **Assign a profile** page, you can either pick an existing profile or create a new one.</span></span> <span data-ttu-id="aaefa-129">Ha még nincs ilyen fiókja, a rendszer kérni fogja, hogy hozzon létre egyet.</span><span class="sxs-lookup"><span data-stu-id="aaefa-129">If you don't have one yet, you'll be prompted to create one.</span></span> 
    
    <span data-ttu-id="aaefa-130">A profil azoknak a beállításoknak a gyűjteménye, amelyek egyetlen eszközre vagy eszközök csoportjára lehet alkalmazni.</span><span class="sxs-lookup"><span data-stu-id="aaefa-130">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="aaefa-131">Az alapértelmezett funkciók kötelezők, és automatikusan vannak beállítva.</span><span class="sxs-lookup"><span data-stu-id="aaefa-131">The default features are required and are set automatically.</span></span> <span data-ttu-id="aaefa-132">Az alapértelmezett funkciók az alábbiak:</span><span class="sxs-lookup"><span data-stu-id="aaefa-132">The default features are:</span></span>
    
    - <span data-ttu-id="aaefa-133">Kihagyhatja Cortana, a OneDrive és az OEM-regisztrációt.</span><span class="sxs-lookup"><span data-stu-id="aaefa-133">Skip Cortana, OneDrive, and OEM registration.</span></span>
    
    - <span data-ttu-id="aaefa-134">Bejelentkezés céges márkával.</span><span class="sxs-lookup"><span data-stu-id="aaefa-134">Create sign-in experience with your company brand.</span></span>
    
    - <span data-ttu-id="aaefa-135">Csatlakozás az eszközeit a Azure Active Directory fiókokhoz, és automatikusan regisztrálja őket a Microsoft 365 Vállalati prémium verzió.</span><span class="sxs-lookup"><span data-stu-id="aaefa-135">Connect your devices to Azure Active Directory accounts, and automatically enroll them to be managed by Microsoft 365 Business Premium.</span></span>
    
    <span data-ttu-id="aaefa-136">További információ: [Az AutoPilot-profil beállításai.](autopilot-profile-settings.md)</span><span class="sxs-lookup"><span data-stu-id="aaefa-136">For more information, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span> 
    
5. <span data-ttu-id="aaefa-137">A további beállítások: **Adatvédelmi beállítások kihagyása** és **Nem léptethető elő a felhasználó a helyi rendszergazdává**. Mindkettő értéke alapértelmezés szerint **Kikapcsolva**.</span><span class="sxs-lookup"><span data-stu-id="aaefa-137">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="aaefa-138">Válassza a **Tovább** gombot.</span><span class="sxs-lookup"><span data-stu-id="aaefa-138">Choose **Next**.</span></span>
    
6. <span data-ttu-id="aaefa-139">**Ha végzett,** az azt jelenti, hogy a létrehozott (vagy kiválasztott) profilt a rendszer az eszközlista feltöltésével létrehozott eszközcsoportra alkalmazza.</span><span class="sxs-lookup"><span data-stu-id="aaefa-139">**You're done** indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices.</span></span> <span data-ttu-id="aaefa-140">A beállítások akkor lépnek életbe, amikor az eszköz felhasználói legközelebb bejelentkeznek.</span><span class="sxs-lookup"><span data-stu-id="aaefa-140">The settings will be in effect when the device users sign in next.</span></span> <span data-ttu-id="aaefa-141">Válassza a **Bezárás** gombot.</span><span class="sxs-lookup"><span data-stu-id="aaefa-141">Choose **Close**.</span></span>

## <a name="related-content"></a><span data-ttu-id="aaefa-142">Kapcsolódó tartalom</span><span class="sxs-lookup"><span data-stu-id="aaefa-142">Related content</span></span>

<span data-ttu-id="aaefa-143">[Az AutoPilot-profil beállításai](autopilot-profile-settings.md) (cikk)</span><span class="sxs-lookup"><span data-stu-id="aaefa-143">[About AutoPilot Profile settings](autopilot-profile-settings.md) (article)</span></span>\
<span data-ttu-id="aaefa-144">[Az eszközök és az alkalmazásadatok védelmére vonatkozó](../admin/devices/choose-device-security.md) beállítások (cikk)</span><span class="sxs-lookup"><span data-stu-id="aaefa-144">[Options for protecting your devices and app data](../admin/devices/choose-device-security.md) (article)</span></span>

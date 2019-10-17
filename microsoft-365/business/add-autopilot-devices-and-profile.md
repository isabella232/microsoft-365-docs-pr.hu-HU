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
ms.openlocfilehash: d028ea3e902965d55c445dc3b3a02aa315201b25
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/17/2019
ms.locfileid: "37574788"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="8ef4e-103">Autopilot-eszközök és -profilok hozzáadása a lépésenkénti útmutatóval</span><span class="sxs-lookup"><span data-stu-id="8ef4e-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="8ef4e-104">Használhatja a Windows AutoPilot, hogy hozzanak létre **új** Windows 10 eszközök a vállalkozás számára, így azok készen állnak a hatékony használatra, amint megadja nekik az alkalmazottak.</span><span class="sxs-lookup"><span data-stu-id="8ef4e-104">You can use Windows AutoPilot to set up **new** Windows 10 devices for your business so they are ready for productive use as soon as you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="8ef4e-105">Eszközkövetelmények</span><span class="sxs-lookup"><span data-stu-id="8ef4e-105">Device requirements</span></span>

<span data-ttu-id="8ef4e-106">Az eszközöknek meg kell felelniük az alábbi követelményeknek:</span><span class="sxs-lookup"><span data-stu-id="8ef4e-106">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="8ef4e-107">A Windows 10 rendszer 1703-as vagy újabb verzióját kell futtatniuk.</span><span class="sxs-lookup"><span data-stu-id="8ef4e-107">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="8ef4e-108">Olyan új eszközöknek kell lenniük, amelyeken még nem használták a Windowst.</span><span class="sxs-lookup"><span data-stu-id="8ef4e-108">New devices that have not been through Windows out-of-box experience.</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="8ef4e-109">Eszközök és profilok létrehozása a beállítási útmutató használatával</span><span class="sxs-lookup"><span data-stu-id="8ef4e-109">Use the setup guide to create devices and profiles</span></span>

<span data-ttu-id="8ef4e-110">[![Label, hogy tudd, az admin központ változik, és találsz további részleteket a aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="8ef4e-110">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="8ef4e-111">Ha még nem hozott létre eszközcsoportokat vagy profilokat, a legjobb, ha azzal kezdi, hogy elolvassa a részletes útmutatót, de azt is megteheti, hogy az útmutató nélkül [vesz fel eszközöket](create-and-edit-autopilot-devices.md) és [rendel hozzájuk profilokat](create-and-edit-autopilot-profiles.md).</span><span class="sxs-lookup"><span data-stu-id="8ef4e-111">If you have no device groups or profiles created yet, the best way to get started is by using the step-by-step guide, but you can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="8ef4e-112">Menj az admin központba <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span><span class="sxs-lookup"><span data-stu-id="8ef4e-112">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="8ef4e-113">A bal oldali NAV válasszon **eszközök** \> **robotpilóta**.</span><span class="sxs-lookup"><span data-stu-id="8ef4e-113">On the left nav choose **Devices** \> **AutoPilot**.</span></span>

    ![Az Admin Center válasszon eszközöket, majd robotpilóta.](media/AutoPilot.png)
  
2. <span data-ttu-id="8ef4e-115">A **robotpilóta** oldalon kattintson vagy koppintson a **Start Guide**elemre.</span><span class="sxs-lookup"><span data-stu-id="8ef4e-115">On the **AutoPilot** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="8ef4e-p101">Az **Eszközlistát tartalmazó CSV-fájl feltöltése** lapon tallózással keresse meg az előkészített CSV-fájlt, és válassza a **Megnyitás** \> **Tovább** lehetőséget. A fájlnak három fejlécet kell tartalmaznia:</span><span class="sxs-lookup"><span data-stu-id="8ef4e-p101">On the **Upload .csv file with list of devices** page, browse to a locations where you have the prepared .CSV file, then **Open** \> **Next**. The file should have three headers:</span></span>
    
  - <span data-ttu-id="8ef4e-119">A oszlop: Eszköz sorozatszáma</span><span class="sxs-lookup"><span data-stu-id="8ef4e-119">Column A: Device Serial Number</span></span>
    
  - <span data-ttu-id="8ef4e-120">B oszlop: Windows-termékazonosító</span><span class="sxs-lookup"><span data-stu-id="8ef4e-120">Column B: Windows Product ID</span></span>
    
  - <span data-ttu-id="8ef4e-121">C oszlop: Hardverkivonat</span><span class="sxs-lookup"><span data-stu-id="8ef4e-121">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="8ef4e-122">Ezeket az adatokat beszerezheti a hardvergyártójától, vagy használhatja a [Get-WindowsAutoPilotInfo PowerShell-parancsfájlt](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), amely elkészíti a CSV-fájlt.</span><span class="sxs-lookup"><span data-stu-id="8ef4e-122">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a CSV file.</span></span> 
    
    <span data-ttu-id="8ef4e-p102">További információ: [Eszközlistát tartalmazó CSV-fájl](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Az **Eszközlistát tartalmazó CSV-fájl feltöltése** lapon egy mintafájlt is letölthet.</span><span class="sxs-lookup"><span data-stu-id="8ef4e-p102">For more information, see [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
4. <span data-ttu-id="8ef4e-p103">A **Profil hozzárendelése** lapon kiválaszthat egy meglévő profilt, vagy létrehozhat egy újat. Ha még nincs profilja, a rendszer új profil létrehozására fogja kérni.</span><span class="sxs-lookup"><span data-stu-id="8ef4e-p103">On the **Assign a profile** page, you can either pick an existing profile, or create a new one. If you don't have one yet, you will be prompted to create a new one.</span></span> 
    
    <span data-ttu-id="8ef4e-127">A profil azoknak a beállításoknak a gyűjteménye, amelyek egyetlen eszközre vagy eszközök csoportjára lehet alkalmazni.</span><span class="sxs-lookup"><span data-stu-id="8ef4e-127">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="8ef4e-p104">Az alapértelmezett funkciók kötelezők, és beállításuk automatikusan megtörténik. Az alapértelmezett funkciók az alábbiak:</span><span class="sxs-lookup"><span data-stu-id="8ef4e-p104">The default features are required and will be set automatically. The default features are:</span></span>
    
  - <span data-ttu-id="8ef4e-130">A Cortana, a OneDrive és a számítógépgyártók regisztrációja kihagyva.</span><span class="sxs-lookup"><span data-stu-id="8ef4e-130">Cortana, OneDrive and OEM registration is skipped.</span></span>
    
  - <span data-ttu-id="8ef4e-131">Bejelentkezés céges márkával.</span><span class="sxs-lookup"><span data-stu-id="8ef4e-131">Create sign-in experience with your company brand.</span></span>
    
  - <span data-ttu-id="8ef4e-132">Az eszközöket ezzel csatlakoztatja az Azure Active Directory-fiókokhoz, és automatikusan regisztrálja őket a Microsoft 365 Business általi kezelésre.</span><span class="sxs-lookup"><span data-stu-id="8ef4e-132">Your devices are going to be connected to Azure Active Directory accounts and automatically enrolled to be managed by Microsoft 365 Business.</span></span>
    
    <span data-ttu-id="8ef4e-133">További információ:</span><span class="sxs-lookup"><span data-stu-id="8ef4e-133">For more information, see</span></span>
    
    <span data-ttu-id="8ef4e-134">[Az AutoPilot-profil beállításai](autopilot-profile-settings.md) .</span><span class="sxs-lookup"><span data-stu-id="8ef4e-134">[About AutoPilot Profile settings](autopilot-profile-settings.md) .</span></span> 
    
5. <span data-ttu-id="8ef4e-135">A további beállítások: **Adatvédelmi beállítások kihagyása** és **Nem léptethető elő a felhasználó a helyi rendszergazdává**. Mindkettő értéke alapértelmezés szerint **Kikapcsolva**.</span><span class="sxs-lookup"><span data-stu-id="8ef4e-135">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="8ef4e-136">Válassza a **Tovább** gombot.</span><span class="sxs-lookup"><span data-stu-id="8ef4e-136">Choose **Next**.</span></span>
    
6. <span data-ttu-id="8ef4e-p105">Az **Elkészült!** lap megjelenése jelzi, hogy a rendszer a létrehozott (vagy kiválasztott) profilt alkalmazza arra az eszközcsoportra, amelyet Ön az eszközlista feltöltésével létrehozott. Ezek a beállítások lesznek érvényben legközelebb, amikor az eszköz felhasználói bejelentkeznek. Válassza a **Bezárás** gombot.</span><span class="sxs-lookup"><span data-stu-id="8ef4e-p105">**You're done** page indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices. These settings will be in effect when the device users sign in next. Choose **Close**.</span></span>
    
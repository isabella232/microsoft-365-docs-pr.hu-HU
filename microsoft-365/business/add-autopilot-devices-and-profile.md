---
title: Autopilot-eszközök és -profilok hozzáadása a lépésenkénti útmutatóval
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Útmutató a Windows automata segítségével állítsa be az új Windows 10 eszközök a vállalkozás számára.
ms.openlocfilehash: e0802ddcc0964d0b8d102f7dbdb9116b33cdcf58
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32277120"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="8cd3f-103">Autopilot-eszközök és -profilok hozzáadása a lépésenkénti útmutatóval</span><span class="sxs-lookup"><span data-stu-id="8cd3f-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="8cd3f-104">A Windows AutoPilot segítségével előkészítheti cégének új Windows 10-es eszközeit, így az alkalmazottak azonnal hatékonyan munkához láthatnak, amint megkapják az eszközüket.</span><span class="sxs-lookup"><span data-stu-id="8cd3f-104">You can use Windows AutoPilot to set up new Windows 10 devices for your business so they are ready for productive use as soon as you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="8cd3f-105">Eszközkövetelmények</span><span class="sxs-lookup"><span data-stu-id="8cd3f-105">Device requirements</span></span>

<span data-ttu-id="8cd3f-106">Az eszközöknek meg kell felelniük az alábbi követelményeknek:</span><span class="sxs-lookup"><span data-stu-id="8cd3f-106">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="8cd3f-107">A Windows 10 rendszer 1703-as vagy újabb verzióját kell futtatniuk.</span><span class="sxs-lookup"><span data-stu-id="8cd3f-107">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="8cd3f-108">Olyan új eszközöknek kell lenniük, amelyeken még nem használták a Windowst.</span><span class="sxs-lookup"><span data-stu-id="8cd3f-108">New devices that have not been through Windows out-of-box experience.</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="8cd3f-109">Eszközök és profilok létrehozása a beállítási útmutató használatával</span><span class="sxs-lookup"><span data-stu-id="8cd3f-109">Use the setup guide to create devices and profiles</span></span>

<span data-ttu-id="8cd3f-110">Ha még nem hozott létre eszközcsoportokat vagy profilokat, a legjobb, ha azzal kezdi, hogy elolvassa a részletes útmutatót, de azt is megteheti, hogy az útmutató nélkül [vesz fel eszközöket](create-and-edit-autopilot-devices.md) és [rendel hozzájuk profilokat](create-and-edit-autopilot-profiles.md).</span><span class="sxs-lookup"><span data-stu-id="8cd3f-110">If you have no device groups or profiles created yet, the best way to get started is by using the step-by-step guide, but you can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="8cd3f-111">A Microsoft 365 Business Felügyeleti központban keresse meg az **Eszközműveletek** kártyát, és válassza **A Windows üzembe helyezése az Autopilottal** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="8cd3f-111">In the Microsoft 365 Business admin center, locate the **Device actions** card, and choose **Deploy Windows with Autopilot**.</span></span>
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. <span data-ttu-id="8cd3f-113">**A Windows előkészítése** lapon kattintson vagy koppintson az **Útmutató indítása** elemre.</span><span class="sxs-lookup"><span data-stu-id="8cd3f-113">On the **Prepare Windows** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="8cd3f-p101">Az **Eszközlistát tartalmazó CSV-fájl feltöltése** lapon tallózással keresse meg az előkészített CSV-fájlt, és válassza a **Megnyitás** \> **Tovább** lehetőséget. A fájlnak három fejlécet kell tartalmaznia:</span><span class="sxs-lookup"><span data-stu-id="8cd3f-p101">On the **Upload .csv file with list of devices** page, browse to a locations where you have the prepared .CSV file, then **Open** \> **Next**. The file should have three headers:</span></span>
    
  - <span data-ttu-id="8cd3f-117">A oszlop: Eszköz sorozatszáma</span><span class="sxs-lookup"><span data-stu-id="8cd3f-117">Column A: Device Serial Number</span></span>
    
  - <span data-ttu-id="8cd3f-118">B oszlop: Windows-termékazonosító</span><span class="sxs-lookup"><span data-stu-id="8cd3f-118">Column B: Windows Product ID</span></span>
    
  - <span data-ttu-id="8cd3f-119">C oszlop: Hardverkivonat</span><span class="sxs-lookup"><span data-stu-id="8cd3f-119">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="8cd3f-120">Ezeket az adatokat beszerezheti a hardvergyártójától, vagy használhatja a [Get-WindowsAutoPilotInfo PowerShell-parancsfájlt](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), amely elkészíti a CSV-fájlt.</span><span class="sxs-lookup"><span data-stu-id="8cd3f-120">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a CSV file.</span></span> 
    
    <span data-ttu-id="8cd3f-p102">További információ: [Eszközlistát tartalmazó CSV-fájl](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). Az **Eszközlistát tartalmazó CSV-fájl feltöltése** lapon egy mintafájlt is letölthet.</span><span class="sxs-lookup"><span data-stu-id="8cd3f-p102">For more information, see [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
4. <span data-ttu-id="8cd3f-p103">A **Profil hozzárendelése** lapon kiválaszthat egy meglévő profilt, vagy létrehozhat egy újat. Ha még nincs profilja, a rendszer új profil létrehozására fogja kérni.</span><span class="sxs-lookup"><span data-stu-id="8cd3f-p103">On the **Assign a profile** page, you can either pick an existing profile, or create a new one. If you don't have one yet, you will be prompted to create a new one.</span></span> 
    
    <span data-ttu-id="8cd3f-125">A profil azoknak a beállításoknak a gyűjteménye, amelyek egyetlen eszközre vagy eszközök csoportjára lehet alkalmazni.</span><span class="sxs-lookup"><span data-stu-id="8cd3f-125">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="8cd3f-p104">Az alapértelmezett funkciók kötelezők, és beállításuk automatikusan megtörténik. Az alapértelmezett funkciók az alábbiak:</span><span class="sxs-lookup"><span data-stu-id="8cd3f-p104">The default features are required and will be set automatically. The default features are:</span></span>
    
  - <span data-ttu-id="8cd3f-128">A Cortana, a OneDrive és a számítógépgyártók regisztrációja kihagyva.</span><span class="sxs-lookup"><span data-stu-id="8cd3f-128">Cortana, OneDrive and OEM registration is skipped.</span></span>
    
  - <span data-ttu-id="8cd3f-129">Bejelentkezés céges márkával.</span><span class="sxs-lookup"><span data-stu-id="8cd3f-129">Create sign-in experience with your company brand.</span></span>
    
  - <span data-ttu-id="8cd3f-130">Az eszközöket ezzel csatlakoztatja az Azure Active Directory-fiókokhoz, és automatikusan regisztrálja őket a Microsoft 365 Business általi kezelésre.</span><span class="sxs-lookup"><span data-stu-id="8cd3f-130">Your devices are going to be connected to Azure Active Directory accounts and automatically enrolled to be managed by Microsoft 365 Business.</span></span>
    
    <span data-ttu-id="8cd3f-131">További információ:</span><span class="sxs-lookup"><span data-stu-id="8cd3f-131">For more information, see</span></span>
    
    <span data-ttu-id="8cd3f-132">[Az AutoPilot-profil beállításai](autopilot-profile-settings.md) .</span><span class="sxs-lookup"><span data-stu-id="8cd3f-132">[About AutoPilot Profile settings](autopilot-profile-settings.md) .</span></span> 
    
5. <span data-ttu-id="8cd3f-133">A további beállítások: **Adatvédelmi beállítások kihagyása** és **Nem léptethető elő a felhasználó a helyi rendszergazdává**. Mindkettő értéke alapértelmezés szerint **Kikapcsolva**.</span><span class="sxs-lookup"><span data-stu-id="8cd3f-133">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="8cd3f-134">Válassza a **Tovább** gombot.</span><span class="sxs-lookup"><span data-stu-id="8cd3f-134">Choose **Next**.</span></span>
    
6. <span data-ttu-id="8cd3f-p105">Az **Elkészült!** lap megjelenése jelzi, hogy a rendszer a létrehozott (vagy kiválasztott) profilt alkalmazza arra az eszközcsoportra, amelyet Ön az eszközlista feltöltésével létrehozott. Ezek a beállítások lesznek érvényben legközelebb, amikor az eszköz felhasználói bejelentkeznek. Válassza a **Bezárás** gombot.</span><span class="sxs-lookup"><span data-stu-id="8cd3f-p105">**You're done** page indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices. These settings will be in effect when the device users sign in next. Choose **Close**.</span></span>
    
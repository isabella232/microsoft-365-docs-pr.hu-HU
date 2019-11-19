---
title: Windows 10-es eszközök védelme
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_BCSSetup4WindowsConfig
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 21e5551f-fa35-4f13-9418-f80d668b6a2b
description: 'Információ a Windows 10-eszközök biztonságossá tétele érdekében használt alapértelmezett és egyéb beállításokról. '
ms.openlocfilehash: fef1bc3e19bada5785232047d37f4bc2393a974d
ms.sourcegitcommit: 5d11f516e78ea4a74145e19ba2300f0792c8bac1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38715102"
---
# <a name="secure-windows-10-devices"></a><span data-ttu-id="ce8fa-103">Windows 10-es eszközök védelme</span><span class="sxs-lookup"><span data-stu-id="ce8fa-103">Secure Windows 10 devices</span></span>

<span data-ttu-id="ce8fa-104">Az itt megadott beállítások a Windows 10-es eszközökre vonatkozó alapértelmezett eszközházirend részei lesznek.</span><span class="sxs-lookup"><span data-stu-id="ce8fa-104">The settings that you configure here are part of the default device policy for Windows 10.</span></span> <span data-ttu-id="ce8fa-105">A Windows 10 eszközt, beleértve a mobileszközöket és a számítógépeket, a saját munkafiókjuk segítségével összekapcsolók minden felhasználó automatikusan megkapja ezeket a beállításokat.</span><span class="sxs-lookup"><span data-stu-id="ce8fa-105">All users who connect a Windows 10 device, including mobile devices and PCs, by signing in with their work account will automatically receive these settings.</span></span> <span data-ttu-id="ce8fa-106">Azt javasoljuk, hogy a telepítés során az alapértelmezett házirendet fogadja el, az egyes felhasználói csoportokra vonatkozó házirendeket pedig a telepítés után adja hozzá.</span><span class="sxs-lookup"><span data-stu-id="ce8fa-106">We recommend that you accept the default policy during setup and add policies later that target specific groups of users.</span></span>
  
## <a name="settings-to-secure-windows-10-devices"></a><span data-ttu-id="ce8fa-107">Windows 10-es eszközök biztonságára vonatkozó beállítások</span><span class="sxs-lookup"><span data-stu-id="ce8fa-107">Settings to secure Windows 10 devices</span></span>

<span data-ttu-id="ce8fa-p102">Alapértelmezés szerint minden beállítás **Be** állapotban van. Az alábbi beállítások érhetők el:</span><span class="sxs-lookup"><span data-stu-id="ce8fa-p102">By default all settings are **On**. The following settings are available:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="ce8fa-110">Beállítás</span><span class="sxs-lookup"><span data-stu-id="ce8fa-110">Setting</span></span>  <br/> |<span data-ttu-id="ce8fa-111">Leírás</span><span class="sxs-lookup"><span data-stu-id="ce8fa-111">Description</span></span>  <br/> |
|<span data-ttu-id="ce8fa-112">PC-k védelme a vírusokkal és más fenyegetésekkel szemben a Windows Defender víruskereső használatával</span><span class="sxs-lookup"><span data-stu-id="ce8fa-112">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="ce8fa-113">Használatához a Windows Defender víruskeresőnek bekapcsolt állapotban kell lennie, hogy a PC-ket védeni lehessen az internetes kapcsolat során előforduló fenyegetésekkel szemben.</span><span class="sxs-lookup"><span data-stu-id="ce8fa-113">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="ce8fa-114">PC-k védelme a webes fenyegetésekkel szemben a Microsoft Edge böngészőben</span><span class="sxs-lookup"><span data-stu-id="ce8fa-114">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="ce8fa-115">Bekapcsolja a Microsoft Edge böngészőben azokat a beállításokat, amelyek segítenek megvédeni a felhasználót a kártékony webhelyek és letöltések által okozott veszélyektől.</span><span class="sxs-lookup"><span data-stu-id="ce8fa-115">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="ce8fa-116">Az eszköz képernyőjének kikapcsolása ennyi üresjárati idő után</span><span class="sxs-lookup"><span data-stu-id="ce8fa-116">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="ce8fa-p103">Biztosítja a céges adatok védelmét, amikor a felhasználó inaktív. Előfordulhat, hogy a felhasználó nyilvános helyen, például egy kávézóban végez munkát, és ilyenkor ha csak rövid időre is elvonják a figyelmét az eszközről, akkor annak kijelzőjét illetéktelen személyek is láthatják. Ezzel a beállítással azt határozhatja meg, hogy a felhasználó mennyi ideig maradhat inaktív, mielőtt az eszköz kijelzője kikapcsol.</span><span class="sxs-lookup"><span data-stu-id="ce8fa-p103">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
|<span data-ttu-id="ce8fa-120">A felhasználók letölthetnek appokat innen: Microsoft Áruház</span><span class="sxs-lookup"><span data-stu-id="ce8fa-120">Allow users to download apps from Microsoft Store</span></span>  <br/> |<span data-ttu-id="ce8fa-p104">Lehetővé teszi, hogy a felhasználók appokat tölthessenek le és telepíthessenek a Microsoft Áruházból. Az appok között játékok és munkára használható eszközök egyaránt lehetnek, ezért ez a beállítás **Be** állapotban van, de a fokozott biztonság érdekében ki is kapcsolhatja.  </span><span class="sxs-lookup"><span data-stu-id="ce8fa-p104">Lets users download and install apps from the Microsoft Store. Apps include everything from games to productivity tools, so we leave this setting **On**, but you can turn it off for extra security.  </span></span><br/> |
|<span data-ttu-id="ce8fa-123">A felhasználók igénybe vehetik Cortana segítségét</span><span class="sxs-lookup"><span data-stu-id="ce8fa-123">Allow users to access Cortana</span></span>  <br/> |<span data-ttu-id="ce8fa-124">Cortana nagyon hasznos lehet.</span><span class="sxs-lookup"><span data-stu-id="ce8fa-124">Cortana can be very helpful!</span></span> <span data-ttu-id="ce8fa-125">A Cortana be-vagy kikapcsolja a beállításokat, útmutatást ad, és a találkozók ideje alatt biztos lehet, hogy ezt **a beállítást alapértelmezés** szerint megtartja.</span><span class="sxs-lookup"><span data-stu-id="ce8fa-125">Cortana can turn settings on or off for you, give directions, and make sure you're on time for appointments, so we keep this setting **On** by default.</span></span>  <br/> |
|<span data-ttu-id="ce8fa-126">A felhasználók kaphatnak tippeket és hirdetéseket a Windowszal kapcsolatban a Microsofttól</span><span class="sxs-lookup"><span data-stu-id="ce8fa-126">Allow users to receive Windows tips and advertisements from Microsoft</span></span>  <br/> |<span data-ttu-id="ce8fa-127">A Windows-tippek hasznosak lehetnek, és új funkciók megjelenésekor segíthetnek a felhasználóknak a funkciók megismerésében.</span><span class="sxs-lookup"><span data-stu-id="ce8fa-127">Windows tips can be handy and help orient users when new features are released.</span></span>  <br/> |
|<span data-ttu-id="ce8fa-128">A Windows 10-es eszközök automatikus naprakészen tartása</span><span class="sxs-lookup"><span data-stu-id="ce8fa-128">Keep Windows 10 devices up to date automatically</span></span>  <br/> |<span data-ttu-id="ce8fa-129">Biztosítja, hogy a Windows 10-es eszközök automatikusan megkapják a legújabb frissítéseket.</span><span class="sxs-lookup"><span data-stu-id="ce8fa-129">Makes sure that Windows 10 devices automatically receive the latest updates.</span></span>  <br/> |
   


---
title: Windows 10-es eszközök védelme
f1.keywords:
- CSH
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
ms.assetid: 21e5551f-fa35-4f13-9418-f80d668b6a2b
description: Ismerje meg, hogyan konfigurálja az alapértelmezett eszközházirend beállításait, amelyet bármely Windows 10-eszköz kap, amikor bejelentkezik a munkahelyi vagy iskolai fiókjába.
ms.openlocfilehash: 03ae86861ddb0cb83cd39b7834f19e01bf3e99e2
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44470627"
---
# <a name="secure-windows-10-devices"></a><span data-ttu-id="cd009-103">Windows 10-es eszközök védelme</span><span class="sxs-lookup"><span data-stu-id="cd009-103">Secure Windows 10 devices</span></span>

<span data-ttu-id="cd009-104">Ez a cikk a Microsoft 365 Business Premium szolgáltatásra vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="cd009-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="cd009-105">Az itt megadott beállítások a Windows 10-es eszközökre vonatkozó alapértelmezett eszközházirend részei lesznek.</span><span class="sxs-lookup"><span data-stu-id="cd009-105">The settings that you configure here are part of the default device policy for Windows 10.</span></span> <span data-ttu-id="cd009-106">Minden olyan felhasználó, aki munkahelyi fiókjával bejelentkezve windows 10-es eszközt csatlakoztat, beleértve a mobileszközöket és a számítógépeket is, automatikusan megkapja ezeket a beállításokat.</span><span class="sxs-lookup"><span data-stu-id="cd009-106">All users who connect a Windows 10 device, including mobile devices and PCs, by signing in with their work account will automatically receive these settings.</span></span> <span data-ttu-id="cd009-107">Azt javasoljuk, hogy a telepítés során az alapértelmezett házirendet fogadja el, az egyes felhasználói csoportokra vonatkozó házirendeket pedig a telepítés után adja hozzá.</span><span class="sxs-lookup"><span data-stu-id="cd009-107">We recommend that you accept the default policy during setup and add policies later that target specific groups of users.</span></span>
  
## <a name="settings-to-secure-windows-10-devices"></a><span data-ttu-id="cd009-108">Windows 10-es eszközök biztonságára vonatkozó beállítások</span><span class="sxs-lookup"><span data-stu-id="cd009-108">Settings to secure Windows 10 devices</span></span>

<span data-ttu-id="cd009-p102">Alapértelmezés szerint minden beállítás **Be** állapotban van. Az alábbi beállítások érhetők el:</span><span class="sxs-lookup"><span data-stu-id="cd009-p102">By default all settings are **On**. The following settings are available:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="cd009-111">Beállítás</span><span class="sxs-lookup"><span data-stu-id="cd009-111">Setting</span></span>  <br/> |<span data-ttu-id="cd009-112">Leírás</span><span class="sxs-lookup"><span data-stu-id="cd009-112">Description</span></span>  <br/> |
|<span data-ttu-id="cd009-113">PC-k védelme a vírusokkal és más fenyegetésekkel szemben a Windows Defender víruskereső használatával</span><span class="sxs-lookup"><span data-stu-id="cd009-113">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="cd009-114">Használatához a Windows Defender víruskeresőnek bekapcsolt állapotban kell lennie, hogy a PC-ket védeni lehessen az internetes kapcsolat során előforduló fenyegetésekkel szemben.</span><span class="sxs-lookup"><span data-stu-id="cd009-114">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="cd009-115">PC-k védelme a webes fenyegetésekkel szemben a Microsoft Edge böngészőben</span><span class="sxs-lookup"><span data-stu-id="cd009-115">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="cd009-116">Bekapcsolja a Microsoft Edge böngészőben azokat a beállításokat, amelyek segítenek megvédeni a felhasználót a kártékony webhelyek és letöltések által okozott veszélyektől.</span><span class="sxs-lookup"><span data-stu-id="cd009-116">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="cd009-117">Az eszköz képernyőjének kikapcsolása ennyi üresjárati idő után</span><span class="sxs-lookup"><span data-stu-id="cd009-117">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="cd009-p103">Biztosítja a céges adatok védelmét, amikor a felhasználó inaktív. Előfordulhat, hogy a felhasználó nyilvános helyen, például egy kávézóban végez munkát, és ilyenkor ha csak rövid időre is elvonják a figyelmét az eszközről, akkor annak kijelzőjét illetéktelen személyek is láthatják. Ezzel a beállítással azt határozhatja meg, hogy a felhasználó mennyi ideig maradhat inaktív, mielőtt az eszköz kijelzője kikapcsol.</span><span class="sxs-lookup"><span data-stu-id="cd009-p103">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
|<span data-ttu-id="cd009-121">A felhasználók letölthetnek appokat innen: Microsoft Áruház</span><span class="sxs-lookup"><span data-stu-id="cd009-121">Allow users to download apps from Microsoft Store</span></span>  <br/> |<span data-ttu-id="cd009-p104">Lehetővé teszi, hogy a felhasználók appokat tölthessenek le és telepíthessenek a Microsoft Áruházból. Az appok között játékok és munkára használható eszközök egyaránt lehetnek, ezért ez a beállítás **Be** állapotban van, de a fokozott biztonság érdekében ki is kapcsolhatja.  </span><span class="sxs-lookup"><span data-stu-id="cd009-p104">Lets users download and install apps from the Microsoft Store. Apps include everything from games to productivity tools, so we leave this setting **On**, but you can turn it off for extra security.  </span></span><br/> |
|<span data-ttu-id="cd009-124">A felhasználók igénybe vehetik Cortana segítségét</span><span class="sxs-lookup"><span data-stu-id="cd009-124">Allow users to access Cortana</span></span>  <br/> |<span data-ttu-id="cd009-125">Cortana nagyon hasznos lehet.</span><span class="sxs-lookup"><span data-stu-id="cd009-125">Cortana can be very helpful!</span></span> <span data-ttu-id="cd009-126">Cortana be- és kikapcsolhatja a beállításokat, útbaigazítást adhat, és meggyőződhet arról, hogy időben van a találkozókhoz, ezért alapértelmezés szerint **bekapcsolva** tartjuk ezt a beállítást.</span><span class="sxs-lookup"><span data-stu-id="cd009-126">Cortana can turn settings on or off for you, give directions, and make sure you're on time for appointments, so we keep this setting **On** by default.</span></span>  <br/> |
|<span data-ttu-id="cd009-127">A felhasználók kaphatnak tippeket és hirdetéseket a Windowszal kapcsolatban a Microsofttól</span><span class="sxs-lookup"><span data-stu-id="cd009-127">Allow users to receive Windows tips and advertisements from Microsoft</span></span>  <br/> |<span data-ttu-id="cd009-128">A Windows-tippek hasznosak lehetnek, és új funkciók megjelenésekor segíthetnek a felhasználóknak a funkciók megismerésében.</span><span class="sxs-lookup"><span data-stu-id="cd009-128">Windows tips can be handy and help orient users when new features are released.</span></span>  <br/> |
|<span data-ttu-id="cd009-129">A Windows 10-es eszközök automatikus naprakészen tartása</span><span class="sxs-lookup"><span data-stu-id="cd009-129">Keep Windows 10 devices up to date automatically</span></span>  <br/> |<span data-ttu-id="cd009-130">Biztosítja, hogy a Windows 10-es eszközök automatikusan megkapják a legújabb frissítéseket.</span><span class="sxs-lookup"><span data-stu-id="cd009-130">Makes sure that Windows 10 devices automatically receive the latest updates.</span></span>  <br/> |
   


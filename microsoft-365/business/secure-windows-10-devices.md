---
title: Windows 10-es eszközök védelme
ms.author: sirkkuw
author: sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: overview
f1_keywords:
- O365E_BCSSetup4WindowsConfig
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 21e5551f-fa35-4f13-9418-f80d668b6a2b
description: 'Tudnivalók az alapértelmezett és az egyéb beállítások megadása Windows 10 eszközök biztonságos. '
ms.openlocfilehash: 0bdf6a56d880cb84f4a4f50550539d97c006ba49
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/16/2019
ms.locfileid: "26983655"
---
# <a name="secure-windows-10-devices"></a><span data-ttu-id="9a381-103">Windows 10-es eszközök védelme</span><span class="sxs-lookup"><span data-stu-id="9a381-103">Secure Windows 10 devices</span></span>

<span data-ttu-id="9a381-p101">Az itt megadott beállítások a Windows 10-es eszközökre vonatkozó alapértelmezett eszközházirend részei lesznek. Ha egy felhasználó valamely Windows 10-es eszközön jelentkezik be munkahelyi fiókjába (beleértve a mobileszközöket és a PC-ket is), akkor automatikusan érvényesek lesznek rá ezek a beállítások. Azt javasoljuk, hogy a telepítés során az alapértelmezett házirendet fogadja el, az egyes felhasználói csoportokra vonatkozó házirendeket pedig a telepítés után adja hozzá.</span><span class="sxs-lookup"><span data-stu-id="9a381-p101">The settings that you configure here are part of the default device policy for Windows 10. All users that connect a Windows 10 device, including mobile devices and PCs, by signing in with their work account, will automatically receive these settings. We recommend that you accept the default policy during setup and add policies later that target specific groups of users.</span></span>
  
## <a name="settings-to-secure-windows-10-devices"></a><span data-ttu-id="9a381-107">Windows 10-es eszközök biztonságára vonatkozó beállítások</span><span class="sxs-lookup"><span data-stu-id="9a381-107">Settings to secure Windows 10 devices</span></span>

<span data-ttu-id="9a381-p102">Alapértelmezés szerint minden beállítás **Be** állapotban van. Az alábbi beállítások érhetők el:</span><span class="sxs-lookup"><span data-stu-id="9a381-p102">By default all settings are **On**. The following settings are available:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="9a381-110">Beállítás</span><span class="sxs-lookup"><span data-stu-id="9a381-110">Setting</span></span>  <br/> |<span data-ttu-id="9a381-111">Leírás</span><span class="sxs-lookup"><span data-stu-id="9a381-111">Description</span></span>  <br/> |
|<span data-ttu-id="9a381-112">PC-k védelme a vírusokkal és más fenyegetésekkel szemben a Windows Defender víruskereső használatával</span><span class="sxs-lookup"><span data-stu-id="9a381-112">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="9a381-113">Használatához a Windows Defender víruskeresőnek bekapcsolt állapotban kell lennie, hogy védelmet nyújthasson a PC-knek az internethez csatlakozva jelentkező veszélyekkel szemben.</span><span class="sxs-lookup"><span data-stu-id="9a381-113">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="9a381-114">PC-k védelme a webes fenyegetésekkel szemben a Microsoft Edge böngészőben</span><span class="sxs-lookup"><span data-stu-id="9a381-114">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="9a381-115">Bekapcsolja a Microsoft Edge böngészőben azokat a beállításokat, amelyek segítenek megvédeni a felhasználót a kártékony webhelyek és letöltések által okozott veszélyektől.</span><span class="sxs-lookup"><span data-stu-id="9a381-115">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="9a381-116">Az eszköz képernyőjének kikapcsolása ennyi üresjárati idő után</span><span class="sxs-lookup"><span data-stu-id="9a381-116">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="9a381-p103">Biztosítja a céges adatok védelmét, amikor a felhasználó inaktív. Tegyük fel például, hogy a felhasználó nyilvános helyen, például egy kávézóban dolgozik. Ilyenkor, ha akár csak rövid időre is, de elvonhatják a figyelmét, és így illetéktelen személyek is láthatják az eszköz kijelzőjét. Ezzel a beállítással szabályozhatja, hogy a felhasználó mennyi ideig maradhat inaktív, mielőtt a kijelző kikapcsol.</span><span class="sxs-lookup"><span data-stu-id="9a381-p103">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
|<span data-ttu-id="9a381-120">A felhasználók letölthetnek appokat innen: Microsoft Áruház</span><span class="sxs-lookup"><span data-stu-id="9a381-120">Allow users to download apps from Microsoft Store</span></span>  <br/> |<span data-ttu-id="9a381-p104">Lehetővé teszi, hogy a felhasználók appokat tölthessenek le és telepíthessenek a Microsoft Áruházból. Az appok között játékok és munkára használható eszközök egyaránt lehetnek, ezért ez a beállítás **Be** állapotban van, de a fokozott biztonság érdekében ki is kapcsolhatja.  </span><span class="sxs-lookup"><span data-stu-id="9a381-p104">Lets users download and install apps from the Microsoft Store. Apps include everything from games to productivity tools, so we leave this setting **On**, but you can turn it off for extra security.  </span></span><br/> |
|<span data-ttu-id="9a381-123">A felhasználók igénybe vehetik Cortana segítségét</span><span class="sxs-lookup"><span data-stu-id="9a381-123">Allow users to access Cortana</span></span>  <br/> |<span data-ttu-id="9a381-p105">Cortana nagyon hasznos lehet. Beállításokat képes be- és kikapcsolni, útbaigazítást tud adni, és ügyelni tud arra, hogy Ön ne késsen el a megbeszéléseiről, ezért ez a beállítás alapértelmezés szerint **Be** állapotban van.  </span><span class="sxs-lookup"><span data-stu-id="9a381-p105">Cortana can be very helpful! She can turn settings on or off for you, give directions, and make sure you're on time for appointments, so we keep this **On** by default.  </span></span><br/> |
|<span data-ttu-id="9a381-126">A felhasználók kaphatnak tippeket és hirdetéseket a Windowszal kapcsolatban a Microsofttól</span><span class="sxs-lookup"><span data-stu-id="9a381-126">Allow users to receive Windows tips and advertisements from Microsoft</span></span>  <br/> |<span data-ttu-id="9a381-127">A Windows-tippek hasznosak lehetnek, és új funkciók megjelenésekor segíthetnek a felhasználóknak a funkciók megismerésében.</span><span class="sxs-lookup"><span data-stu-id="9a381-127">Windows tips can be handy and help orient users when new features are released.</span></span>  <br/> |
|<span data-ttu-id="9a381-128">A Windows 10-es eszközök automatikus naprakészen tartása</span><span class="sxs-lookup"><span data-stu-id="9a381-128">Keep Windows 10 devices up to date automatically</span></span>  <br/> |<span data-ttu-id="9a381-129">Biztosítja, hogy a Windows 10-es eszközök automatikusan megkapják a legújabb frissítéseket.</span><span class="sxs-lookup"><span data-stu-id="9a381-129">Makes sure that Windows 10 devices automatically receive the latest updates.</span></span>  <br/> |
   


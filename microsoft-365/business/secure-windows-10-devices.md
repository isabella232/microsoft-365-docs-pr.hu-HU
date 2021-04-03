---
title: Windows 10-es eszközök védelme
f1.keywords:
- CSH
ms.author: sharik
author: skjerland
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
description: Megtudhatja, hogy hogyan konfigurálhatja az alapértelmezett eszköz-házirendet, amit minden Windows 10-es eszköz a munkahelyi vagy iskolai fiókjába való bejelentkezés után fog megkapni.
ms.openlocfilehash: 86db1c152f9f6ac1fe6093b4a55a74b69fbd8b0f
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579974"
---
# <a name="secure-windows-10-devices"></a><span data-ttu-id="830c3-103">Windows 10-es eszközök védelme</span><span class="sxs-lookup"><span data-stu-id="830c3-103">Secure Windows 10 devices</span></span>

<span data-ttu-id="830c3-104">Ez a cikk a Microsoft 365 Vállalati prémium verzióra vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="830c3-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="830c3-105">Az itt megadott beállítások a Windows 10-es eszközökre vonatkozó alapértelmezett eszközházirend részei lesznek.</span><span class="sxs-lookup"><span data-stu-id="830c3-105">The settings that you configure here are part of the default device policy for Windows 10.</span></span> <span data-ttu-id="830c3-106">Minden olyan felhasználó, aki munkahelyi fiókjával bejelentkezve Windows 10-es eszközt – beleértve a mobileszközöket és a PC-ket – csatlakozik, automatikusan megkapja ezeket a beállításokat.</span><span class="sxs-lookup"><span data-stu-id="830c3-106">All users who connect a Windows 10 device, including mobile devices and PCs, by signing in with their work account will automatically receive these settings.</span></span> <span data-ttu-id="830c3-107">Azt javasoljuk, hogy a telepítés során az alapértelmezett házirendet fogadja el, az egyes felhasználói csoportokra vonatkozó házirendeket pedig a telepítés után adja hozzá.</span><span class="sxs-lookup"><span data-stu-id="830c3-107">We recommend that you accept the default policy during setup and add policies later that target specific groups of users.</span></span>
  
## <a name="settings-to-secure-windows-10-devices"></a><span data-ttu-id="830c3-108">Windows 10-es eszközök biztonságára vonatkozó beállítások</span><span class="sxs-lookup"><span data-stu-id="830c3-108">Settings to secure Windows 10 devices</span></span>

<span data-ttu-id="830c3-p102">Alapértelmezés szerint minden beállítás **Be** állapotban van. Az alábbi beállítások érhetők el:</span><span class="sxs-lookup"><span data-stu-id="830c3-p102">By default all settings are **On**. The following settings are available:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="830c3-111">Beállítás</span><span class="sxs-lookup"><span data-stu-id="830c3-111">Setting</span></span>  <br/> |<span data-ttu-id="830c3-112">Leírás</span><span class="sxs-lookup"><span data-stu-id="830c3-112">Description</span></span>  <br/> |
|<span data-ttu-id="830c3-113">PC-k védelme a vírusokkal és más fenyegetésekkel szemben a Windows Defender víruskereső használatával</span><span class="sxs-lookup"><span data-stu-id="830c3-113">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="830c3-114">Használatához a Windows Defender víruskeresőnek bekapcsolt állapotban kell lennie, hogy a PC-ket védeni lehessen az internetes kapcsolat során előforduló fenyegetésekkel szemben.</span><span class="sxs-lookup"><span data-stu-id="830c3-114">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="830c3-115">PC-k védelme a webes fenyegetésekkel szemben a Microsoft Edge böngészőben</span><span class="sxs-lookup"><span data-stu-id="830c3-115">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="830c3-116">Bekapcsolja a Microsoft Edge böngészőben azokat a beállításokat, amelyek segítenek megvédeni a felhasználót a kártékony webhelyek és letöltések által okozott veszélyektől.</span><span class="sxs-lookup"><span data-stu-id="830c3-116">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="830c3-117">PC-ken lévő fájlok és mappák illetéktelen hozzáféréssel szembeni védelme BitLocker-titkosítással</span><span class="sxs-lookup"><span data-stu-id="830c3-117">Help protect files and folders on PCs from unauthorized access with BitLocker</span></span>  <br/> |<span data-ttu-id="830c3-118">A Bitlocker a számítógép merevlemezének titkosításával és a számítógép elvesztése vagy ellopása esetén az adatok kinyerése elleni védelemmel biztosítja adatai védelmét.</span><span class="sxs-lookup"><span data-stu-id="830c3-118">Bitlocker protects data by encrypting the computer hard drives and protect against data exposure if a computer is lost or stolen.</span></span> <span data-ttu-id="830c3-119">További információt a Bitlocker – gyakori [kérdések című témakörben talál.](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions)</span><span class="sxs-lookup"><span data-stu-id="830c3-119">For more information, see [Bitlocker FAQ](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions).</span></span>  <br/> |
|<span data-ttu-id="830c3-120">Az eszköz képernyőjének kikapcsolása ennyi üresjárati idő után</span><span class="sxs-lookup"><span data-stu-id="830c3-120">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="830c3-p104">Biztosítja a céges adatok védelmét, amikor a felhasználó inaktív. Előfordulhat, hogy a felhasználó nyilvános helyen, például egy kávézóban végez munkát, és ilyenkor ha csak rövid időre is elvonják a figyelmét az eszközről, akkor annak kijelzőjét illetéktelen személyek is láthatják. Ezzel a beállítással azt határozhatja meg, hogy a felhasználó mennyi ideig maradhat inaktív, mielőtt az eszköz kijelzője kikapcsol.</span><span class="sxs-lookup"><span data-stu-id="830c3-p104">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
|
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
description: Megtudhatja, hogy miként konfigurálhatja az alapértelmezett eszköz-házirend beállításait, amelyet bármely Windows 10-es eszköz kap a munkahelyi vagy iskolai fiókjába való bejelentkezéskor.
ms.openlocfilehash: 85448507835b6310ca4136849be6a40caf6bb919
ms.sourcegitcommit: abf63669daf12993ad3353e4b578f41c8910b20f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/27/2020
ms.locfileid: "47289077"
---
# <a name="secure-windows-10-devices"></a><span data-ttu-id="b02af-103">Windows 10-es eszközök védelme</span><span class="sxs-lookup"><span data-stu-id="b02af-103">Secure Windows 10 devices</span></span>

<span data-ttu-id="b02af-104">Ez a cikk a Microsoft 365 vállalati prémium verzióra vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="b02af-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="b02af-105">Az itt megadott beállítások a Windows 10-es eszközökre vonatkozó alapértelmezett eszközházirend részei lesznek.</span><span class="sxs-lookup"><span data-stu-id="b02af-105">The settings that you configure here are part of the default device policy for Windows 10.</span></span> <span data-ttu-id="b02af-106">Azok a felhasználók, akik a saját munkahelyi fiókjával együtt csatlakoznak a Windows 10-es eszközökhöz, például mobileszközökön és PC-k, automatikusan megkapják ezeket a beállításokat.</span><span class="sxs-lookup"><span data-stu-id="b02af-106">All users who connect a Windows 10 device, including mobile devices and PCs, by signing in with their work account will automatically receive these settings.</span></span> <span data-ttu-id="b02af-107">Azt javasoljuk, hogy a telepítés során az alapértelmezett házirendet fogadja el, az egyes felhasználói csoportokra vonatkozó házirendeket pedig a telepítés után adja hozzá.</span><span class="sxs-lookup"><span data-stu-id="b02af-107">We recommend that you accept the default policy during setup and add policies later that target specific groups of users.</span></span>
  
## <a name="settings-to-secure-windows-10-devices"></a><span data-ttu-id="b02af-108">Windows 10-es eszközök biztonságára vonatkozó beállítások</span><span class="sxs-lookup"><span data-stu-id="b02af-108">Settings to secure Windows 10 devices</span></span>

<span data-ttu-id="b02af-p102">Alapértelmezés szerint minden beállítás **Be** állapotban van. Az alábbi beállítások érhetők el:</span><span class="sxs-lookup"><span data-stu-id="b02af-p102">By default all settings are **On**. The following settings are available:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="b02af-111">Beállítás</span><span class="sxs-lookup"><span data-stu-id="b02af-111">Setting</span></span>  <br/> |<span data-ttu-id="b02af-112">Leírás</span><span class="sxs-lookup"><span data-stu-id="b02af-112">Description</span></span>  <br/> |
|<span data-ttu-id="b02af-113">PC-k védelme a vírusokkal és más fenyegetésekkel szemben a Windows Defender víruskereső használatával</span><span class="sxs-lookup"><span data-stu-id="b02af-113">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="b02af-114">Használatához a Windows Defender víruskeresőnek bekapcsolt állapotban kell lennie, hogy a PC-ket védeni lehessen az internetes kapcsolat során előforduló fenyegetésekkel szemben.</span><span class="sxs-lookup"><span data-stu-id="b02af-114">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="b02af-115">PC-k védelme a webes fenyegetésekkel szemben a Microsoft Edge böngészőben</span><span class="sxs-lookup"><span data-stu-id="b02af-115">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="b02af-116">Bekapcsolja a Microsoft Edge böngészőben azokat a beállításokat, amelyek segítenek megvédeni a felhasználót a kártékony webhelyek és letöltések által okozott veszélyektől.</span><span class="sxs-lookup"><span data-stu-id="b02af-116">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="b02af-117">PC-ken lévő fájlok és mappák illetéktelen hozzáféréssel szembeni védelme BitLocker-titkosítással</span><span class="sxs-lookup"><span data-stu-id="b02af-117">Help protect files and folders on PCs from unauthorized access with BitLocker</span></span>  <br/> |<span data-ttu-id="b02af-118">A Bitlocker a számítógép merevlemezének titkosításával és a számítógép elvesztése vagy ellopása esetén az adatok kinyerése elleni védelemmel biztosítja adatai védelmét.</span><span class="sxs-lookup"><span data-stu-id="b02af-118">Bitlocker protects data by encrypting the computer hard drives and protect against data exposure if a computer is lost or stolen.</span></span> <span data-ttu-id="b02af-119">További információt a [BitLocker – gyakori kérdések](https://go.microsoft.com/fwlink/?linkid=871000)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="b02af-119">For more information, see [Bitlocker FAQ](https://go.microsoft.com/fwlink/?linkid=871000).</span></span>  <br/> |
|<span data-ttu-id="b02af-120">Az eszköz képernyőjének kikapcsolása ennyi üresjárati idő után</span><span class="sxs-lookup"><span data-stu-id="b02af-120">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="b02af-p104">Biztosítja a céges adatok védelmét, amikor a felhasználó inaktív. Előfordulhat, hogy a felhasználó nyilvános helyen, például egy kávézóban végez munkát, és ilyenkor ha csak rövid időre is elvonják a figyelmét az eszközről, akkor annak kijelzőjét illetéktelen személyek is láthatják. Ezzel a beállítással azt határozhatja meg, hogy a felhasználó mennyi ideig maradhat inaktív, mielőtt az eszköz kijelzője kikapcsol.</span><span class="sxs-lookup"><span data-stu-id="b02af-p104">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
|
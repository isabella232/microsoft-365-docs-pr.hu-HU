---
title: Munkahelyi fájlok védelme elveszett vagy ellopott eszközön
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_BCSSetup4StolenDevice
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c12164c7-6190-4294-b88a-590580c9869a
description: Ismerje meg a munkahelyi fájlok védelmére rendelkezésre álló beállításokat, ha a felhasználó eszköze elveszett vagy ellopták.
ms.openlocfilehash: 5f137354b51a0151e57e5e109b1ebbb043c68f60
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593556"
---
# <a name="protect-work-files-when-a-mobile-device-is-lost-or-stolen"></a><span data-ttu-id="6022f-103">Munkahelyi fájlok védelme elveszett vagy ellopott eszközön</span><span class="sxs-lookup"><span data-stu-id="6022f-103">Protect work files when a mobile device is lost or stolen</span></span>

<span data-ttu-id="6022f-104">A házirendbeállítások azt határozzák meg, hogy mi történjen automatikusan az elveszett vagy ellopott eszközök védelme érdekében.</span><span class="sxs-lookup"><span data-stu-id="6022f-104">The policy settings determine what happens automatically to protect a device that is lost or stolen.</span></span> <span data-ttu-id="6022f-105">Azt javasoljuk, hogy a telepítés során fogadja el az alapértelmezett értékeket az Android, az iOS és a Windows 10 alkalmazásházirendjeinek létrehozásához, amelyek minden felhasználóra vonatkoznak.</span><span class="sxs-lookup"><span data-stu-id="6022f-105">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="6022f-106">A telepítés után további házirendeket is létrehozhat majd.</span><span class="sxs-lookup"><span data-stu-id="6022f-106">You can create more policies after setup completes.</span></span>
  
## <a name="settings-that-protect-work-files"></a><span data-ttu-id="6022f-107">Munkahelyi fájlok védelmére szolgáló beállítások</span><span class="sxs-lookup"><span data-stu-id="6022f-107">Settings that protect work files</span></span>

<span data-ttu-id="6022f-108">Az alábbi beállításokkal védhetők meg a munkahelyi fájlok, ha az eszköz elveszett vagy ellopták:</span><span class="sxs-lookup"><span data-stu-id="6022f-108">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="6022f-109">Beállítás</span><span class="sxs-lookup"><span data-stu-id="6022f-109">Setting</span></span>  <br/> |<span data-ttu-id="6022f-110">Leírás</span><span class="sxs-lookup"><span data-stu-id="6022f-110">Description</span></span>  <br/> |
|<span data-ttu-id="6022f-111">Munkahelyi fájlok törlése az inaktív eszközökről ennyi nap után</span><span class="sxs-lookup"><span data-stu-id="6022f-111">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="6022f-112">Ha egy eszközt nem használnak az itt megadott számú napig, az eszközön tárolt munkafájlok automatikusan törlődnek.</span><span class="sxs-lookup"><span data-stu-id="6022f-112">If a device isn't used for the number of days that you specify here, any work files stored on the device are automatically deleted.</span></span>  <br/> |
|<span data-ttu-id="6022f-113">A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió</span><span class="sxs-lookup"><span data-stu-id="6022f-113">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="6022f-114">Ha ez a beállítás **Be van,** a munkahelyi fájlok csak a OneDrive Vállalati verzió számára érhető el mentési hely.</span><span class="sxs-lookup"><span data-stu-id="6022f-114">If this setting is **On**, the only available save location for work files is OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="6022f-115">Munkahelyi fájlok titkosítása</span><span class="sxs-lookup"><span data-stu-id="6022f-115">Encrypt work files</span></span>  <br/> |<span data-ttu-id="6022f-116">A munkahelyi fájlok titkosítással való védelméhez ezt a beállítást tartsa **Be** állapotban.</span><span class="sxs-lookup"><span data-stu-id="6022f-116">Keep this setting **On** so that work files are protected by encryption.</span></span> <span data-ttu-id="6022f-117">Még akkor is, ha az eszköz elveszett vagy ellopták, senki sem tudja olvasni a vállalati adatokat.</span><span class="sxs-lookup"><span data-stu-id="6022f-117">Even if the device is lost or stolen, no one can read your company data.</span></span>  <br/> |
   


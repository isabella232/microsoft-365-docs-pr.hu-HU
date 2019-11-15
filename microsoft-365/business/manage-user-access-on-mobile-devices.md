---
title: Office-dokumentumok felhasználói mobileszközökön történő elérésének felügyelete
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_BCSSetup4OfficeMobile
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: aa31319c-9196-48c9-a90b-4057e0494c7a
description: Ismerje meg a védelmi házirendeket, amelyek segítik az Office alkalmazások mobileszközökről való biztonságos elérését.
ms.openlocfilehash: c24dae7e0eea777e728ebead9a2abcc3785763dd
ms.sourcegitcommit: 9a057e70637dcfe06d4f729a96c02be989cf9e25
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/14/2019
ms.locfileid: "38633349"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="fd61f-103">Office-dokumentumok felhasználói mobileszközökön történő elérésének felügyelete</span><span class="sxs-lookup"><span data-stu-id="fd61f-103">Manage how users access Office documents on mobile devices</span></span>

 <span data-ttu-id="fd61f-104">Az Office-dokumentumok felhasználói mobileszközökön történő elérésének felügyeletét végző házirendek alapértelmezés szerint **Ki** értékre van állítva.</span><span class="sxs-lookup"><span data-stu-id="fd61f-104">Policy settings that control how users access Office files from their mobile devices are **Off** by default.</span></span> <span data-ttu-id="fd61f-105">Javasoljuk, hogy a telepítés során fogadja el az alapértelmezett értékeket, hogy az összes felhasználóra érvényes Android, iOS és Windows 10 alkalmazások házirendjeit hozza létre.</span><span class="sxs-lookup"><span data-stu-id="fd61f-105">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="fd61f-106">A telepítés után további házirendeket is létrehozhat majd.</span><span class="sxs-lookup"><span data-stu-id="fd61f-106">You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="fd61f-107">Az Office-fájlok mobileszközökön történő elérésének felügyeletét meghatározó beállítások</span><span class="sxs-lookup"><span data-stu-id="fd61f-107">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="fd61f-108">Az alábbi beállítások használhatók a munkahelyi Office-fájlok elérésének kezelésére:</span><span class="sxs-lookup"><span data-stu-id="fd61f-108">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="fd61f-109">Beállítás</span><span class="sxs-lookup"><span data-stu-id="fd61f-109">Setting</span></span>  <br/> |<span data-ttu-id="fd61f-110">Leírás</span><span class="sxs-lookup"><span data-stu-id="fd61f-110">Description</span></span>  <br/> |
|<span data-ttu-id="fd61f-111">PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez</span><span class="sxs-lookup"><span data-stu-id="fd61f-111">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="fd61f-112">Ha ez a beállítás **be van kapcsolva**, akkor a felhasználóknak a felhasználónevükön és a jelszavuk mellett egy másik hitelesítési formát kell biztosítaniuk, mielőtt az Office alkalmazásokat mobileszközükön használhatják.</span><span class="sxs-lookup"><span data-stu-id="fd61f-112">If this setting is **On**, users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="fd61f-113">PIN-kód visszaállítása ennyi sikertelen bejelentkezési kísérlet után</span><span class="sxs-lookup"><span data-stu-id="fd61f-113">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="fd61f-114">Annak érdekében, hogy ne lehessen a PIN-kódot véletlenszerű próbálkozásokkal megfejteni, az Ön által megadott számú téves próbálkozás után a PIN-kód alaphelyzetbe áll.</span><span class="sxs-lookup"><span data-stu-id="fd61f-114">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="fd61f-115">A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után</span><span class="sxs-lookup"><span data-stu-id="fd61f-115">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="fd61f-116">Ez a beállítás határozza meg, hogy a felhasználók mennyi ideig lehetnek üresjáratban, mielőtt a rendszer újra bejelentkezne.</span><span class="sxs-lookup"><span data-stu-id="fd61f-116">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="fd61f-117">Hozzáférés letiltása a munkahelyi fájlokhoz a feltört vagy rootolással feltört eszközökön</span><span class="sxs-lookup"><span data-stu-id="fd61f-117">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="fd61f-118">A hozzáértő felhasználók esetleg feltört vagy rootolással feltört eszközzel is rendelkezhetnek.</span><span class="sxs-lookup"><span data-stu-id="fd61f-118">Clever users may have a device that is jailbroken or rooted.</span></span> <span data-ttu-id="fd61f-119">Ez azt jelenti, hogy a felhasználó módosíthatja az operációs rendszer, amely lehet, hogy az eszköz hajlamosabbak a malware.</span><span class="sxs-lookup"><span data-stu-id="fd61f-119">This means that the user can modify the operating system, which can make the device more susceptible to malware.</span></span> <span data-ttu-id="fd61f-120">Ha ez a beállítás **Be** állapotban van, az ilyen eszközök le lesznek tiltva.</span><span class="sxs-lookup"><span data-stu-id="fd61f-120">These devices are blocked when this setting is **On**.</span></span>  <br/> |
|<span data-ttu-id="fd61f-121">A felhasználók nem másolnak tartalmat az Office alkalmazásokból a személyes alkalmazásba</span><span class="sxs-lookup"><span data-stu-id="fd61f-121">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="fd61f-122">Ha a beállítás **be van kapcsolva**, a felhasználó nem másolhatja az adatokat egy munkahelyi fájlba egy személyes fájlba.</span><span class="sxs-lookup"><span data-stu-id="fd61f-122">When the setting is **On**, the user can't copy information in a work file to a personal file.</span></span> <span data-ttu-id="fd61f-123">Ha a beállítás **ki van kapcsolva**, a felhasználó átmásolhatja az adatokat egy munkahelyi fájlból egy személyes alkalmazásba vagy személyes fiókba.</span><span class="sxs-lookup"><span data-stu-id="fd61f-123">If the setting is **Off**, the user can copy information from a work file to a personal app or personal account.</span></span>  <br/> |
   


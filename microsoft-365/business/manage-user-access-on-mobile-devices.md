---
title: Office-dokumentumok felhasználói mobileszközökön történő elérésének felügyelete
f1.keywords:
- NOCSH
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: aa31319c-9196-48c9-a90b-4057e0494c7a
description: Megismerhet olyan védelmi házirendeket, amelyek lehetővé teszik, hogy a felhasználók hogyan férnek hozzá az Office-alkalmazásokhoz és a munkahelyi fájlokhoz mobileszközről.
ms.openlocfilehash: b2b828cf2e201360f12b8fadcb395e72958230f6
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471067"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="40858-103">Office-dokumentumok felhasználói mobileszközökön történő elérésének felügyelete</span><span class="sxs-lookup"><span data-stu-id="40858-103">Manage how users access Office documents on mobile devices</span></span>

<span data-ttu-id="40858-104">Ez a cikk a Microsoft 365 Vállalati prémium verzióra vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="40858-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="40858-105">Az Office-dokumentumok felhasználói mobileszközökön történő elérésének felügyeletét végző házirendek alapértelmezés szerint **Ki** értékre van állítva.</span><span class="sxs-lookup"><span data-stu-id="40858-105">Policy settings that control how users access Office files from their mobile devices are **Off** by default.</span></span> <span data-ttu-id="40858-106">Azt javasoljuk, hogy a telepítés során fogadja el az alapértelmezett értékeket az összes felhasználóra vonatkozó alkalmazás-házirendek létrehozásához Android, iOS és Windows 10 rendszeren.</span><span class="sxs-lookup"><span data-stu-id="40858-106">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="40858-107">A telepítés után további házirendeket is létrehozhat majd.</span><span class="sxs-lookup"><span data-stu-id="40858-107">You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="40858-108">Az Office-fájlok mobileszközökön történő elérésének felügyeletét meghatározó beállítások</span><span class="sxs-lookup"><span data-stu-id="40858-108">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="40858-109">Az alábbi beállítások használhatók a munkahelyi Office-fájlok elérésének kezelésére:</span><span class="sxs-lookup"><span data-stu-id="40858-109">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="40858-110">Beállítás</span><span class="sxs-lookup"><span data-stu-id="40858-110">Setting</span></span>  <br/> |<span data-ttu-id="40858-111">Leírás</span><span class="sxs-lookup"><span data-stu-id="40858-111">Description</span></span>  <br/> |
|<span data-ttu-id="40858-112">PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez</span><span class="sxs-lookup"><span data-stu-id="40858-112">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="40858-113">Ha ez a beállítás **Be,** a felhasználóknak a felhasználónév és a jelszó mellett más hitelesítési módszert is meg kell adniuk ahhoz, hogy használni tudják az Office-appokat a mobileszközükön.</span><span class="sxs-lookup"><span data-stu-id="40858-113">If this setting is **On**, users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="40858-114">PIN-kód visszaállítása ennyi sikertelen bejelentkezési kísérlet után</span><span class="sxs-lookup"><span data-stu-id="40858-114">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="40858-115">Annak érdekében, hogy ne lehessen a PIN-kódot véletlenszerű próbálkozásokkal megfejteni, az Ön által megadott számú téves próbálkozás után a PIN-kód alaphelyzetbe áll.</span><span class="sxs-lookup"><span data-stu-id="40858-115">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="40858-116">A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után</span><span class="sxs-lookup"><span data-stu-id="40858-116">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="40858-117">Ez a beállítás azt határozza meg, hogy egy felhasználó mennyi ideig inaktív, mielőtt a rendszer ismét a bejelentkezésre kéri.</span><span class="sxs-lookup"><span data-stu-id="40858-117">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="40858-118">Hozzáférés letiltása a munkahelyi fájlokhoz a feltört vagy rootolással feltört eszközökön</span><span class="sxs-lookup"><span data-stu-id="40858-118">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="40858-119">A hozzáértő felhasználók esetleg feltört vagy rootolással feltört eszközzel is rendelkezhetnek.</span><span class="sxs-lookup"><span data-stu-id="40858-119">Clever users may have a device that is jailbroken or rooted.</span></span> <span data-ttu-id="40858-120">Ez azt jelenti, hogy a felhasználó módosíthatja az operációs rendszert, így az eszköz jobban ki van téve a kártevőknek.</span><span class="sxs-lookup"><span data-stu-id="40858-120">This means that the user can modify the operating system, which can make the device more susceptible to malware.</span></span> <span data-ttu-id="40858-121">Ha ez a beállítás **Be** állapotban van, az ilyen eszközök le lesznek tiltva.</span><span class="sxs-lookup"><span data-stu-id="40858-121">These devices are blocked when this setting is **On**.</span></span>  <br/> |
|<span data-ttu-id="40858-122">Nem engedélyezi a felhasználóknak, hogy tartalmat másoljanak az Office-alkalmazásokból a személyes appokba</span><span class="sxs-lookup"><span data-stu-id="40858-122">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="40858-123">Ha a beállítás **be van** va, a felhasználó nem másolhat adatokat munkahelyi fájlból személyes fájlba.</span><span class="sxs-lookup"><span data-stu-id="40858-123">When the setting is **On**, the user can't copy information in a work file to a personal file.</span></span> <span data-ttu-id="40858-124">Ha a beállítás ki **van** kapcsolva, a felhasználó átmásolhat adatokat egy munkahelyi fájlból egy személyes appba vagy személyes fiókba.</span><span class="sxs-lookup"><span data-stu-id="40858-124">If the setting is **Off**, the user can copy information from a work file to a personal app or personal account.</span></span>  <br/> |
   


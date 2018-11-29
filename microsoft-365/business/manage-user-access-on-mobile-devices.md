---
title: Office-dokumentumok felhasználói mobileszközökön történő elérésének felügyelete
ms.author: sirkkuw
author: sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: overview
f1_keywords:
- 'O365E_BCSSetup4OfficeMobile '
ms.service: o365-administration
localization_priority: Normal
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
description: Tudnivalók a védelmi politika, amely segít a mobil eszközök az Office alkalmazások biztonságos hozzáférést.
ms.openlocfilehash: 75dbe79acccabd851c43259a165e79bfe3c509c0
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983185"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="ba24c-103">Office-dokumentumok felhasználói mobileszközökön történő elérésének felügyelete</span><span class="sxs-lookup"><span data-stu-id="ba24c-103">Manage how users access Office documents on mobile devices</span></span>

 <span data-ttu-id="ba24c-p101">Az Office-dokumentumok felhasználói mobileszközökön történő elérésének felügyeletét végző házirendek alapértelmezés szerint **Ki** értékre van állítva. Azt javasoljuk, hogy a telepítés során fogadja el azokat az alapértelmezett értékeket, amelyekkel minden felhasználóra vonatkozó alkalmazásházirendeket hozhat létre Android, iOS és Windows 10 rendszerekre. A telepítés után további házirendeket is létrehozhat majd.</span><span class="sxs-lookup"><span data-stu-id="ba24c-p101">Policy settings that control how users access Office files from their mobile devices are **Off** by default. We recommend you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users. You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="ba24c-107">Az Office-fájlok mobileszközökön való elérését szabályozó beállítások</span><span class="sxs-lookup"><span data-stu-id="ba24c-107">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="ba24c-108">Az alábbi beállítások használhatók a munkahelyi Office-fájlok elérésének kezelésére:</span><span class="sxs-lookup"><span data-stu-id="ba24c-108">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="ba24c-109">Beállítás</span><span class="sxs-lookup"><span data-stu-id="ba24c-109">Setting</span></span>  <br/> |<span data-ttu-id="ba24c-110">Leírás</span><span class="sxs-lookup"><span data-stu-id="ba24c-110">Description</span></span>  <br/> |
|<span data-ttu-id="ba24c-111">PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez</span><span class="sxs-lookup"><span data-stu-id="ba24c-111">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="ba24c-112">Ha ez a beállítás **Be** állapotban van, a mobileszközön lévő Office-appok használatához a felhasználónéven és a jelszón kívül a felhasználóknak további hitelesítési módszert is használniuk kell.</span><span class="sxs-lookup"><span data-stu-id="ba24c-112">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="ba24c-113">PIN-kód visszaállítása ennyi sikertelen bejelentkezési kísérlet után</span><span class="sxs-lookup"><span data-stu-id="ba24c-113">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="ba24c-114">Annak érdekében, hogy ne lehessen a PIN-kódot véletlenszerű próbálkozásokkal megfejteni, az Ön által megadott számú téves próbálkozás után a PIN-kód alaphelyzetbe áll.</span><span class="sxs-lookup"><span data-stu-id="ba24c-114">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="ba24c-115">A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után</span><span class="sxs-lookup"><span data-stu-id="ba24c-115">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="ba24c-116">Ezzel a beállítással azt határozhatja meg, hogy a felhasználó mennyi ideig maradhat inaktív, mielőtt újra be kellene jelentkeznie.</span><span class="sxs-lookup"><span data-stu-id="ba24c-116">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="ba24c-117">Hozzáférés letiltása a munkahelyi fájlokhoz a feltört vagy rootolással feltört eszközökön</span><span class="sxs-lookup"><span data-stu-id="ba24c-117">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="ba24c-p102">A hozzáértő felhasználók esetleg feltört vagy rootolással feltört eszközzel is rendelkezhetnek. Ez azt jelenti, hogy a felhasználó képes módosítani az operációs rendszert, ami sebezhetőbbé teheti az eszközt a kártevőkkel szemben. Ha ez a beállítás **Be** állapotban van, az ilyen eszközök le lesznek tiltva.  </span><span class="sxs-lookup"><span data-stu-id="ba24c-p102">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="ba24c-121">A felhasználók másolhatnak tartalmakat az Office-appokból személyes appokba</span><span class="sxs-lookup"><span data-stu-id="ba24c-121">Allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="ba24c-p103">Ez alapértelmezés szerint engedélyezve van, de ha a beállítás **Be** állapotban van, a felhasználó munkahelyi fájlból személyes fájlba másolhat adatot. Ha a beállítás **Ki** állapotban van, akkor a felhasználó nem másolhat adatot munkahelyi fájlból személyes alkalmazásba vagy személyes fiókba.  </span><span class="sxs-lookup"><span data-stu-id="ba24c-p103">We allow this by default, but when the setting is **On**, the user can copy information in a work file to a personal file. If the setting is **Off**, the user can't copy information from a work file to a personal app or personal account.  </span></span><br/> |
   


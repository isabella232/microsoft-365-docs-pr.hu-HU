---
title: Office-dokumentumok felhasználói mobileszközökön történő elérésének felügyelete
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: Ismerje meg a védelmi házirendeket, amelyek lehetővé teszik annak kezelését, hogy a felhasználók hogyan férnek hozzá Office alkalmazásokhoz és munkahelyi fájlokhoz mobileszközről.
ms.openlocfilehash: 7602b712f2dfc3ba369fd76979baaaa8d5da5c5c
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/14/2021
ms.locfileid: "52925279"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="024ee-103">Office-dokumentumok felhasználói mobileszközökön történő elérésének felügyelete</span><span class="sxs-lookup"><span data-stu-id="024ee-103">Manage how users access Office documents on mobile devices</span></span>

<span data-ttu-id="024ee-104">Ez a cikk a Microsoft 365 Vállalati prémium verzió.</span><span class="sxs-lookup"><span data-stu-id="024ee-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="024ee-105">Az Office-dokumentumok felhasználói mobileszközökön történő elérésének felügyeletét végző házirendek alapértelmezés szerint **Ki** értékre van állítva.</span><span class="sxs-lookup"><span data-stu-id="024ee-105">Policy settings that control how users access Office files from their mobile devices are **Off** by default.</span></span> <span data-ttu-id="024ee-106">Azt javasoljuk, hogy a telepítés során fogadja el az alapértelmezett értékeket az összes felhasználóra vonatkozó alkalmazás-házirendek létrehozásához androidos, iOS- Windows 10- és Windows 10 házirendek létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="024ee-106">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="024ee-107">A telepítés után további házirendeket is létrehozhat majd.</span><span class="sxs-lookup"><span data-stu-id="024ee-107">You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="024ee-108">Az Office-fájlok mobileszközökön történő elérésének felügyeletét meghatározó beállítások</span><span class="sxs-lookup"><span data-stu-id="024ee-108">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="024ee-109">Az alábbi beállítások használhatók a munkahelyi Office-fájlok elérésének kezelésére:</span><span class="sxs-lookup"><span data-stu-id="024ee-109">The following settings are available to manage how users access Office work files:</span></span>

|<span data-ttu-id="024ee-110">Beállítás</span><span class="sxs-lookup"><span data-stu-id="024ee-110">Setting</span></span>  <br/> |<span data-ttu-id="024ee-111">Leírás</span><span class="sxs-lookup"><span data-stu-id="024ee-111">Description</span></span>  <br/> |
|:-----|:-----|
|<span data-ttu-id="024ee-112">PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez</span><span class="sxs-lookup"><span data-stu-id="024ee-112">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="024ee-113">Ha ez a beállítás **Be,** a felhasználóknak a felhasználónéven és a jelszavukon kívül más hitelesítési módszert is meg kell adniuk, mielőtt Office a mobileszközükön.</span><span class="sxs-lookup"><span data-stu-id="024ee-113">If this setting is **On**, users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="024ee-114">PIN-kód visszaállítása ennyi sikertelen bejelentkezési kísérlet után</span><span class="sxs-lookup"><span data-stu-id="024ee-114">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="024ee-115">Annak érdekében, hogy ne lehessen a PIN-kódot véletlenszerű próbálkozásokkal megfejteni, az Ön által megadott számú téves próbálkozás után a PIN-kód alaphelyzetbe áll.</span><span class="sxs-lookup"><span data-stu-id="024ee-115">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="024ee-116">A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után</span><span class="sxs-lookup"><span data-stu-id="024ee-116">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="024ee-117">Ez a beállítás azt határozza meg, hogy a felhasználó mennyi ideig inaktív, mielőtt a rendszer ismét arra kéri, hogy jelentkezzen be.</span><span class="sxs-lookup"><span data-stu-id="024ee-117">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="024ee-118">Hozzáférés letiltása a munkahelyi fájlokhoz a feltört vagy rootolással feltört eszközökön</span><span class="sxs-lookup"><span data-stu-id="024ee-118">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="024ee-119">A hozzáértő felhasználók esetleg feltört vagy rootolással feltört eszközzel is rendelkezhetnek.</span><span class="sxs-lookup"><span data-stu-id="024ee-119">Clever users may have a device that is jailbroken or rooted.</span></span> <span data-ttu-id="024ee-120">Ez azt jelenti, hogy a felhasználó módosíthatja az operációs rendszert, így az eszköz érzékenyebb lehet a kártevőkre.</span><span class="sxs-lookup"><span data-stu-id="024ee-120">This means that the user can modify the operating system, which can make the device more susceptible to malware.</span></span> <span data-ttu-id="024ee-121">Ha ez a beállítás **Be** állapotban van, az ilyen eszközök le lesznek tiltva.</span><span class="sxs-lookup"><span data-stu-id="024ee-121">These devices are blocked when this setting is **On**.</span></span>  <br/> |
|<span data-ttu-id="024ee-122">Nem engedélyezem a felhasználóknak, hogy tartalmakat másoljanak Office-alkalmazásokból a személyes alkalmazásokba</span><span class="sxs-lookup"><span data-stu-id="024ee-122">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="024ee-123">Ha a beállítás **Be,** a felhasználó nem másolhat adatokat munkahelyi fájlból személyes fájlba.</span><span class="sxs-lookup"><span data-stu-id="024ee-123">When the setting is **On**, the user can't copy information in a work file to a personal file.</span></span> <span data-ttu-id="024ee-124">Ha a beállítás **Ki,** a felhasználó másolhat adatokat egy munkahelyi fájlból egy személyes appba vagy személyes fiókba.</span><span class="sxs-lookup"><span data-stu-id="024ee-124">If the setting is **Off**, the user can copy information from a work file to a personal app or personal account.</span></span>  <br/> |
   


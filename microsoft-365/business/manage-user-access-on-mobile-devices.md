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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: aa31319c-9196-48c9-a90b-4057e0494c7a
description: Ismerje meg a védelmi szabályzatokat, amelyek segítségével biztonságos hozzáférést biztosíthat nak az Office-alkalmazásokhoz mobileszközökről.
ms.openlocfilehash: 39d28a3a78fb06d0020c484b1782b544f6a8c656
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593821"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="33257-103">Office-dokumentumok felhasználói mobileszközökön történő elérésének felügyelete</span><span class="sxs-lookup"><span data-stu-id="33257-103">Manage how users access Office documents on mobile devices</span></span>

 <span data-ttu-id="33257-104">Az Office-dokumentumok felhasználói mobileszközökön történő elérésének felügyeletét végző házirendek alapértelmezés szerint **Ki** értékre van állítva.</span><span class="sxs-lookup"><span data-stu-id="33257-104">Policy settings that control how users access Office files from their mobile devices are **Off** by default.</span></span> <span data-ttu-id="33257-105">Azt javasoljuk, hogy a telepítés során fogadja el az alapértelmezett értékeket az Android, az iOS és a Windows 10 alkalmazásházirendjeinek létrehozásához, amelyek minden felhasználóra vonatkoznak.</span><span class="sxs-lookup"><span data-stu-id="33257-105">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="33257-106">A telepítés után további házirendeket is létrehozhat majd.</span><span class="sxs-lookup"><span data-stu-id="33257-106">You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="33257-107">Az Office-fájlok mobileszközökön történő elérésének felügyeletét meghatározó beállítások</span><span class="sxs-lookup"><span data-stu-id="33257-107">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="33257-108">Az alábbi beállítások használhatók a munkahelyi Office-fájlok elérésének kezelésére:</span><span class="sxs-lookup"><span data-stu-id="33257-108">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="33257-109">Beállítás</span><span class="sxs-lookup"><span data-stu-id="33257-109">Setting</span></span>  <br/> |<span data-ttu-id="33257-110">Leírás</span><span class="sxs-lookup"><span data-stu-id="33257-110">Description</span></span>  <br/> |
|<span data-ttu-id="33257-111">PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez</span><span class="sxs-lookup"><span data-stu-id="33257-111">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="33257-112">Ha ez a beállítás Be van **kapcsolva,** a felhasználóknak a felhasználónevükön és jelszavukon kívül más hitelesítési formát is meg kell adniuk ahhoz, hogy mobileszközükön használhassák az Office-alkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="33257-112">If this setting is **On**, users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="33257-113">PIN-kód visszaállítása ennyi sikertelen bejelentkezési kísérlet után</span><span class="sxs-lookup"><span data-stu-id="33257-113">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="33257-114">Annak érdekében, hogy ne lehessen a PIN-kódot véletlenszerű próbálkozásokkal megfejteni, az Ön által megadott számú téves próbálkozás után a PIN-kód alaphelyzetbe áll.</span><span class="sxs-lookup"><span data-stu-id="33257-114">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="33257-115">A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után</span><span class="sxs-lookup"><span data-stu-id="33257-115">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="33257-116">Ez a beállítás határozza meg, hogy a felhasználó mennyi ideig lehet tétlen, mielőtt a rendszer ismételten bejelentkezne.</span><span class="sxs-lookup"><span data-stu-id="33257-116">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="33257-117">Hozzáférés letiltása a munkahelyi fájlokhoz a feltört vagy rootolással feltört eszközökön</span><span class="sxs-lookup"><span data-stu-id="33257-117">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="33257-118">A hozzáértő felhasználók esetleg feltört vagy rootolással feltört eszközzel is rendelkezhetnek.</span><span class="sxs-lookup"><span data-stu-id="33257-118">Clever users may have a device that is jailbroken or rooted.</span></span> <span data-ttu-id="33257-119">Ez azt jelenti, hogy a felhasználó módosíthatja az operációs rendszert, ami az eszközt fogékonyabbá teheti a rosszindulatú programokra.</span><span class="sxs-lookup"><span data-stu-id="33257-119">This means that the user can modify the operating system, which can make the device more susceptible to malware.</span></span> <span data-ttu-id="33257-120">Ha ez a beállítás **Be** állapotban van, az ilyen eszközök le lesznek tiltva.</span><span class="sxs-lookup"><span data-stu-id="33257-120">These devices are blocked when this setting is **On**.</span></span>  <br/> |
|<span data-ttu-id="33257-121">Nem engedélyezze a felhasználóknak, hogy tartalmakat másoljanak az Office-alkalmazásokból személyes alkalmazásokba</span><span class="sxs-lookup"><span data-stu-id="33257-121">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="33257-122">Ha a beállítás Be van **kapcsolva,** a felhasználó nem másolhat át adatokat egy munkahelyi fájlban egy személyes fájlba.</span><span class="sxs-lookup"><span data-stu-id="33257-122">When the setting is **On**, the user can't copy information in a work file to a personal file.</span></span> <span data-ttu-id="33257-123">Ha a beállítás Ki van **kapcsolva,** a felhasználó átmásolhatja az adatokat egy munkahelyi fájlból egy személyes alkalmazásba vagy személyes fiókba.</span><span class="sxs-lookup"><span data-stu-id="33257-123">If the setting is **Off**, the user can copy information from a work file to a personal app or personal account.</span></span>  <br/> |
   


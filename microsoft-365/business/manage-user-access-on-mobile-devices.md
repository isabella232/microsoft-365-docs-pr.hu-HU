---
title: Office-dokumentumok felhasználói mobileszközökön történő elérésének felügyelete
ms.author: sirkkuw
author: sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: conceptual
f1_keywords:
- 'O365E_BCSSetup4OfficeMobile '
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
description: Tudnivalók a védelmi politika, amely segít a mobil eszközök az Office alkalmazások biztonságos hozzáférést.
ms.openlocfilehash: b77d30686b26f95de684238d1b9afd57550a7c7f
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32278609"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a>Office-dokumentumok felhasználói mobileszközökön történő elérésének felügyelete

 Az Office-dokumentumok felhasználói mobileszközökön történő elérésének felügyeletét végző házirendek alapértelmezés szerint **Ki** értékre van állítva. Azt javasoljuk, hogy a telepítés során fogadja el azokat az alapértelmezett értékeket, amelyekkel minden felhasználóra vonatkozó alkalmazásházirendeket hozhat létre Android, iOS és Windows 10 rendszerekre. A telepítés után további házirendeket is létrehozhat majd. 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Az Office-fájlok mobileszközökön történő elérésének felügyeletét meghatározó beállítások

Az alábbi beállítások használhatók a munkahelyi Office-fájlok elérésének kezelésére:
  
|||
|:-----|:-----|
|Beállítás  <br/> |Leírás  <br/> |
|PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez  <br/> |Ha ez a beállítás **Be** állapotban van, a mobileszközön lévő Office-appok használatához a felhasználónéven és a jelszón kívül a felhasználóknak további hitelesítési módszert is használniuk kell.  <br/> |
|PIN-kód visszaállítása ennyi sikertelen bejelentkezési kísérlet után  <br/> |Annak érdekében, hogy ne lehessen a PIN-kódot véletlenszerű próbálkozásokkal megfejteni, az Ön által megadott számú téves próbálkozás után a PIN-kód alaphelyzetbe áll.  <br/> |
|A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után  <br/> |Ezzel a beállítással azt határozhatja meg, hogy a felhasználó mennyi ideig maradhat inaktív, mielőtt újra be kellene jelentkeznie.  <br/> |
|Hozzáférés letiltása a munkahelyi fájlokhoz a feltört vagy rootolással feltört eszközökön  <br/> |A hozzáértő felhasználók esetleg feltört vagy rootolással feltört eszközzel is rendelkezhetnek. Ez azt jelenti, hogy a felhasználó módosíthatja az operációs rendszert, ami viszont kártevők által sebezhetőbbé teheti az eszközt. Ha ez a beállítás **Be** állapotban van, az ilyen eszközök le lesznek tiltva.  <br/> |
|A felhasználók másolhatnak tartalmakat az Office-appokból személyes appokba  <br/> |Ez alapértelmezés szerint engedélyezve van, de ha a beállítás **Be** állapotban van, a felhasználó munkahelyi fájlból személyes fájlba másolhat adatot. Ha a beállítás **Ki** állapotban van, akkor a felhasználó nem másolhat adatot munkahelyi fájlból személyes alkalmazásba vagy személyes fiókba.  <br/> |
   


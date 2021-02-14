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
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a>Office-dokumentumok felhasználói mobileszközökön történő elérésének felügyelete

Ez a cikk a Microsoft 365 Vállalati prémium verzióra vonatkozik.

Az Office-dokumentumok felhasználói mobileszközökön történő elérésének felügyeletét végző házirendek alapértelmezés szerint **Ki** értékre van állítva. Azt javasoljuk, hogy a telepítés során fogadja el az alapértelmezett értékeket az összes felhasználóra vonatkozó alkalmazás-házirendek létrehozásához Android, iOS és Windows 10 rendszeren. A telepítés után további házirendeket is létrehozhat majd. 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Az Office-fájlok mobileszközökön történő elérésének felügyeletét meghatározó beállítások

Az alábbi beállítások használhatók a munkahelyi Office-fájlok elérésének kezelésére:
  
|||
|:-----|:-----|
|Beállítás  <br/> |Leírás  <br/> |
|PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez  <br/> |Ha ez a beállítás **Be,** a felhasználóknak a felhasználónév és a jelszó mellett más hitelesítési módszert is meg kell adniuk ahhoz, hogy használni tudják az Office-appokat a mobileszközükön.  <br/> |
|PIN-kód visszaállítása ennyi sikertelen bejelentkezési kísérlet után  <br/> |Annak érdekében, hogy ne lehessen a PIN-kódot véletlenszerű próbálkozásokkal megfejteni, az Ön által megadott számú téves próbálkozás után a PIN-kód alaphelyzetbe áll.  <br/> |
|A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után  <br/> |Ez a beállítás azt határozza meg, hogy egy felhasználó mennyi ideig inaktív, mielőtt a rendszer ismét a bejelentkezésre kéri.  <br/> |
|Hozzáférés letiltása a munkahelyi fájlokhoz a feltört vagy rootolással feltört eszközökön  <br/> |A hozzáértő felhasználók esetleg feltört vagy rootolással feltört eszközzel is rendelkezhetnek. Ez azt jelenti, hogy a felhasználó módosíthatja az operációs rendszert, így az eszköz jobban ki van téve a kártevőknek. Ha ez a beállítás **Be** állapotban van, az ilyen eszközök le lesznek tiltva.  <br/> |
|Nem engedélyezi a felhasználóknak, hogy tartalmat másoljanak az Office-alkalmazásokból a személyes appokba  <br/> |Ha a beállítás **be van** va, a felhasználó nem másolhat adatokat munkahelyi fájlból személyes fájlba. Ha a beállítás ki **van** kapcsolva, a felhasználó átmásolhat adatokat egy munkahelyi fájlból egy személyes appba vagy személyes fiókba.  <br/> |
   


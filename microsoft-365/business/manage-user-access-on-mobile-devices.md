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
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a>Office-dokumentumok felhasználói mobileszközökön történő elérésének felügyelete

 Az Office-dokumentumok felhasználói mobileszközökön történő elérésének felügyeletét végző házirendek alapértelmezés szerint **Ki** értékre van állítva. Javasoljuk, hogy a telepítés során fogadja el az alapértelmezett értékeket, hogy az összes felhasználóra érvényes Android, iOS és Windows 10 alkalmazások házirendjeit hozza létre. A telepítés után további házirendeket is létrehozhat majd. 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Az Office-fájlok mobileszközökön történő elérésének felügyeletét meghatározó beállítások

Az alábbi beállítások használhatók a munkahelyi Office-fájlok elérésének kezelésére:
  
|||
|:-----|:-----|
|Beállítás  <br/> |Leírás  <br/> |
|PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez  <br/> |Ha ez a beállítás **be van kapcsolva**, akkor a felhasználóknak a felhasználónevükön és a jelszavuk mellett egy másik hitelesítési formát kell biztosítaniuk, mielőtt az Office alkalmazásokat mobileszközükön használhatják.  <br/> |
|PIN-kód visszaállítása ennyi sikertelen bejelentkezési kísérlet után  <br/> |Annak érdekében, hogy ne lehessen a PIN-kódot véletlenszerű próbálkozásokkal megfejteni, az Ön által megadott számú téves próbálkozás után a PIN-kód alaphelyzetbe áll.  <br/> |
|A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után  <br/> |Ez a beállítás határozza meg, hogy a felhasználók mennyi ideig lehetnek üresjáratban, mielőtt a rendszer újra bejelentkezne.  <br/> |
|Hozzáférés letiltása a munkahelyi fájlokhoz a feltört vagy rootolással feltört eszközökön  <br/> |A hozzáértő felhasználók esetleg feltört vagy rootolással feltört eszközzel is rendelkezhetnek. Ez azt jelenti, hogy a felhasználó módosíthatja az operációs rendszer, amely lehet, hogy az eszköz hajlamosabbak a malware. Ha ez a beállítás **Be** állapotban van, az ilyen eszközök le lesznek tiltva.  <br/> |
|A felhasználók nem másolnak tartalmat az Office alkalmazásokból a személyes alkalmazásba  <br/> |Ha a beállítás **be van kapcsolva**, a felhasználó nem másolhatja az adatokat egy munkahelyi fájlba egy személyes fájlba. Ha a beállítás **ki van kapcsolva**, a felhasználó átmásolhatja az adatokat egy munkahelyi fájlból egy személyes alkalmazásba vagy személyes fiókba.  <br/> |
   


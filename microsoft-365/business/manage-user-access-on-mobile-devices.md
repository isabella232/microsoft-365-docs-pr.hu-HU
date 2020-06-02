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
description: Ismerje meg azokat a védelmi irányelveket, amelyek lehetővé teszik annak kezelését, hogy a felhasználók hogyan férhetnek hozzá az Office-alkalmazásokhoz és a munkahelyi fájlokhoz mobileszközökről.
ms.openlocfilehash: b2b828cf2e201360f12b8fadcb395e72958230f6
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471067"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a>Office-dokumentumok felhasználói mobileszközökön történő elérésének felügyelete

Ez a cikk a Microsoft 365 Business Premium szolgáltatásra vonatkozik.

Az Office-dokumentumok felhasználói mobileszközökön történő elérésének felügyeletét végző házirendek alapértelmezés szerint **Ki** értékre van állítva. Azt javasoljuk, hogy a telepítés során fogadja el az alapértelmezett értékeket, és hozzon létre alkalmazásházirendeket Az Android, iOS és Windows 10, amelyek minden felhasználóra vonatkoznak. A telepítés után további házirendeket is létrehozhat majd. 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Az Office-fájlok mobileszközökön történő elérésének felügyeletét meghatározó beállítások

Az alábbi beállítások használhatók a munkahelyi Office-fájlok elérésének kezelésére:
  
|||
|:-----|:-----|
|Beállítás  <br/> |Leírás  <br/> |
|PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez  <br/> |Ha ez a beállítás **Be**beállítás, a felhasználóknak a felhasználónevükön és jelszavukon kívül más hitelesítési módot is meg kell adniuk, mielőtt mobileszközükön használhatnák az Office-alkalmazásokat.  <br/> |
|PIN-kód visszaállítása ennyi sikertelen bejelentkezési kísérlet után  <br/> |Annak érdekében, hogy ne lehessen a PIN-kódot véletlenszerű próbálkozásokkal megfejteni, az Ön által megadott számú téves próbálkozás után a PIN-kód alaphelyzetbe áll.  <br/> |
|A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után  <br/> |Ez a beállítás határozza meg, hogy a felhasználó mennyi ideig lehet tétlen, mielőtt a rendszer újra bejelentkezne.  <br/> |
|Hozzáférés letiltása a munkahelyi fájlokhoz a feltört vagy rootolással feltört eszközökön  <br/> |A hozzáértő felhasználók esetleg feltört vagy rootolással feltört eszközzel is rendelkezhetnek. Ez azt jelenti, hogy a felhasználó módosíthatja az operációs rendszert, amely az eszközt érzékenyebbé teheti a rosszindulatú programokra. Ha ez a beállítás **Be** állapotban van, az ilyen eszközök le lesznek tiltva.  <br/> |
|Ne engedélyezze a felhasználóknak, hogy tartalmat másoljanak az Office-alkalmazásokból személyes alkalmazásokba  <br/> |Ha a beállítás **Be**beállítás, a felhasználó nem másolhatja a munkafájladatait személyes fájlba. Ha a beállítás ki van **kapcsolva,** a felhasználó átmásolhatja az adatokat egy munkafájlból egy személyes alkalmazásba vagy személyes fiókba.  <br/> |
   


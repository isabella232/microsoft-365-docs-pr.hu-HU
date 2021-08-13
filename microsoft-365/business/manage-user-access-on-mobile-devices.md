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
ms.openlocfilehash: 6e48ef857de8046854a94d470b28ba5db96b373bc8b190dc1062d4f408a9802c
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53809252"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a>Office-dokumentumok felhasználói mobileszközökön történő elérésének felügyelete

Ez a cikk a Microsoft 365 Vállalati prémium verzió.

Az Office-dokumentumok felhasználói mobileszközökön történő elérésének felügyeletét végző házirendek alapértelmezés szerint **Ki** értékre van állítva. Azt javasoljuk, hogy a telepítés során fogadja el az alapértelmezett értékeket az összes felhasználóra vonatkozó alkalmazás-házirendek létrehozásához androidos, iOS- Windows 10- és Windows 10 házirendek létrehozásához. A telepítés után további házirendeket is létrehozhat majd. 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Az Office-fájlok mobileszközökön történő elérésének felügyeletét meghatározó beállítások

Az alábbi beállítások használhatók a munkahelyi Office-fájlok elérésének kezelésére:

|Beállítás  <br/> |Leírás  <br/> |
|:-----|:-----|
|PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez  <br/> |Ha ez a beállítás **Be,** a felhasználóknak a felhasználónéven és a jelszavukon kívül más hitelesítési módszert is meg kell adniuk, mielőtt Office a mobileszközükön.  <br/> |
|PIN-kód visszaállítása ennyi sikertelen bejelentkezési kísérlet után  <br/> |Annak érdekében, hogy ne lehessen a PIN-kódot véletlenszerű próbálkozásokkal megfejteni, az Ön által megadott számú téves próbálkozás után a PIN-kód alaphelyzetbe áll.  <br/> |
|A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után  <br/> |Ez a beállítás azt határozza meg, hogy a felhasználó mennyi ideig inaktív, mielőtt a rendszer ismét arra kéri, hogy jelentkezzen be.  <br/> |
|Hozzáférés letiltása a munkahelyi fájlokhoz a feltört vagy rootolással feltört eszközökön  <br/> |A hozzáértő felhasználók esetleg feltört vagy rootolással feltört eszközzel is rendelkezhetnek. Ez azt jelenti, hogy a felhasználó módosíthatja az operációs rendszert, így az eszköz érzékenyebb lehet a kártevőkre. Ha ez a beállítás **Be** állapotban van, az ilyen eszközök le lesznek tiltva.  <br/> |
|Nem engedélyezem a felhasználóknak, hogy tartalmakat másoljanak Office-alkalmazásokból a személyes alkalmazásokba  <br/> |Ha a beállítás **Be,** a felhasználó nem másolhat adatokat munkahelyi fájlból személyes fájlba. Ha a beállítás **Ki,** a felhasználó másolhat adatokat egy munkahelyi fájlból egy személyes appba vagy személyes fiókba.  <br/> |
   


---
title: Az AutoPilottal kapcsolatos eszközhibák elhárítása
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: troubleshooting
f1_keywords:
- ZTDTroubleshootDeviceErrors
- O365E_ZTDTroubleshootDeviceErrors
- BCS365_ZTDTroubleshootDeviceErrors
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: 'Útmutató: automata eszköz fájl hibáinak elhárítása.'
ms.openlocfilehash: 88b59ec20ddda401c1dac45ff729ac38497a767e
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/15/2019
ms.locfileid: "34074360"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Az AutoPilottal kapcsolatos eszközhibák elhárítása

## <a name="device-file-error-messages"></a>Eszköz fájl hibaüzenetek

Az alábbiakban tájékoztató a hibák jelenhetnek meg a Microsoft 365 üzleti automata eszköz fájlok használata közben. 
  
|**Hibakód:**|**Javításra**|
|:-----|:-----|
|Érvénytelen kérelemtörzset  <br/> |Ez a hiba csak ritkán, történjen, ha ez a hiba jelenik meg, ismételje meg a műveletet.  <br/> |
|Jellemző hardverujjlenyomat-értéket az eszköz nem megfelelő.  <br/> |Ha ez a hiba jelenik meg, az azt jelenti, hogy a CSV-fájlban, a rendszer a hardverujjlenyomatot az egyik eszköz a megadott érték nem helyes. Először ellenőrizze, hogy az érték helyesen írta-e. Ha úgy gondolja, hogy az értéke helyes-e, de ez a hiba továbbra is történik, kérjen segítséget a hardver forgalmazójához.  <br/> |
|Egy másik bérlő rendelt eszköz  <br/> |Ha ez a hiba jelenik meg, az azt jelenti, hogy a sorozatszám vagy egy vagy több eszközt, a termékkulcs a CSV-fájlban megadott érték nem megfelelő. Először ellenőrizze, hogy az érték helyesen írta-e. Ha úgy gondolja, hogy az értéke helyes-e, de ez a hiba továbbra is történik, kérjen segítséget a hardver forgalmazójához.  <br/> |
|A CSV-fájl érvénytelen sorozatszám vagy termékazonosító kulcsot tartalmaz  <br/> |Ha megjelenik ez a hiba azt jelenti, hogy az eszköz regisztrálja tyring már regisztrálva van egy másik szervezet által. Probléma megoldásához kérjen segítséget a hardver forgalmazójához.  <br/> |
|Ez az eszköz nem támogatott beállítás automata segítségével  <br/> | Ez a hiba azt jelenti, hogy az eszköz nem felel meg az automata telepítés követelményeinek. Az eszközöknek meg kell felelniük az alábbi követelményeknek:  <br/>  A Windows 10 rendszer 1703-as vagy újabb verzióját kell futtatniuk.  <br/>  Olyan új eszközöknek kell lenniük, amelyeken még nem használták a Windowst.  <br/> |
|Az eszköz nem található  <br/> |Ez a hiba azt jelenti, hogy egy vagy több eszközt a CSV-fájl nincs regisztrálva a szervezet számára. Probléma megoldásához kérjen segítséget a hardver forgalmazójához.  <br/> |
   

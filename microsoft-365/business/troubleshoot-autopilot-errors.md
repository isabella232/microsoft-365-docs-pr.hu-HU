---
title: Az AutoPilottal kapcsolatos eszközhibák elhárítása
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
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
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Megtudhatja, hogy miként háríthatja el azokat a hibákat, amelyek a Microsoft 365 Business Premium AutoPilot eszközfájljainak használata során jelenhetnek meg.
ms.openlocfilehash: 0c0742e5bf17c85cedfb421cabfd87c0e2184ba5
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/21/2020
ms.locfileid: "43635044"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Az AutoPilottal kapcsolatos eszközhibák elhárítása

## <a name="device-file-error-messages"></a>Eszközfájl-hibaüzenetek

Az alábbiakban információkat talál a Microsoft 365 Business Premium AutoPilot eszközfájljainak használata során előforduló hibákról. 
  
|**Hibakód**|**Fix kipróbálni**|
|:-----|:-----|
|Érvénytelen kérelemtörzs  <br/> |Ez a hiba ritkán fordulhat elő, ha ezt a hibát látja, próbálja meg újra a műveletet.  <br/> |
|Az eszköz hardverkivonat-értéke nem megfelelő.  <br/> |Ha ez a hiba jelenik meg, az azt jelenti, hogy a CSV-fájlban megadott érték az egyik eszköz hardverkivonatához nem megfelelő. Először ellenőrizze, hogy az érték helyesen lett-e bejelentve. Ha úgy gondolja, hogy az érték helyes, de ez a hiba továbbra is fennáll, kérjen segítséget a hardver gyártójától.  <br/> |
|Másik bérlőhöz rendelt eszköz  <br/> |Ha ez a hiba jelenik meg, az azt jelenti, hogy a CSV-fájlban megadott érték egy vagy több eszköz sorozatszáma vagy termékkulcsa nem megfelelő. Először ellenőrizze, hogy az érték helyesen lett-e bejelentve. Ha úgy gondolja, hogy az érték helyes, de ez a hiba továbbra is fennáll, kérjen segítséget a hardver gyártójától.  <br/> |
|A CSV-fájl érvénytelen sorozatszámot vagy termékkulcsot tartalmaz  <br/> |Ha ez a hiba jelenik meg, az azt jelenti, hogy a regisztrálni kívánt eszközt már regisztrálta egy másik szervezet. A hiba megoldásához kérjen segítséget a hardver forgalmazójához.  <br/> |
|Ez az eszköz nem támogatott az AutoPilot használatával történő beállításhoz  <br/> | Ez a hiba azt jelenti, hogy az eszköz nem felel meg az AutoPilot telepítési követelményeinek. Az eszközöknek meg kell felelniük az alábbi követelményeknek:  <br/>  A Windows 10 rendszer 1703-as vagy újabb verzióját kell futtatniuk.  <br/>  Új eszközök, amelyek nem mentik át a Windows beépített élményét.  <br/> |
|Az eszköz nem található  <br/> |Ez a hiba azt jelenti, hogy a CSV-fájlban lévő egy vagy több eszköz nincs regisztrálva a szervezetben. A probléma megoldásához kérjen segítséget a hardver forgalmazójához.  <br/> |

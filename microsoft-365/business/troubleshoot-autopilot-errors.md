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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Megtudhatja, hogy miként háríthatja el az AutoPilot-eszközfájlok használata közben a Microsoft 365 Vállalati prémium verzióban előforduló hibákat.
ms.openlocfilehash: bec5126696ee322db42e4b7c5cd8e0df485ab2c9
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403410"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Az AutoPilottal kapcsolatos eszközhibák elhárítása

## <a name="device-file-error-messages"></a>Eszközfájllal jelzett hibaüzenetek

Az alábbi információk az AutoPilot-eszközfájlok Használata közben a Microsoft 365 Vállalati prémium verzióban előforduló hibák némelyikével kapcsolatosak. 
  
|**Hibakód**|**Javítás a kipróbálható megoldáshoz**|
|:-----|:-----|
|Érvénytelen kérés törzse  <br/> |Ez a hiba ritkán fordul elő, ha ezt a hibaüzenetet látja, próbálkozzon újra a művelettel.  <br/> |
|Az eszköz hardveres kivonatértéke nem helyes.  <br/> |Ha ez a hibaüzenet jelenik meg, az azt jelenti, hogy az egyik eszköz hardveres kivonatának CSV-fájljában megadott érték helytelen. Először ellenőrizze, hogy az érték helyesen lett-e begépelve. Ha úgy gondolja, hogy az érték helyes, de ez a hiba továbbra is megtörténik, kérjen segítséget a hardvergyártótól.  <br/> |
|Másik bérlőhöz rendelt eszköz  <br/> |Ha ez a hibaüzenet jelenik meg, az azt jelenti, hogy a CSV-fájlban egy vagy több eszköz sorozatszámához vagy termékkulcsához megadott érték helytelen. Először ellenőrizze, hogy az érték helyesen lett-e begépelve. Ha úgy gondolja, hogy az érték helyes, de ez a hiba továbbra is megtörténik, kérjen segítséget a hardvergyártótól.  <br/> |
|A CSV-fájl érvénytelen sorozatszámot vagy termékkulcsot tartalmaz  <br/> |Ha ez a hibaüzenet jelenik meg, az azt jelenti, hogy a regisztrálni próbált eszközt már regisztrálta egy másik szervezet. A hiba kijavíthatja, ha segítségért a hardvergyártótól kér segítséget.  <br/> |
|Ez az eszköz nem támogatott az AutoPilot használatával való beállításhoz  <br/> | Ez a hiba azt jelenti, hogy az eszköz nem felel meg az AutoPilot telepítési követelményeinek. Az eszközöknek meg kell felelniük az alábbi követelményeknek:  <br/>  A Windows 10 rendszer 1703-as vagy újabb verzióját kell futtatniuk.  <br/>  Új eszközök, amelyek még nem voltak használhatók a Windows rendszerben.  <br/> |
|Az eszköz nem található  <br/> |Ez a hiba azt jelenti, hogy a CSV-fájlban található egy vagy több eszköz nincs regisztrálva a szervezetben. A probléma megoldáshoz kérje a hardvergyártó segítségét.  <br/> |

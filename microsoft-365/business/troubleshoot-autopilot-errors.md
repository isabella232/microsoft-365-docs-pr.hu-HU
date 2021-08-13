---
title: Az AutoPilottal kapcsolatos eszközhibák elhárítása
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: Ebből a cikkből megtudhatja, hogy miként háríthatja el az AutoPilot-eszközfájlok használata közben a Microsoft 365 Vállalati prémium verzió.
ms.openlocfilehash: b74c57acbaa5682f6db97e7d8a090e6e28a40dcc3246f00cacc7984cb52cc758
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53809180"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Az AutoPilottal kapcsolatos eszközhibák elhárítása

## <a name="device-file-error-messages"></a>Eszközfájllal jelzett hibaüzenetek

Az itt található információk az AutoPilot-eszközfájlok használata közben a Microsoft 365 Vállalati prémium verzió. 
  
|**Hibakód**|**Javítás a kipróbálható megoldáshoz**|
|:-----|:-----|
|Érvénytelen kérés törzse  <br/> |Ez a hiba ritkán fordul elő, ha ezt a hibaüzenetet látja, próbálkozzon újra a művelettel.  <br/> |
|Az eszköz hardveres kivonatértéke nem helyes.  <br/> |Ha ez a hibaüzenet jelenik meg, az azt jelenti, hogy az egyik eszköz hardveres kivonata esetén a CSV-fájlban megadott érték helytelen. Először ellenőrizze, hogy az érték helyesen lett-e begépelve. Ha úgy gondolja, hogy az érték helyes, de ez a hiba még mindig megtörténik, kérjen segítséget a hardvergyártójától.  <br/> |
|Másik bérlőhöz rendelt eszköz  <br/> |Ha ez a hibaüzenet jelenik meg, az azt jelenti, hogy a CSV-fájlban egy vagy több eszköz sorozatszámához vagy termékkulcsához megadott érték helytelen. Először ellenőrizze, hogy az érték helyesen lett-e begépelve. Ha úgy gondolja, hogy az érték helyes, de ez a hiba még mindig megtörténik, kérjen segítséget a hardvergyártójától.  <br/> |
|A CSV-fájl érvénytelen sorozatszámot vagy termékkulcsot tartalmaz  <br/> |Ha ez a hibaüzenet jelenik meg, az azt jelenti, hogy a regisztrálni próbált eszközt egy másik szervezet már regisztrálta. A hiba kijavít ehhez a hardvergyártótól tud segítséget kérni.  <br/> |
|Ez az eszköz nem támogatott az AutoPilot használatával való beállításhoz  <br/> | Ez a hiba azt jelzi, hogy az eszköz nem felel meg az AutoPilot telepítési követelményeinek. Az eszközöknek meg kell felelniük az alábbi követelményeknek:  <br/>  A Windows 10 rendszer 1703-as vagy újabb verzióját kell futtatniuk.  <br/>  Olyan új eszközök, amelyek még nem Windows nem voltak bevetve.  <br/> |
|Az eszköz nem található  <br/> |Ez a hiba azt jelzi, hogy a CSV-fájlban található egy vagy több eszköz nincs regisztrálva a szervezetéhez. A hiba kijavít ehhez a hardvergyártótól tud segítséget kérni.  <br/> |

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
description: Útmutató az eszköz-fájlhibák automatikus vezérléssel kapcsolatos hibaelhárításához.
ms.openlocfilehash: 1b5358bd6686c2548e82ec5297ac0ad675835718
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38718699"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Az AutoPilottal kapcsolatos eszközhibák elhárítása

## <a name="device-file-error-messages"></a>Eszközfájl hibaüzenetei

Eretnekségek ' értesít-ra néhány hiba ön erő lát rövid idő működő-val robotpilóta berendezés fájlokat-ban Mikroszkóp 365 teendő. 
  
|**Hibakód**|**Erősít-hoz megpróbál**|
|:-----|:-----|
|Érvénytelen kérelemtörzs  <br/> |Ez a hiba ritkán, ha látja ezt a hibát, próbálkozzon újra a művelettel.  <br/> |
|Az eszköz hardverujjlenyomat-értéke nem megfelelő.  <br/> |Ha ezt a hibát látja, az azt jelenti, hogy az egyik eszköz hardveres kivonatának a CSV-fájlban megadott értéke nem megfelelő. Először ellenőrizze, hogy helyesen írta-e be az értéket. Ha úgy gondolja, hogy az érték helyes, de ez a hiba még mindig történik, kérje a hardver forgalmazójától a segítséget.  <br/> |
|Másik bérlőre rendelt eszköz  <br/> |Ha ezt a hibát látja, az azt jelenti, hogy a CSV-fájlban a sorozatszám vagy egy vagy több eszköz termékkulcsa számára megadott érték nem megfelelő. Először ellenőrizze, hogy helyesen írta-e be az értéket. Ha úgy gondolja, hogy az érték helyes, de ez a hiba még mindig történik, kérje a hardver forgalmazójától a segítséget.  <br/> |
|A CSV-fájl érvénytelen sorozatszámot vagy termékkulcsot tartalmaz.  <br/> |Ha ezt a hibát látja, az azt jelenti, hogy a regisztrálni próbált eszközt egy másik szervezet már regisztrálta. A hiba kijavításához kérjen segítséget a hardver forgalmazójától.  <br/> |
|Az eszközt nem támogatja a telepítő a robotpilóta használatával  <br/> | Ez a hiba azt jelenti, hogy az eszköz nem felel meg a robotpilóta telepítési követelményeinek. Az eszközöknek meg kell felelniük az alábbi követelményeknek:  <br/>  A Windows 10 rendszer 1703-as vagy újabb verzióját kell futtatniuk.  <br/>  Új berendezés amit kikötő ' átmenő Windows ki--ból-doboz tapasztalat.  <br/> |
|Az eszköz nem található  <br/> |Ez a hiba azt jelenti, hogy a CSV-fájlban lévő egy vagy több eszköz nem szerepel a szervezetben. A kijavításához kérjen segítséget a hardver forgalmazójától.  <br/> |

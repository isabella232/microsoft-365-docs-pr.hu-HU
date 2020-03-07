---
title: Az AutoPilottal kapcsolatos eszközhibák elhárítása
f1.keywords:
- NOCSH
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
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Megtudhatja, hogy miként háríthatja el az AutoPilot eszközfájljainak használata során a Microsoft 365 Vállalati verzióban előforduló hibákat.
ms.openlocfilehash: dc1abd508156c8525859f6ca7e291ab38fc8859c
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/07/2020
ms.locfileid: "42560700"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Az AutoPilottal kapcsolatos eszközhibák elhárítása

## <a name="device-file-error-messages"></a>Eszközfájl-hibaüzenetek

Az alábbiakban az AutoPilot eszközfájlokkal végzett munka során a Microsoft 365 Business ben előforduló hibákról olvashat. 
  
|**Hibakód**|**Javítás a kipróbáláshoz**|
|:-----|:-----|
|Érvénytelen kérelemtörzs  <br/> |Ez a hiba ritkán fordulhat elő, ha ez a hiba jelenik meg, próbálkozzon újra a művelettel.  <br/> |
|Az eszköz hardverkivonat-értéke nem megfelelő.  <br/> |Ha ez a hiba jelenik meg, az azt jelenti, hogy a CSV-fájlban megadott érték az egyik eszköz hardverkivonatához nem megfelelő. Először ellenőrizze, hogy helyesen írta-e be az értéket. Ha úgy gondolja, hogy az érték helyes, de ez a hiba továbbra is fennáll, kérjen segítséget a hardver gyártójától.  <br/> |
|Másik bérlőhöz rendelt eszköz  <br/> |Ha ez a hiba jelenik meg, az azt jelenti, hogy a CSV-fájlban megadott érték vagy a sorozatszám, vagy egy vagy több eszköz termékkulcsa nem megfelelő. Először ellenőrizze, hogy helyesen írta-e be az értéket. Ha úgy gondolja, hogy az érték helyes, de ez a hiba továbbra is fennáll, kérjen segítséget a hardver gyártójától.  <br/> |
|A CSV-fájl érvénytelen sorozatszámot vagy termékkulcsot tartalmaz  <br/> |Ha ez a hiba jelenik meg, az azt jelenti, hogy a regisztrálni kívánt eszközt már regisztrálta egy másik szervezet. A hiba megoldásához kérjen segítséget a hardver gyártójától.  <br/> |
|Ez az eszköz nem támogatott az AutoPilot használatával történő telepítéshez  <br/> | Ez a hiba azt jelenti, hogy az eszköz nem felel meg az AutoPilot telepítési követelményeinek. Az eszközöknek meg kell felelniük az alábbi követelményeknek:  <br/>  A Windows 10 rendszer 1703-as vagy újabb verzióját kell futtatniuk.  <br/>  Új eszközök, amelyek nem voltak a Windows beépített élményén.  <br/> |
|Az eszköz nem található  <br/> |Ez a hiba azt jelenti, hogy a CSV-fájl egy vagy több eszköze nincs regisztrálva a szervezetben. A probléma megoldásához kérjen segítséget a hardver gyártójától.  <br/> |

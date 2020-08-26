---
title: Windows 10-es eszközök védelme
f1.keywords:
- CSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_BCSSetup4WindowsConfig
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 21e5551f-fa35-4f13-9418-f80d668b6a2b
description: Megtudhatja, hogy miként konfigurálhatja az alapértelmezett eszköz-házirend beállításait, amelyet bármely Windows 10-es eszköz kap a munkahelyi vagy iskolai fiókjába való bejelentkezéskor.
ms.openlocfilehash: b586e687d6b61873b77fac8586396ab51fd90b9b
ms.sourcegitcommit: 90efec455336b4cecc06a8cbf0ce287740433523
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/26/2020
ms.locfileid: "46898068"
---
# <a name="secure-windows-10-devices"></a>Windows 10-es eszközök védelme

Ez a cikk a Microsoft 365 vállalati prémium verzióra vonatkozik.

Az itt megadott beállítások a Windows 10-es eszközökre vonatkozó alapértelmezett eszközházirend részei lesznek. Azok a felhasználók, akik a saját munkahelyi fiókjával együtt csatlakoznak a Windows 10-es eszközökhöz, például mobileszközökön és PC-k, automatikusan megkapják ezeket a beállításokat. Azt javasoljuk, hogy a telepítés során az alapértelmezett házirendet fogadja el, az egyes felhasználói csoportokra vonatkozó házirendeket pedig a telepítés után adja hozzá.
  
## <a name="settings-to-secure-windows-10-devices"></a>Windows 10-es eszközök biztonságára vonatkozó beállítások

Alapértelmezés szerint minden beállítás **Be** állapotban van. Az alábbi beállítások érhetők el:
  
|||
|:-----|:-----|
|Beállítás  <br/> |Leírás  <br/> |
|PC-k védelme a vírusokkal és más fenyegetésekkel szemben a Windows Defender víruskereső használatával  <br/> |Használatához a Windows Defender víruskeresőnek bekapcsolt állapotban kell lennie, hogy a PC-ket védeni lehessen az internetes kapcsolat során előforduló fenyegetésekkel szemben.  <br/> |
|PC-k védelme a webes fenyegetésekkel szemben a Microsoft Edge böngészőben  <br/> |Bekapcsolja a Microsoft Edge böngészőben azokat a beállításokat, amelyek segítenek megvédeni a felhasználót a kártékony webhelyek és letöltések által okozott veszélyektől.  <br/> |
|Az eszköz képernyőjének kikapcsolása ennyi üresjárati idő után  <br/> |Biztosítja a céges adatok védelmét, amikor a felhasználó inaktív. Előfordulhat, hogy a felhasználó nyilvános helyen, például egy kávézóban végez munkát, és ilyenkor ha csak rövid időre is elvonják a figyelmét az eszközről, akkor annak kijelzőjét illetéktelen személyek is láthatják. Ezzel a beállítással azt határozhatja meg, hogy a felhasználó mennyi ideig maradhat inaktív, mielőtt az eszköz kijelzője kikapcsol.  <br/> |
|A felhasználók letölthetnek appokat innen: Microsoft Áruház  <br/> |Lehetővé teszi, hogy a felhasználók appokat tölthessenek le és telepíthessenek a Microsoft Áruházból. Az appok között játékok és munkára használható eszközök egyaránt lehetnek, ezért ez a beállítás **Be** állapotban van, de a fokozott biztonság érdekében ki is kapcsolhatja.  <br/> |
|
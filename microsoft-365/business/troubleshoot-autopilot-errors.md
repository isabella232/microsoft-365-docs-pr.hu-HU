---
title: Az AutoPilottal kapcsolatos eszközhibák elhárítása
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: troubleshooting
f1_keywords:
- ZTDTroubleshootDeviceErrors
- O365E_ZTDTroubleshootDeviceErrors
- BCS365_ZTDTroubleshootDeviceErrors
ms.service: o365-administration
localization_priority: Normal
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
ms.openlocfilehash: 9b8d8ab424dd3189ff5c228dab8f5c513ff5dafc
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982745"
---
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="586be-103">Az AutoPilottal kapcsolatos eszközhibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="586be-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="586be-104">Eszköz fájl hibaüzenetek</span><span class="sxs-lookup"><span data-stu-id="586be-104">Device file error messages</span></span>

<span data-ttu-id="586be-105">Az alábbiakban tájékoztató a hibák jelenhetnek meg a Microsoft 365 üzleti automata eszköz fájlok használata közben.</span><span class="sxs-lookup"><span data-stu-id="586be-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business.</span></span> 
  
|<span data-ttu-id="586be-106">**Hibakód:**</span><span class="sxs-lookup"><span data-stu-id="586be-106">**Error code**</span></span>|<span data-ttu-id="586be-107">**Javításra**</span><span class="sxs-lookup"><span data-stu-id="586be-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="586be-108">Érvénytelen kérelemtörzset</span><span class="sxs-lookup"><span data-stu-id="586be-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="586be-109">Ez a hiba csak ritkán, történjen, ha ez a hiba jelenik meg, ismételje meg a műveletet.</span><span class="sxs-lookup"><span data-stu-id="586be-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="586be-110">Jellemző hardverujjlenyomat-értéket az eszköz nem megfelelő.</span><span class="sxs-lookup"><span data-stu-id="586be-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="586be-p101">Ha ez a hiba jelenik meg, az azt jelenti, hogy a CSV-fájlban, a rendszer a hardverujjlenyomatot az egyik eszköz a megadott érték nem helyes. Először ellenőrizze, hogy az érték helyesen írta-e. Ha úgy gondolja, hogy az értéke helyes-e, de ez a hiba továbbra is történik, kérjen segítséget a hardver forgalmazójához.</span><span class="sxs-lookup"><span data-stu-id="586be-p101">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct. First, verify that the value was typed correctly. If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="586be-114">Egy másik bérlő rendelt eszköz</span><span class="sxs-lookup"><span data-stu-id="586be-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="586be-p102">Ha ez a hiba jelenik meg, az azt jelenti, hogy a sorozatszám vagy egy vagy több eszközt, a termékkulcs a CSV-fájlban megadott érték nem megfelelő. Először ellenőrizze, hogy az érték helyesen írta-e. Ha úgy gondolja, hogy az értéke helyes-e, de ez a hiba továbbra is történik, kérjen segítséget a hardver forgalmazójához.</span><span class="sxs-lookup"><span data-stu-id="586be-p102">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct. First, verify that the value was typed correctly. If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="586be-118">A CSV-fájl érvénytelen sorozatszám vagy termékazonosító kulcsot tartalmaz</span><span class="sxs-lookup"><span data-stu-id="586be-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="586be-p103">Ha megjelenik ez a hiba azt jelenti, hogy az eszköz regisztrálja tyring már regisztrálva van egy másik szervezet által. Probléma megoldásához kérjen segítséget a hardver forgalmazójához.</span><span class="sxs-lookup"><span data-stu-id="586be-p103">If you see this error it means that the device you are tyring to register is already registered by an other organization. To fix this, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="586be-121">Ez az eszköz nem támogatott beállítás automata segítségével</span><span class="sxs-lookup"><span data-stu-id="586be-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="586be-p104">Ez a hiba azt jelenti, hogy az eszköz nem felel meg az automata telepítés követelményeinek. Eszközöket kell megfelelni ezeknek a követelményeknek:</span><span class="sxs-lookup"><span data-stu-id="586be-p104">This error means the device does not meet AutoPilot deployment requirements. Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="586be-124">A Windows 10 rendszer 1703-as vagy újabb verzióját kell futtatniuk.</span><span class="sxs-lookup"><span data-stu-id="586be-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="586be-125">Olyan új eszközöknek kell lenniük, amelyeken még nem használták a Windowst.</span><span class="sxs-lookup"><span data-stu-id="586be-125">New devices that have not been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="586be-126">Az eszköz nem található</span><span class="sxs-lookup"><span data-stu-id="586be-126">Device not found</span></span>  <br/> |<span data-ttu-id="586be-p105">Ez a hiba azt jelenti, hogy egy vagy több eszközt a CSV-fájl nincs regisztrálva a szervezet számára. Probléma megoldásához kérjen segítséget a hardver forgalmazójához.</span><span class="sxs-lookup"><span data-stu-id="586be-p105">This error means that one or more devices in your CSV file is not registered to your organization. To fix this, ask your hardware vendor for help.</span></span>  <br/> |
   

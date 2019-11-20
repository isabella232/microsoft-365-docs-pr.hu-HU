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
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="782d2-103">Az AutoPilottal kapcsolatos eszközhibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="782d2-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="782d2-104">Eszközfájl hibaüzenetei</span><span class="sxs-lookup"><span data-stu-id="782d2-104">Device file error messages</span></span>

<span data-ttu-id="782d2-105">Eretnekségek ' értesít-ra néhány hiba ön erő lát rövid idő működő-val robotpilóta berendezés fájlokat-ban Mikroszkóp 365 teendő.</span><span class="sxs-lookup"><span data-stu-id="782d2-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business.</span></span> 
  
|<span data-ttu-id="782d2-106">**Hibakód**</span><span class="sxs-lookup"><span data-stu-id="782d2-106">**Error code**</span></span>|<span data-ttu-id="782d2-107">**Erősít-hoz megpróbál**</span><span class="sxs-lookup"><span data-stu-id="782d2-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="782d2-108">Érvénytelen kérelemtörzs</span><span class="sxs-lookup"><span data-stu-id="782d2-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="782d2-109">Ez a hiba ritkán, ha látja ezt a hibát, próbálkozzon újra a művelettel.</span><span class="sxs-lookup"><span data-stu-id="782d2-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="782d2-110">Az eszköz hardverujjlenyomat-értéke nem megfelelő.</span><span class="sxs-lookup"><span data-stu-id="782d2-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="782d2-111">Ha ezt a hibát látja, az azt jelenti, hogy az egyik eszköz hardveres kivonatának a CSV-fájlban megadott értéke nem megfelelő.</span><span class="sxs-lookup"><span data-stu-id="782d2-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="782d2-112">Először ellenőrizze, hogy helyesen írta-e be az értéket.</span><span class="sxs-lookup"><span data-stu-id="782d2-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="782d2-113">Ha úgy gondolja, hogy az érték helyes, de ez a hiba még mindig történik, kérje a hardver forgalmazójától a segítséget.</span><span class="sxs-lookup"><span data-stu-id="782d2-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="782d2-114">Másik bérlőre rendelt eszköz</span><span class="sxs-lookup"><span data-stu-id="782d2-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="782d2-115">Ha ezt a hibát látja, az azt jelenti, hogy a CSV-fájlban a sorozatszám vagy egy vagy több eszköz termékkulcsa számára megadott érték nem megfelelő.</span><span class="sxs-lookup"><span data-stu-id="782d2-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="782d2-116">Először ellenőrizze, hogy helyesen írta-e be az értéket.</span><span class="sxs-lookup"><span data-stu-id="782d2-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="782d2-117">Ha úgy gondolja, hogy az érték helyes, de ez a hiba még mindig történik, kérje a hardver forgalmazójától a segítséget.</span><span class="sxs-lookup"><span data-stu-id="782d2-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="782d2-118">A CSV-fájl érvénytelen sorozatszámot vagy termékkulcsot tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="782d2-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="782d2-119">Ha ezt a hibát látja, az azt jelenti, hogy a regisztrálni próbált eszközt egy másik szervezet már regisztrálta.</span><span class="sxs-lookup"><span data-stu-id="782d2-119">If you see this error, it means that the device you are trying to register is already registered by another organization.</span></span> <span data-ttu-id="782d2-120">A hiba kijavításához kérjen segítséget a hardver forgalmazójától.</span><span class="sxs-lookup"><span data-stu-id="782d2-120">To fix this error, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="782d2-121">Az eszközt nem támogatja a telepítő a robotpilóta használatával</span><span class="sxs-lookup"><span data-stu-id="782d2-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="782d2-122">Ez a hiba azt jelenti, hogy az eszköz nem felel meg a robotpilóta telepítési követelményeinek.</span><span class="sxs-lookup"><span data-stu-id="782d2-122">This error means the device doesn't meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="782d2-123">Az eszközöknek meg kell felelniük az alábbi követelményeknek:</span><span class="sxs-lookup"><span data-stu-id="782d2-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="782d2-124">A Windows 10 rendszer 1703-as vagy újabb verzióját kell futtatniuk.</span><span class="sxs-lookup"><span data-stu-id="782d2-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="782d2-125">Új berendezés amit kikötő ' átmenő Windows ki--ból-doboz tapasztalat.</span><span class="sxs-lookup"><span data-stu-id="782d2-125">New devices that haven't been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="782d2-126">Az eszköz nem található</span><span class="sxs-lookup"><span data-stu-id="782d2-126">Device not found</span></span>  <br/> |<span data-ttu-id="782d2-127">Ez a hiba azt jelenti, hogy a CSV-fájlban lévő egy vagy több eszköz nem szerepel a szervezetben.</span><span class="sxs-lookup"><span data-stu-id="782d2-127">This error means that one or more devices in your CSV file isn't registered to your organization.</span></span> <span data-ttu-id="782d2-128">A kijavításához kérjen segítséget a hardver forgalmazójától.</span><span class="sxs-lookup"><span data-stu-id="782d2-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |

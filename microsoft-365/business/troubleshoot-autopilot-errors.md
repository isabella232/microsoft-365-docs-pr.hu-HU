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
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="3ccaf-103">Az AutoPilottal kapcsolatos eszközhibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="3ccaf-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="3ccaf-104">Eszközfájllal jelzett hibaüzenetek</span><span class="sxs-lookup"><span data-stu-id="3ccaf-104">Device file error messages</span></span>

<span data-ttu-id="3ccaf-105">Az alábbi információk az AutoPilot-eszközfájlok Használata közben a Microsoft 365 Vállalati prémium verzióban előforduló hibák némelyikével kapcsolatosak.</span><span class="sxs-lookup"><span data-stu-id="3ccaf-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business Premium.</span></span> 
  
|<span data-ttu-id="3ccaf-106">**Hibakód**</span><span class="sxs-lookup"><span data-stu-id="3ccaf-106">**Error code**</span></span>|<span data-ttu-id="3ccaf-107">**Javítás a kipróbálható megoldáshoz**</span><span class="sxs-lookup"><span data-stu-id="3ccaf-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3ccaf-108">Érvénytelen kérés törzse</span><span class="sxs-lookup"><span data-stu-id="3ccaf-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="3ccaf-109">Ez a hiba ritkán fordul elő, ha ezt a hibaüzenetet látja, próbálkozzon újra a művelettel.</span><span class="sxs-lookup"><span data-stu-id="3ccaf-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="3ccaf-110">Az eszköz hardveres kivonatértéke nem helyes.</span><span class="sxs-lookup"><span data-stu-id="3ccaf-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="3ccaf-111">Ha ez a hibaüzenet jelenik meg, az azt jelenti, hogy az egyik eszköz hardveres kivonatának CSV-fájljában megadott érték helytelen.</span><span class="sxs-lookup"><span data-stu-id="3ccaf-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="3ccaf-112">Először ellenőrizze, hogy az érték helyesen lett-e begépelve.</span><span class="sxs-lookup"><span data-stu-id="3ccaf-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="3ccaf-113">Ha úgy gondolja, hogy az érték helyes, de ez a hiba továbbra is megtörténik, kérjen segítséget a hardvergyártótól.</span><span class="sxs-lookup"><span data-stu-id="3ccaf-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="3ccaf-114">Másik bérlőhöz rendelt eszköz</span><span class="sxs-lookup"><span data-stu-id="3ccaf-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="3ccaf-115">Ha ez a hibaüzenet jelenik meg, az azt jelenti, hogy a CSV-fájlban egy vagy több eszköz sorozatszámához vagy termékkulcsához megadott érték helytelen.</span><span class="sxs-lookup"><span data-stu-id="3ccaf-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="3ccaf-116">Először ellenőrizze, hogy az érték helyesen lett-e begépelve.</span><span class="sxs-lookup"><span data-stu-id="3ccaf-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="3ccaf-117">Ha úgy gondolja, hogy az érték helyes, de ez a hiba továbbra is megtörténik, kérjen segítséget a hardvergyártótól.</span><span class="sxs-lookup"><span data-stu-id="3ccaf-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="3ccaf-118">A CSV-fájl érvénytelen sorozatszámot vagy termékkulcsot tartalmaz</span><span class="sxs-lookup"><span data-stu-id="3ccaf-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="3ccaf-119">Ha ez a hibaüzenet jelenik meg, az azt jelenti, hogy a regisztrálni próbált eszközt már regisztrálta egy másik szervezet.</span><span class="sxs-lookup"><span data-stu-id="3ccaf-119">If you see this error, it means that the device you are trying to register is already registered by another organization.</span></span> <span data-ttu-id="3ccaf-120">A hiba kijavíthatja, ha segítségért a hardvergyártótól kér segítséget.</span><span class="sxs-lookup"><span data-stu-id="3ccaf-120">To fix this error, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="3ccaf-121">Ez az eszköz nem támogatott az AutoPilot használatával való beállításhoz</span><span class="sxs-lookup"><span data-stu-id="3ccaf-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="3ccaf-122">Ez a hiba azt jelenti, hogy az eszköz nem felel meg az AutoPilot telepítési követelményeinek.</span><span class="sxs-lookup"><span data-stu-id="3ccaf-122">This error means the device doesn't meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="3ccaf-123">Az eszközöknek meg kell felelniük az alábbi követelményeknek:</span><span class="sxs-lookup"><span data-stu-id="3ccaf-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="3ccaf-124">A Windows 10 rendszer 1703-as vagy újabb verzióját kell futtatniuk.</span><span class="sxs-lookup"><span data-stu-id="3ccaf-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="3ccaf-125">Új eszközök, amelyek még nem voltak használhatók a Windows rendszerben.</span><span class="sxs-lookup"><span data-stu-id="3ccaf-125">New devices that haven't been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="3ccaf-126">Az eszköz nem található</span><span class="sxs-lookup"><span data-stu-id="3ccaf-126">Device not found</span></span>  <br/> |<span data-ttu-id="3ccaf-127">Ez a hiba azt jelenti, hogy a CSV-fájlban található egy vagy több eszköz nincs regisztrálva a szervezetben.</span><span class="sxs-lookup"><span data-stu-id="3ccaf-127">This error means that one or more devices in your CSV file isn't registered to your organization.</span></span> <span data-ttu-id="3ccaf-128">A probléma megoldáshoz kérje a hardvergyártó segítségét.</span><span class="sxs-lookup"><span data-stu-id="3ccaf-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |

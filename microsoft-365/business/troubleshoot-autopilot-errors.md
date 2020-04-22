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
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="28cd1-103">Az AutoPilottal kapcsolatos eszközhibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="28cd1-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="28cd1-104">Eszközfájl-hibaüzenetek</span><span class="sxs-lookup"><span data-stu-id="28cd1-104">Device file error messages</span></span>

<span data-ttu-id="28cd1-105">Az alábbiakban információkat talál a Microsoft 365 Business Premium AutoPilot eszközfájljainak használata során előforduló hibákról.</span><span class="sxs-lookup"><span data-stu-id="28cd1-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business Premium.</span></span> 
  
|<span data-ttu-id="28cd1-106">**Hibakód**</span><span class="sxs-lookup"><span data-stu-id="28cd1-106">**Error code**</span></span>|<span data-ttu-id="28cd1-107">**Fix kipróbálni**</span><span class="sxs-lookup"><span data-stu-id="28cd1-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="28cd1-108">Érvénytelen kérelemtörzs</span><span class="sxs-lookup"><span data-stu-id="28cd1-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="28cd1-109">Ez a hiba ritkán fordulhat elő, ha ezt a hibát látja, próbálja meg újra a műveletet.</span><span class="sxs-lookup"><span data-stu-id="28cd1-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="28cd1-110">Az eszköz hardverkivonat-értéke nem megfelelő.</span><span class="sxs-lookup"><span data-stu-id="28cd1-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="28cd1-111">Ha ez a hiba jelenik meg, az azt jelenti, hogy a CSV-fájlban megadott érték az egyik eszköz hardverkivonatához nem megfelelő.</span><span class="sxs-lookup"><span data-stu-id="28cd1-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="28cd1-112">Először ellenőrizze, hogy az érték helyesen lett-e bejelentve.</span><span class="sxs-lookup"><span data-stu-id="28cd1-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="28cd1-113">Ha úgy gondolja, hogy az érték helyes, de ez a hiba továbbra is fennáll, kérjen segítséget a hardver gyártójától.</span><span class="sxs-lookup"><span data-stu-id="28cd1-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="28cd1-114">Másik bérlőhöz rendelt eszköz</span><span class="sxs-lookup"><span data-stu-id="28cd1-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="28cd1-115">Ha ez a hiba jelenik meg, az azt jelenti, hogy a CSV-fájlban megadott érték egy vagy több eszköz sorozatszáma vagy termékkulcsa nem megfelelő.</span><span class="sxs-lookup"><span data-stu-id="28cd1-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="28cd1-116">Először ellenőrizze, hogy az érték helyesen lett-e bejelentve.</span><span class="sxs-lookup"><span data-stu-id="28cd1-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="28cd1-117">Ha úgy gondolja, hogy az érték helyes, de ez a hiba továbbra is fennáll, kérjen segítséget a hardver gyártójától.</span><span class="sxs-lookup"><span data-stu-id="28cd1-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="28cd1-118">A CSV-fájl érvénytelen sorozatszámot vagy termékkulcsot tartalmaz</span><span class="sxs-lookup"><span data-stu-id="28cd1-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="28cd1-119">Ha ez a hiba jelenik meg, az azt jelenti, hogy a regisztrálni kívánt eszközt már regisztrálta egy másik szervezet.</span><span class="sxs-lookup"><span data-stu-id="28cd1-119">If you see this error, it means that the device you are trying to register is already registered by another organization.</span></span> <span data-ttu-id="28cd1-120">A hiba megoldásához kérjen segítséget a hardver forgalmazójához.</span><span class="sxs-lookup"><span data-stu-id="28cd1-120">To fix this error, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="28cd1-121">Ez az eszköz nem támogatott az AutoPilot használatával történő beállításhoz</span><span class="sxs-lookup"><span data-stu-id="28cd1-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="28cd1-122">Ez a hiba azt jelenti, hogy az eszköz nem felel meg az AutoPilot telepítési követelményeinek.</span><span class="sxs-lookup"><span data-stu-id="28cd1-122">This error means the device doesn't meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="28cd1-123">Az eszközöknek meg kell felelniük az alábbi követelményeknek:</span><span class="sxs-lookup"><span data-stu-id="28cd1-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="28cd1-124">A Windows 10 rendszer 1703-as vagy újabb verzióját kell futtatniuk.</span><span class="sxs-lookup"><span data-stu-id="28cd1-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="28cd1-125">Új eszközök, amelyek nem mentik át a Windows beépített élményét.</span><span class="sxs-lookup"><span data-stu-id="28cd1-125">New devices that haven't been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="28cd1-126">Az eszköz nem található</span><span class="sxs-lookup"><span data-stu-id="28cd1-126">Device not found</span></span>  <br/> |<span data-ttu-id="28cd1-127">Ez a hiba azt jelenti, hogy a CSV-fájlban lévő egy vagy több eszköz nincs regisztrálva a szervezetben.</span><span class="sxs-lookup"><span data-stu-id="28cd1-127">This error means that one or more devices in your CSV file isn't registered to your organization.</span></span> <span data-ttu-id="28cd1-128">A probléma megoldásához kérjen segítséget a hardver forgalmazójához.</span><span class="sxs-lookup"><span data-stu-id="28cd1-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |

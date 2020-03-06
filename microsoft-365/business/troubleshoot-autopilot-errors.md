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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Megtudhatja, hogy miként háríthatja el az AutoPilot eszközfájljainak használata során a Microsoft 365 Vállalati verzióban előforduló hibákat.
ms.openlocfilehash: 7569f18097a1f5959b3dd491958c78886e1e05d6
ms.sourcegitcommit: 41c0bc5cf50f4ca63b4286d1ea0f58ab82984b7a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42547471"
---
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="12255-103">Az AutoPilottal kapcsolatos eszközhibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="12255-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="12255-104">Eszközfájl-hibaüzenetek</span><span class="sxs-lookup"><span data-stu-id="12255-104">Device file error messages</span></span>

<span data-ttu-id="12255-105">Az alábbiakban az AutoPilot eszközfájlokkal végzett munka során a Microsoft 365 Business ben előforduló hibákról olvashat.</span><span class="sxs-lookup"><span data-stu-id="12255-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business.</span></span> 
  
|<span data-ttu-id="12255-106">**Hibakód**</span><span class="sxs-lookup"><span data-stu-id="12255-106">**Error code**</span></span>|<span data-ttu-id="12255-107">**Javítás a kipróbáláshoz**</span><span class="sxs-lookup"><span data-stu-id="12255-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="12255-108">Érvénytelen kérelemtörzs</span><span class="sxs-lookup"><span data-stu-id="12255-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="12255-109">Ez a hiba ritkán fordulhat elő, ha ez a hiba jelenik meg, próbálkozzon újra a művelettel.</span><span class="sxs-lookup"><span data-stu-id="12255-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="12255-110">Az eszköz hardverkivonat-értéke nem megfelelő.</span><span class="sxs-lookup"><span data-stu-id="12255-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="12255-111">Ha ez a hiba jelenik meg, az azt jelenti, hogy a CSV-fájlban megadott érték az egyik eszköz hardverkivonatához nem megfelelő.</span><span class="sxs-lookup"><span data-stu-id="12255-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="12255-112">Először ellenőrizze, hogy helyesen írta-e be az értéket.</span><span class="sxs-lookup"><span data-stu-id="12255-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="12255-113">Ha úgy gondolja, hogy az érték helyes, de ez a hiba továbbra is fennáll, kérjen segítséget a hardver gyártójától.</span><span class="sxs-lookup"><span data-stu-id="12255-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="12255-114">Másik bérlőhöz rendelt eszköz</span><span class="sxs-lookup"><span data-stu-id="12255-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="12255-115">Ha ez a hiba jelenik meg, az azt jelenti, hogy a CSV-fájlban megadott érték vagy a sorozatszám, vagy egy vagy több eszköz termékkulcsa nem megfelelő.</span><span class="sxs-lookup"><span data-stu-id="12255-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="12255-116">Először ellenőrizze, hogy helyesen írta-e be az értéket.</span><span class="sxs-lookup"><span data-stu-id="12255-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="12255-117">Ha úgy gondolja, hogy az érték helyes, de ez a hiba továbbra is fennáll, kérjen segítséget a hardver gyártójától.</span><span class="sxs-lookup"><span data-stu-id="12255-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="12255-118">A CSV-fájl érvénytelen sorozatszámot vagy termékkulcsot tartalmaz</span><span class="sxs-lookup"><span data-stu-id="12255-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="12255-119">Ha ez a hiba jelenik meg, az azt jelenti, hogy a regisztrálni kívánt eszközt már regisztrálta egy másik szervezet.</span><span class="sxs-lookup"><span data-stu-id="12255-119">If you see this error, it means that the device you are trying to register is already registered by another organization.</span></span> <span data-ttu-id="12255-120">A hiba megoldásához kérjen segítséget a hardver gyártójától.</span><span class="sxs-lookup"><span data-stu-id="12255-120">To fix this error, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="12255-121">Ez az eszköz nem támogatott az AutoPilot használatával történő telepítéshez</span><span class="sxs-lookup"><span data-stu-id="12255-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="12255-122">Ez a hiba azt jelenti, hogy az eszköz nem felel meg az AutoPilot telepítési követelményeinek.</span><span class="sxs-lookup"><span data-stu-id="12255-122">This error means the device doesn't meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="12255-123">Az eszközöknek meg kell felelniük az alábbi követelményeknek:</span><span class="sxs-lookup"><span data-stu-id="12255-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="12255-124">A Windows 10 rendszer 1703-as vagy újabb verzióját kell futtatniuk.</span><span class="sxs-lookup"><span data-stu-id="12255-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="12255-125">Új eszközök, amelyek nem voltak a Windows beépített élményén.</span><span class="sxs-lookup"><span data-stu-id="12255-125">New devices that haven't been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="12255-126">Az eszköz nem található</span><span class="sxs-lookup"><span data-stu-id="12255-126">Device not found</span></span>  <br/> |<span data-ttu-id="12255-127">Ez a hiba azt jelenti, hogy a CSV-fájl egy vagy több eszköze nincs regisztrálva a szervezetben.</span><span class="sxs-lookup"><span data-stu-id="12255-127">This error means that one or more devices in your CSV file isn't registered to your organization.</span></span> <span data-ttu-id="12255-128">A probléma megoldásához kérjen segítséget a hardver gyártójától.</span><span class="sxs-lookup"><span data-stu-id="12255-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |

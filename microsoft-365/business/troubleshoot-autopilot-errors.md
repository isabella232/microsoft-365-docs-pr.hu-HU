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
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="7cc24-103">Az AutoPilottal kapcsolatos eszközhibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="7cc24-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="7cc24-104">Eszközfájl-hibaüzenetek</span><span class="sxs-lookup"><span data-stu-id="7cc24-104">Device file error messages</span></span>

<span data-ttu-id="7cc24-105">Az alábbiakban az AutoPilot eszközfájlokkal végzett munka során a Microsoft 365 Business ben előforduló hibákról olvashat.</span><span class="sxs-lookup"><span data-stu-id="7cc24-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business.</span></span> 
  
|<span data-ttu-id="7cc24-106">**Hibakód**</span><span class="sxs-lookup"><span data-stu-id="7cc24-106">**Error code**</span></span>|<span data-ttu-id="7cc24-107">**Javítás a kipróbáláshoz**</span><span class="sxs-lookup"><span data-stu-id="7cc24-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7cc24-108">Érvénytelen kérelemtörzs</span><span class="sxs-lookup"><span data-stu-id="7cc24-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="7cc24-109">Ez a hiba ritkán fordulhat elő, ha ez a hiba jelenik meg, próbálkozzon újra a művelettel.</span><span class="sxs-lookup"><span data-stu-id="7cc24-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="7cc24-110">Az eszköz hardverkivonat-értéke nem megfelelő.</span><span class="sxs-lookup"><span data-stu-id="7cc24-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="7cc24-111">Ha ez a hiba jelenik meg, az azt jelenti, hogy a CSV-fájlban megadott érték az egyik eszköz hardverkivonatához nem megfelelő.</span><span class="sxs-lookup"><span data-stu-id="7cc24-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="7cc24-112">Először ellenőrizze, hogy helyesen írta-e be az értéket.</span><span class="sxs-lookup"><span data-stu-id="7cc24-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="7cc24-113">Ha úgy gondolja, hogy az érték helyes, de ez a hiba továbbra is fennáll, kérjen segítséget a hardver gyártójától.</span><span class="sxs-lookup"><span data-stu-id="7cc24-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="7cc24-114">Másik bérlőhöz rendelt eszköz</span><span class="sxs-lookup"><span data-stu-id="7cc24-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="7cc24-115">Ha ez a hiba jelenik meg, az azt jelenti, hogy a CSV-fájlban megadott érték vagy a sorozatszám, vagy egy vagy több eszköz termékkulcsa nem megfelelő.</span><span class="sxs-lookup"><span data-stu-id="7cc24-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="7cc24-116">Először ellenőrizze, hogy helyesen írta-e be az értéket.</span><span class="sxs-lookup"><span data-stu-id="7cc24-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="7cc24-117">Ha úgy gondolja, hogy az érték helyes, de ez a hiba továbbra is fennáll, kérjen segítséget a hardver gyártójától.</span><span class="sxs-lookup"><span data-stu-id="7cc24-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="7cc24-118">A CSV-fájl érvénytelen sorozatszámot vagy termékkulcsot tartalmaz</span><span class="sxs-lookup"><span data-stu-id="7cc24-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="7cc24-119">Ha ez a hiba jelenik meg, az azt jelenti, hogy a regisztrálni kívánt eszközt már regisztrálta egy másik szervezet.</span><span class="sxs-lookup"><span data-stu-id="7cc24-119">If you see this error, it means that the device you are trying to register is already registered by another organization.</span></span> <span data-ttu-id="7cc24-120">A hiba megoldásához kérjen segítséget a hardver gyártójától.</span><span class="sxs-lookup"><span data-stu-id="7cc24-120">To fix this error, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="7cc24-121">Ez az eszköz nem támogatott az AutoPilot használatával történő telepítéshez</span><span class="sxs-lookup"><span data-stu-id="7cc24-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="7cc24-122">Ez a hiba azt jelenti, hogy az eszköz nem felel meg az AutoPilot telepítési követelményeinek.</span><span class="sxs-lookup"><span data-stu-id="7cc24-122">This error means the device doesn't meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="7cc24-123">Az eszközöknek meg kell felelniük az alábbi követelményeknek:</span><span class="sxs-lookup"><span data-stu-id="7cc24-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="7cc24-124">A Windows 10 rendszer 1703-as vagy újabb verzióját kell futtatniuk.</span><span class="sxs-lookup"><span data-stu-id="7cc24-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="7cc24-125">Új eszközök, amelyek nem voltak a Windows beépített élményén.</span><span class="sxs-lookup"><span data-stu-id="7cc24-125">New devices that haven't been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="7cc24-126">Az eszköz nem található</span><span class="sxs-lookup"><span data-stu-id="7cc24-126">Device not found</span></span>  <br/> |<span data-ttu-id="7cc24-127">Ez a hiba azt jelenti, hogy a CSV-fájl egy vagy több eszköze nincs regisztrálva a szervezetben.</span><span class="sxs-lookup"><span data-stu-id="7cc24-127">This error means that one or more devices in your CSV file isn't registered to your organization.</span></span> <span data-ttu-id="7cc24-128">A probléma megoldásához kérjen segítséget a hardver gyártójától.</span><span class="sxs-lookup"><span data-stu-id="7cc24-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |

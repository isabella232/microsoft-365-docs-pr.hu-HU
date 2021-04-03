---
title: Eszközállapotok
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Az eszköz különböző államokról a Microsoft 365 Vállalati verzió Rendszergazdai kezdőlapja Eszközműveletek listájában olvashat.
ms.openlocfilehash: e6f1b428413d094e0a1ce3afb026528074038736
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578467"
---
# <a name="device-states"></a><span data-ttu-id="7fd9c-103">Eszközállapotok</span><span class="sxs-lookup"><span data-stu-id="7fd9c-103">Device states</span></span>

<span data-ttu-id="7fd9c-104">Ez a cikk a Microsoft 365 Vállalati prémium verzióra vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="7fd9c-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="7fd9c-105">Az **Eszközműveletek** listában (Rendszergazdai kezdőlap \> **Eszközműveletek**) szereplő eszközöknek az alábbi állapotai lehetnek.</span><span class="sxs-lookup"><span data-stu-id="7fd9c-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="7fd9c-107">**Állapot**</span><span class="sxs-lookup"><span data-stu-id="7fd9c-107">**Status**</span></span>|<span data-ttu-id="7fd9c-108">**Leírás**</span><span class="sxs-lookup"><span data-stu-id="7fd9c-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7fd9c-109">Kezeli az Intune</span><span class="sxs-lookup"><span data-stu-id="7fd9c-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="7fd9c-110">A Microsoft 365 Vállalati prémium verzió kezeli.</span><span class="sxs-lookup"><span data-stu-id="7fd9c-110">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="7fd9c-111">Kivezetés függőben</span><span class="sxs-lookup"><span data-stu-id="7fd9c-111">Retire pending</span></span>  <br/> |<span data-ttu-id="7fd9c-112">A Microsoft 365 Vállalati prémium verzió készen áll a céges adatok eltávolítására az eszközről.</span><span class="sxs-lookup"><span data-stu-id="7fd9c-112">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="7fd9c-113">Kivezetés folyamatban</span><span class="sxs-lookup"><span data-stu-id="7fd9c-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="7fd9c-114">A Microsoft 365 Vállalati prémium verzió jelenleg eltávolítja a céges adatokat az eszközről.</span><span class="sxs-lookup"><span data-stu-id="7fd9c-114">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="7fd9c-115">Kivezetés sikertelen</span><span class="sxs-lookup"><span data-stu-id="7fd9c-115">Retire failed</span></span>  <br/> | <span data-ttu-id="7fd9c-116">A vállalati adatok eltávolításának művelete nem sikerült.</span><span class="sxs-lookup"><span data-stu-id="7fd9c-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="7fd9c-117">Kivezetve lemondva</span><span class="sxs-lookup"><span data-stu-id="7fd9c-117">Retire canceled</span></span>  <br/> |<span data-ttu-id="7fd9c-118">A kivezető művelet visszavonva.</span><span class="sxs-lookup"><span data-stu-id="7fd9c-118">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="7fd9c-119">Törlés függőben</span><span class="sxs-lookup"><span data-stu-id="7fd9c-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="7fd9c-120">Várakozás a gyári állapot visszaállításának megkezdésére.</span><span class="sxs-lookup"><span data-stu-id="7fd9c-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="7fd9c-121">Törlés folyamatban</span><span class="sxs-lookup"><span data-stu-id="7fd9c-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="7fd9c-122">Megkezdődött a gyári állapot visszaállítása.</span><span class="sxs-lookup"><span data-stu-id="7fd9c-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="7fd9c-123">Törlés sikertelen</span><span class="sxs-lookup"><span data-stu-id="7fd9c-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="7fd9c-124">Nem sikerült a gyári adatok visszaállítása.</span><span class="sxs-lookup"><span data-stu-id="7fd9c-124">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="7fd9c-125">Törlés visszavonva</span><span class="sxs-lookup"><span data-stu-id="7fd9c-125">Wipe canceled</span></span>  <br/> |<span data-ttu-id="7fd9c-126">A gyári törlés törölve lett.</span><span class="sxs-lookup"><span data-stu-id="7fd9c-126">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="7fd9c-127">Nem kifogástalan</span><span class="sxs-lookup"><span data-stu-id="7fd9c-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="7fd9c-128">Egy művelet függőben van (vagy folyamatban van), de az eszköz már több mint 30 napja nem jelentkezett be.</span><span class="sxs-lookup"><span data-stu-id="7fd9c-128">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="7fd9c-129">Törlés függőben</span><span class="sxs-lookup"><span data-stu-id="7fd9c-129">Delete pending</span></span>  <br/> |<span data-ttu-id="7fd9c-130">Egy törlési művelet függőben van.</span><span class="sxs-lookup"><span data-stu-id="7fd9c-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="7fd9c-131">Észlelt</span><span class="sxs-lookup"><span data-stu-id="7fd9c-131">Discovered</span></span>  <br/> |<span data-ttu-id="7fd9c-132">A Microsoft 365 Vállalati prémium verzió észlelte az eszközt.</span><span class="sxs-lookup"><span data-stu-id="7fd9c-132">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   

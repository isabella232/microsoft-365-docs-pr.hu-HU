---
title: Eszközállapotok
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
description: Ismerje meg a különböző eszközállapotokat a Microsoft 365 vállalati verzió Felügyeleti otthonának eszközműveletek listájában.
ms.openlocfilehash: 64138e2b6ae73c067709cde1912a96615d08ebf1
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471179"
---
# <a name="device-states"></a><span data-ttu-id="b5a8a-103">Eszközállapotok</span><span class="sxs-lookup"><span data-stu-id="b5a8a-103">Device states</span></span>

<span data-ttu-id="b5a8a-104">Ez a cikk a Microsoft 365 Business Premium szolgáltatásra vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="b5a8a-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="b5a8a-105">Az **Eszközműveletek** listában (Rendszergazdai kezdőlap \> **Eszközműveletek**) szereplő eszközöknek az alábbi állapotai lehetnek.</span><span class="sxs-lookup"><span data-stu-id="b5a8a-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="b5a8a-107">**Állapot**</span><span class="sxs-lookup"><span data-stu-id="b5a8a-107">**Status**</span></span>|<span data-ttu-id="b5a8a-108">**Leírás**</span><span class="sxs-lookup"><span data-stu-id="b5a8a-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b5a8a-109">Kezeli az Intune</span><span class="sxs-lookup"><span data-stu-id="b5a8a-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="b5a8a-110">A Microsoft 365 Business Premium kezeli.</span><span class="sxs-lookup"><span data-stu-id="b5a8a-110">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="b5a8a-111">Kivezetés függőben</span><span class="sxs-lookup"><span data-stu-id="b5a8a-111">Retire pending</span></span>  <br/> |<span data-ttu-id="b5a8a-112">A Microsoft 365 Business Premium készen áll a vállalati adatok eltávolítására az eszközről.</span><span class="sxs-lookup"><span data-stu-id="b5a8a-112">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="b5a8a-113">Kivezetés folyamatban</span><span class="sxs-lookup"><span data-stu-id="b5a8a-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="b5a8a-114">A Microsoft 365 Business Premium jelenleg eltávolítja a vállalati adatokat az eszközről.</span><span class="sxs-lookup"><span data-stu-id="b5a8a-114">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="b5a8a-115">Kivezetés sikertelen</span><span class="sxs-lookup"><span data-stu-id="b5a8a-115">Retire failed</span></span>  <br/> | <span data-ttu-id="b5a8a-116">A vállalati adatok eltávolításának művelete nem sikerült.</span><span class="sxs-lookup"><span data-stu-id="b5a8a-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="b5a8a-117">Visszavonás megszakítva</span><span class="sxs-lookup"><span data-stu-id="b5a8a-117">Retire canceled</span></span>  <br/> |<span data-ttu-id="b5a8a-118">A visszavonási művelet megszakadt.</span><span class="sxs-lookup"><span data-stu-id="b5a8a-118">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="b5a8a-119">Törlés függőben</span><span class="sxs-lookup"><span data-stu-id="b5a8a-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="b5a8a-120">Várakozás a gyári állapot visszaállításának megkezdésére.</span><span class="sxs-lookup"><span data-stu-id="b5a8a-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="b5a8a-121">Törlés folyamatban</span><span class="sxs-lookup"><span data-stu-id="b5a8a-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="b5a8a-122">Megkezdődött a gyári állapot visszaállítása.</span><span class="sxs-lookup"><span data-stu-id="b5a8a-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="b5a8a-123">Törlés sikertelen</span><span class="sxs-lookup"><span data-stu-id="b5a8a-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="b5a8a-124">Nem sikerült a gyári beállítások visszaállítása.</span><span class="sxs-lookup"><span data-stu-id="b5a8a-124">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="b5a8a-125">Törlés megszakítva</span><span class="sxs-lookup"><span data-stu-id="b5a8a-125">Wipe canceled</span></span>  <br/> |<span data-ttu-id="b5a8a-126">A gyári törlés megszakadt.</span><span class="sxs-lookup"><span data-stu-id="b5a8a-126">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="b5a8a-127">Nem kifogástalan</span><span class="sxs-lookup"><span data-stu-id="b5a8a-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="b5a8a-128">Egy művelet függőben van (vagy folyamatban van), de az eszköz több mint 30 napja nem jelentkezett be.</span><span class="sxs-lookup"><span data-stu-id="b5a8a-128">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="b5a8a-129">Törlés függőben</span><span class="sxs-lookup"><span data-stu-id="b5a8a-129">Delete pending</span></span>  <br/> |<span data-ttu-id="b5a8a-130">Egy törlési művelet függőben van.</span><span class="sxs-lookup"><span data-stu-id="b5a8a-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="b5a8a-131">Észlelt</span><span class="sxs-lookup"><span data-stu-id="b5a8a-131">Discovered</span></span>  <br/> |<span data-ttu-id="b5a8a-132">A Microsoft 365 Business Premium észlelte az eszközt.</span><span class="sxs-lookup"><span data-stu-id="b5a8a-132">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   

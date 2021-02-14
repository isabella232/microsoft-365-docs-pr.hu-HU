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
description: Az eszköz különféle államokról a Microsoft 365 Vállalati verzió Rendszergazdai kezdőlapja Eszközműveletek listájában olvashat.
ms.openlocfilehash: 64138e2b6ae73c067709cde1912a96615d08ebf1
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471179"
---
# <a name="device-states"></a><span data-ttu-id="9a148-103">Eszközállapotok</span><span class="sxs-lookup"><span data-stu-id="9a148-103">Device states</span></span>

<span data-ttu-id="9a148-104">Ez a cikk a Microsoft 365 Vállalati prémium verzióra vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="9a148-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="9a148-105">Az **Eszközműveletek** listában (Rendszergazdai kezdőlap \> **Eszközműveletek**) szereplő eszközöknek az alábbi állapotai lehetnek.</span><span class="sxs-lookup"><span data-stu-id="9a148-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="9a148-107">**Állapot**</span><span class="sxs-lookup"><span data-stu-id="9a148-107">**Status**</span></span>|<span data-ttu-id="9a148-108">**Leírás**</span><span class="sxs-lookup"><span data-stu-id="9a148-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9a148-109">Kezeli az Intune</span><span class="sxs-lookup"><span data-stu-id="9a148-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="9a148-110">A Microsoft 365 Vállalati prémium verzió kezeli.</span><span class="sxs-lookup"><span data-stu-id="9a148-110">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="9a148-111">Kivezetés függőben</span><span class="sxs-lookup"><span data-stu-id="9a148-111">Retire pending</span></span>  <br/> |<span data-ttu-id="9a148-112">A Microsoft 365 Vállalati prémium verzió felkészül arra, hogy eltávolítsa a céges adatokat az eszközről.</span><span class="sxs-lookup"><span data-stu-id="9a148-112">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="9a148-113">Kivezetés folyamatban</span><span class="sxs-lookup"><span data-stu-id="9a148-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="9a148-114">A Microsoft 365 Vállalati prémium verzió jelenleg eltávolítja a céges adatokat az eszközről.</span><span class="sxs-lookup"><span data-stu-id="9a148-114">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="9a148-115">Kivezetés sikertelen</span><span class="sxs-lookup"><span data-stu-id="9a148-115">Retire failed</span></span>  <br/> | <span data-ttu-id="9a148-116">A vállalati adatok eltávolításának művelete nem sikerült.</span><span class="sxs-lookup"><span data-stu-id="9a148-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="9a148-117">Visszavonva</span><span class="sxs-lookup"><span data-stu-id="9a148-117">Retire canceled</span></span>  <br/> |<span data-ttu-id="9a148-118">A kivezetett művelet visszavonva.</span><span class="sxs-lookup"><span data-stu-id="9a148-118">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="9a148-119">Törlés függőben</span><span class="sxs-lookup"><span data-stu-id="9a148-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="9a148-120">Várakozás a gyári állapot visszaállításának megkezdésére.</span><span class="sxs-lookup"><span data-stu-id="9a148-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="9a148-121">Törlés folyamatban</span><span class="sxs-lookup"><span data-stu-id="9a148-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="9a148-122">Megkezdődött a gyári állapot visszaállítása.</span><span class="sxs-lookup"><span data-stu-id="9a148-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="9a148-123">Törlés sikertelen</span><span class="sxs-lookup"><span data-stu-id="9a148-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="9a148-124">Nem sikerült a gyári beállítások visszaállítása.</span><span class="sxs-lookup"><span data-stu-id="9a148-124">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="9a148-125">Törlés törölve</span><span class="sxs-lookup"><span data-stu-id="9a148-125">Wipe canceled</span></span>  <br/> |<span data-ttu-id="9a148-126">A gyári törlés törölve lett.</span><span class="sxs-lookup"><span data-stu-id="9a148-126">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="9a148-127">Nem kifogástalan</span><span class="sxs-lookup"><span data-stu-id="9a148-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="9a148-128">Egy művelet függőben van (vagy folyamatban van), de az eszköz több mint 30 napja nem jelentkezett be.</span><span class="sxs-lookup"><span data-stu-id="9a148-128">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="9a148-129">Törlés függőben</span><span class="sxs-lookup"><span data-stu-id="9a148-129">Delete pending</span></span>  <br/> |<span data-ttu-id="9a148-130">Egy törlési művelet függőben van.</span><span class="sxs-lookup"><span data-stu-id="9a148-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="9a148-131">Észlelt</span><span class="sxs-lookup"><span data-stu-id="9a148-131">Discovered</span></span>  <br/> |<span data-ttu-id="9a148-132">A Microsoft 365 Vállalati prémium verzió észlelte az eszközt.</span><span class="sxs-lookup"><span data-stu-id="9a148-132">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   

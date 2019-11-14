---
title: Eszközállapotok
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Információ a Microsoft 365 Business eszköz eszközállapoiról.
ms.openlocfilehash: b55e6a5d538ec28d195225e93797cea27afd2e8b
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/14/2019
ms.locfileid: "38320208"
---
# <a name="device-states"></a><span data-ttu-id="e261f-103">Eszközállapotok</span><span class="sxs-lookup"><span data-stu-id="e261f-103">Device states</span></span>

<span data-ttu-id="e261f-104">Az **Eszközműveletek** listában (Rendszergazdai kezdőlap \> **Eszközműveletek**) szereplő eszközöknek az alábbi állapotai lehetnek.</span><span class="sxs-lookup"><span data-stu-id="e261f-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="e261f-106">**Állapot**</span><span class="sxs-lookup"><span data-stu-id="e261f-106">**Status**</span></span>|<span data-ttu-id="e261f-107">**Leírás**</span><span class="sxs-lookup"><span data-stu-id="e261f-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e261f-108">Kezeli az Intune</span><span class="sxs-lookup"><span data-stu-id="e261f-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="e261f-109">Az eszköz a Microsoft 365 Business felügyelete alatt áll.</span><span class="sxs-lookup"><span data-stu-id="e261f-109">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="e261f-110">Kivezetés függőben</span><span class="sxs-lookup"><span data-stu-id="e261f-110">Retire pending</span></span>  <br/> |<span data-ttu-id="e261f-111">A Microsoft 365 Business felkészülőben van a vállalati adatok eszközről való eltávolítására.</span><span class="sxs-lookup"><span data-stu-id="e261f-111">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="e261f-112">Kivezetés folyamatban</span><span class="sxs-lookup"><span data-stu-id="e261f-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="e261f-113">A Microsoft 365 Business jelenleg a vállalati adatok eszközről való eltávolításán dolgozik.</span><span class="sxs-lookup"><span data-stu-id="e261f-113">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="e261f-114">Kivezetés sikertelen</span><span class="sxs-lookup"><span data-stu-id="e261f-114">Retire failed</span></span>  <br/> | <span data-ttu-id="e261f-115">A vállalati adatok eltávolításának művelete nem sikerült.</span><span class="sxs-lookup"><span data-stu-id="e261f-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="e261f-116">Visszavonva</span><span class="sxs-lookup"><span data-stu-id="e261f-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="e261f-117">Visszavonta a műveletet.</span><span class="sxs-lookup"><span data-stu-id="e261f-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="e261f-118">Törlés függőben</span><span class="sxs-lookup"><span data-stu-id="e261f-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="e261f-119">Várakozás a gyári állapot visszaállításának megkezdésére.</span><span class="sxs-lookup"><span data-stu-id="e261f-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="e261f-120">Törlés folyamatban</span><span class="sxs-lookup"><span data-stu-id="e261f-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="e261f-121">Megkezdődött a gyári állapot visszaállítása.</span><span class="sxs-lookup"><span data-stu-id="e261f-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="e261f-122">Törlés sikertelen</span><span class="sxs-lookup"><span data-stu-id="e261f-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="e261f-123">Nem tudott ' csinál gyár orrgazdaság.</span><span class="sxs-lookup"><span data-stu-id="e261f-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="e261f-124">Kitakarás megszakítva</span><span class="sxs-lookup"><span data-stu-id="e261f-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="e261f-125">Gyári törlés törölték.</span><span class="sxs-lookup"><span data-stu-id="e261f-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="e261f-126">Nem kifogástalan</span><span class="sxs-lookup"><span data-stu-id="e261f-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="e261f-127">A művelet függőben (vagy folyamatban) van, de az eszköz 30 + napig nem ellenőrzött.</span><span class="sxs-lookup"><span data-stu-id="e261f-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="e261f-128">Törlés függőben</span><span class="sxs-lookup"><span data-stu-id="e261f-128">Delete pending</span></span>  <br/> |<span data-ttu-id="e261f-129">Egy törlési művelet függőben van.</span><span class="sxs-lookup"><span data-stu-id="e261f-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="e261f-130">Észlelt</span><span class="sxs-lookup"><span data-stu-id="e261f-130">Discovered</span></span>  <br/> |<span data-ttu-id="e261f-131">A Microsoft 365 Business észlelte az eszközt.</span><span class="sxs-lookup"><span data-stu-id="e261f-131">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   

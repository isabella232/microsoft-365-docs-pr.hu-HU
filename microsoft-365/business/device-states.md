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
ms.openlocfilehash: 90c11caa03249408ba2916d303bcb4a59fbcca8c
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44400954"
---
# <a name="device-states"></a><span data-ttu-id="933ec-103">Eszközállapotok</span><span class="sxs-lookup"><span data-stu-id="933ec-103">Device states</span></span>

<span data-ttu-id="933ec-104">Az **Eszközműveletek** listában (Rendszergazdai kezdőlap \> **Eszközműveletek**) szereplő eszközöknek az alábbi állapotai lehetnek.</span><span class="sxs-lookup"><span data-stu-id="933ec-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="933ec-106">**Állapot**</span><span class="sxs-lookup"><span data-stu-id="933ec-106">**Status**</span></span>|<span data-ttu-id="933ec-107">**Leírás**</span><span class="sxs-lookup"><span data-stu-id="933ec-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="933ec-108">Kezeli az Intune</span><span class="sxs-lookup"><span data-stu-id="933ec-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="933ec-109">A Microsoft 365 Business Premium kezeli.</span><span class="sxs-lookup"><span data-stu-id="933ec-109">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="933ec-110">Kivezetés függőben</span><span class="sxs-lookup"><span data-stu-id="933ec-110">Retire pending</span></span>  <br/> |<span data-ttu-id="933ec-111">A Microsoft 365 Business Premium készen áll a vállalati adatok eltávolítására az eszközről.</span><span class="sxs-lookup"><span data-stu-id="933ec-111">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="933ec-112">Kivezetés folyamatban</span><span class="sxs-lookup"><span data-stu-id="933ec-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="933ec-113">A Microsoft 365 Business Premium jelenleg eltávolítja a vállalati adatokat az eszközről.</span><span class="sxs-lookup"><span data-stu-id="933ec-113">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="933ec-114">Kivezetés sikertelen</span><span class="sxs-lookup"><span data-stu-id="933ec-114">Retire failed</span></span>  <br/> | <span data-ttu-id="933ec-115">A vállalati adatok eltávolításának művelete nem sikerült.</span><span class="sxs-lookup"><span data-stu-id="933ec-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="933ec-116">Visszavonás megszakítva</span><span class="sxs-lookup"><span data-stu-id="933ec-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="933ec-117">A visszavonási művelet megszakadt.</span><span class="sxs-lookup"><span data-stu-id="933ec-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="933ec-118">Törlés függőben</span><span class="sxs-lookup"><span data-stu-id="933ec-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="933ec-119">Várakozás a gyári állapot visszaállításának megkezdésére.</span><span class="sxs-lookup"><span data-stu-id="933ec-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="933ec-120">Törlés folyamatban</span><span class="sxs-lookup"><span data-stu-id="933ec-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="933ec-121">Megkezdődött a gyári állapot visszaállítása.</span><span class="sxs-lookup"><span data-stu-id="933ec-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="933ec-122">Törlés sikertelen</span><span class="sxs-lookup"><span data-stu-id="933ec-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="933ec-123">Nem sikerült a gyári beállítások visszaállítása.</span><span class="sxs-lookup"><span data-stu-id="933ec-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="933ec-124">Törlés megszakítva</span><span class="sxs-lookup"><span data-stu-id="933ec-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="933ec-125">A gyári törlés megszakadt.</span><span class="sxs-lookup"><span data-stu-id="933ec-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="933ec-126">Nem kifogástalan</span><span class="sxs-lookup"><span data-stu-id="933ec-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="933ec-127">Egy művelet függőben van (vagy folyamatban van), de az eszköz több mint 30 napja nem jelentkezett be.</span><span class="sxs-lookup"><span data-stu-id="933ec-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="933ec-128">Törlés függőben</span><span class="sxs-lookup"><span data-stu-id="933ec-128">Delete pending</span></span>  <br/> |<span data-ttu-id="933ec-129">Egy törlési művelet függőben van.</span><span class="sxs-lookup"><span data-stu-id="933ec-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="933ec-130">Észlelt</span><span class="sxs-lookup"><span data-stu-id="933ec-130">Discovered</span></span>  <br/> |<span data-ttu-id="933ec-131">A Microsoft 365 Business Premium észlelte az eszközt.</span><span class="sxs-lookup"><span data-stu-id="933ec-131">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   

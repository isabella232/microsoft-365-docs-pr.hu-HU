---
title: Eszközállapotok
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
description: 'További tudnivalók: Microsoft 365 üzleti eszköz államok.'
ms.openlocfilehash: 15114835a5014f5bfac600eac79bcdffdaec481a
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32276981"
---
# <a name="device-states"></a><span data-ttu-id="6f880-103">Eszközállapotok</span><span class="sxs-lookup"><span data-stu-id="6f880-103">Device states</span></span>

## <a name="device-states"></a><span data-ttu-id="6f880-104">Eszközállapotok</span><span class="sxs-lookup"><span data-stu-id="6f880-104">Device states</span></span>

<span data-ttu-id="6f880-105">Az **Eszközműveletek** listában (Rendszergazdai kezdőlap \> **Eszközműveletek**) szereplő eszközöknek az alábbi állapotai lehetnek.</span><span class="sxs-lookup"><span data-stu-id="6f880-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="6f880-107">**Állapot**</span><span class="sxs-lookup"><span data-stu-id="6f880-107">**Status**</span></span>|<span data-ttu-id="6f880-108">**Leírás**</span><span class="sxs-lookup"><span data-stu-id="6f880-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6f880-109">Kezeli az Intune</span><span class="sxs-lookup"><span data-stu-id="6f880-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="6f880-110">Az eszköz a Microsoft 365 Business felügyelete alatt áll.</span><span class="sxs-lookup"><span data-stu-id="6f880-110">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="6f880-111">Kivezetés függőben</span><span class="sxs-lookup"><span data-stu-id="6f880-111">Retire pending</span></span>  <br/> |<span data-ttu-id="6f880-112">A Microsoft 365 Business felkészülőben van a vállalati adatok eszközről való eltávolítására.</span><span class="sxs-lookup"><span data-stu-id="6f880-112">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="6f880-113">Kivezetés folyamatban</span><span class="sxs-lookup"><span data-stu-id="6f880-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="6f880-114">A Microsoft 365 Business jelenleg a vállalati adatok eszközről való eltávolításán dolgozik.</span><span class="sxs-lookup"><span data-stu-id="6f880-114">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="6f880-115">Kivezetés sikertelen</span><span class="sxs-lookup"><span data-stu-id="6f880-115">Retire failed</span></span>  <br/> | <span data-ttu-id="6f880-116">A vállalati adatok eltávolításának művelete nem sikerült.</span><span class="sxs-lookup"><span data-stu-id="6f880-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="6f880-117">Kivezetés visszavonva</span><span class="sxs-lookup"><span data-stu-id="6f880-117">Retire cancelled</span></span>  <br/> |<span data-ttu-id="6f880-118">A kivezetési művelet vissza lett vonva.</span><span class="sxs-lookup"><span data-stu-id="6f880-118">Retire action was cancelled.</span></span>  <br/> |
|<span data-ttu-id="6f880-119">Törlés függőben</span><span class="sxs-lookup"><span data-stu-id="6f880-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="6f880-120">Várakozás a gyári állapot visszaállításának megkezdésére.</span><span class="sxs-lookup"><span data-stu-id="6f880-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="6f880-121">Törlés folyamatban</span><span class="sxs-lookup"><span data-stu-id="6f880-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="6f880-122">Megkezdődött a gyári állapot visszaállítása.</span><span class="sxs-lookup"><span data-stu-id="6f880-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="6f880-123">Törlés sikertelen</span><span class="sxs-lookup"><span data-stu-id="6f880-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="6f880-124">Nem sikerült végrehajtani a gyári állapot visszaállítását.</span><span class="sxs-lookup"><span data-stu-id="6f880-124">Couldn't perform factory reset.</span></span>  <br/> |
|<span data-ttu-id="6f880-125">Törlés visszavonva</span><span class="sxs-lookup"><span data-stu-id="6f880-125">Wipe cancelled</span></span>  <br/> |<span data-ttu-id="6f880-126">A gyári állapot visszaállítása vissza lett vonva.</span><span class="sxs-lookup"><span data-stu-id="6f880-126">Factory wipe was cancelled.</span></span>  <br/> |
|<span data-ttu-id="6f880-127">Nem kifogástalan</span><span class="sxs-lookup"><span data-stu-id="6f880-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="6f880-128">Ez azt jelenti, hogy egy művelet függőben (vagy folyamatban) van, de az eszköz nem jelentkezett be több mint 30 napja.</span><span class="sxs-lookup"><span data-stu-id="6f880-128">This means that an action is pending (or in progress) but the device has not checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="6f880-129">Törlés függőben</span><span class="sxs-lookup"><span data-stu-id="6f880-129">Delete pending</span></span>  <br/> |<span data-ttu-id="6f880-130">Egy törlési művelet függőben van.</span><span class="sxs-lookup"><span data-stu-id="6f880-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="6f880-131">Észlelt</span><span class="sxs-lookup"><span data-stu-id="6f880-131">Discovered</span></span>  <br/> |<span data-ttu-id="6f880-132">A Microsoft 365 Business észlelte az eszközt.</span><span class="sxs-lookup"><span data-stu-id="6f880-132">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   

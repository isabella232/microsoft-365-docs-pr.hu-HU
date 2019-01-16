---
title: Eszközállapotok
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: overview
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
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
ms.openlocfilehash: bd6f1ad7f7671d9616fd14d477dfcfb164ff6bd0
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982905"
---
# <a name="device-states"></a><span data-ttu-id="ea9d0-103">Eszközállapotok</span><span class="sxs-lookup"><span data-stu-id="ea9d0-103">Device states</span></span>

## <a name="device-states"></a><span data-ttu-id="ea9d0-104">Eszközállapotok</span><span class="sxs-lookup"><span data-stu-id="ea9d0-104">Device states</span></span>

<span data-ttu-id="ea9d0-105">Az **Eszközműveletek** listában (Rendszergazdai kezdőlap \> **Eszközműveletek**) szereplő eszközöknek az alábbi állapotai lehetnek.</span><span class="sxs-lookup"><span data-stu-id="ea9d0-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="ea9d0-107">**Állapot**</span><span class="sxs-lookup"><span data-stu-id="ea9d0-107">**Status**</span></span>|<span data-ttu-id="ea9d0-108">**Leírás**</span><span class="sxs-lookup"><span data-stu-id="ea9d0-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ea9d0-109">Kezeli az Intune</span><span class="sxs-lookup"><span data-stu-id="ea9d0-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="ea9d0-110">Az eszköz a Microsoft 365 Business felügyelete alatt áll.</span><span class="sxs-lookup"><span data-stu-id="ea9d0-110">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="ea9d0-111">Kivezetés függőben</span><span class="sxs-lookup"><span data-stu-id="ea9d0-111">Retire pending</span></span>  <br/> |<span data-ttu-id="ea9d0-112">A Microsoft 365 Business felkészülőben van a vállalati adatok eszközről való eltávolítására.</span><span class="sxs-lookup"><span data-stu-id="ea9d0-112">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="ea9d0-113">Kivezetés folyamatban</span><span class="sxs-lookup"><span data-stu-id="ea9d0-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="ea9d0-114">A Microsoft 365 Business jelenleg a vállalati adatok eszközről való eltávolításán dolgozik.</span><span class="sxs-lookup"><span data-stu-id="ea9d0-114">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="ea9d0-115">Kivezetés sikertelen</span><span class="sxs-lookup"><span data-stu-id="ea9d0-115">Retire failed</span></span>  <br/> | <span data-ttu-id="ea9d0-116">A vállalati adatok eltávolításának művelete nem sikerült.</span><span class="sxs-lookup"><span data-stu-id="ea9d0-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="ea9d0-117">Kivezetés visszavonva</span><span class="sxs-lookup"><span data-stu-id="ea9d0-117">Retire cancelled</span></span>  <br/> |<span data-ttu-id="ea9d0-118">A kivezetési művelet vissza lett vonva.</span><span class="sxs-lookup"><span data-stu-id="ea9d0-118">Retire action was cancelled.</span></span>  <br/> |
|<span data-ttu-id="ea9d0-119">Törlés függőben</span><span class="sxs-lookup"><span data-stu-id="ea9d0-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="ea9d0-120">Várakozás a gyári állapot visszaállításának megkezdésére.</span><span class="sxs-lookup"><span data-stu-id="ea9d0-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="ea9d0-121">Törlés folyamatban</span><span class="sxs-lookup"><span data-stu-id="ea9d0-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="ea9d0-122">Megkezdődött a gyári állapot visszaállítása.</span><span class="sxs-lookup"><span data-stu-id="ea9d0-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="ea9d0-123">Törlés sikertelen</span><span class="sxs-lookup"><span data-stu-id="ea9d0-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="ea9d0-124">Nem sikerült végrehajtani a gyári állapot visszaállítását.</span><span class="sxs-lookup"><span data-stu-id="ea9d0-124">Couldn't perform factory reset.</span></span>  <br/> |
|<span data-ttu-id="ea9d0-125">Törlés visszavonva</span><span class="sxs-lookup"><span data-stu-id="ea9d0-125">Wipe cancelled</span></span>  <br/> |<span data-ttu-id="ea9d0-126">A gyári állapot visszaállítása vissza lett vonva.</span><span class="sxs-lookup"><span data-stu-id="ea9d0-126">Factory wipe was cancelled.</span></span>  <br/> |
|<span data-ttu-id="ea9d0-127">Nem kifogástalan</span><span class="sxs-lookup"><span data-stu-id="ea9d0-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="ea9d0-128">Ez azt jelenti, hogy egy művelet függőben (vagy folyamatban) van, de az eszköz nem jelentkezett be több mint 30 napja.</span><span class="sxs-lookup"><span data-stu-id="ea9d0-128">This means that an action is pending (or in progress) but the device has not checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="ea9d0-129">Törlés függőben</span><span class="sxs-lookup"><span data-stu-id="ea9d0-129">Delete pending</span></span>  <br/> |<span data-ttu-id="ea9d0-130">Egy törlési művelet függőben van.</span><span class="sxs-lookup"><span data-stu-id="ea9d0-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="ea9d0-131">Észlelt</span><span class="sxs-lookup"><span data-stu-id="ea9d0-131">Discovered</span></span>  <br/> |<span data-ttu-id="ea9d0-132">A Microsoft 365 Business észlelte az eszközt.</span><span class="sxs-lookup"><span data-stu-id="ea9d0-132">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   

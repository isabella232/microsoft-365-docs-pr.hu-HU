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
description: 'További tudnivalók: Microsoft 365 üzleti eszköz államok.'
ms.openlocfilehash: 06e5c800e6a104785c1fd0724223e05d7729722e
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/15/2019
ms.locfileid: "34072720"
---
# <a name="device-states"></a><span data-ttu-id="bbc9e-103">Eszközállapotok</span><span class="sxs-lookup"><span data-stu-id="bbc9e-103">Device states</span></span>

## <a name="device-states"></a><span data-ttu-id="bbc9e-104">Eszközállapotok</span><span class="sxs-lookup"><span data-stu-id="bbc9e-104">Device states</span></span>

<span data-ttu-id="bbc9e-105">Az **Eszközműveletek** listában (Rendszergazdai kezdőlap \> **Eszközműveletek**) szereplő eszközöknek az alábbi állapotai lehetnek.</span><span class="sxs-lookup"><span data-stu-id="bbc9e-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="bbc9e-107">**Állapot**</span><span class="sxs-lookup"><span data-stu-id="bbc9e-107">**Status**</span></span>|<span data-ttu-id="bbc9e-108">**Leírás**</span><span class="sxs-lookup"><span data-stu-id="bbc9e-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bbc9e-109">Kezeli az Intune</span><span class="sxs-lookup"><span data-stu-id="bbc9e-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="bbc9e-110">Az eszköz a Microsoft 365 Business felügyelete alatt áll.</span><span class="sxs-lookup"><span data-stu-id="bbc9e-110">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="bbc9e-111">Kivezetés függőben</span><span class="sxs-lookup"><span data-stu-id="bbc9e-111">Retire pending</span></span>  <br/> |<span data-ttu-id="bbc9e-112">A Microsoft 365 Business felkészülőben van a vállalati adatok eszközről való eltávolítására.</span><span class="sxs-lookup"><span data-stu-id="bbc9e-112">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="bbc9e-113">Kivezetés folyamatban</span><span class="sxs-lookup"><span data-stu-id="bbc9e-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="bbc9e-114">A Microsoft 365 Business jelenleg a vállalati adatok eszközről való eltávolításán dolgozik.</span><span class="sxs-lookup"><span data-stu-id="bbc9e-114">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="bbc9e-115">Kivezetés sikertelen</span><span class="sxs-lookup"><span data-stu-id="bbc9e-115">Retire failed</span></span>  <br/> | <span data-ttu-id="bbc9e-116">A vállalati adatok eltávolításának művelete nem sikerült.</span><span class="sxs-lookup"><span data-stu-id="bbc9e-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="bbc9e-117">Kivezetés visszavonva</span><span class="sxs-lookup"><span data-stu-id="bbc9e-117">Retire cancelled</span></span>  <br/> |<span data-ttu-id="bbc9e-118">A kivezetési művelet vissza lett vonva.</span><span class="sxs-lookup"><span data-stu-id="bbc9e-118">Retire action was cancelled.</span></span>  <br/> |
|<span data-ttu-id="bbc9e-119">Törlés függőben</span><span class="sxs-lookup"><span data-stu-id="bbc9e-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="bbc9e-120">Várakozás a gyári állapot visszaállításának megkezdésére.</span><span class="sxs-lookup"><span data-stu-id="bbc9e-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="bbc9e-121">Törlés folyamatban</span><span class="sxs-lookup"><span data-stu-id="bbc9e-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="bbc9e-122">Megkezdődött a gyári állapot visszaállítása.</span><span class="sxs-lookup"><span data-stu-id="bbc9e-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="bbc9e-123">Törlés sikertelen</span><span class="sxs-lookup"><span data-stu-id="bbc9e-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="bbc9e-124">Nem sikerült végrehajtani a gyári állapot visszaállítását.</span><span class="sxs-lookup"><span data-stu-id="bbc9e-124">Couldn't perform factory reset.</span></span>  <br/> |
|<span data-ttu-id="bbc9e-125">Törlés visszavonva</span><span class="sxs-lookup"><span data-stu-id="bbc9e-125">Wipe cancelled</span></span>  <br/> |<span data-ttu-id="bbc9e-126">A gyári állapot visszaállítása vissza lett vonva.</span><span class="sxs-lookup"><span data-stu-id="bbc9e-126">Factory wipe was cancelled.</span></span>  <br/> |
|<span data-ttu-id="bbc9e-127">Nem kifogástalan</span><span class="sxs-lookup"><span data-stu-id="bbc9e-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="bbc9e-128">Ez azt jelenti, hogy egy művelet függőben (vagy folyamatban) van, de az eszköz nem jelentkezett be több mint 30 napja.</span><span class="sxs-lookup"><span data-stu-id="bbc9e-128">This means that an action is pending (or in progress) but the device has not checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="bbc9e-129">Törlés függőben</span><span class="sxs-lookup"><span data-stu-id="bbc9e-129">Delete pending</span></span>  <br/> |<span data-ttu-id="bbc9e-130">Egy törlési művelet függőben van.</span><span class="sxs-lookup"><span data-stu-id="bbc9e-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="bbc9e-131">Észlelt</span><span class="sxs-lookup"><span data-stu-id="bbc9e-131">Discovered</span></span>  <br/> |<span data-ttu-id="bbc9e-132">A Microsoft 365 Business észlelte az eszközt.</span><span class="sxs-lookup"><span data-stu-id="bbc9e-132">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   

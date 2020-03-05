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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Ismerje meg a Microsoft 365 Vállalati verzió Rendszergazdai kezdőlapjának Eszközműveletek listájában található különböző eszközállapotokat.
ms.openlocfilehash: 878050fbe11acca1d5d434a5d2ab0b5b48510e45
ms.sourcegitcommit: ab916c216053999c9c4ef4838217e82cd861f23f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2020
ms.locfileid: "42415665"
---
# <a name="device-states"></a><span data-ttu-id="16110-103">Eszközállapotok</span><span class="sxs-lookup"><span data-stu-id="16110-103">Device states</span></span>

<span data-ttu-id="16110-104">Az **Eszközműveletek** listában (Rendszergazdai kezdőlap \> **Eszközműveletek**) szereplő eszközöknek az alábbi állapotai lehetnek.</span><span class="sxs-lookup"><span data-stu-id="16110-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="16110-106">**Állapot**</span><span class="sxs-lookup"><span data-stu-id="16110-106">**Status**</span></span>|<span data-ttu-id="16110-107">**Leírás**</span><span class="sxs-lookup"><span data-stu-id="16110-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="16110-108">Kezeli az Intune</span><span class="sxs-lookup"><span data-stu-id="16110-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="16110-109">Az eszköz a Microsoft 365 Business felügyelete alatt áll.</span><span class="sxs-lookup"><span data-stu-id="16110-109">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="16110-110">Kivezetés függőben</span><span class="sxs-lookup"><span data-stu-id="16110-110">Retire pending</span></span>  <br/> |<span data-ttu-id="16110-111">A Microsoft 365 Business felkészülőben van a vállalati adatok eszközről való eltávolítására.</span><span class="sxs-lookup"><span data-stu-id="16110-111">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="16110-112">Kivezetés folyamatban</span><span class="sxs-lookup"><span data-stu-id="16110-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="16110-113">A Microsoft 365 Business jelenleg a vállalati adatok eszközről való eltávolításán dolgozik.</span><span class="sxs-lookup"><span data-stu-id="16110-113">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="16110-114">Kivezetés sikertelen</span><span class="sxs-lookup"><span data-stu-id="16110-114">Retire failed</span></span>  <br/> | <span data-ttu-id="16110-115">A vállalati adatok eltávolításának művelete nem sikerült.</span><span class="sxs-lookup"><span data-stu-id="16110-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="16110-116">Visszavont megszüntetés</span><span class="sxs-lookup"><span data-stu-id="16110-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="16110-117">A megszüntetési művelet meglett szakítva.</span><span class="sxs-lookup"><span data-stu-id="16110-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="16110-118">Törlés függőben</span><span class="sxs-lookup"><span data-stu-id="16110-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="16110-119">Várakozás a gyári állapot visszaállításának megkezdésére.</span><span class="sxs-lookup"><span data-stu-id="16110-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="16110-120">Törlés folyamatban</span><span class="sxs-lookup"><span data-stu-id="16110-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="16110-121">Megkezdődött a gyári állapot visszaállítása.</span><span class="sxs-lookup"><span data-stu-id="16110-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="16110-122">Törlés sikertelen</span><span class="sxs-lookup"><span data-stu-id="16110-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="16110-123">Nem sikerült gyári beállítások visszaállítása.</span><span class="sxs-lookup"><span data-stu-id="16110-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="16110-124">Törlés megszakítva</span><span class="sxs-lookup"><span data-stu-id="16110-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="16110-125">A gyári törlőkendő törölve lett.</span><span class="sxs-lookup"><span data-stu-id="16110-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="16110-126">Nem kifogástalan</span><span class="sxs-lookup"><span data-stu-id="16110-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="16110-127">Egy művelet függőben van (vagy folyamatban van), de az eszköz több mint 30 napig nem jelentkezett be.</span><span class="sxs-lookup"><span data-stu-id="16110-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="16110-128">Törlés függőben</span><span class="sxs-lookup"><span data-stu-id="16110-128">Delete pending</span></span>  <br/> |<span data-ttu-id="16110-129">Egy törlési művelet függőben van.</span><span class="sxs-lookup"><span data-stu-id="16110-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="16110-130">Észlelt</span><span class="sxs-lookup"><span data-stu-id="16110-130">Discovered</span></span>  <br/> |<span data-ttu-id="16110-131">A Microsoft 365 Business észlelte az eszközt.</span><span class="sxs-lookup"><span data-stu-id="16110-131">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   

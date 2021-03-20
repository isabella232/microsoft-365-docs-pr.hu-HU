---
title: Appvédelmi beállítások érvényességének ellenőrzése Windows 10-es PC-ken
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
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
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Megtudhatja, hogyan ellenőrizheti, hogy a Microsoft 365 Vállalati verzió appvédelmi beállításai hatályba lépnek-e a felhasználók Windows 10-es eszközein.
ms.openlocfilehash: ff99b3a4fce49aebdb5c72f51e46678a7821e186
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912414"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="5ed52-103">Eszközvédelmi beállítások érvényességének ellenőrzése Windows 10-es PC-ken</span><span class="sxs-lookup"><span data-stu-id="5ed52-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="5ed52-104">Windows 10-eszközházirendek érvénybe lépésének ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="5ed52-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="5ed52-105">Miután [beállította az eszközházirendeket](protection-settings-for-windows-10-pcs.md), néhány óra is eltelhet, amíg a házirendek érvénybe lépnek a felhasználók eszközein.</span><span class="sxs-lookup"><span data-stu-id="5ed52-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="5ed52-106">A házirendek érvénybe lépéséről úgy bizonyosodhat meg, ha ellenőrzi a felhasználók eszközein a Windows Gépház bizonyos beállításlapjait.</span><span class="sxs-lookup"><span data-stu-id="5ed52-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="5ed52-107">Mivel a felhasználók nem tudják módosítani a Windows Update és a Windows Defender víruskereső beállításait a Windows 10-es eszközeiken, számos beállítás szürkén jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="5ed52-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, many options will be grayed out.</span></span>
  
1. <span data-ttu-id="5ed52-108">A Windows Update **újraindítási** beállításai között ellenőrizze, hogy minden \> **&amp;** \>  \>  beállítás szürkén jelenik-e meg.</span><span class="sxs-lookup"><span data-stu-id="5ed52-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are grayed out.</span></span> 
    
    ![Az Újraindítási beállítások szürkén jelennek meg.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="5ed52-110">A **Windows** Update speciális beállításai a Biztonsági beállítások frissítése lapon győződjön meg arról, hogy az összes beállítás \> **&amp;** \>  \>  szürkén jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="5ed52-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are grayed out.</span></span> 
    
    ![A Windows speciális frissítésének beállításai szürkén jelennek meg.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="5ed52-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span><span class="sxs-lookup"><span data-stu-id="5ed52-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="5ed52-113">Győződjön meg arról, hogy látja (piros színnel) azt az üzenetet, hogy egyes beállítások rejtettek vagy a szervezet által kezeltek, és hogy az összes beállítás szürkén jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="5ed52-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are grayed out.</span></span>
    
    ![Choose how updates are delivered page indicates settings are hidden or managed by your organization.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="5ed52-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span><span class="sxs-lookup"><span data-stu-id="5ed52-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="5ed52-116">Ellenőrizze, hogy minden beállítás szürkén jelenik-e meg.</span><span class="sxs-lookup"><span data-stu-id="5ed52-116">Verify that all options are grayed out.</span></span> 
    
    ![A vírus- és veszélyforrás-védelmi beállítások szürkén jelennek meg.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="5ed52-118">Kapcsolódó témakörök</span><span class="sxs-lookup"><span data-stu-id="5ed52-118">Related Topics</span></span>

[<span data-ttu-id="5ed52-119">A Microsoft 365 Vállalati verzió dokumentációja és forrásai</span><span class="sxs-lookup"><span data-stu-id="5ed52-119">Microsoft 365 for business documentation and resources</span></span>](./index.yml)
  
[<span data-ttu-id="5ed52-120">A Microsoft 365 Vállalati verzió első lépések</span><span class="sxs-lookup"><span data-stu-id="5ed52-120">Get started with Microsoft 365 for business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="5ed52-121">A Microsoft 365 Vállalati verzió kezelése</span><span class="sxs-lookup"><span data-stu-id="5ed52-121">Manage Microsoft 365 for business</span></span>](manage.md)
  
[<span data-ttu-id="5ed52-122">Eszközkonfigurációk megadása Windows 10-es PC-ken</span><span class="sxs-lookup"><span data-stu-id="5ed52-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)

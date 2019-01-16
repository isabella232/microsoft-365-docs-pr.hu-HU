---
title: Appvédelmi beállítások érvényességének ellenőrzése Windows 10-es PC-ken
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
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
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Útmutató a Microsoft 365 üzleti alkalmazás beállításai Windows 10 eszközök ellenőrzése.
ms.openlocfilehash: db05c86bd75cc30e22e025034a3dab478d0f5365
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982705"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="38f00-103">Eszközvédelmi beállítások érvényességének ellenőrzése Windows 10-es PC-ken</span><span class="sxs-lookup"><span data-stu-id="38f00-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="38f00-104">Windows 10-eszközházirendek érvénybe lépésének ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="38f00-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="38f00-p101">Miután [beállította az eszközházirendeket](protection-settings-for-windows-10-pcs.md), néhány óra is eltelhet, amíg a házirendek érvénybe lépnek a felhasználók eszközein. A házirendek érvénybe lépéséről úgy bizonyosodhat meg, ha ellenőrzi a felhasználók eszközein a Windows Gépház bizonyos beállításlapjait. Mivel a házirendek használatakor a felhasználók nem módosíthatják a Windows Update és a Windows Defender víruskereső beállításait a Windows 10-es eszközeiken, sok beállításnak kiszürkítve kell megjelennie.</span><span class="sxs-lookup"><span data-stu-id="38f00-p101">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices. You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices. Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, a lot of those options will be greyed out.</span></span>
  
1. <span data-ttu-id="38f00-108">Menjen a **Beállítások** \> **frissítés &amp; biztonsági** \> **A Windows Update** \> **Indítsa újra a beállításokat** , és győződjön meg arról, hogy minden beállítás szürkévé.</span><span class="sxs-lookup"><span data-stu-id="38f00-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are greyed out.</span></span> 
    
    ![All the Restart options are greyed out.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="38f00-110">Ugrás a **Beállítások** \> **frissítés &amp; biztonsági** \> **A Windows Update** \> **Speciális beállítások** , és győződjön meg arról, hogy minden beállítás szürkévé.</span><span class="sxs-lookup"><span data-stu-id="38f00-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are greyed out.</span></span> 
    
    ![Windows Advanced updates options are all greyed out.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="38f00-112">Ugrás a **Beállítások** \> **frissítés &amp; biztonsági** \> **A Windows Update** \> **Speciális beállítások** \> **hogyan érkeznek frissítések kiválasztása**.</span><span class="sxs-lookup"><span data-stu-id="38f00-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="38f00-113">Győződjön meg róla, hogy látható egy piros színű üzenet, mely jelzi, hogy egyes beállítások rejtettek vagy a szervezet által kezeltek, és hogy az összes beállítás kiszürkítve jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="38f00-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are greyed out.</span></span>
    
    ![Choose how updates are delivered page indicates settings are hidden or managed by your organization.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="38f00-115">A Windows Defender biztonsági központ megnyitásához nyissa meg a **Beállítások** \> **frissítés &amp; biztonsági** \> **A Windows Defender** \> kattintson a **Windows Defender a biztonsági központ** \> **vírus &amp; szál védelem** \> **vírus &amp; veszélyt a védelmi beállítások**.</span><span class="sxs-lookup"><span data-stu-id="38f00-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="38f00-116">Győződjön meg róla, hogy az összes beállítás kiszürkítve jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="38f00-116">Verify that all options are greyed out.</span></span> 
    
    ![The Virus and threat protection settings are greyed out.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="38f00-118">Kapcsolódó témakörök</span><span class="sxs-lookup"><span data-stu-id="38f00-118">Related Topics</span></span>

[<span data-ttu-id="38f00-119">A Microsoft 365 Business dokumentációja és forrásai</span><span class="sxs-lookup"><span data-stu-id="38f00-119">Microsoft 365 Business documentation and resources</span></span>](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[<span data-ttu-id="38f00-120">A Microsoft 365 Business használatbavétele</span><span class="sxs-lookup"><span data-stu-id="38f00-120">Get started with Microsoft 365 Business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="38f00-121">A Microsoft 365 Business kezelése</span><span class="sxs-lookup"><span data-stu-id="38f00-121">Manage Microsoft 365 Business</span></span>](manage.md)
  
[<span data-ttu-id="38f00-122">Eszközkonfigurációk megadása Windows 10-es PC-ken</span><span class="sxs-lookup"><span data-stu-id="38f00-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  


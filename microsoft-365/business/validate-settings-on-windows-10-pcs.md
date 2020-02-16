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
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Megtudhatja, hogy miként ellenőrizheti a Microsoft 365 Vállalati alkalmazásvédelmi beállításait Windows 10-es eszközökön.
ms.openlocfilehash: 1762382aec00a80e006cf38b66c28d02c0c25989
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/15/2020
ms.locfileid: "42056667"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="f3cc6-103">Eszközvédelmi beállítások érvényességének ellenőrzése Windows 10-es PC-ken</span><span class="sxs-lookup"><span data-stu-id="f3cc6-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="f3cc6-104">Windows 10-eszközházirendek érvénybe lépésének ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="f3cc6-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="f3cc6-105">Miután [beállította az eszközházirendeket](protection-settings-for-windows-10-pcs.md), néhány óra is eltelhet, amíg a házirendek érvénybe lépnek a felhasználók eszközein.</span><span class="sxs-lookup"><span data-stu-id="f3cc6-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="f3cc6-106">A házirendek érvénybe lépéséről úgy bizonyosodhat meg, ha ellenőrzi a felhasználók eszközein a Windows Gépház bizonyos beállításlapjait.</span><span class="sxs-lookup"><span data-stu-id="f3cc6-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="f3cc6-107">Mivel a felhasználók nem tudják módosítani a Windows Update és a Windows Defender víruskereső beállításait a Windows 10-es eszközeiken, számos lehetőség szürkén jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="f3cc6-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, many options will be grayed out.</span></span>
  
1. <span data-ttu-id="f3cc6-108">Nyissa meg a **Beállítások** \> **frissítése &amp; biztonsági** \> **Windows Update** \> Újraindítás **beállításait,** és ellenőrizze, hogy az összes beállítás szürkén jelenik-e meg.</span><span class="sxs-lookup"><span data-stu-id="f3cc6-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are grayed out.</span></span> 
    
    ![Az összes Újraindítás beállítás szürkén jelenik meg.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="f3cc6-110">Nyissa meg a **Beállítások** \> **frissítése &amp; biztonsági** \> **Windows Update** \> Speciális **beállításokat,** és ellenőrizze, hogy az összes beállítás szürkén jelenik-e meg.</span><span class="sxs-lookup"><span data-stu-id="f3cc6-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are grayed out.</span></span> 
    
    ![A Windows speciális frissítési beállításai mind szürkén jelennek meg.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="f3cc6-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span><span class="sxs-lookup"><span data-stu-id="f3cc6-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="f3cc6-113">Ellenőrizze, hogy látható-e az üzenet (pirossal) arról, hogy egyes beállítások rejtve vannak vagy a szervezet által kezeltek, és az összes beállítás szürkén jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="f3cc6-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are grayed out.</span></span>
    
    ![Choose how updates are delivered page indicates settings are hidden or managed by your organization.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="f3cc6-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span><span class="sxs-lookup"><span data-stu-id="f3cc6-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="f3cc6-116">Ellenőrizze, hogy minden beállítás szürkén jelenik-e meg.</span><span class="sxs-lookup"><span data-stu-id="f3cc6-116">Verify that all options are grayed out.</span></span> 
    
    ![A vírus- és veszélyforrások elleni védelem beállításai szürkén jelennek meg.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="f3cc6-118">Kapcsolódó témakörök</span><span class="sxs-lookup"><span data-stu-id="f3cc6-118">Related Topics</span></span>

[<span data-ttu-id="f3cc6-119">A Microsoft 365 Business dokumentációja és forrásai</span><span class="sxs-lookup"><span data-stu-id="f3cc6-119">Microsoft 365 Business documentation and resources</span></span>](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[<span data-ttu-id="f3cc6-120">A Microsoft 365 Business használatbavétele</span><span class="sxs-lookup"><span data-stu-id="f3cc6-120">Get started with Microsoft 365 Business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="f3cc6-121">A Microsoft 365 Business kezelése</span><span class="sxs-lookup"><span data-stu-id="f3cc6-121">Manage Microsoft 365 Business</span></span>](manage.md)
  
[<span data-ttu-id="f3cc6-122">Eszközkonfigurációk megadása Windows 10-es PC-ken</span><span class="sxs-lookup"><span data-stu-id="f3cc6-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  


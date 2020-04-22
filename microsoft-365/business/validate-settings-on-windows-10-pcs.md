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
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Megtudhatja, hogy miként ellenőrizheti, hogy a Microsoft 365 vállalati verziós alkalmazások védelmére vonatkozó beállítások érvénybe léptek-e a felhasználók Windows 10-es eszközein.
ms.openlocfilehash: b63681f040b0fe49127693e9cb7aac7ba6c41af6
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/21/2020
ms.locfileid: "43635704"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="5b447-103">Eszközvédelmi beállítások érvényességének ellenőrzése Windows 10-es PC-ken</span><span class="sxs-lookup"><span data-stu-id="5b447-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="5b447-104">Windows 10-eszközházirendek érvénybe lépésének ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="5b447-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="5b447-105">Miután [beállította az eszközházirendeket](protection-settings-for-windows-10-pcs.md), néhány óra is eltelhet, amíg a házirendek érvénybe lépnek a felhasználók eszközein.</span><span class="sxs-lookup"><span data-stu-id="5b447-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="5b447-106">A házirendek érvénybe lépéséről úgy bizonyosodhat meg, ha ellenőrzi a felhasználók eszközein a Windows Gépház bizonyos beállításlapjait.</span><span class="sxs-lookup"><span data-stu-id="5b447-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="5b447-107">Mivel a felhasználók nem tudják módosítani a Windows Update és a Windows Defender víruskereső beállításait a Windows 10-es eszközeiken, számos lehetőség szürkén jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="5b447-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, many options will be grayed out.</span></span>
  
1. <span data-ttu-id="5b447-108">Nyissa meg a **Beállítások** \> **frissítése &amp; biztonsági** \> **ablakok at A Windows Update** \> **Újraindítás beállításait,** és ellenőrizze, hogy minden beállítás szürkén jelenik-e meg.</span><span class="sxs-lookup"><span data-stu-id="5b447-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are grayed out.</span></span> 
    
    ![Az újraindítás imbusza szürkén jelenik meg.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="5b447-110">Nyissa meg a **Beállítások** \> **frissítése &amp; biztonsági** \> **ablakOt A Windows Update** \> Speciális **beállításait,** és ellenőrizze, hogy minden beállítás szürkén jelenik-e meg.</span><span class="sxs-lookup"><span data-stu-id="5b447-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are grayed out.</span></span> 
    
    ![A Windows Speciális frissítések beállításai szürkén jelennek meg.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="5b447-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span><span class="sxs-lookup"><span data-stu-id="5b447-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="5b447-113">Ellenőrizze, hogy láthatja-e az üzenetet (pirossal), hogy egyes beállítások at a szervezet rejtett vagy kezelt, és az összes beállítás szürkén jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="5b447-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are grayed out.</span></span>
    
    ![Choose how updates are delivered page indicates settings are hidden or managed by your organization.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="5b447-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span><span class="sxs-lookup"><span data-stu-id="5b447-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="5b447-116">Ellenőrizze, hogy minden beállítás szürkén jelenik-e meg.</span><span class="sxs-lookup"><span data-stu-id="5b447-116">Verify that all options are grayed out.</span></span> 
    
    ![A vírus- és veszélyforrások elleni védelem beállításai szürkén jelennek meg.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="5b447-118">Kapcsolódó témakörök</span><span class="sxs-lookup"><span data-stu-id="5b447-118">Related Topics</span></span>

[<span data-ttu-id="5b447-119">Microsoft 365 üzleti dokumentációés források</span><span class="sxs-lookup"><span data-stu-id="5b447-119">Microsoft 365 for business documentation and resources</span></span>](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[<span data-ttu-id="5b447-120">Ismerkedés a Microsoft 365 vállalati verzióval</span><span class="sxs-lookup"><span data-stu-id="5b447-120">Get started with Microsoft 365 for business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="5b447-121">A Microsoft 365 vállalati verzió kezelése</span><span class="sxs-lookup"><span data-stu-id="5b447-121">Manage Microsoft 365 for business</span></span>](manage.md)
  
[<span data-ttu-id="5b447-122">Eszközkonfigurációk megadása Windows 10-es PC-ken</span><span class="sxs-lookup"><span data-stu-id="5b447-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  


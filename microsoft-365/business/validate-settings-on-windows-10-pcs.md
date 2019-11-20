---
title: Appvédelmi beállítások érvényességének ellenőrzése Windows 10-es PC-ken
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
description: Útmutató a Microsoft 365 Business app védelmi beállításainak érvényesítéséhez Windows 10 eszközökön.
ms.openlocfilehash: b8793ab7f77bbc7f608f237e2455f6fd12c3bb26
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38721800"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="17a50-103">Eszközvédelmi beállítások érvényességének ellenőrzése Windows 10-es PC-ken</span><span class="sxs-lookup"><span data-stu-id="17a50-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="17a50-104">Windows 10-eszközházirendek érvénybe lépésének ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="17a50-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="17a50-105">Miután [beállította az eszközházirendeket](protection-settings-for-windows-10-pcs.md), néhány óra is eltelhet, amíg a házirendek érvénybe lépnek a felhasználók eszközein.</span><span class="sxs-lookup"><span data-stu-id="17a50-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="17a50-106">A házirendek érvénybe lépéséről úgy bizonyosodhat meg, ha ellenőrzi a felhasználók eszközein a Windows Gépház bizonyos beállításlapjait.</span><span class="sxs-lookup"><span data-stu-id="17a50-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="17a50-107">Mivel a felhasználók nem tudják módosítani a Windows Update és a Windows Defender víruskereső beállításait a Windows 10 eszközükön, számos beállítás kiszürkítve jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="17a50-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, many options will be grayed out.</span></span>
  
1. <span data-ttu-id="17a50-108">Megy **elintézés** \> **korszerűsíteni &amp; biztonság** \> **Windows Korszerűsíteni** \> **újból kifejt választások** és igazol amit minden elintézés van szürke ki.</span><span class="sxs-lookup"><span data-stu-id="17a50-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are grayed out.</span></span> 
    
    ![Minden újraindítási beállítás szürkén jelenik meg.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="17a50-110">Megy **elintézés** \> \*\* &amp; korszerűsíteni biztonság\*\* \> **Windows Korszerűsíteni** \> **haladó választások** és igazol amit minden elintézés van szürke ki.</span><span class="sxs-lookup"><span data-stu-id="17a50-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are grayed out.</span></span> 
    
    ![A Windows speciális frissítések beállításai mind szürkén jelennek meg.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="17a50-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span><span class="sxs-lookup"><span data-stu-id="17a50-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="17a50-113">Ellenőrizze, hogy az üzenet (piros) látható-e a szervezet által elrejtett vagy kezelt egyes beállításokkal, és az összes beállítás ki van-e szürkítve.</span><span class="sxs-lookup"><span data-stu-id="17a50-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are grayed out.</span></span>
    
    ![Choose how updates are delivered page indicates settings are hidden or managed by your organization.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="17a50-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span><span class="sxs-lookup"><span data-stu-id="17a50-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="17a50-116">Ellenőrizze, hogy minden beállítás ki van-e szürkítve.</span><span class="sxs-lookup"><span data-stu-id="17a50-116">Verify that all options are grayed out.</span></span> 
    
    ![A vírus-és veszélyvédelmi beállítások szürkén jelennek meg.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="17a50-118">Kapcsolódó témakörök</span><span class="sxs-lookup"><span data-stu-id="17a50-118">Related Topics</span></span>

[<span data-ttu-id="17a50-119">A Microsoft 365 Business dokumentációja és forrásai</span><span class="sxs-lookup"><span data-stu-id="17a50-119">Microsoft 365 Business documentation and resources</span></span>](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[<span data-ttu-id="17a50-120">A Microsoft 365 Business használatbavétele</span><span class="sxs-lookup"><span data-stu-id="17a50-120">Get started with Microsoft 365 Business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="17a50-121">A Microsoft 365 Business kezelése</span><span class="sxs-lookup"><span data-stu-id="17a50-121">Manage Microsoft 365 Business</span></span>](manage.md)
  
[<span data-ttu-id="17a50-122">Eszközkonfigurációk megadása Windows 10-es PC-ken</span><span class="sxs-lookup"><span data-stu-id="17a50-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  


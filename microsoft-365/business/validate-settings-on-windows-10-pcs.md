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
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>Eszközvédelmi beállítások érvényességének ellenőrzése Windows 10-es PC-ken

## <a name="verify-that-windows-10-device-policies-are-set"></a>Windows 10-eszközházirendek érvénybe lépésének ellenőrzése

Miután [beállította az eszközházirendeket](protection-settings-for-windows-10-pcs.md), néhány óra is eltelhet, amíg a házirendek érvénybe lépnek a felhasználók eszközein. A házirendek érvénybe lépéséről úgy bizonyosodhat meg, ha ellenőrzi a felhasználók eszközein a Windows Gépház bizonyos beállításlapjait. Mivel a felhasználók nem tudják módosítani a Windows Update és a Windows Defender víruskereső beállításait a Windows 10 eszközükön, számos beállítás kiszürkítve jelenik meg.
  
1. Megy **elintézés** \> **korszerűsíteni &amp; biztonság** \> **Windows Korszerűsíteni** \> **újból kifejt választások** és igazol amit minden elintézés van szürke ki. 
    
    ![Minden újraindítási beállítás szürkén jelenik meg.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. Megy **elintézés** \> ** &amp; korszerűsíteni biztonság** \> **Windows Korszerűsíteni** \> **haladó választások** és igazol amit minden elintézés van szürke ki. 
    
    ![A Windows speciális frissítések beállításai mind szürkén jelennek meg.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.
    
    Ellenőrizze, hogy az üzenet (piros) látható-e a szervezet által elrejtett vagy kezelt egyes beállításokkal, és az összes beállítás ki van-e szürkítve.
    
    ![Choose how updates are delivered page indicates settings are hidden or managed by your organization.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**. 
    
5. Ellenőrizze, hogy minden beállítás ki van-e szürkítve. 
    
    ![A vírus-és veszélyvédelmi beállítások szürkén jelennek meg.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Kapcsolódó témakörök

[A Microsoft 365 Business dokumentációja és forrásai](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[A Microsoft 365 Business használatbavétele](microsoft-365-business-overview.md)
  
[A Microsoft 365 Business kezelése](manage.md)
  
[Eszközkonfigurációk megadása Windows 10-es PC-ken](protection-settings-for-windows-10-pcs.md)
  


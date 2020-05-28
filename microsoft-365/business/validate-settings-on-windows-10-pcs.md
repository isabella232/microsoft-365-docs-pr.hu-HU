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
description: Megtudhatja, hogy miként ellenőrizheti, hogy a Microsoft 365 vállalati verziós alkalmazások védelmére vonatkozó beállítások érvénybe léptek-e a felhasználók Windows 10-es eszközein.
ms.openlocfilehash: 39aee3bc811cb0090d58f9a282de7a8162c097b3
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403590"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>Eszközvédelmi beállítások érvényességének ellenőrzése Windows 10-es PC-ken

## <a name="verify-that-windows-10-device-policies-are-set"></a>Windows 10-eszközházirendek érvénybe lépésének ellenőrzése

Miután [beállította az eszközházirendeket](protection-settings-for-windows-10-pcs.md), néhány óra is eltelhet, amíg a házirendek érvénybe lépnek a felhasználók eszközein. A házirendek érvénybe lépéséről úgy bizonyosodhat meg, ha ellenőrzi a felhasználók eszközein a Windows Gépház bizonyos beállításlapjait. Mivel a felhasználók nem tudják módosítani a Windows Update és a Windows Defender víruskereső beállításait a Windows 10-es eszközeiken, számos lehetőség szürkén jelenik meg.
  
1. Nyissa meg a **Beállítások** \> **frissítése &amp; biztonsági** \> **ablakok at A Windows Update** \> **Újraindítás beállításait,** és ellenőrizze, hogy minden beállítás szürkén jelenik-e meg. 
    
    ![Az újraindítás imbusza szürkén jelenik meg.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. Nyissa meg a **Beállítások** \> **frissítése &amp; biztonsági** \> **ablakOt A Windows Update** Speciális \> **beállításait,** és ellenőrizze, hogy minden beállítás szürkén jelenik-e meg. 
    
    ![A Windows Speciális frissítések beállításai szürkén jelennek meg.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.
    
    Ellenőrizze, hogy láthatja-e az üzenetet (pirossal), hogy egyes beállítások at a szervezet rejtett vagy kezelt, és az összes beállítás szürkén jelenik meg.
    
    ![Choose how updates are delivered page indicates settings are hidden or managed by your organization.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**. 
    
5. Ellenőrizze, hogy minden beállítás szürkén jelenik-e meg. 
    
    ![A vírus- és veszélyforrások elleni védelem beállításai szürkén jelennek meg.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Kapcsolódó témakörök

[Microsoft 365 üzleti dokumentációés források](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Ismerkedés a Microsoft 365 vállalati verzióval](microsoft-365-business-overview.md)
  
[A Microsoft 365 vállalati verzió kezelése](manage.md)
  
[Eszközkonfigurációk megadása Windows 10-es PC-ken](protection-settings-for-windows-10-pcs.md)
  


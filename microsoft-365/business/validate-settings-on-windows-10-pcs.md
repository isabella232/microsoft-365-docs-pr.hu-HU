---
title: Az appvédelmi beállítások ellenőrzése Windows 10 PC-khez
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
description: Megtudhatja, hogyan ellenőrizheti, hogy Microsoft 365 Vállalati verziós appvédelmi beállítások hatályba lépnek-e a felhasználók Windows 10 eszközein.
ms.openlocfilehash: 464a246a0da65dcffeb70946287ce4fa0e67ae7c
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/14/2021
ms.locfileid: "52925259"
---
# <a name="validate-device-protection-settings-for-windows-10-pcs"></a>Eszközvédelmi beállítások ellenőrzése Windows 10 PC-khez

## <a name="verify-that-windows-10-device-policies-are-set"></a>Windows 10-eszközházirendek érvénybe lépésének ellenőrzése

Miután [beállította az eszközházirendeket](protection-settings-for-windows-10-pcs.md), néhány óra is eltelhet, amíg a házirendek érvénybe lépnek a felhasználók eszközein. A házirendek érvénybe lépéséről úgy bizonyosodhat meg, ha ellenőrzi a felhasználók eszközein a Windows Gépház bizonyos beállításlapjait. Mivel a felhasználók nem tudják módosítani a Windows Frissítési és Windows Defender víruskereső beállításokat a Windows 10-eszközeiken, számos beállítás szürkén jelenik meg.
  
1. A Biztonsági **beállítások Gépház** újraindítási Windows lapon ellenőrizze, hogy az összes beállítás szürkén \> **&amp;** \>  \>  jelenik-e meg. 
    
    ![Az Újraindítási beállítások szürkén jelennek meg.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. A Biztonsági **Gépház** és Windows beállítások frissítése lehetőséget, és győződjön meg arról, hogy az összes beállítás \> **&amp;** \>  \>  szürkén jelenik meg. 
    
    ![Windows A speciális frissítések beállításai szürkén jelennek meg.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.
    
    Győződjön meg arról, hogy látja (piros színnel) azt az üzenetet, hogy egyes beállítások rejtettek vagy a szervezet által kezeltek, és hogy az összes beállítás szürkén jelenik meg.
    
    ![Choose how updates are delivered page indicates settings are hidden or managed by your organization.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**. 
    
5. Ellenőrizze, hogy minden beállítás szürkén jelenik-e meg. 
    
    ![A vírus- és veszélyforrás-védelmi beállítások szürkén jelennek meg.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Kapcsolódó témakörök

[Microsoft 365 vállalati verzió dokumentációja és forrásai](./index.yml)
  
[Első lépések a Microsoft 365 vállalati verzióban](microsoft-365-business-overview.md)
  
[Vállalati Microsoft 365 kezelése](manage.md)
  
[Eszközkonfigurációk megadása Windows 10-es PC-ken](protection-settings-for-windows-10-pcs.md)

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
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>Eszközvédelmi beállítások érvényességének ellenőrzése Windows 10-es PC-ken

## <a name="verify-that-windows-10-device-policies-are-set"></a>Windows 10-eszközházirendek érvénybe lépésének ellenőrzése

Miután [beállította az eszközházirendeket](protection-settings-for-windows-10-pcs.md), néhány óra is eltelhet, amíg a házirendek érvénybe lépnek a felhasználók eszközein. A házirendek érvénybe lépéséről úgy bizonyosodhat meg, ha ellenőrzi a felhasználók eszközein a Windows Gépház bizonyos beállításlapjait. Mivel a házirendek használatakor a felhasználók nem módosíthatják a Windows Update és a Windows Defender víruskereső beállításait a Windows 10-es eszközeiken, sok beállításnak kiszürkítve kell megjelennie.
  
1. Menjen a **Beállítások** \> **frissítés &amp; biztonsági** \> **A Windows Update** \> **Indítsa újra a beállításokat** , és győződjön meg arról, hogy minden beállítás szürkévé. 
    
    ![All the Restart options are greyed out.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. Ugrás a **Beállítások** \> **frissítés &amp; biztonsági** \> **A Windows Update** \> **Speciális beállítások** , és győződjön meg arról, hogy minden beállítás szürkévé. 
    
    ![Windows Advanced updates options are all greyed out.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Ugrás a **Beállítások** \> **frissítés &amp; biztonsági** \> **A Windows Update** \> **Speciális beállítások** \> **hogyan érkeznek frissítések kiválasztása**.
    
    Győződjön meg róla, hogy látható egy piros színű üzenet, mely jelzi, hogy egyes beállítások rejtettek vagy a szervezet által kezeltek, és hogy az összes beállítás kiszürkítve jelenik meg.
    
    ![Choose how updates are delivered page indicates settings are hidden or managed by your organization.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. A Windows Defender biztonsági központ megnyitásához nyissa meg a **Beállítások** \> **frissítés &amp; biztonsági** \> **A Windows Defender** \> kattintson a **Windows Defender a biztonsági központ** \> **vírus &amp; szál védelem** \> **vírus &amp; veszélyt a védelmi beállítások**. 
    
5. Győződjön meg róla, hogy az összes beállítás kiszürkítve jelenik meg. 
    
    ![The Virus and threat protection settings are greyed out.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Kapcsolódó témakörök

[A Microsoft 365 Business dokumentációja és forrásai](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[A Microsoft 365 Business használatbavétele](microsoft-365-business-overview.md)
  
[A Microsoft 365 Business kezelése](manage.md)
  
[Eszközkonfigurációk megadása Windows 10-es PC-ken](protection-settings-for-windows-10-pcs.md)
  


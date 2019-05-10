---
title: Alkalmazásvédelmi beállítások megadása Windows 10-es eszközökhöz
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
f1_keywords:
- Win10AppPolicy
- O365E_Win10AppPolicy
- BCS365_Win10AppPolicy
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Útmutató az app adatkezelési házirend létrehozása és munka fájlok Windows 10 eszközök védelme.
ms.openlocfilehash: f649454417dceae05255df6b37760af99c0b8d4f
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660374"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a>Alkalmazásvédelmi beállítások megadása Windows 10-es eszközökhöz

## <a name="create-an-app-management-policy-for-windows-10"></a>Appkezelési házirend létrehozása Windows 10-es eszközhöz

Ha a felhasználók munkahelyi feladatokra is használják saját Windows 10-es eszközeiket, az azokon tárolt munkahelyi adatok is védhetők.
  
1. Ugrás az admin center <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>. 
    
2. A bal oldali navigációs sáv, válassza az **eszközök** \> **politika** \> **hozzáadása**.

3. A **Házirend felvétele** ablaktáblában adja meg a házirend egyedi nevét. 
    
4. A **Házirend típusa** beállításnál válassza az **Alkalmazáskezelés Windows 10-es eszközökhöz** lehetőséget.
    
5. **Eszköz típusa**csoportban válasszon a **személyes** vagy a **Vállalat birtokában**.
    
6. A **Munkahelyi fájlok titkosítása** lehetőség automatikusan be van kapcsolva. 
    
7. Ha nem szeretné, hogy a felhasználók a saját számítógépükre mentsék a munkahelyi fájlokat, állítsa **A felhasználók nem másolhatnak céges adatokat saját fájljaikba, a munkahelyi fájlokat pedig csak a OneDrive Vállalati verzióba menthetik** beállítást **Be** értékre. 
    
9. Bontsa ki a **Windowsos eszközökön lévő adatok helyreállítása** beállítást, és ajánlott, hogy azt állítsa **Be** értékre.
    
    Ahhoz, hogy megkereshesse az adat-helyreállítási megbízott tanúsítványának helyét, először létre kell hoznia egyet. Pontos utasításokat [A titkosított fájlrendszer (EFS) adat-helyreállítási megbízottja (DRA) tanúsítványának létrehozása és ellenőrzése](https://go.microsoft.com/fwlink/p/?linkid=853700) című témakörben találhat.
    
    A munkahelyi fájlok alapértelmezés szerint egy az eszközön tárolt és a felhasználó profiljához társított titkos kulccsal vannak titkosítva. Csak a felhasználó tudja megnyitni és visszafejteni a fájlt. Így tehát, ha valaki elveszít egy eszközt, vagy törölnek egy felhasználót, egy szükséges fájl titkosított állapotban ragadhat. A kizárólag rendszergazda által használható adat-helyreállítási megbízott (DRA) tanúsítvánnyal visszafejthető a fájl.
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. Bontsa ki a **További hálózati és felhőbeli helyek védelme** beállítást, ha szeretne további tartományokat vagy SharePoint Online-helyeket felvenni a felsorolt appokban lévő fájlok védelmének biztosítása érdekében. Ha bármelyik mezőben egynél több elemet kell megadnia, pontosvesszővel (;) válassza el őket egymástól.
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.
    
12. Végül válassza a **Hozzáadás** lehetőséget a házirend mentéséhez és eszközökhöz való hozzárendeléséhez. 
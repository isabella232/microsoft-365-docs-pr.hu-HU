---
title: Alkalmazásvédelmi beállítások megadása Windows 10-es eszközökhöz
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Itt megtudhatja, hogyan hozhat létre Alkalmazáskezelési házirendet, és védheti a Windows 10 eszközökön lévő munkahelyi fájlokat.
ms.openlocfilehash: ca6d789e0242975a0395e6cf5653d3f43f819801
ms.sourcegitcommit: 5d11f516e78ea4a74145e19ba2300f0792c8bac1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38715252"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a>Alkalmazásvédelmi beállítások megadása Windows 10-es eszközökhöz

## <a name="create-an-app-management-policy-for-windows-10"></a>Appkezelési házirend létrehozása Windows 10-es eszközhöz

Ha a felhasználók munkahelyi feladatokra is használják saját Windows 10-es eszközeiket, az azokon tárolt munkahelyi adatok is védhetők.
  
1. Menj az admin központba <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>. 
    
2. Kattintson a bal oldali NAV \> **eszközházirendek** \> **hozzáadása**parancsára. ****

3. A **Házirend felvétele** ablaktáblában adja meg a házirend egyedi nevét. 
    
4. A **Házirend típusa** beállításnál válassza az **Alkalmazáskezelés Windows 10-es eszközökhöz** lehetőséget.
    
5. Az **eszköztípus**területen válassza a **személyes** vagy **vállalati tulajdont**.
    
6. A **Munkahelyi fájlok titkosítása** lehetőség automatikusan be van kapcsolva. 
    
7. Ha nem szeretné, hogy a felhasználók a saját számítógépükre mentsék a munkahelyi fájlokat, állítsa **A felhasználók nem másolhatnak céges adatokat saját fájljaikba, a munkahelyi fájlokat pedig csak a OneDrive Vállalati verzióba menthetik** beállítást **Be** értékre. 
    
9. Bontsa ki az **adatok helyreállítása Windows-eszközökön**. Javasoljuk **, hogy kapcsolja be.**
    
    Ahhoz, hogy megkereshesse az adat-helyreállítási megbízott tanúsítványának helyét, először létre kell hoznia egyet. További útmutatást a [titkosító fájlrendszer (EFS) adat-helyreállítási megbízott (DRA) tanúsítványának létrehozása és ellenőrzése](https://go.microsoft.com/fwlink/p/?linkid=853700)című témakörben talál.
    
    A munkahelyi fájlok alapértelmezés szerint egy az eszközön tárolt és a felhasználó profiljához társított titkos kulccsal vannak titkosítva. Csak a felhasználó tudja megnyitni és visszafejteni a fájlt. Így tehát, ha valaki elveszít egy eszközt, vagy törölnek egy felhasználót, egy szükséges fájl titkosított állapotban ragadhat. A rendszergazda az adat-helyreállítási megbízott (DRA) tanúsítványa segítségével visszafejtheti a fájlt.
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. Bontsa ki a **további hálózati és felhőalapú helyek védelmét** , ha további tartományokat vagy SharePoint Online-helyeket szeretne hozzáadni, hogy megbizonyosodjon arról, hogy a felsorolt alkalmazások fájljai védve vannak. Ha bármelyik mezőben egynél több elemet kell megadnia, pontosvesszővel (;) válassza el őket egymástól.
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.
    
12. Végül válassza a **Hozzáadás** lehetőséget a házirend mentéséhez és eszközökhöz való hozzárendeléséhez. 
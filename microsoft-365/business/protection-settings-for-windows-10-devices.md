---
title: Windows 10-es eszközök alkalmazás-védelmi beállításainak szerkesztése és beállítása
f1.keywords:
- NOCSH
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Megtudhatja, hogy miként hozhat létre és szerkeszthet app-kezelési házirendeket, és hogyan védheti a munkahelyi fájlokat a felhasználók személyes Windows 10-es eszközein.
ms.openlocfilehash: f85a59649e43c141b62091337b842a490d411833
ms.sourcegitcommit: abf63669daf12993ad3353e4b578f41c8910b20f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/27/2020
ms.locfileid: "47289199"
---
# <a name="set-or-edit-application-protection-settings-for-windows-10-devices"></a>Alkalmazás-védelmi beállítások megadása vagy szerkesztése Windows 10-es eszközökön

Ez a cikk a Microsoft 365 vállalati prémium verzióra vonatkozik.

## <a name="edit-an-app-management-policy-for-windows-10"></a>A Windows 10 app-kezelési házirendjének szerkesztése

1. Nyissa meg a felügyeleti központot <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .     
2. A bal oldali navigációs sávon válassza az **eszközök** \> **házirendek** elemet.
1. Válasszon egy meglévő Windows-alkalmazás-házirendet, és kattintson a **Szerkesztés**elemre.
1. Válassza a **Szerkesztés** lehetőséget a módosítani kívánt beállítás mellett, majd kattintson a **Mentés**gombra.

## <a name="create-an-app-management-policy-for-windows-10"></a>Appkezelési házirend létrehozása Windows 10-es eszközhöz

Ha a felhasználók munkahelyi feladatokra is használják saját Windows 10-es eszközeiket, az azokon tárolt munkahelyi adatok is védhetők.
  
1. Nyissa meg a felügyeleti központot <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> . 
2. A bal oldali navigációs sávon válassza az **eszközök** \> **házirendek** \> **hozzáadása**lehetőséget.
3. A **Házirend felvétele** ablaktáblában adja meg a házirend egyedi nevét. 
4. A **Házirend típusa** beállításnál válassza az **Alkalmazáskezelés Windows 10-es eszközökhöz** lehetőséget.
5. Az **eszköz típusa**csoportban válassza a **személyes** vagy a **vállalati**verzió lehetőséget.
6. A **Munkahelyi fájlok titkosítása** lehetőség automatikusan be van kapcsolva. 
7. Ha nem szeretné, hogy a felhasználók a saját számítógépükre mentsék a munkahelyi fájlokat, állítsa **A felhasználók nem másolhatnak céges adatokat saját fájljaikba, a munkahelyi fájlokat pedig csak a OneDrive Vállalati verzióba menthetik** beállítást **Be** értékre. 
9. Bontsa ki **a Windows-eszközökön tárolt adathelyreállítást**. Azt javasoljuk, hogy kapcsolja be **.**
    Ahhoz, hogy megkereshesse az adat-helyreállítási megbízott tanúsítványának helyét, először létre kell hoznia egyet. Útmutatást a [titkosított fájlrendszer (EFS) adathelyreállítási megbízotti tanúsítvány létrehozása és ellenőrzése](https://go.microsoft.com/fwlink/p/?linkid=853700)című témakörben találhat.
    
    A munkahelyi fájlok alapértelmezés szerint egy az eszközön tárolt és a felhasználó profiljához társított titkos kulccsal vannak titkosítva. Csak a felhasználó tudja megnyitni és visszafejteni a fájlt. Így tehát, ha valaki elveszít egy eszközt, vagy törölnek egy felhasználót, egy szükséges fájl titkosított állapotban ragadhat. A rendszergazda az adathelyreállítási megbízott (DRA) tanúsítvány segítségével visszafejtheti a fájlt.
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. Bontsa ki a **további hálózati és Felhőbeli helyek védelme** lehetőséget, ha további tartományokat vagy SharePoint Online-helyeket szeretne hozzáadni, és győződjön meg arról, hogy a felsorolt alkalmazások fájljai védettek. Ha bármelyik mezőben egynél több elemet kell megadnia, pontosvesszővel (;) válassza el őket egymástól.
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.
12. Végül válassza a **Hozzáadás** lehetőséget a házirend mentéséhez és eszközökhöz való hozzárendeléséhez. 

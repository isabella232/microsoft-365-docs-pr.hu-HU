---
title: Alkalmazásvédelmi beállítások szerkesztése vagy beállítása Windows 10-es eszközökhöz
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
description: Megtudhatja, hogy miként hozhat létre és szerkeszthet alkalmazáskezelési házirendeket, és hogyan védheti meg a munkahelyi fájlokat a felhasználók személyes Windows 10-es eszközein.
ms.openlocfilehash: aa270c563e6bdce6fd48f8713d7db3ce23921925
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580014"
---
# <a name="set-or-edit-application-protection-settings-for-windows-10-devices"></a>Alkalmazásvédelmi beállítások megadása és szerkesztése Windows 10-es eszközökhöz

Ez a cikk a Microsoft 365 Vállalati prémium verzióra vonatkozik.

## <a name="edit-an-app-management-policy-for-windows-10"></a>Alkalmazáskezelési házirend szerkesztése Windows 10-ben

1. A felügyeleti központ megnyitásához: <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .     
2. A bal oldali  navigációs sávon válassza az Eszköz \> **házirendek lehetőséget.**
1. Válasszon ki egy meglévő Windows-alkalmazás-házirendet, majd a **Szerkesztés gombra.**
1. Válassza **a Szerkesztés** lehetőséget a módosítani kívánt beállítás mellett, majd a Mentés **gombra.**

## <a name="create-an-app-management-policy-for-windows-10"></a>Appkezelési házirend létrehozása Windows 10-es eszközhöz

Ha a felhasználók munkahelyi feladatokra is használják saját Windows 10-es eszközeiket, az azokon tárolt munkahelyi adatok is védhetők.
  
1. A felügyeleti központ megnyitásához: <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> . 
2. A bal oldali navigációs sávon válassza az **Eszköz** \> **házirendek hozzáadása** \> **lehetőséget.**
3. A **Házirend felvétele** ablaktáblában adja meg a házirend egyedi nevét. 
4. A **Házirend típusa** beállításnál válassza az **Alkalmazáskezelés Windows 10-es eszközökhöz** lehetőséget.
5. Az **Eszköz típusa alatt** válassza a Személyes vagy a **Céges** **lehetőséget.**
6. A **Munkahelyi fájlok titkosítása** lehetőség automatikusan be van kapcsolva. 
7. Ha nem szeretné, hogy a felhasználók a saját számítógépükre mentsék a munkahelyi fájlokat, állítsa **A felhasználók nem másolhatnak céges adatokat saját fájljaikba, a munkahelyi fájlokat pedig csak a OneDrive Vállalati verzióba menthetik** beállítást **Be** értékre. 
9. **Bontsa ki az Adatok helyreállítása Windows-eszközökön bontsa ki az adatokat.** Azt javasoljuk, hogy kapcsolja **be.**
    Ahhoz, hogy megkereshesse az adat-helyreállítási megbízott tanúsítványának helyét, először létre kell hoznia egyet. Az utasításokat a Titkosított fájlrendszer (EFS) adat-helyreállítási [megbízottja (DRA)](/windows/security/information-protection/windows-information-protection/create-and-verify-an-efs-dra-certificate)tanúsítványának létrehozása és ellenőrzése.
    
    A munkahelyi fájlok alapértelmezés szerint egy az eszközön tárolt és a felhasználó profiljához társított titkos kulccsal vannak titkosítva. Csak a felhasználó tudja megnyitni és visszafejteni a fájlt. Így tehát, ha valaki elveszít egy eszközt, vagy törölnek egy felhasználót, egy szükséges fájl titkosított állapotban ragadhat. A rendszergazda az adat-helyreállítási megbízott (DRA) tanúsítványával visszafejtheti a fájlt.
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. **Bontsa** ki a További hálózati és felhőbeli helyek védelme lehetőséget, ha további tartományokat vagy SharePoint Online-helyeket szeretne felvenni, hogy a felsorolt appokban lévő fájlok védettek legyen. Ha bármelyik mezőben egynél több elemet kell megadnia, pontosvesszővel (;) válassza el őket egymástól.
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.
12. Végül válassza a **Hozzáadás** lehetőséget a házirend mentéséhez és eszközökhöz való hozzárendeléséhez.
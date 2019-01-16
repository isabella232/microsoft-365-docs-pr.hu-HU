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
ms.openlocfilehash: acf19a72d994185a35b2e425f8334a73a121ee10
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982825"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a>Alkalmazásvédelmi beállítások megadása Windows 10-es eszközökhöz

## <a name="create-an-app-management-policy-for-windows-10"></a>Appkezelési házirend létrehozása Windows 10-es eszközhöz

Ha a felhasználók munkahelyi feladatokra is használják saját Windows 10-es eszközeiket, az azokon tárolt munkahelyi adatok is védhetők.
  
1. Jelentkezzen be a [Microsoft 365 Vállalati verzióba](https://portal.office.com) globális rendszergazdai hitelesítő adatokkal. Az **Admin** csempét választva lépjen a felügyeleti központba. 
    
2. A felügyeleti portál **Eszközházirendek** kártyáján válassza a **Házirend felvétele** lehetőséget.
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. A **Házirend felvétele** ablaktáblában adja meg a házirend egyedi nevét. 
    
4. A **Házirend típusa** beállításnál válassza az **Alkalmazáskezelés Windows 10-es eszközökhöz** lehetőséget.
    
5. A ** eszköztípus **, válassza a **személyes** vagy a **Vállalat birtokában**.
    
6. A **Munkahelyi fájlok titkosítása** lehetőség automatikusan be van kapcsolva. 
    
7. Ha nem szeretné, hogy a felhasználók a saját számítógépükre mentsék a munkahelyi fájlokat, állítsa **A felhasználók nem másolhatnak céges adatokat saját fájljaikba, a munkahelyi fájlokat pedig csak a OneDrive Vállalati verzióba menthetik** beállítást **Be** értékre. 
    
8. Bontsa ki a **kezelése, hogy a felhasználók miként férhetnek hozzá a eszközök Office fájlok** \> hogyan szeretné a beállításokat. Alapértelmezés szerint nincs **bekapcsolva** a **kezelése, hogy a felhasználók miként férhetnek hozzá a mobil eszközökön található Office-eszközöket** , de ajánlott, hogy kapcsolja **be** , és elfogadhatja az alapértelmezett értékeket. További tudnivalókért tanulmányozza a [rendelkezésre álló beállításokat](protection-settings-for-windows-10-devices.md#bkmk_settings) . 
    
    Az **Alapértelmezett beállítások visszaállítása** hivatkozásra kattintva bármikor visszatérhet az alapértelmezett beállításokhoz. 
    
9. Bontsa ki a **Windowsos eszközökön lévő adatok helyreállítása** beállítást, és ajánlott, hogy azt állítsa **Be** értékre.
    
    Ahhoz, hogy megkereshesse az adat-helyreállítási megbízott tanúsítványának helyét, először létre kell hoznia egyet. Pontos utasításokat [A titkosított fájlrendszer (EFS) adat-helyreállítási megbízottja (DRA) tanúsítványának létrehozása és ellenőrzése](https://go.microsoft.com/fwlink/p/?linkid=853700) című témakörben találhat.
    
    A munkahelyi fájlok alapértelmezés szerint egy az eszközön tárolt és a felhasználó profiljához társított titkos kulccsal vannak titkosítva. Csak a felhasználó tudja megnyitni és visszafejteni a fájlt. Így tehát, ha valaki elveszít egy eszközt, vagy törölnek egy felhasználót, egy szükséges fájl titkosított állapotban ragadhat. A kizárólag rendszergazda által használható adat-helyreállítási megbízott (DRA) tanúsítvánnyal visszafejthető a fájl.
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. Bontsa ki a **További hálózati és felhőbeli helyek védelme** beállítást, ha szeretne további tartományokat vagy SharePoint Online-helyeket felvenni a felsorolt appokban lévő fájlok védelmének biztosítása érdekében. Ha bármelyik mezőben egynél több elemet kell megadnia, pontosvesszővel (;) válassza el őket egymástól. 
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. Ezután döntse el, **fog kapni, akik ezeket a beállításokat?** Ha nem szeretné az alapértelmezett **Felhasználók** biztonsági csoporthoz, választhat **módosítása**, a biztonsági csoportok, akik ezeket a beállításokat kap \> **kiválasztása**.
    
12. Végül válassza a **Hozzáadás** lehetőséget a házirend mentéséhez és eszközökhöz való hozzárendeléséhez. 
    
## <a name="available-settings"></a>Rendelkezésre álló beállítások

Az alábbi beállítások használhatók a munkahelyi Office-fájlok elérésének kezelésére.
  
További információt [A Microsoft 365 Vállalati verzió védelmi funkcióinak megfelelő Intune-beállítások](map-protection-features-to-intune-settings.md) című témakörben talál.
  
|**Beállítás**|**Leírás**|
|:-----|:-----|
|PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez  <br/> |Ha ez a beállítás **Be** állapotban van, a mobileszközön lévő Office-appok használatához a felhasználónéven és a jelszón kívül a felhasználóknak további hitelesítési módszert is használniuk kell.  <br/> |
|PIN-kód visszaállítása ennyi sikertelen bejelentkezési kísérlet után  <br/> |Annak érdekében, hogy ne lehessen a PIN-kódot véletlenszerű próbálkozásokkal megfejteni, az Ön által megadott számú téves próbálkozás után a PIN-kód alaphelyzetbe áll.  <br/> |
|A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után  <br/> |Ezzel a beállítással azt határozhatja meg, hogy a felhasználó mennyi ideig maradhat inaktív, mielőtt újra be kellene jelentkeznie.  <br/> |
   


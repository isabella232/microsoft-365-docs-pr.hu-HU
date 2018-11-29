---
title: Appvédelmi beállítások megadása androidos vagy iOS-es eszközökhöz
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
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Útmutató létrehozása, szerkesztése, vagy app kezelési házirend törlése és Android vagy iOS eszközökön Munkafájlok védelme.
ms.openlocfilehash: ed03227496120369b94bf2396974eebfd7798678
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983665"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a>Appvédelmi beállítások megadása androidos vagy iOS-es eszközökhöz

## <a name="create-an-app-management-policy"></a>Appkezelési házirend létrehozása

1. Jelentkezzen be a [Microsoft 365 Business](https://portal.office.com) szolgáltatásba globális rendszergazdai hitelesítő adatokkal. 
    
2. A felügyeleti központ **Eszközházirendek** kártyáján válassza a **Házirend felvétele** lehetőséget.
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. A **Házirend felvétele** ablaktáblában adja meg a házirend egyedi nevét. 
    
4. A **Házirend típusa** csoportban válassza az **Alkalmazáskezelés Android-eszközökhöz** vagy az **Alkalmazáskezelés iOS-eszközökhöz** lehetőséget attól függően, hogy milyen házirendkészletet szeretne létrehozni. 
    
5. Bontsa ki a **védelem Munkafájlok, ha az eszköz elveszett vagy ellopott** és **kezelése, hogy a felhasználók miként férhetnek hozzá a mobil eszközökön található Office-fájlok** \> hogyan szeretné a beállításokat. Alapértelmezés szerint nincs **bekapcsolva** **kezelése, hogy a felhasználók miként férhetnek hozzá a mobil eszközökön található Office-fájlokat** , de javasoljuk, hogy kapcsolja **be** , és elfogadhatja az alapértelmezett értékeket. További tudnivalókért tanulmányozza a [rendelkezésre álló beállításokat](app-protection-settings-for-android-and-ios.md#bkmk_availablesettings) . 
    
    Az **Alapértelmezett beállítások visszaállítása** hivatkozásra kattintva bármikor visszatérhet az alapértelmezett beállításokhoz. 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. Ezután döntse el, **fog kapni, akik ezeket a beállításokat?** Ha nem szeretné az alapértelmezett **Felhasználók** biztonsági csoporthoz, választhat **módosítása**, a biztonsági csoportok, akik ezeket a beállításokat kap \> **kiválasztása**.
    
7. Végül válassza a **Kész** lehetőséget a házirend mentéséhez és eszközökhöz való hozzárendeléséhez. 
    
## <a name="edit-an-app-management-policy"></a>Appkezelési házirend szerkesztése

1. A **házirendek** kartonon válassza a **házirend szerkesztése**.
    
2. A **Házirend szerkesztése** ablaktáblában válassza ki a módosítani kívánt házirendet. 
    
3. Válassza a **Szerkesztés** elemet az egyes beállítások mellett a házirend értékeinek módosításához. Amikor módosít egy értéket, azt a rendszer automatikusan menti a házirendben. 
    
4. Ha végzett, zárja be a **Házirend szerkesztése** ablaktáblát. 
    
## <a name="delete-an-app-management-policy"></a>Appkezelési házirend törlése

1. A **Házirendek** kártyán válassza a **Házirend törlése** elemet.
    
2. **Házirend törlése** ablakban válassza ki a törölni kívánt házirendek \> **Jelölje ki**, majd **megerősítése** a házirend vagy a választott házirendek törlése. 
    
## <a name="available-settings"></a>Rendelkezésre álló beállítások

Az alábbi táblázatok részletes információkkal szolgálnak azokról a beállításokról, amelyekkel védelmet nyújthat az eszközökön lévő fájloknak, valamint azokról is, amelyekkel szabályozhatja, hogy a felhasználók hogyan férhessenek hozzá az Office-fájlokhoz mobileszközükről.
  
 További információt [A Microsoft 365 Vállalati verzió védelmi funkcióinak megfelelő Intune-beállítások](map-protection-features-to-intune-settings.md) című témakör tartalmaz. 
  
### <a name="settings-that-protect-work-files"></a>Munkahelyi fájlok védelmére szolgáló beállítások

Az alábbi beállításokkal védhetők meg a munkahelyi fájlok, ha az eszköz elveszett vagy ellopták:
  
|||
|:-----|:-----|
|Beállítás  <br/> |Leírás  <br/> |
|Munkahelyi fájlok törlése az inaktív eszközökről ennyi nap után  <br/> |Ha az eszközt az itt megadott számú napig nem használják, akkor a rajta tárolt összes munkahelyi fájl automatikusan törlődik.  <br/> |
|A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió  <br/> |Ha ez a beállítás **Be** állapotban van, akkor a munkahelyi fájlok mentési helye kizárólag a OneDrive Vállalati verzió lehet.  <br/> |
|Munkahelyi fájlok titkosítása  <br/> |A munkahelyi fájlok titkosítással való védelméhez ezt a beállítást tartsa **Be** állapotban. A céges adatait még az eszköz elvesztése vagy ellopása esetén sem fogja tudni senki olvasni.  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Az Office-fájlok mobileszközökön való elérését szabályozó beállítások

Az alábbi beállítások használhatók a munkahelyi Office-fájlok elérésének kezelésére:
  
|||
|:-----|:-----|
|Beállítás  <br/> |Leírás  <br/> |
|PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez  <br/> |Ha ez a beállítás **Be** állapotban van, a mobileszközön lévő Office-appok használatához a felhasználónéven és a jelszón kívül a felhasználóknak további hitelesítési módszert is használniuk kell.  <br/> |
|PIN-kód visszaállítása ennyi sikertelen bejelentkezési kísérlet után  <br/> |Annak érdekében, hogy ne lehessen a PIN-kódot véletlenszerű próbálkozásokkal megfejteni, az Ön által megadott számú téves próbálkozás után a PIN-kód alaphelyzetbe áll.  <br/> |
|A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után  <br/> |Ezzel a beállítással azt határozhatja meg, hogy a felhasználó mennyi ideig maradhat inaktív, mielőtt újra be kellene jelentkeznie.  <br/> |
|Hozzáférés letiltása a munkahelyi fájlokhoz a feltört vagy rootolással feltört eszközökön  <br/> |A hozzáértő felhasználók esetleg feltört vagy rootolással feltört eszközzel is rendelkezhetnek. Ez azt jelenti, hogy a felhasználó képes módosítani az operációs rendszert, ami sebezhetőbbé teheti az eszközt a kártevőkkel szemben. Ha ez a beállítás **Be** állapotban van, az ilyen eszközök le lesznek tiltva.  <br/> |
|A felhasználók másolhatnak tartalmakat az Office-appokból személyes appokba  <br/> |Azt alapértelmezés szerint engedélyezi, de ha a beállítás be **kapcsolva**, a felhasználó tudta átmásolni információk munkafájlt a személyes fájlok. Ha a beállítás ki **kapcsolva**, a felhasználói információ másolása egy munka fiókból személyes app vagy személyes fiók nem lesz.<br/> |
   

  


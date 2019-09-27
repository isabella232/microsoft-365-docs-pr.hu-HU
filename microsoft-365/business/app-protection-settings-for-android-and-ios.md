---
title: Appvédelmi beállítások megadása androidos vagy iOS-es eszközökhöz
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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Itt megtudhatja, hogyan hozhat létre, szerkeszthet és törölhet egy Alkalmazáskezelési házirendet, és hogyan védheti meg a munkahelyi fájlokat az Android vagy iOS rendszerű eszközökön.
ms.openlocfilehash: 68a338ffb4f9b6cab16c677f80d27481ccec4bd8
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "37287695"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a>Appvédelmi beállítások megadása androidos vagy iOS-es eszközökhöz

![Banner, hogy pont https://aka.ms/aboutM365preview-hoz.](media/m365admincenterchanging.png)

## <a name="create-an-app-management-policy"></a>Appkezelési házirend létrehozása

1. Menj az admin központba <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>. 
    
2. Kattintson a bal oldali NAV \> **eszközházirendek** \> **hozzáadása**parancsára. ****
  
3. A **Házirend felvétele** ablaktáblában adja meg a házirend egyedi nevét. 
    
4. A **Házirend típusa** csoportban válassza az **Alkalmazáskezelés Android-eszközökhöz** vagy az **Alkalmazáskezelés iOS-eszközökhöz** lehetőséget attól függően, hogy milyen házirendkészletet szeretne létrehozni. 
    
5. Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** \> configure the settings how you would like. The **Manage how users access Office files on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values. További információért tekintse meg az [elérhető beállításokat](#available-settings) . 
    
    Az **Alapértelmezett beállítások visszaállítása** hivatkozásra kattintva bármikor visszatérhet az alapértelmezett beállításokhoz. 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.
    
7. Végül válassza a **Kész** lehetőséget a házirend mentéséhez és eszközökhöz való hozzárendeléséhez. 
    
## <a name="edit-an-app-management-policy"></a>Appkezelési házirend szerkesztése

1. A **házirendek** kartonon kattintson a **házirend szerkesztése**lehetőségre.
    
2. A **Házirend szerkesztése** ablaktáblában válassza ki a módosítani kívánt házirendet. 
    
3. Válassza a **Szerkesztés** elemet az egyes beállítások mellett a házirend értékeinek módosításához. Amikor módosít egy értéket, azt a rendszer automatikusan menti a házirendben. 
    
4. Ha végzett, zárja be a **Házirend szerkesztése** ablaktáblát. 
    
## <a name="delete-an-app-management-policy"></a>Appkezelési házirend törlése

1. A **házirendek** lapon válasszon egy házirendet, majd **törölje**.
    
2. A **házirend törlése** ablaktáblában a házirend-vagy a választott házirendek **törlése parancsra kattintson a Törlés parancsra** . 
    
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
|Munkahelyi fájlok titkosítása  <br/> |A munkahelyi fájlok titkosítással való védelméhez ezt a beállítást tartsa **Be** állapotban. A céges adatokat még akkor sem tudják majd elolvasni, ha az eszköz elvész vagy ellopják.  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Az Office-fájlok mobileszközökön való elérését szabályozó beállítások

Az alábbi beállítások használhatók a munkahelyi Office-fájlok elérésének kezelésére:
  
|||
|:-----|:-----|
|Beállítás  <br/> |Leírás  <br/> |
|PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez  <br/> |Ha ez a beállítás **Be** állapotban van, a mobileszközön lévő Office-appok használatához a felhasználónéven és a jelszón kívül a felhasználóknak további hitelesítési módszert is használniuk kell.  <br/> |
|PIN-kód visszaállítása ennyi sikertelen bejelentkezési kísérlet után  <br/> |Annak érdekében, hogy ne lehessen a PIN-kódot véletlenszerű próbálkozásokkal megfejteni, az Ön által megadott számú téves próbálkozás után a PIN-kód alaphelyzetbe áll.  <br/> |
|A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után  <br/> |Ezzel a beállítással azt határozhatja meg, hogy a felhasználó mennyi ideig maradhat inaktív, mielőtt újra be kellene jelentkeznie.  <br/> |
|Hozzáférés letiltása a munkahelyi fájlokhoz a feltört vagy rootolással feltört eszközökön  <br/> |A hozzáértő felhasználók esetleg feltört vagy rootolással feltört eszközzel is rendelkezhetnek. Ez azt jelenti, hogy a felhasználó módosíthatja az operációs rendszert, ami viszont kártevők által sebezhetőbbé teheti az eszközt. Ha ez a beállítás **Be** állapotban van, az ilyen eszközök le lesznek tiltva.  <br/> |
|A felhasználók másolhatnak tartalmakat az Office-appokból személyes appokba  <br/> |Ezt alapértelmezésben engedélyezi, de ha a beállítás **be van kapcsolva**, a felhasználó egy munkahelyi fájlban lévő információt átmásolhatja egy személyes fájlba. Ha a beállítás **ki van kapcsolva**, a felhasználó nem tud adatokat másolni munkahelyi fiókból személyes alkalmazásba vagy személyes fiókba.  <br/> |
   

  


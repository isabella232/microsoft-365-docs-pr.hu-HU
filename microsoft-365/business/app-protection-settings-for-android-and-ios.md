---
title: Appvédelmi beállítások megadása androidos vagy iOS-es eszközökhöz
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Megtudhatja, hogy miként hozhat létre, szerkeszthet vagy törölhet alkalmazáskezelési szabályzatot, és hogyan védheti meg a munkahelyi fájlokat Android vagy iOS rendszerű eszközökön.
ms.openlocfilehash: f4366230805c50fe82183431e3bd2bdfa9fddd68
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/15/2020
ms.locfileid: "42068647"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a>Appvédelmi beállítások megadása androidos vagy iOS-es eszközökhöz

![Banner, hogy https://aka.ms/aboutM365previewpont .](../media/m365admincenterchanging.png)

## <a name="create-an-app-management-policy"></a>Appkezelési házirend létrehozása

1. Nyissa meg a <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>felügyeleti központot a . 
    
2. A bal oldali navigációs sávon válassza az **Eszközök** \> **házirendek** \> **hozzáadása**lehetőséget.
  
3. A **Házirend felvétele** ablaktáblában adja meg a házirend egyedi nevét. 
    
4. A **Házirend típusa**csoportban válassza az Android **alkalmazáskezelés** vagy az **iOS alkalmazáskezelés**lehetőséget, attól függően, hogy mely házirendeket szeretné létrehozni. 
    
5. Bontsa ki a Munkahelyi fájlok védelme az **eszközök ellopása vagy ellopása** esetén, és **kezelje, hogy a felhasználók hogyan férnek hozzá az Office-fájlokhoz mobileszközökön.** Adja meg a beállításokat, hogyan szeretné. **A felhasználók mobileszközökön** való **** hozzáférésének alapértelmezett beállítását kezelheti, de azt javasoljuk, hogy kapcsolja be **és** fogadja el az alapértelmezett értékeket. További információ: [Elérhető beállítások](#available-settings). 
    
    Az **Alapértelmezett beállítások visszaállítása** hivatkozásra kattintva bármikor visszatérhet az alapértelmezett beállításokhoz. 
    
    ![Screenshot of Create a policy with Application management for Android selected](../media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. Next decide **Who will get these settings?** Ha nem szeretné használni az alapértelmezett **Minden felhasználó** biztonsági csoportot, válassza a **Módosítás**lehetőséget, válassza a beállításokat \> bekapó biztonsági csoportokat **Válassza.**
    
7. Végül válassza a **Kész** lehetőséget a házirend mentéséhez és eszközökhöz való hozzárendeléséhez. 
    
## <a name="edit-an-app-management-policy"></a>Appkezelési házirend szerkesztése

1. A **Házirendek** kartonon válassza a **Házirend szerkesztése**lehetőséget.
    
2. A **Házirend szerkesztése** ablaktáblában válassza ki a módosítani kívánt házirendet. 
    
3. Válassza a **Szerkesztés** elemet az egyes beállítások mellett a házirend értékeinek módosításához. Ha módosít egy értéket, az automatikusan mentésre kerül a házirendbe.
    
4. Ha végzett, zárja be a **Házirend szerkesztése** ablaktáblát. 
    
## <a name="delete-an-app-management-policy"></a>Appkezelési házirend törlése

1. A **Házirendek** lapon válasszon egy házirendet, majd törölje a **fájlt.**
    
2. A **Házirend törlése** ablaktáblán válassza a **Megerősítés** lehetőséget a választott házirend vagy házirendek törléséhez. 
    
## <a name="available-settings"></a>Rendelkezésre álló beállítások

Az alábbi táblázatok részletes információkat nyújtanak az eszközökön lévő munkahelyi fájlok védelmére rendelkezésre álló beállításokról, valamint azokról a beállításokról, amelyek szabályozzák, hogy a felhasználók hogyan férnek hozzá az Office-fájlokhoz a mobileszközükről.
  
 További információt [A Microsoft 365 Vállalati verzió védelmi funkcióinak megfelelő Intune-beállítások](map-protection-features-to-intune-settings.md) című témakörben talál. 
  
### <a name="settings-that-protect-work-files"></a>Munkahelyi fájlok védelmére szolgáló beállítások

Az alábbi beállításokkal védhetők meg a munkahelyi fájlok, ha az eszköz elveszett vagy ellopták:
  
|||
|:-----|:-----|
|Beállítás  <br/> |Leírás  <br/> |
|Munkahelyi fájlok törlése az inaktív eszközökről ennyi nap után  <br/> |Ha egy eszközt nem használ az itt megadott számú napig, az eszközön tárolt munkafájlok automatikusan törlődnek.  <br/> |
|A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió  <br/> |Ha ez a beállítás **Be van,** a munkahelyi fájlok csak a OneDrive Vállalati verzió számára érhető el mentési hely.  <br/> |
|Munkahelyi fájlok titkosítása  <br/> |A munkahelyi fájlok titkosítással való védelméhez ezt a beállítást tartsa **Be** állapotban. Még akkor is, ha az eszköz elveszett vagy ellopták, senki sem tudja olvasni a vállalati adatokat.  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Az Office-fájlok mobileszközökön történő elérésének felügyeletét meghatározó beállítások

Az alábbi beállítások használhatók a munkahelyi Office-fájlok elérésének kezelésére:
  
|||
|:-----|:-----|
|Beállítás  <br/> |Leírás  <br/> |
|PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez  <br/> |Ha ez a beállítás **A** felhasználónak a felhasználónévés jelszava mellett más hitelesítési formát is meg kell adnia ahhoz, hogy mobileszközeiken használhassák az Office-alkalmazásokat.<br/> |
|PIN-kód visszaállítása ennyi sikertelen bejelentkezési kísérlet után  <br/> |Annak érdekében, hogy ne lehessen a PIN-kódot véletlenszerű próbálkozásokkal megfejteni, az Ön által megadott számú téves próbálkozás után a PIN-kód alaphelyzetbe áll.  <br/> |
|A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után  <br/> |Ez a beállítás határozza meg, hogy a felhasználó mennyi ideig lehet tétlen, mielőtt a rendszer ismételten bejelentkezne.  <br/> |
|Hozzáférés letiltása a munkahelyi fájlokhoz a feltört vagy rootolással feltört eszközökön  <br/> |A hozzáértő felhasználók esetleg feltört vagy rootolással feltört eszközzel is rendelkezhetnek. Ez azt jelenti, hogy a felhasználó módosíthatja az operációs rendszert, ami viszont kártevők által sebezhetőbbé teheti az eszközt. Ha ez a beállítás **Be** állapotban van, az ilyen eszközök le lesznek tiltva.  <br/> |
|A felhasználók másolhatnak tartalmakat az Office-appokból személyes appokba  <br/> |Alapértelmezés szerint engedélyezieztünk, de ha a beállítás Be van **kapcsolva,** a felhasználó átmásolhatja a munkahelyi fájlban lévő adatokat egy személyes fájlba. Ha a beállítás ki van **kapcsolva,** a felhasználó nem tudja átmásolni az adatokat egy munkahelyi fiókból egy személyes alkalmazásba vagy személyes fiókba.  <br/> |

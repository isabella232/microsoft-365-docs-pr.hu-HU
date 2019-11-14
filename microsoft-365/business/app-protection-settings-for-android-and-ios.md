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
description: Itt megtudhatja, hogyan hozhat létre, szerkeszthet és törölhet egy Alkalmazáskezelési házirendet, és hogyan védheti meg a munkahelyi fájlokat az Android vagy iOS rendszerű eszközökön.
ms.openlocfilehash: 2eebe5b603837d7e4125ab7e88b61792ca3a1e5d
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/14/2019
ms.locfileid: "38321845"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a>Appvédelmi beállítások megadása androidos vagy iOS-es eszközökhöz

![Banner, hogy pont https://aka.ms/aboutM365preview-hoz.](media/m365admincenterchanging.png)

## <a name="create-an-app-management-policy"></a>Appkezelési házirend létrehozása

1. Menj az admin központba <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>. 
    
2. Kattintson a bal oldali NAV \> **eszközházirendek** \> **hozzáadása**parancsára. ****
  
3. A **Házirend felvétele** ablaktáblában adja meg a házirend egyedi nevét. 
    
4. A **házirendtípus**területen válassza az **Alkalmazáskezelés az Android rendszerhez** vagy **az Alkalmazáskezelés az iOS rendszerhez**típust, attól függően, hogy milyen házirendeket szeretne létrehozni. 
    
5. Bontsa ki a **munkahelyi fájlok védelmét az eszközök elvesztése vagy ellopása esetén** , és **kezelje a felhasználók által a mobileszközökön elérhető Office-fájlokat**. Konfigurálja a beállításokat, hogy hogyan szeretné. Annak kezelése, hogy a **felhasználók hogyan férhetnek hozzá a mobileszközökön található Office-fájlokhoz** , alapértelmezés szerint **ki van kapcsolva** , de azt javasoljuk, hogy kapcsolja **be és fogadja** el az alapértelmezett értékeket. További tudnivalókért tanulmányozza az [elérhető beállítások](#available-settings)című témakört. 
    
    Az **Alapértelmezett beállítások visszaállítása** hivatkozásra kattintva bármikor visszatérhet az alapértelmezett beállításokhoz. 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. Next decide **Who will get these settings?** Ha nem kívánja használni az alapértelmezett **minden felhasználó** biztonsági csoportot, válassza a **módosítás**beállítást, válassza ki azokat a biztonsági csoportokat, amelyek \> ezeket **a beállításokat**megkapnak.
    
7. Végül válassza a **Kész** lehetőséget a házirend mentéséhez és eszközökhöz való hozzárendeléséhez. 
    
## <a name="edit-an-app-management-policy"></a>Appkezelési házirend szerkesztése

1. A **házirendek** kartonon kattintson a **házirend szerkesztése**lehetőségre.
    
2. A **Házirend szerkesztése** ablaktáblában válassza ki a módosítani kívánt házirendet. 
    
3. Válassza a **Szerkesztés** elemet az egyes beállítások mellett a házirend értékeinek módosításához. Az érték módosítása automatikusan a házirendbe kerül.
    
4. Ha végzett, zárja be a **házirend szerkesztése** ablaktáblát. 
    
## <a name="delete-an-app-management-policy"></a>Appkezelési házirend törlése

1. A **házirendek** lapon válasszon egy házirendet, majd **törölje**.
    
2. A **házirend törlése** párbeszédpanelen kattintson a **megerősítés** elemre a kiválasztott házirend vagy házirendek törléséhez. 
    
## <a name="available-settings"></a>Rendelkezésre álló beállítások

A következő táblázatok részletes információt adnak azokról a beállításokról, amelyek az eszközök munkafájlok védelmére használhatók, valamint azok a beállítások, amelyek a felhasználók számára az Office fájlokhoz való hozzáférést a mobileszköztől vezérelhetik.
  
 További információt [A Microsoft 365 Vállalati verzió védelmi funkcióinak megfelelő Intune-beállítások](map-protection-features-to-intune-settings.md) című témakörben talál. 
  
### <a name="settings-that-protect-work-files"></a>Munkahelyi fájlok védelmére szolgáló beállítások

Az alábbi beállításokkal védhetők meg a munkahelyi fájlok, ha az eszköz elveszett vagy ellopták:
  
|||
|:-----|:-----|
|Beállítás  <br/> |Leírás  <br/> |
|Munkahelyi fájlok törlése az inaktív eszközökről ennyi nap után  <br/> |Ha egy eszköz nem az itt megadott számú napra van használatban, akkor az eszközön tárolt minden munka automatikusan törlődik.  <br/> |
|A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió  <br/> |Ha ez elintézés van- **on**, egyetlen elérhető megment elhelyezés részére dolgozik fájlokat van OneDrive részére teendő.  <br/> |
|Munkahelyi fájlok titkosítása  <br/> |A munkahelyi fájlok titkosítással való védelméhez ezt a beállítást tartsa **Be** állapotban. Még ha az eszköz elvész vagy ellopják is, senki nem tudja elolvasni a vállalat adatait.  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Az Office-fájlok mobileszközökön történő elérésének felügyeletét meghatározó beállítások

Az alábbi beállítások használhatók a munkahelyi Office-fájlok elérésének kezelésére:
  
|||
|:-----|:-----|
|Beállítás  <br/> |Leírás  <br/> |
|PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez  <br/> |Ha **a felhasználónak a felhasználónévvel** és a jelszóval kapcsolatban egy másik hitelesítési formát kell adnia, akkor az Office alkalmazások mobileszközökön való használata előtt.<br/> |
|PIN-kód visszaállítása ennyi sikertelen bejelentkezési kísérlet után  <br/> |Annak érdekében, hogy ne lehessen a PIN-kódot véletlenszerű próbálkozásokkal megfejteni, az Ön által megadott számú téves próbálkozás után a PIN-kód alaphelyzetbe áll.  <br/> |
|A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után  <br/> |Ez a beállítás határozza meg, hogy a felhasználók mennyi ideig lehetnek üresjáratban, mielőtt a rendszer újra bejelentkezne.  <br/> |
|Hozzáférés letiltása a munkahelyi fájlokhoz a feltört vagy rootolással feltört eszközökön  <br/> |A hozzáértő felhasználók esetleg feltört vagy rootolással feltört eszközzel is rendelkezhetnek. Ez azt jelenti, hogy a felhasználó módosíthatja az operációs rendszert, ami viszont kártevők által sebezhetőbbé teheti az eszközt. Ha ez a beállítás **Be** állapotban van, az ilyen eszközök le lesznek tiltva.  <br/> |
|A felhasználók másolhatnak tartalmakat az Office-appokból személyes appokba  <br/> |Ezt alapértelmezésben engedélyezi, de ha a beállítás **be van kapcsolva**, a felhasználó egy munkahelyi fájlban lévő információt átmásolhatja egy személyes fájlba. Ha a beállítás **ki van kapcsolva**, a felhasználó nem tud adatokat másolni munkahelyi fiókból személyes alkalmazásba vagy személyes fiókba.  <br/> |

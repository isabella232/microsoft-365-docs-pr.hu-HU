---
title: Appvédelmi beállítások megadása androidos vagy iOS-es eszközökhöz
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Megtudhatja, hogy miként hozhat létre, szerkeszthet és törölhet appkezelési házirendeket, és hogyan védheti meg a munkahelyi fájlokat Android- vagy iOS-eszközökön.
ms.openlocfilehash: 2e157737990c7aca6e87a676e90f62f0d40ad372
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580294"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a>Appvédelmi beállítások megadása androidos vagy iOS-es eszközökhöz

Ez a cikk a Microsoft 365 Vállalati prémium verzióra vonatkozik.

## <a name="create-an-app-management-policy"></a>Appkezelési házirend létrehozása

1. A felügyeleti központ megnyitásához: <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> . 
    
2. A bal oldali navigációs sávon válassza az **Eszköz** \> **házirendek** \> **hozzáadása lehetőséget.**
  
3. A **Házirend felvétele** ablaktáblában adja meg a házirend egyedi nevét. 
    
4. A **Házirend típusa csoportban** válassza az **Alkalmazáskezelés Androidhoz** vagy **az Alkalmazáskezelés iOS** rendszerhez lehetőséget attól függően, hogy milyen házirendkészletet szeretne létrehozni. 
    
5. **Bontsa ki a Munkahelyi fájlok védelme az eszközök elveszett** vagy ellopása esetén és az Office-fájlok felhasználói mobileszközökön való elérésének kezelése **ot.** Adja meg a beállításokat a megfelelő módon. **Az Office-fájlok felhasználói mobileszközökön** való elérésének kezelése alapértelmezés  szerint Ki van kapcsolva, de azt javasoljuk, hogy kapcsolja be, és fogadja el az alapértelmezett értékeket.  További információt a Rendelkezésre álló [beállítások lapon található.](#available-settings) 
    
    Az **Alapértelmezett beállítások visszaállítása** hivatkozásra kattintva bármikor visszatérhet az alapértelmezett beállításokhoz. 
    
    ![Screenshot of Create a policy with Application management for Android selected](../media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. Next decide **Who will get these settings?** Ha nem szeretné az alapértelmezett  Minden felhasználó biztonsági csoportot használni, válassza a Módosítás gombot, és válassza ki azokat a biztonsági csoportokat, amelyekben meg vannak jelölve ezek a \> **beállítások. Válassza a lehetőséget.**
    
7. Végül válassza a **Kész** lehetőséget a házirend mentéséhez és eszközökhöz való hozzárendeléséhez. 
    
## <a name="edit-an-app-management-policy"></a>Appkezelési házirend szerkesztése

1. A **Házirendek kártyán** válassza a **Házirend szerkesztése lehetőséget.**
    
2. A **Házirend szerkesztése** ablaktáblában válassza ki a módosítani kívánt házirendet. 
    
3. Válassza a **Szerkesztés** elemet az egyes beállítások mellett a házirend értékeinek módosításához. Amikor módosít egy értéket, a rendszer automatikusan menti azt a házirendben.
    
4. Ha végzett, zárja be a Házirend szerkesztése **ablaktáblát.** 
    
## <a name="delete-an-app-management-policy"></a>Appkezelési házirend törlése

1. A **Házirendek lapon** válasszon ki egy házirendet, majd kattintson a **Törlés gombra.**
    
2. A Házirend **törlése ablaktáblában** válassza a Megerősítés gombot a választott házirend vagy házirendek törléséhez.  
    
## <a name="available-settings"></a>Rendelkezésre álló beállítások

Az alábbi táblázatok részletes információkat tartalmaznak az eszközök munkahelyi fájljainak védelmére vonatkozó beállításokról, valamint az Office-fájlok mobileszközről való elérésének szabályozására vonatkozó beállításokról.
  
 További információ: [A Microsoft 365 Vállalati prémium](map-protection-features-to-intune-settings.md)verzió védelmi funkcióinak megfelelő Intune-beállítások. 
  
### <a name="settings-that-protect-work-files"></a>Munkahelyi fájlok védelmére szolgáló beállítások

Az alábbi beállításokkal védhetők meg a munkahelyi fájlok, ha az eszköz elveszett vagy ellopták:
  
|||
|:-----|:-----|
|Beállítás  <br/> |Leírás  <br/> |
|Munkahelyi fájlok törlése az inaktív eszközökről ennyi nap után  <br/> |Ha az itt megadott számú napig nem használ egy eszközt, az eszközön tárolt munkahelyi fájlok automatikusan törlődnek.  <br/> |
|A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió  <br/> |Ha ez a beállítás **Be,** a munkahelyi fájlok mentésének egyetlen helye a OneDrive Vállalati verzió.  <br/> |
|Munkahelyi fájlok titkosítása  <br/> |A munkahelyi fájlok titkosítással való védelméhez ezt a beállítást tartsa **Be** állapotban. A céges adatokat még akkor sem olvashatják el, ha az eszközt ellopják vagy ellopják.  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Az Office-fájlok mobileszközökön történő elérésének felügyeletét meghatározó beállítások

Az alábbi beállítások használhatók a munkahelyi Office-fájlok elérésének kezelésére:
  
|||
|:-----|:-----|
|Beállítás  <br/> |Leírás  <br/> |
|PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez  <br/> |Ha ez a beállítás **Be,** a mobileszközön való használat előtt a felhasználóknak a felhasználónéven és a jelszón kívül más hitelesítési módszert is meg kell adniuk.<br/> |
|PIN-kód visszaállítása ennyi sikertelen bejelentkezési kísérlet után  <br/> |Annak érdekében, hogy ne lehessen a PIN-kódot véletlenszerű próbálkozásokkal megfejteni, az Ön által megadott számú téves próbálkozás után a PIN-kód alaphelyzetbe áll.  <br/> |
|A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után  <br/> |Ez a beállítás azt határozza meg, hogy a felhasználó mennyi ideig inaktív, mielőtt a rendszer ismét arra kéri, hogy jelentkezzen be.  <br/> |
|Hozzáférés letiltása a munkahelyi fájlokhoz a feltört vagy rootolással feltört eszközökön  <br/> |A hozzáértő felhasználók esetleg feltört vagy rootolással feltört eszközzel is rendelkezhetnek. Ez azt jelenti, hogy a felhasználó módosíthatja az operációs rendszert, ami viszont kártevők által sebezhetőbbé teheti az eszközt. Ha ez a beállítás **Be** állapotban van, az ilyen eszközök le lesznek tiltva.  <br/> |
|Nem engedélyezem a felhasználóknak, hogy tartalmakat másoljanak az Office-alkalmazásokból a személyes appokba  <br/> |Ez alapértelmezés szerint engedélyezett, de ha a beállítás Be van kapcsolva, a felhasználó átmásolhatja egy munkahelyi fájl adatait egy személyes fájlba. Ha a beállítás **Ki** van kapcsolva, a felhasználó nem tud adatokat másolni egy munkahelyi fiókból egy személyes appba vagy személyes fiókba.  <br/> |

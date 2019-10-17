---
title: A Microsoft 365 Business védelmi funkcióinak megfelelő Intune-beállítások
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 8/13/2018
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
ms.assetid: aad21b1a-c775-469a-b89c-c5d1d59d27db
description: Információ a Microsoft 365 Business Térkép és az Intune-beállítások védelmi szolgáltatásairól. Az előfizetés engedélyt biztosít az Intune-beállítások módosítására.
ms.openlocfilehash: 2e26bffe289170eb17b07325ab8b57285eecee38
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575938"
---
# <a name="how-do-protection-features-in-microsoft-365-business-map-to-intune-settings"></a>A Microsoft 365 Business védelmi funkcióinak megfelelő Intune-beállítások

## <a name="android-and-ios-application-protection-settings"></a>Android- és iOS-alkalmazásvédelmi beállítások

Az alábbi táblázat részletesen ismerteti, hogy az Android és az iOS alkalmazásházirend-beállításai hogyan felelnek meg az Intune-beállításoknak.
  
Ha meg szeretné keresni az Intune-beállítást, miközben be van jelentkezve a Microsoft 365 Business rendszergazdai hitelesítő adataival, nyissa meg a **Felügyeleti központokat**, majd az **Intune-t**.
  
 **Fontos:** A Microsoft 365 Business előfizetés egy licencet biztosít az összes Intune-beállítás módosítására. Az elinduláshoz tekintse meg az [Intune bemutatása](https://docs.microsoft.com/intune/introduction-intune) című témakört.
  
Kattintson a kijelölni kívánt házirend nevére (például Alkalmazás-házirend Android-eszközhöz), majd válassza a **Házirend-beállítások** lehetőséget.
  
A **Munkahelyi fájlok védelme abban ez esetben, ha a készülék elveszik vagy ellopják** csoportban
  
|**Androidos vagy iOS-es alkalmazásházirend-beállítás**|**Intune-beállítás(ok)**|
|:-----|:-----|
|Munkahelyi fájlok törlése az inaktív eszközökről ennyi idő után:  <br/> |Offline időtartam (nap) az alkalmazásadatok törlése előtt  <br/> |
|A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió  <br/> Ne feledje, hogy csak a OneDrive Vállalati verzió engedélyezett  <br/> |A társzolgáltatások kijelölése, amelyekbe menthetők a céges adatok  <br/> |
|||
   
Az **Office-fájlok mobileszközökön történő elérésének felügyelete** csoportban
  
|**Androidos vagy iOS-es alkalmazásházirend-beállítás**|**Intune-beállítás(ok)**|
|:-----|:-----|
|Munkahelyi fájlok törlése az inaktív eszközökről ennyi idő után:  <br/> |Offline időtartam (nap) az alkalmazásadatok törlése előtt  <br/> |
|A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió  <br/> Ne feledje, hogy csak a OneDrive Vállalati verzió engedélyezett  <br/> |A társzolgáltatások kijelölése, amelyekbe menthetők a céges adatok  <br/> |
|Munkahelyi fájlok titkosítása  <br/> |Alkalmazás adatainak titkosítása  <br/> |
|Az **Office-fájlok mobileszközökön történő elérésének felügyelete** csoportban <br/> ||
|PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez  <br/> | PIN-kód megkövetelése a hozzáféréshez  <br/>  Ez a beállítás az alábbiakat is megadja:  <br/> **Egyszerű PIN-kód engedélyezése** az **Igen** értékre <br/> **PIN-kód hossza** a 4-es értékre  <br/> **Ujjlenyomat használatának engedélyezése PIN-kód helyett** az **Igen** értékre <br/> **Disable app PIN when device PIN is managed** to **No** <br/> |
|Új PIN-kód létrehozása, ha ennyiszer sikertelen a bejelentkezés: (ez le van tiltva, ha nem kell PIN-kódot megadni)  <br/> |Próbálkozások száma a PIN-kód alaphelyzetbe állítása előtt  <br/> |
|Újbóli bejelentkezés szükséges, ha ennyi ideje nem történt felhasználói művelet az Office-appokban: (ez le van tiltva, ha nem kell PIN-kódot megadni)  <br/> | Hozzáférési követelmények újbóli ellenőrzése ennyi idő után (perc)  <br/>  Ez a beállítás az alábbiakat is megadja:  <br/> Az **Időtúllépés** percekben van megadva  <br/>  Ez megegyezik a Microsoft 365 Business esetén megadott percek számával.  <br/> Az **Offline türelmi időszak** alapértelmezés szerint 720 percre van beállítva  <br/> |
|Munkahelyi fájlokhoz való hozzáférés letiltása függetlenített vagy feltört eszközökön  <br/> |A felügyelt alkalmazások futásának letiltása a függetlenített vagy feltört eszközökön  <br/> |
|A felhasználók másolhatnak tartalmakat az Office-appokból személyes appokba  <br/> | Kivágás, másolás és beillesztés tiltása más alkalmazásokkal  <br/>  Ha a Microsoft 365 Business beállítás **Be** értékre van állítva, akkor az alábbi három beállítás is **Minden alkalmazás** értékre van állítva az Intune-ban:  <br/> **Az alkalmazás átadhat adatokat más alkalmazásoknak** <br/> **Az alkalmazás fogadhat adatokat más alkalmazásokból** <br/> **Kivágás, másolás és beillesztés tiltása más alkalmazásokkal** <br/>  Ha a Microsoft 365 Business beállítás **Be** értékre van állítva, akkor az összes Intune-beállítás az alábbiakra van állítva:  <br/> **Az alkalmazás átadhat adatokat más alkalmazásoknak** beállításhoz a **Szabályzattal felügyelt alkalmazások** érték van megadva <br/> **Az alkalmazás fogadhat adatokat más alkalmazásokból** beállításhoz a **Minden alkalmazás** érték van megadva <br/> A **Kivágás, másolás és beillesztés tiltása más alkalmazásokkal** beállításhoz a **Szabályzattal felügyelt alkalmazások beillesztési lehetőséggel** érték van megadva <br/> |
|||
   
## <a name="windows-10-app-protection-settings"></a>Windows 10-es appvédelmi beállítások

Az alábbi táblázat részletesen ismerteti, hogy a Windows 10-es alkalmazásházirend-beállítások hogyan felelnek meg az Intune-beállításoknak.
  
Az Intune-beállítás megkereséséhez, miközben bejelentkezett a Microsoft 365 üzleti rendszergazdai hitelesítő adataival, látogasson el az [Azure portálra](https://portal.azure.com), majd válassza ki a **további szolgáltatásokat**, és a **szűrőbe**írja be az Intune beállítást, majd válassza az **Alkalmazásvédelem** \> ** Alkalmazásházirend**.
  
 **Fontos:** A Microsoft 365 Vállalati verziós előfizetések olyan licencet nyújtanak, amely csak a Microsoft 365 Vállalati verzióban elérhető beállításokra vonatkozó Intune-beállítások módosítására szolgál. 
  
Kattintson a kijelölni kívánt házirend nevére, és az elérhető beállítások felfedezéséhez válassza az **Általános, Hozzárendelések**, az **Engedélyezett alkalmazások**, a **Mentesített alkalmazások**, a **Kötelező beállítások** vagy a **Speciális beállítások** lehetőséget a bal oldali navigációs ablakban. 
  
|**Windows 10-es alkalmazásházirend-beállítás**|**Intune-beállítás(ok)**|
|:-----|:-----|
|Munkahelyi fájlok titkosítása  <br/> |**Speciális beállítások** \> **Adatvédelem**: a **Titkosítási kulcsok visszavonása regisztráció törlésekor** és a **Védett adatokhoz való hozzáférés visszavonása, ha az eszközt regisztrálják az MDM-ben** beállítás is **Be** értékre van állítva.  <br/> |
|A felhasználók nem másolhatnak céges adatokat saját fájljaikba  <br/> |**Kötelező beállítások** \> **Windows Information Protection módja**. A Microsoft 365 Business **Be** értéke megfelel a következőnek: **Felülbírálások elrejtése**, a Microsoft 365 Business **Ki** értéke megfelel a következőnek: **Ki**.  <br/> |
|Office-dokumentumok elérésének szabályozása  <br/> | Ha ennek értéke **Be** a Microsoft 365 Business esetén, akkor a  <br/> **Speciális beállítások** \> **Hozzáférés**, **A Vállalati Windows Hello használata a Windowsba való bejelentkezéshez** beállításhoz a **Be** érték van megadva, az alábbi további beállításokkal:  <br/> **Adja meg a PIN-kód minimális hosszát karakterben** beállításhoz a **4**-es érték van megadva.  <br/> **A Vállalati Windows Hello PIN-kódjában használandó nagybetűk konfigurálása** a **Nagybetűk használatának tiltása a PIN-kódban** értékre van állítva.  <br/> **A Vállalati Windows Hello PIN-kódjában használandó kisbetűk konfigurálása** a **Kisbetűk használatának tiltása a PIN-kódban** értékre van állítva.  <br/> **A Vállalati Windows Hello PIN-kódjában használandó speciális karakterek konfigurálása** a **Speciális karakterek használatának tiltása a PIN-kódban** értékre van állítva.  <br/> **Specify the period of time (in days) that a PIN can be used before the system requires the user to change** it is set to **0**.  <br/> **Specify the number of past PINs that can be associated to a user account that can't be reused** is set to **0**.  <br/> **Ennyi sikertelen hitelesítési kísérlet után lesz törölve az eszköz tartalma** - megegyezik a Microsoft 365 Business beállított értékével (alapértelmezés szerint 5).  <br/> **Az eszköz által inaktív állapotban eltöltött idő (percben), amelynek elteltével a PIN-kóddal vagy jelszóval feloldható zárolás bekapcsol** - megegyezik a Microsoft 365 Business beállított értékével.  <br/> |
|Védett adatok helyreállításának engedélyezése  <br/> |**Speciális beállítások** \> **Adatvédelem**: **Nagyvállalati adatvédelem ikonjának megjelenítése** és **Azure RMS használata a Windows Információvédelemhez** - mindkettő **Be** értékre van állítva.  <br/> |
|További céges felhőbeli helyek védelme  <br/> |A **Speciális beállítások** \> **Védett tartományok** és **Felhőerőforrások** megjelenítik a tartományokat és a SharePoint-webhelyeket.  <br/> |
|Az ezen appok által használt fájlok védettek  <br/> |A védett alkalmazások az **Engedélyezett alkalmazások** listában szerepelnek.  <br/> |
|||
   
## <a name="windows-10-device-protection-settings"></a>Eszközvédelmi beállítások Windows 10-es eszközökhöz

Az alábbi táblázat részletesen ismerteti, hogy a Windows 10 rendszerű eszköz konfigurációs beállításai hogyan felelnek meg az Intune-beállításoknak.
  
Az Intune-beállítás megkereséséhez, miközben bejelentkezett a Microsoft 365 üzleti rendszergazdai hitelesítő adataival, látogasson el az [Azure portálra](https://portal.azure.com), majd válassza ki a **további szolgáltatásokat**, és a **szűrőbe**írja be a **Intune beállítást, majd válassza** \> az **eszköz konfigurációs** \> **profilokat**. Then select **Device policy for Windows 10** \> **Properties** \> **Settings**.
  
|**Eszközházirend Windows 10-es eszközhöz**|**Intune-beállítás(ok)**|
|:-----|:-----|
|A Windows Defender víruskereső használatával segíthet a PC-k vírusokkal és más fenyegetésekkel szembeni védelmében  <br/> |Valós idejű figyelés engedélyezése = BE  <br/> Felhővédelem engedélyezése = BE  <br/> Minták küldésének kérése a felhasználóktól = Biztonságos minták automatikus elküldése (személyazonosításra nem alkalmas alapértelmezett adatok automatikus elküldése)  <br/> |
|Segíthet megvédeni a PC-ket a Microsoft Edge-beli webes veszélyforrások ellen  <br/> |A **SmartScreen** a **Microsoft Edge böngésző beállításai** között **Kötelező** értékre van állítva.  <br/> |
|Az eszköz képernyőjének kikapcsolása ennyi üresjárati idő után (perc):  <br/> |Képernyőzárolás legfeljebb ennyi perc inaktivitás után  <br/> |
|A felhasználók letölthetnek appokat innen: Microsoft Áruház  <br/> |Egyéni URI-szabályzat  <br/> |
|A felhasználók hozzáférhetnek Cortanához  <br/> |Az **Általános** \> **Cortana** beállítás **blokkolás** értékre van állítva az Intune-ban, amikor **ki** értékre van beállítva a Microsoft 365 Business esetén.  <br/> |
|A felhasználók kaphatnak a Windowszal kapcsolatos tippeket és a hirdetéseket a Microsofttól  <br/> |**Windows Reflektorfény**, minden le van tiltva, ha ez **ki** értékre van állítva a Microsoft 365 Business esetén.  <br/> |
|A Windows 10-es eszközök automatikus naprakészen tartása  <br/> | Ez a beállítás a **Microsoft Intune** \> **Szolgáltatásfrissítések - Windows 10-es frissítési körök** részen található. Válassza a **Windows 10-es eszközök frissítési házirendje** lehetőséget, majd a **Tulajdonságok** \> **Beállítások** elemet.      <br/>  Amikor a Microsoft 365 Business beállítás **Be** értékre van állítva, az összes alábbi beállítás meg van adva:  <br/> A **szolgáltatási ág** a **CB** értékre van állítva (CBB értékre, ha ez ki van kapcsolva a Microsoft 365 Businessban).  <br/> A **Microsoft-termékfrissítések** beállítása **Engedélyezés**.  <br/> A **Windows-illesztőprogramok** beállítása **Engedélyezés**.  <br/> Az **Automatikus frissítési viselkedés** az **Automatikus telepítés karbantartáskor** értékre van állítva az alábbi beállításokkal:  <br/> Az **Aktív órák kezdete** **de. 6** órára van állítva.  <br/> Az **Aktív órák vége** **du. 10** órára van állítva.  <br/> A **Minőségi frissítések elhalasztása (nap)** **0** értékre van állítva.  <br/> A **Szolgáltatásfrissítések elhalasztása (nap)** **0** értékre van állítva.  <br/> A **Kézbesítésoptimalizálásos letöltési mód** a **HTTP ugyanazon NAT mögötti társviszony-létesítéssel kombinálva** értékre van állítva.  <br/> |
|||
   


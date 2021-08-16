---
title: Hogyan használhatja az Intune Microsoft 365 Vállalati prémium verzió védelmi funkcióit az Intune-beállításoknak?
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: aad21b1a-c775-469a-b89c-c5d1d59d27db
description: Ismerje meg, hogyan használhatja a Microsoft 365 Vállalati prémium verzió Intune-beállításoknak megfelelő védelmi funkciókat. Az előfizetés licencet biztosít Az Intune beállításainak módosításához.
ms.openlocfilehash: 844b83bca9483f72fd322d666803c42b90fee41d3e0047ea93b4b6b07717b0dd
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53852731"
---
# <a name="how-do-protection-features-in-microsoft-365-business-premium-map-to-intune-settings"></a>Hogyan használhatja az Intune Microsoft 365 Vállalati prémium verzió védelmi funkcióit az Intune-beállításoknak?

## <a name="android-and-ios-application-protection-settings"></a>Android- és iOS-alkalmazásvédelmi beállítások

Az alábbi táblázat részletesen ismerteti, hogy az Android és az iOS alkalmazásházirend-beállításai hogyan felelnek meg az Intune-beállításoknak.
  
Az Intune-beállítás megkereshez jelentkezzen be a rendszergazdai Microsoft 365 Vállalati prémium verzió, és válassza a Felügyeleti központok **,** majd az **Intune ot.**
  
 > [!IMPORTANT]
 > 
 > A Microsoft 365 Vállalati prémium verzió-előfizetés licencet biztosít Önnek az összes Intune-beállítás módosításához. Első [lépések: Bevezetés az Intune-ba.](/intune/introduction-intune)
  
Jelölje ki a kívánt házirendnevet &mdash; (például Alkalmazás-házirend Androidhoz) és &mdash; válassza a **Házirend-beállítások lehetőséget.**
  
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
|A PIN-kód alaphelyzetbe állítása, ha ennyiszer sikertelen a bejelentkezés (ez le van tiltva, ha nincs szükség PIN-kódra)  <br/> |Próbálkozások száma a PIN-kód alaphelyzetbe állítása előtt  <br/> |
|A felhasználóknak újra be kell jelentkezniük, miután Office az appok ennyi ideig inaktívak voltak (ez le van tiltva, ha nincs szükség PIN-kódra)  <br/> | Hozzáférési követelmények újbóli ellenőrzése ennyi idő után (perc)  <br/>  Ez a beállítás az alábbiakat is megadja:  <br/> Az **Időtúllépés** percekben van megadva  <br/>  Ez megegyezik a Microsoft 365 Business esetén megadott percek számával.  <br/> Az **Offline türelmi időszak** alapértelmezés szerint 720 percre van beállítva  <br/> |
|Munkahelyi fájlokhoz való hozzáférés letiltása függetlenített vagy feltört eszközökön  <br/> |A felügyelt alkalmazások futásának letiltása a függetlenített vagy feltört eszközökön  <br/> |
|A felhasználók másolhatnak tartalmakat az Office-appokból személyes appokba  <br/> | Kivágás, másolás és beillesztés korlátozása más alkalmazásokkal  <br/>  Ha a Microsoft 365 Vállalati prémium verzió Be van állítva, akkor a következő  három beállítás is a Minden alkalmazás az Intune-ban beállításra van állítva:   <br/> **Az alkalmazás átadhat adatokat más alkalmazásoknak** <br/> **Az alkalmazás fogadhat adatokat más alkalmazásokból** <br/> **Kivágás, másolás és beillesztés tiltása más alkalmazásokkal** <br/>  Ha a Microsoft 365 Business beállítás **Be** értékre van állítva, akkor az összes Intune-beállítás az alábbiakra van állítva:  <br/> **Az alkalmazás átadhat adatokat más alkalmazásoknak** beállításhoz a **Szabályzattal felügyelt alkalmazások** érték van megadva <br/> **Az alkalmazás fogadhat adatokat más alkalmazásokból** beállításhoz a **Minden alkalmazás** érték van megadva <br/> A **Kivágás, másolás és beillesztés tiltása más alkalmazásokkal** beállításhoz a **Szabályzattal felügyelt alkalmazások beillesztési lehetőséggel** érték van megadva <br/> |
|||
   
## <a name="windows-10-app-protection-settings"></a>Windows 10-es appvédelmi beállítások

Az alábbi táblázat részletesen ismerteti, hogy a Windows 10-es alkalmazásházirend-beállítások hogyan felelnek meg az Intune-beállításoknak.
  
Az Intune-beállítás megkereshez jelentkezzen be a rendszergazdai Microsoft 365 Vállalati prémium verzió, és keresse fel az [Azure Portal webhelyet.](https://portal.azure.com) Válassza **a További szolgáltatások lehetőséget,** és írja be az Intune parancsot a Szűrő **mezőbe.** Válassza **az Intune appvédelmi** \> **alkalmazásra vonatkozó házirend lehetőséget.**
  
 > [!IMPORTANT]
 >
 >A Microsoft 365 Vállalati prémium verzió-előfizetés licencet biztosít Önnek arra, hogy csak az Intune-beállításokat módosítsa, amelyek az adott előfizetésben elérhető Microsoft 365 Vállalati prémium verzió. 
  
A rendelkezésre álló beállítások felfedezéséhez jelölje ki a kívánt házirendnevet, majd válassza az  **Általános,** a Hozzárendelések , az Engedélyezett **alkalmazások**, a Kivételként használt alkalmazások , a Kötelező beállítások vagy a Speciális beállítások lehetőséget a bal oldali navigációs ablakban.   
  
|**Windows 10-es alkalmazásházirend-beállítás**|**Intune-beállítás(ok)**|
|:-----|:-----|
|Munkahelyi fájlok titkosítása  <br/> |**Speciális beállítások** \> **Adatvédelem**: a **Titkosítási kulcsok visszavonása regisztráció törlésekor** és a **Védett adatokhoz való hozzáférés visszavonása, ha az eszközt regisztrálják az MDM-ben** beállítás is **Be** értékre van állítva.  <br/> |
|A felhasználók nem másolhatnak céges adatokat saját fájljaikba  <br/> |**Kötelező beállítások** \> **Windows Information Protection módja**. **A be** Microsoft 365 Vállalati prémium verzió a következőnek: **Felülbírálások** elrejtése **,** a Beállítás Microsoft 365 Vállalati prémium verzió ki értékhez van **kapcsolva.**  <br/> |
|Office-dokumentumok elérésének szabályozása  <br/> | Ha a beállítás Be van **állítva a** Microsoft 365 Vállalati prémium verzió, akkor a  <br/> **Speciális beállítások** \> **Hozzáférés**, **A Vállalati Windows Hello használata a Windowsba való bejelentkezéshez** beállításhoz a **Be** érték van megadva, az alábbi további beállításokkal:  <br/> **Adja meg a PIN-kód minimális hosszát karakterben** beállításhoz a **4**-es érték van megadva.  <br/> **A Vállalati Windows Hello PIN-kódjában használandó nagybetűk konfigurálása** a **Nagybetűk használatának tiltása a PIN-kódban** értékre van állítva.  <br/> **A Vállalati Windows Hello PIN-kódjában használandó kisbetűk konfigurálása** a **Kisbetűk használatának tiltása a PIN-kódban** értékre van állítva.  <br/> **A Vállalati Windows Hello PIN-kódjában használandó speciális karakterek konfigurálása** a **Speciális karakterek használatának tiltása a PIN-kódban** értékre van állítva.  <br/> **Adja meg, hogy a PIN-kód** 0-ra van-e állítva, mielőtt a rendszer **módosítja** azt (napokban).  <br/> **Specify the number of past PINs that can be associated to a user account that can't be reused** is set to **0**.  <br/> **Ennyi sikertelen hitelesítési kísérlet után lesz törölve az eszköz tartalma** - megegyezik a Microsoft 365 Business beállított értékével (alapértelmezés szerint 5).  <br/> **Az eszköz által inaktív állapotban eltöltött idő (percben), amelynek elteltével a PIN-kóddal vagy jelszóval feloldható zárolás bekapcsol** - megegyezik a Microsoft 365 Business beállított értékével.  <br/> |
|Védett adatok helyreállításának engedélyezése  <br/> |**Speciális beállítások** \> **Adatvédelem**: **Nagyvállalati adatvédelem ikonjának megjelenítése** és **Azure RMS használata a Windows Információvédelemhez** - mindkettő **Be** értékre van állítva.  <br/> |
|További céges felhőbeli helyek védelme  <br/> |A **Speciális beállítások** \> **Védett tartományok** és **Felhőerőforrások** megjelenítik a tartományokat és a SharePoint-webhelyeket.  <br/> |
|Az ezen appok által használt fájlok védettek  <br/> |A védett alkalmazások az **Engedélyezett alkalmazások** listában szerepelnek.  <br/> |
|||
   
## <a name="windows-10-device-protection-settings"></a>Eszközvédelmi beállítások Windows 10-es eszközökhöz

Az alábbi táblázat részletesen ismerteti, hogy a Windows 10 rendszerű eszköz konfigurációs beállításai hogyan felelnek meg az Intune-beállításoknak.
  
Az Intune-beállítás megkereséhez jelentkezzen be az Microsoft 365 Vállalati prémium verzió-rendszergazdai hitelesítő adataival, majd az [Azure Portal](https://portal.azure.com)webhelyen válassza a További szolgáltatások **lehetőséget,** írja be az Intune-t a Szűrő **mezőbe,** és válassza az **Intune** \> **Eszközkonfigurációs** profilok \> **lehetőséget.** Then select **Device policy for Windows 10** \> **Properties** \> **Settings**.
  
|**Eszközházirend Windows 10-es eszközhöz**|**Intune-beállítás(ok)**|
|:-----|:-----|
|A Windows Defender víruskereső használatával segíthet a PC-k vírusokkal és más fenyegetésekkel szembeni védelmében  <br/> |Valós idejű figyelés engedélyezése = BE  <br/> Felhővédelem engedélyezése = BE  <br/> Minták küldésének kérése a felhasználóktól = Biztonságos minták automatikus elküldése (személyazonosításra nem alkalmas alapértelmezett adatok automatikus elküldése)  <br/> |
|Segíthet megvédeni a PC-ket a Microsoft Edge-beli webes veszélyforrások ellen  <br/> |A **SmartScreen** a **Microsoft Edge böngésző beállításai** között **Kötelező** értékre van állítva.  <br/> |
|Az eszköz képernyőjének kikapcsolása ennyi üresjárati idő után (perc):  <br/> |Képernyőzárolás legfeljebb ennyi perc inaktivitás után  <br/> |
|A felhasználók letölthetnek appokat innen: Microsoft Áruház  <br/> |Egyéni URI-szabályzat  <br/> |
|A felhasználók hozzáférhetnek Cortanához  <br/> |**Általános** \> **Cortana** az Intune-ban **a** letiltás  van beállítva, ha a beállítás ki Microsoft 365 Vállalati prémium verzió.  <br/> |
|A felhasználók kaphatnak tippeket és hirdetéseket a Windowszal kapcsolatban a Microsofttól  <br/> |**Windows ,** minden le van tiltva, ha ez ki van kapcsolva **a** Microsoft 365 Vállalati prémium verzió.  <br/> |
|A Windows 10-es eszközök automatikus naprakészen tartása  <br/> | Ez a beállítás az **Microsoft Intune** \> **szolgáltatásfrissítések – Windows 10 Frissítési** körök , a Frissítési **házirend** beállítása Windows 10 eszközhöz , majd a **Tulajdonságok** és \> **Gépház.**  <br/>  Ha a Microsoft 365 Vállalati prémium verzió Be van **állítva,** az összes alábbi beállítás meg van állítva:  <br/> **A szolgáltatási ág** a **CB** (CBB, ha ez ki van kapcsolva a Microsoft 365 Vállalati prémium verzió).  <br/> A **Microsoft-termékfrissítések** beállítása **Engedélyezés**.  <br/> A **Windows-illesztőprogramok** beállítása **Engedélyezés**.  <br/> Az **Automatikus frissítési viselkedés** az **Automatikus telepítés karbantartáskor** értékre van állítva az alábbi beállításokkal:  <br/> Az **Aktív órák kezdete** **de. 6** órára van állítva.  <br/> Az **Aktív órák vége** **du. 10** órára van állítva.  <br/> A **Minőségi frissítések elhalasztása (nap)** **0** értékre van állítva.  <br/> A **Szolgáltatásfrissítések elhalasztása (nap)** **0** értékre van állítva.  <br/> A **Kézbesítésoptimalizálásos letöltési mód** a **HTTP ugyanazon NAT mögötti társviszony-létesítéssel kombinálva** értékre van állítva.  <br/> |
|||

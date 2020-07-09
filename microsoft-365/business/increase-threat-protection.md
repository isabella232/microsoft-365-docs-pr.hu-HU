---
title: A fenyegetések elleni védelem növelése a Microsoft 365 vállalati verzióban
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
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Állítsa be az Office 365 Komplex veszélyforrások elleni védelmet, és védje a bizalmas adatokat az adathalászattól, a rosszindulatú programoktól és más fenyegetésektől.
ms.openlocfilehash: 0e6cb7ed13a0851ef249e1f599d17e03c052414a
ms.sourcegitcommit: 3951147f74510e2ead6c11ceab92854f0937426b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/08/2020
ms.locfileid: "45083602"
---
# <a name="increase-threat-protection"></a>A veszélyforrások elleni védelem növelése

Ez a cikk segít növelni a Microsoft 365-előfizetés védelmét az adathalászat, a rosszindulatú programok és más fenyegetések elleni védelem érdekében. Ezek az ajánlások megfelelőek a fokozott biztonsági igényű szervezetek, például az ügyvédi irodák és az egészségügyi klinikák számára.

Mielőtt elkezdené, ellenőrizze az Office 365 biztonságos pontszámát. Az Office 365 biztonságos pontszáma a szokásos tevékenységek és biztonsági beállítások alapján elemzi a szervezet biztonságát, és pontokat rendel hozzá. Kezdje azzal, hogy tudomásul veszi a jelenlegi pontszámot. A pontszám növeléséhez végezze el a cikkben ajánlott műveleteket. A cél nem a maximális pontszám elérése, hanem a környezet védelmének lehetőségei, amelyek nem befolyásolják hátrányosan a felhasználók termelékenységét. 

További információt a [Microsoft biztonságos pontszáma című témakörben talál.](https://docs.microsoft.com/microsoft-365/security/mtp/microsoft-secure-score)

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>A rosszindulatú programok elleni védelem szintjének növelése e-mailben

Office 365-ös vagy Microsoft 365-ös környezete védelmet nyújt a kártevők ellen. Ezt a védelmet növelheti, ha blokkolja a rosszindulatú programokhoz gyakran használt fájltípusokkal rendelkező mellékleteket. A rosszindulatú programok elleni védelem növelése e-mailben:
  
1. Lépjen a [https://protection.office.com](https://protection.office.com) rendszergazdai fiók hitelesítő adataival, és jelentkezzen be. 
    
2. A Biztonsági &amp; megfelelőségi központ bal oldali navigációs ablakában, a **Fenyegetéskezelés**csoportban válassza a **Házirend** \> **kártevőirtó**lehetőséget.
    
3. Kattintson duplán az alapértelmezett házirendre a vállalati szintű házirend szerkesztéséhez.
    
4. Válassza a **Beállítások lehetőséget.**
    
5. A **Közös melléklettípusok szűrője**csoportban válassza **a Be**lehetőséget. A letiltott fájltípusok közvetlenül a vezérlő alatti ablakban jelennek meg. Győződjön meg arról, hogy hozzáadja a következő fájltípusokat:
   - ade, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, job, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, WSC, WSF, wsh, exe, pifif  <br/> 
   
   Szükség esetén később is hozzáadhat vagy törölhet fájltípusokat.
    
6. Válassza a **Mentés gombot.**
    
További információ: [Anti-malware protection](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409).
  
## <a name="protect-against-ransomware"></a>Védelem a zsarolóprogramok ellen

A zsarolóprogramok a fájlok titkosításával vagy a számítógép képernyőjének zárolásával korlátozzák az adatokhoz való hozzáférést. Ezután megpróbálja kizsarolni a pénzt az áldozatoktól azáltal, hogy "váltságdíjat" kér, általában kriptovaluták, mint a Bitcoin formájában, az adatokhoz való hozzáférésért cserébe. 
  
A zsarolóprogramok elleni védelem érdekében hozzon létre egy vagy több levelezési szabályt a zsarolóprogramokhoz gyakran használt fájlkiterjesztések letiltására. (Ezeket a szabályokat a [mail lépésben a rosszindulatú programok elleni védelem szintjének emelésében](#raise-the-level-of-protection-against-malware-in-mail) adta hozzá.) Figyelmeztetheti azokat a felhasználókat is, akik e-mailben kapják meg ezeket a mellékleteket.

Az előző lépésben letiltott fájlokon kívül célszerű olyan szabályt létrehozni, amely figyelmezteti a felhasználókat a makrókat tartalmazó Office-fájlmellékletek megnyitása előtt. A zsarolóprogramok elrejthetők a makrókban, ezért figyelmeztesse a felhasználókat, hogy ne nyissák meg ezeket a fájlokat olyan személyektől, akiket nem ismernek.

Levelezési átviteli szabály létrehozása:
  
1. Nyissa meg a felügyeleti központot <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> a területen, és válassza az Exchange **felügyeleti központok lehetőséget.** \> **Exchange**
    
2. A **levelezési** kategóriában válassza ki a **szabályokat.**
    
3. Válassza **+** a lehetőséget, majd válassza **az Új szabály létrehozása**lehetőséget.
    
4. A beállítások teljes készletének megtekintéséhez válassza a párbeszédpanel alján található **További beállítások** lehetőséget. 
    
5. Alkalmazza a szabályra vonatkozó alábbi táblázat beállításait. Használja az alapértelmezett értékeket a többi beállításhoz, hacsak nem szeretné módosítani őket.
    
6. Válassza a **Mentés** gombot.
    
|**Beállítás**|**A felhasználók figyelmeztetése az Office-fájlok mellékleteinek megnyitása előtt**||
|:-----|:-----|:-----|
|Name (Név)  <br/> |Zsarolóprogramok elleni szabály: figyelmeztesse a felhasználókat  <br/>  |
|Alkalmazza ezt a szabályt, ha a . . .  <br/> |Bármilyen mellékletet . . . fájlkiterjesztés megegyezik . . .  <br/> |
|Szavak vagy kifejezések megadása  <br/> |Adja hozzá a következő fájltípusokat:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm  <br/>|
|Tegye a következőket . . .  <br/> |A címzett értesítése üzenettel  <br/> |
|Üzenet szövegének megadásá  <br/> |Ne nyisson meg ilyen típusú fájlokat olyan személyektől, akiket nem ismer, mert rosszindulatú kódot tartalmazó makrókat tartalmazhatnak.  <br/> |
   
További információ:
  
- [Hogyan kezeljük a zsarolóprogramokat?](https://go.microsoft.com/fwlink/?linkid=2016501)
    
- [A OneDrive visszaállítása](https://support.microsoft.com/office/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>E-mailek automatikus továbbításának leállítása

Azok a hackerek, akik hozzáférnek egy felhasználó postaládájához, ellophatják az e-maileket, ha úgy állítja be a postaládát, hogy automatikusan továbbítsa az e-maileket. Ez akkor is megtörténhet, anélkül, hogy a felhasználó figyelmét. Ennek elkerülése érdekében állítson be egy levelezési szabályt. 
  
E-mail átviteli szabály létrehozásához tekintse meg [ezt a rövid videót,](https://support.microsoft.com/office/f9d693ba-5c78-47c0-b156-8e461e062aa7) vagy kövesse az alábbi lépéseket:
  
1. A Microsoft 365 Felügyeleti központban válassza az Exchange **felügyeleti központok lehetőséget.** \> **Exchange**
    
2. A **levelezési** kategóriában válassza ki a **szabályokat.**
    
3. Válassza **+** a lehetőséget, majd válassza **az Új szabály létrehozása**lehetőséget.
    
4. Az összes beállítás megtekintéséhez válassza a párbeszédpanel alján található **További beállítások lehetőséget.** 
    
5. Alkalmazza az alábbi táblázat beállításait. Használja az alapértelmezett értékeket a többi beállításhoz, hacsak nem szeretné módosítani őket.
    
6. Válassza a **Mentés** gombot.
    
|**Beállítás**|**A felhasználók figyelmeztetése az Office-fájlok mellékleteinek megnyitása előtt**|
|:-----|:-----|
|Name (Név)  <br/> |Az e-mailek külső tartományokba történő automatikus továbbításának megakadályozása  <br/> |
|Alkalmazza ezt a szabályt, ha ...  <br/> |A feladó . . . külső/belső. . . A szervezeten belül  <br/> |
|Feltétel hozzáadása  <br/> |Az üzenet tulajdonságai . . . tartalmazza az üzenet típusát . . . Automatikus előre  <br/> |
|Tegye a következőket ...  <br/> |Az üzenet blokkolása . . . elutasítja az üzenetet, és magyarázatot tartalmaz.  <br/> |
|Üzenet szövegének megadásá  <br/> |Biztonsági okokból az e-mailek szervezeten kívüli automatikus továbbítása nem történik meg.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Az e-mailek védelme az adathalász támadások ellen

Ha egy vagy több egyéni tartományt konfigurált az Office 365- vagy microsoft 365-ös környezetéhez, beállíthatja a célzott adathalászat elleni védelmet. Az Office 365 Komplex veszélyforrások elleni védelem részét vevő ATP adathalászat elleni védelem segít megvédeni a szervezetet a rosszindulatú, megszemélyesítésen alapuló adathalász támadásoktól és más adathalász támadásoktól. Ha még nem konfigurált egyéni tartományt, erre nincs szükség.
  
Javasoljuk, hogy a legfontosabb felhasználók és az egyéni tartomány védelmét szolgáló házirend létrehozásával kezdje el ezt a védelmet. 

Az adathalászat elleni ATP-házirend létrehozásához tekintse meg [ezt a rövid oktatóvideót,](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)vagy hajtsa végre az alábbi lépéseket:
  
1. Nyissa meg a [https://protection.office.com](https://protection.office.com) lapot. 
    
2. A Biztonsági &amp; megfelelőségi központ bal oldali navigációs ablakában, a **Fenyegetéskezelés**csoportban válassza a **Házirend**lehetőséget.
    
3. A **Szabályzat** lapon válassza az **ATP adathalászat elleni**lehetőséget.
    
4. Az **Adathalászat elleni** lapon válassza a + Create **(Létrehozás) lehetőséget.** Egy varázsló elindítja, amely végigvezeti az adathalászat elleni házirend meghatározásán.
    
5. Adja meg a házirend nevét, leírását és beállításait az alábbi táblázatban ajánlott módon. További információt az [Adathalászat elleni atp-házirendek című](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies)témakörben talál. 
    
6. Miután áttekintette a beállításokat, válassza **a Házirend létrehozása** vagy a **Mentés**lehetőséget.
    

|**Beállítás vagy beállítás**<br/>|**Ajánlott beállítás** <br/>|
|:-----|:-----|
|Name (Név)  <br/> |Domain és legértékesebb kampányszemélyzet  <br/> |
|Leírás  <br/> |Győződjön meg róla, hogy a legfontosabb munkatársak és a birtokunk nem személyesítik meg őket.  <br/> |
|Felhasználók hozzáadása a védelemhez  <br/> |Válassza a **+ Feltétel hozzáadása lehetőséget, a címzett .** Írja be a felhasználóneveket, vagy adja meg a jelölt, a kampánymenedzser és más fontos munkatársak e-mail címét. Legfeljebb 20 belső és külső címet adhat hozzá, amelyeket meg szeretne védeni a megszemélyesítéstől.  <br/> |
|Tartományok hozzáadása a védelemhez  <br/> |Válassza a **+ Feltétel hozzáadása lehetőséget, A címzett tartomány .** Ha definiált egyet, adja meg a Microsoft 365-előfizetéséhez társított egyéni tartományt. Több tartományt is megadhat.  <br/> |
|Műveletek kiválasztása  <br/> |Ha egy megszemélyesített felhasználó küld e-mailt: Válassza **az Üzenet átirányítása másik e-mail címre**lehetőséget, majd írja be a biztonsági rendszergazda e-mail címét; *például: Alice <span> <span> @contoso.com*. Ha az e-mailt megszemélyesített tartomány küldi: Válassza a **Karantén üzenet**lehetőséget.  <br/> |
|Postaláda-intelligencia  <br/> |Alapértelmezés szerint a postaláda-intelligencia lesz kiválasztva, amikor új adathalászat elleni házirendet hoz létre. A legjobb eredmény érdekében hagyja **bekapcsolva** ezt a beállítást.  <br/> |
|Megbízható feladók és tartományok hozzáadása  <br/> |Itt hozzáadhatja saját tartományát vagy bármely más megbízható tartományát.  <br/> |
|Alkalmazása  <br/> |Válassza a **Címzett tartomány t.** **A(z) Bármelyik csoportban**válassza a **Választás lehetőséget.** Válassza **a + Hozzáadás lehetőséget.** Jelölje be a tartomány neve melletti jelölőnégyzetet, például *contoso. <span> <span> com*, a listában, majd válassza **a Hozzáadás**lehetőséget. Válassza a **Kész**lehetőséget.  <br/> |
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>A rosszindulatú mellékletek és fájlok elleni védelem az ATP biztonságos mellékletekkel

A személyek rendszeresen küldenek, fogadnak és osztanak meg mellékleteket, például dokumentumokat, bemutatókat, táblázatokat stb. Nem mindig könnyű megállapítani, hogy egy melléklet biztonságos vagy rosszindulatú-e, csak egy e-mail üzenet ből. Az Office 365 Komplex veszélyforrások elleni védelem tartalmazza az ATP biztonságos mellékletek védelmét, de ez a védelem alapértelmezés szerint nincs bekapcsolva. Azt javasoljuk, hogy hozzon létre egy új szabályt a védelem használatának megkezdéséhez. Ez a védelem kiterjed a SharePoint, a OneDrive és a Microsoft Teams fájljaira is.
  
Az ATP biztonságos csatolási házirendjének létrehozásához tekintse meg [ezt a rövid videót,](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)vagy hajtsa végre az alábbi lépéseket:
  
1. Nyissa meg a [https://protection.office.com](https://protection.office.com) t, és jelentkezzen be a rendszergazdai fiókjával. 
    
2. A Biztonsági &amp; megfelelőségi központ bal oldali navigációs ablakában, a **Fenyegetéskezelés**csoportban válassza a **Házirend**lehetőséget.
    
3. A Házirend lapon válassza az **ATP biztonságos mellékletek**lehetőséget.
    
4. A Biztonságos mellékletek lapon széles körben alkalmazhatja ezt a védelmet a SharePoint, a OneDrive és a **Microsoft Teams atp bekapcsolása** jelölőnégyzet bejelölésével. 
    
5. Új házirend létrehozásához válassza ezt **+** a lehetőséget. 
    
6. Alkalmazza az alábbi táblázat beállításait. 
    
7. Miután áttekintette a beállításokat, válassza **a Házirend létrehozása** vagy a **Mentés**lehetőséget.
    

|**Beállítás vagy beállítás**|**Ajánlott beállítás** <br/>|
|:-----|:-----|
|Name (Név)  <br/> |Blokkolja a jelenlegi és jövőbeli e-maileket észlelt rosszindulatú programokkal.  <br/> |
|Leírás  <br/> |Blokkolja a jelenlegi és jövőbeli e-maileket és mellékleteket az észlelt rosszindulatú programokkal.  <br/> |
|Mellékletek mentése ismeretlen kártevőválasz  <br/> |Válassza **a Blokk - A jelenlegi és jövőbeli e-mailek és mellékletek blokkolása észlelt rosszindulatú programokkal.**  <br/> |
|Melléklet átirányítása észleléseken  <br/> |Átirányítás engedélyezése (jelölje be ezt a jelölőnégyzetet) Adja meg a rendszergazdai fiókot vagy a karanténhoz beállított postaláda-beállítást.          Alkalmazza a fenti kijelölést, ha a mellékletek rosszindulatú keresése túllépi az idődet vagy hiba történik (jelölje be ezt a jelölőnégyzetet).  <br/> |
|Alkalmazása  <br/> |A címzett tartomány a. . . válassza ki a tartományt.  <br/> |
   
További információt az [Office 365 ATP adathalászat elleni irányelveinek beállítása](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies)című témakörben talál.
  
## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Az ATP safe links segítségével védelmet nyújt az adathalász támadások ellen

A hackerek néha elrejtik a rosszindulatú webhelyeket az e-mailben vagy más fájlokban található hivatkozásokban. Az Office 365 Komplex veszélyforrások elleni védelem részét szolgáló Office 365 ATP safe links (ATP Safe Links) az E-mail üzenetekben és az Office-dokumentumokban található webcímek (URL-címek) ellenőrzésével segít megvédeni a szervezetet. A védelmet az ATP biztonságos hivatkozásokra vonatkozó házirendek határozzák meg.
  
Javasoljuk, hogy tegye a következőket:
  
- Módosítsa az alapértelmezett házirendet a védelem növeléséhez.
    
- Adjon hozzá egy új házirendet a tartomány összes címzettjének.
    
Az ATP Safe Links beállításához tekintse meg [ezt a rövid oktatóvideót,](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)vagy hajtsa végre az alábbi lépéseket:
  
1. Nyissa meg a [https://protection.office.com](https://protection.office.com) t, és jelentkezzen be a rendszergazdai fiókjával. 
    
2. A Biztonsági &amp; megfelelőségi központ bal oldali navigációs ablakában, a **Fenyegetéskezelés**csoportban válassza a **Házirend**lehetőséget.
    
3. A Házirend lapon válassza az **ATP biztonságos hivatkozások lehetőséget.**
    
Az alapértelmezett házirend módosítása:
  
1. A Biztonságos hivatkozások lap **A teljes szervezetre vonatkozó házirendek**csoportban válassza az **Alapértelmezett** házirendet. 
    
2. Az **e-mail kivételével a tartalomra vonatkozó Beállítások csoportban**válassza a **Microsoft 365 Apps for Enterprise, az Office for iOS és az Android**lehetőséget.
    
3. Válassza a **Mentés** gombot. 
    
Új házirend létrehozása a tartomány összes címzettje számára:
  
1. A Biztonságos hivatkozások lap **A teljes szervezetre vonatkozó házirendek**csoportban válassza az **+** új házirend létrehozásához. 
    
2. Alkalmazza az alábbi táblázatban felsorolt beállításokat.
    
3. Válassza a **Mentés** gombot. 

|**Beállítás vagy beállítás**|**Ajánlott beállítás** <br/>|
|:-----|:-----|
|Name (Név)  <br/> |Biztonságos hivatkozásokra vonatkozó házirend a tartomány összes címzettje számára  <br/> |
|Válassza ki az üzenetekben lévő ismeretlen, potenciálisan kártékony URL-ek műveletét  <br/> |Válassza **a Be lehetőséget - Az URL-ek újraírása és összevetése az ismert rosszindulatú hivatkozások listájával, amikor a felhasználó a hivatkozásra kattint.**  <br/> |
|Letölthető tartalmak biztonságos mellékletekkel való bekéseléséhez  <br/> |Jelölje be ezt a jelölőnégyzetet.  <br/> |
|Alkalmazása  <br/> |A címzett tartomány a. . . válassza ki a tartományt.  <br/> |
   
További információt az [Office 365 ATP biztonságos hivatkozásai című témakörben talál.](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409)

## <a name="go-to-intune-admin-center"></a>Ugrás az Intune Felügyeleti központba

1. Jelentkezzen be az [Azure Portalra.](https://portal.azure.com/)

2. Válassza a **Minden szolgáltatás** lehetőséget, és írja be az *Intune-ba* a **Keresőmezőbe jelölőnégyzetet.**

3. Miután az eredmények megjelennek, válassza ki a **Microsoft Intune** melletti startot, hogy az kedvenc legyen, és később könnyen megtalálható legyen.

A felügyeleti központ mellett az Intune-nal is regisztrálhatja és kezelheti a szervezet eszközeit. További információt a [Windows-eszközök höz szükséges beállítások](https://docs.microsoft.com/intune/enrollment/enrollment-method-capab) és az Intune által felügyelt eszközök igénylési beállításai című [témakörben talál.](https://docs.microsoft.com/intune/enrollment-options)

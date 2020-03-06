---
title: A Microsoft 365 Business veszélyforrások elleni védelmének növelése
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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
description: Állítsa be az Office 365 komplex veszélyforrások elleni védelmet, és védje a bizalmas adatokat az adathalászattól, a rosszindulatú programoktól és más fenyegetésektől.
ms.openlocfilehash: 9d7bae60091c87fa0246a697f2a49e1cbc6e2f06
ms.sourcegitcommit: 26e4d5091583765257b7533b5156daa373cd19fe
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/06/2020
ms.locfileid: "42550357"
---
# <a name="increase-threat-protection"></a>A fenyegetésvédelem növelése

Ez a cikk segít növelni a védelmet a Microsoft 365-előfizetésben az adathalászat, a rosszindulatú programok és más fenyegetések elleni védelem érdekében. Ezek az ajánlások megfelelőszervezetek számára fokozott biztonságiránti igény, mint a ügyvédi irodák és az egészségügyi klinikák.

Mielőtt elkezdené, ellenőrizze az Office 365 biztonságos pontszámát. Az Office 365 Biztonságos pontszám a szokásos tevékenységek és biztonsági beállítások alapján elemzi az Office 365-szervezet biztonságát, és hozzárendel egy pontszámot. Kezdje azzal, hogy tudomásul veszi az aktuális pontszámot. A pontszám növeléséhez hajtsa végre az ebben a cikkben ajánlott műveleteket. A cél nem a maximális pontszám elérése, hanem az, hogy tudatában legyünk a környezet védelmére vonatkozó lehetőségeknek, amelyek nem befolyásolják hátrányosan a felhasználók termelékenységét. 

További információt a [Microsoft Secure Score](https://docs.microsoft.com/office365/securitycompliance/microsoft-secure-score)című témakörben talál.

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Növelje a rosszindulatú programok elleni védelem szintjét a levelekben

Az Office 365-ös vagy a Microsoft 365-környezet védelmet nyújt a kártevők ellen. Ezt a védelmet növelheti, ha blokkolja a rosszindulatú programokhoz gyakran használt fájltípusokhoz kapcsolódó mellékleteket. A rosszindulatú programok elleni védelem növelése e-mailben:
  
1. Nyissa [https://protection.office.com](https://protection.office.com) meg és jelentkezzen be a rendszergazdai fiók hitelesítő adataival. 
    
2. Az Office 365 &amp; Biztonsági megfelelőségi központjának bal oldali navigációs ablaktáblájában, a **Veszélykezelés**csoportban válassza a **Házirend** \> **kártevőirtó**ja.
    
3. Kattintson duplán az alapértelmezett házirendre a vállalati szintű házirend szerkesztéséhez.
    
4. Válassza a **Beállítások**lehetőséget.
    
5. A **Gyakori melléklettípusok szűrő**csoportban válassza a **Be**lehetőséget. A letiltott fájltípusok közvetlenül a vezérlő alatti ablakban jelennek meg. Győződjön meg arról, hogy ezeket a fájltípusokat adja hozzá:
   - ade, adp, ani, bas, denevér, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, job, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, PCD, reg, scr, sct, shs, url, vb, vbe, vbs, vbs, wsc, wsf, wsh, exe, pif  <br/> 
   
   Szükség esetén később is hozzáadhat vagy törölhet idõt.
    
6. Válassza a **Mentés gombot.**
    
További [információ: Anti-malware protection](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409).
  
## <a name="protect-against-ransomware"></a>Védelem a zsarolóprogramok ellen

A zsarolóprogramok a fájlok titkosításával vagy a számítógép képernyőinek zárolásával korlátozzák az adatokhoz való hozzáférést. Ezután megpróbálja kizsarolni a pénzt az áldozatoktól a "váltságdíj" kérésével, általában kriptovaluták formájában, mint a Bitcoin, az adatokhoz való hozzáférésért cserébe. 
  
A zsarolóprogramok elleni védelem érdekében hozzon létre egy vagy több levélfolyam-szabályt a zsarolóprogramokhoz gyakran használt fájlkiterjesztések blokkolására. (Ezeket a szabályokat a rosszindulatú programok elleni védelem szintjének emelése a [levelezési lépésben](#raise-the-level-of-protection-against-malware-in-mail) adta hozzá.) Figyelmeztetheti azokat a felhasználókat is, akik e-mailben kapják meg ezeket a mellékleteket.

Az előző lépésben letiltott fájlokon kívül célszerű olyan szabályt létrehozni, amely figyelmezteti a felhasználókat a makrókat tartalmazó Office-fájlmellékletek megnyitása előtt. Zsarolóprogramok lehet rejtett belül makrók, ezért figyelmeztesse a felhasználókat, hogy ne nyissa meg ezeket a fájlokat az emberek nem tudják.

Levélátviteli szabály létrehozása:
  
1. Nyissa meg a <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>felügyeleti központot a , és válassza a **Felügyeleti központok** \> **Exchange**lehetőséget.
    
2. A **levelezési** kategóriában válassza a **szabályokat.**
    
3. Válassza **+** a lehetőséget, majd válassza az **Új szabály létrehozása**lehetőséget.
    
4. A párbeszédpanel alján az **További beállítások** lehetőséget választva megtekintheti a beállítások teljes készletét. 
    
5. Alkalmazza a következő táblázatban szereplő beállításokat a szabályhoz. A többi beállítás alapértelmezett értékeit használja, hacsak nem szeretné módosítani őket.
    
6. Válassza a **Mentés** gombot.
    
|**Beállítás**|**A felhasználók figyelmeztetése az Office-fájlok mellékleteinek megnyitása előtt**||
|:-----|:-----|:-----|
|Name (Név)  <br/> |Zsarolóprogramok elleni szabály: figyelmeztesse a felhasználókat  <br/>  |
|Alkalmazza ezt a szabályt, ha . . .  <br/> |Bármilyen mellékletet . . . fájlkiterjesztés egyezik. . .  <br/> |
|Szavak vagy kifejezések megadása  <br/> |Adja hozzá ezeket a fájltípusokat:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm  <br/>|
|Tegye a következőket. . .  <br/> |A címzett értesítése üzenettel  <br/> |
|Üzenet szövegének biztosítása  <br/> |Ne nyisson meg ilyen típusú fájlokat olyan személyektől, akiket nem ismer, mert rosszindulatú kódot tartalmazó makrókat tartalmazhatnak.  <br/> |
   
További információ:
  
- [Hogyan kezeljük a zsarolóprogramokat?](https://go.microsoft.com/fwlink/?linkid=2016501)
    
- [A OneDrive visszaállítása](https://support.office.com/article/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>E-mailek automatikus továbbításának leállítása

Azok a hackerek, akik hozzáférnek a felhasználó postaládájához, ellophatják az e-maileket, ha a postaládát úgy állítják be, hogy automatikusan továbbítsák az e-maileket. Ez akkor is megtörténhet, ha a felhasználó tudomása nélkül. Ennek elkerülése érdekében állítson be egy levélfolyam-szabályt. 
  
Levélátviteli szabály létrehozásához tekintse meg [ezt a rövid videót,](https://support.office.com/article/f9d693ba-5c78-47c0-b156-8e461e062aa7) vagy kövesse az alábbi lépéseket:
  
1. A Microsoft 365 Felügyeleti központban válassza a **Felügyeleti központok** \> **Exchange**lehetőséget.
    
2. A **levelezési** kategóriában válassza a **szabályokat.**
    
3. Válassza **+** a lehetőséget, majd válassza az **Új szabály létrehozása**lehetőséget.
    
4. Az összes beállítás megtekintéséhez válassza az **Egyebek beállítások** lehetőséget a párbeszédpanel alján. 
    
5. Alkalmazza a beállításokat az alábbi táblázatban. A többi beállítás alapértelmezett értékeit használja, hacsak nem szeretné módosítani őket.
    
6. Válassza a **Mentés** gombot.
    
|**Beállítás**|**A felhasználók figyelmeztetése az Office-fájlok mellékleteinek megnyitása előtt**|
|:-----|:-----|
|Name (Név)  <br/> |Az e-mailek automatikus átvitelének megakadályozása külső tartományokba  <br/> |
|Alkalmazza ezt a szabályt, ha ...  <br/> |A feladó . . . külső/belső . . . A szervezeten belül  <br/> |
|Feltétel hozzáadása  <br/> |Az üzenet tulajdonságai . . . tartalmazza az üzenet típusát . . . Automatikus előrekapcsolás  <br/> |
|Tegye a következő ...  <br/> |Az üzenet blokkolása . . . elutasítja az üzenetet, és magyarázatot tartalmaz.  <br/> |
|Üzenet szövegének biztosítása  <br/> |Biztonsági okokból a szervezeten kívüli automatikus továbbítás a szervezeten kívül reked.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Védje e-mailjeit az adathalász támadásoktól

Ha egy vagy több egyéni tartományt konfigurált az Office 365-ös vagy a Microsoft 365-környezetéhez, konfigurálhatja a célzott adathalászat elleni védelmet. Az Office 365 Komplex veszélyforrások elleni védelem részét kitevő ATP adathalászat elleni védelem segít megvédeni a szervezetet a rosszindulatú megszemélyesítésen alapuló adathalász támadásoktól és más adathalász támadásoktól. Ha még nem konfigurált egyéni tartományt, ezt nem kell megtennie.
  
Azt javasoljuk, hogy kezdje el ezt a védelmet egy szabályzat létrehozásával, amely megvédi a legfontosabb felhasználókat és az egyéni tartományt. 

Atp adathalászat elleni házirend létrehozásához tekintse meg [ezt a rövid oktatóvideót,](https://support.office.com/article/86c425e1-1686-430a-9151-f7176cce4f2c)vagy hajtsa végre az alábbi lépéseket:
  
1. Nyissa meg a [https://protection.office.com](https://protection.office.com) lapot. 
    
2. Az Office 365 &amp; Biztonsági megfelelőségi központ bal oldali navigációs ablakának **Fenyegetéskezelés**területén válassza a **Házirend**lehetőséget.
    
3. Az **Irányelv** lapon válassza az **ATP adathalászat elleni választójogát.**
    
4. Az **adathalászat elleni** lapon válassza a **+ Létrehozás**lehetőséget. Egy varázsló elindítja, amely végigvezeti az adathalászat elleni szabályzat meghatározásán.
    
5. Adja meg a házirend nevét, leírását és beállításait az alábbi táblázatban ajánlott módon. További [részletek: Ismerje meg az ATP adathalászat elleni házirend-beállításait.](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies#learn-about-atp-anti-phishing-policy-options) 
    
6. Miután áttekintette a beállításokat, válassza **a Házirend létrehozása** vagy a **Mentés**lehetőséget.
    

|**Beállítás vagy beállítás**<br/>|**Ajánlott beállítás** <br/>|
|:-----|:-----|
|Name (Név)  <br/> |Domain és legértékesebb kampány személyzet  <br/> |
|Leírás  <br/> |Győződjön meg róla, hogy a legfontosabb személyzet és a domain nem megszemélyesített.  <br/> |
|Felhasználók hozzáadása a védelemhez  <br/> |Válassza **a + Feltétel hozzáadása lehetőséget, a címzett a**. Írja be a felhasználóneveket, vagy adja meg a jelölt, a kampánymenedzser és más fontos munkatársak e-mail címét. Legfeljebb 20 belső és külső címet adhat hozzá, amelyeket meg szeretne védeni a megszemélyesítéstől.  <br/> |
|Védelemre szolgáló tartományok hozzáadása  <br/> |Válassza **a + Feltétel hozzáadása lehetőséget, a címzett tartománya**a . Adja meg a Microsoft 365-előfizetéséhez társított egyéni tartományt, ha definiált egyet. Egynél több tartományt is megadhat.  <br/> |
|Műveletek kiválasztása  <br/> |Ha egy megszemélyesített felhasználó küldi az e-mailt: Válassza **az Átirányítási üzenet másik e-mail címre lehetőséget,** majd írja be a biztonsági rendszergazda e-mail címét; például *Alice<span><span>@contoso.com*. Ha az e-mailt megszemélyesített tartomány küldi: Válassza a **Karantén üzenetet**.  <br/> |
|Postaláda-intelligencia  <br/> |Alapértelmezés szerint a postaláda-intelligencia van kiválasztva, amikor új adathalászat elleni házirendet hoz létre. Hagyja ezt a beállítást **Be** a legjobb eredmény érdekében.  <br/> |
|Megbízható feladók és tartományok hozzáadása  <br/> |Itt hozzáadhatja saját vagy bármely más megbízható tartományát.  <br/> |
|Alkalmazva:  <br/> |Válassza **a címzett tartománya**lehetőséget. Ezek **közül bármelyik**csoportban válassza a **lehetőséget.** Válassza a **+ Hozzáadás**lehetőséget. Jelölje be a tartomány neve melletti jelölőnégyzetet, például *contoso.<span> com <span>*, a listában, majd válassza a **Hozzáadás**lehetőséget. Válassza **a Kész**lehetőséget.  <br/> |
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Védelmet nyújt a rosszindulatú mellékletek és fájlok ellen AZ ATP biztonságos mellékleteivel

A személyek rendszeresen küldenek, fogadnak és osztanak meg mellékleteket, például dokumentumokat, bemutatókat, táblázatokat stb. Nem mindig könnyű megállapítani, hogy egy melléklet biztonságos vagy rosszindulatú-e, ha csak egy e-mailt néz. Az Office 365 komplex veszélyforrások elleni védelem tartalmazza az ATP biztonságos mellékletek védelmét, de ez a védelem alapértelmezés szerint nincs bekapcsolva. Azt javasoljuk, hogy hozzon létre egy új szabályt, hogy elkezdi használni ezt a védelmet. Ez a védelem kiterjed a SharePoint, a OneDrive és a Microsoft Teams fájljaira is.
  
Atp-biztos mellékletre vonatkozó házirend létrehozásához tekintse meg [ezt a rövid videót,](https://support.office.com/article/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)vagy hajtsa végre a következő lépéseket:
  
1. Nyissa [https://protection.office.com](https://protection.office.com)meg a lehetőséget, és jelentkezzen be rendszergazdai fiókjával. 
    
2. Az Office 365 &amp; Biztonsági megfelelőségi központ bal oldali navigációs ablakának **Fenyegetéskezelés**területén válassza a **Házirend**lehetőséget.
    
3. A Házirend lapon válassza az **ATP biztonságos mellékleteit.**
    
4. A Biztonságos mellékletek lapon alkalmazza ezt a védelmet nagyjából a SharePoint, a OneDrive és a **Microsoft Teams ATP-jének bekapcsolása** jelölőnégyzet bejelölésével. 
    
5. Jelölje **+** be új házirend létrehozásához jelölőnégyzetet. 
    
6. Alkalmazza a beállításokat az alábbi táblázatban. 
    
7. Miután áttekintette a beállításokat, válassza **a Házirend létrehozása** vagy a **Mentés**lehetőséget.
    

|**Beállítás vagy beállítás**|**Ajánlott beállítás** <br/>|
|:-----|:-----|
|Name (Név)  <br/> |Tiltsa le az aktuális és jövőbeli e-maileket észlelt kártevőkkel.  <br/> |
|Leírás  <br/> |Tiltsa le az aktuális és jövőbeli e-maileket és mellékleteket észlelt kártevőkkel.  <br/> |
|Mellékletek mentése ismeretlen kártevő-válasz  <br/> |Válassza a **Blokk – Az aktuális és jövőbeli e-mailek és mellékletek letiltása észlelt kártevővel**.  <br/> |
|Melléklet átirányítása észlelésre  <br/> |Átirányítás engedélyezése (jelölje be ezt a jelölőnégyzetet) Adja meg a rendszergazdai fiókot vagy a postaláda beállítását karanténba.          Alkalmazza a fenti beállítást, ha a mellékleteket keresése kori időtúllépés vagy hiba történik (ezt a jelölőnégyzetet jelölve).  <br/> |
|Alkalmazva:  <br/> |A címzett tartománya a . . . válassza ki a tartományt.  <br/> |
   
További információt [az Office 365 ADAThalászat elleni irányelveinek beállítása](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies)című témakörben talál.
  


## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Védelmet nyújt az adathalász támadások ellen az ATP biztonságos hivatkozásaival

A hackerek néha e-mailben vagy más fájlban rejtik el a rosszindulatú webhelyeket. Az Office 365 ATP biztonságos hivatkozásai (ATP biztonságos hivatkozások) az Office 365 komplex veszélyforrások elleni védelem részét képezik, és segíthetnek megvédeni a szervezetet azáltal, hogy az e-mailekben és az Office-dokumentumokban biztosítják a webcímek (URL-ek) kattintásos ellenőrzését. A védelem az ATP biztonságos hivatkozásokra vonatkozó irányelvei vel határozható meg.
  
Javasoljuk, hogy tegye a következőket:
  
- Módosítsa az alapértelmezett házirendet a védelem növelése érdekében.
    
- Adjon hozzá egy új házirendet, amely a tartomány összes címzettjét célozza meg.
    
Az ATP biztonságos hivatkozások beállításához tekintse meg [ezt a rövid oktatóvideót,](https://support.office.com/article/61492713-53c2-47da-a6e7-fa97479e97fa)vagy hajtsa végre az alábbi lépéseket:
  
1. Nyissa [https://protection.office.com](https://protection.office.com)meg a lehetőséget, és jelentkezzen be rendszergazdai fiókjával. 
    
2. Az Office 365 &amp; Biztonsági megfelelőségi központ bal oldali navigációs ablakának **Fenyegetéskezelés**területén válassza a **Házirend**lehetőséget.
    
3. A Házirend lapon válassza az **ATP biztonságos hivatkozások**lehetőséget.
    
Az alapértelmezett házirend módosítása:
  
1. A Biztonságos hivatkozások lap **Házirendek a teljes szervezetre vonatkozó házirendek**csoportban válassza az **Alapértelmezett** házirend lehetőséget. 
    
2. A **levelezésen kívül álló tartalmakra vonatkozó beállítások**csoportban válassza az Office **365 ProPlus,** az iOS és az Android Office lehetőséget.
    
3. Válassza a **Mentés** gombot. 
    
Új házirend létrehozása, amely a tartomány összes címzettjét célozza meg:
  
1. A Biztonságos hivatkozások lap **Házirendek a teljes szervezetre vonatkozó házirendek**csoportban válassza az **+** új házirend létrehozásához lehetőséget. 
    
2. Alkalmazza az alábbi táblázatban felsorolt beállításokat.
    
3. Válassza a **Mentés** gombot. 

|**Beállítás vagy beállítás**|**Ajánlott beállítás** <br/>|
|:-----|:-----|
|Name (Név)  <br/> |Biztonságos hivatkozásra vonatkozó házirend a tartomány összes címzettje számára  <br/> |
|Ismeretlen, potenciálisan rosszindulatú URL-címek műveletének kiválasztása az üzenetekben  <br/> |Válassza a **Be - URL-eket átírják, és összeveti az ismert rosszindulatú linkek listáját, amikor a felhasználó rákattint a linkre**.  <br/> |
|A letölthető tartalmak bevizsgálata biztonságos mellékletekkel  <br/> |Jelölje be ezt a jelölőnégyzetet.  <br/> |
|Alkalmazva:  <br/> |A címzett tartománya a . . . válassza ki a tartományt.  <br/> |
   
További információt az [Office 365 ATP biztonságos hivatkozásai](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409)című témakörben talál.

## <a name="go-to-intune-admin-center"></a>Ugrás az Intune Felügyeleti központra

1. Jelentkezzen be az [Azure Portalra](https://portal.azure.com/).

2. Válassza az **Összes szolgáltatás lehetőséget,** és írja be az *Intune-t* a **Keresőmezőbe.**

3. Miután az eredmények megjelennek, válassza ki a **Microsoft Intune** melletti kezdést, hogy később kedvencés könnyen megtalálható legyen.

A felügyeleti központ mellett az Intune-nal is regisztrálhatja és kezelheti a szervezet eszközeit. További információt a [Windows-eszközök retusáltas sága](https://docs.microsoft.com/intune/enrollment/enrollment-method-capab) és [az Intune által kezelt eszközök igénylési beállításai](https://docs.microsoft.com/intune/enrollment-options)című témakörben talál.

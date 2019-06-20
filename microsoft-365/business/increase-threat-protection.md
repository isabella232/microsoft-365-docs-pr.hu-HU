---
title: Fenyegetés növelhető a Microsoft 365 üzleti
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
search.appverid:
- BCS160
- MET150
description: Állítsa be az Office 365 speciális veszély védelmi, és a bizalmas adatok védelme.
ms.openlocfilehash: b6e9941eee9de4f295b0f8056c1c91b7076e530c
ms.sourcegitcommit: 7ac06563c6ff034358e8fd3f9298fc426187ade2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/31/2019
ms.locfileid: "35086343"
---
# <a name="increase-threat-protection"></a>Fenyegetés növelhető.

Ez a cikk segítséget nyújt a Microsoft 365 előfizetése adathalász, malware és egyéb fenyegetések elleni védelme növelése. Ezeket az ajánlásokat is megfelelő szervezetek számára a biztonság, mint jogi irodák és egészségügyi klinikák fokozott szükségességét.

Mielőtt elkezdené, ellenőrizze az Office 365 biztonságos pontszám. Office 365 biztonságos pontszám alapján rendszeres tevékenységek és a biztonsági beállítások az Office 365 szervezet biztonsági elemzi, és hozzárendel egy pontszámot. Első lépésként a pillanatnyi pontszámunkat tudomásul véve. A cikkben javasolt műveletek végrehajtása a számítógép pontszáma növekszik. Célja nem a maximális pontszám elérése érdekében, de ne feledje, a környezet védelme érdekében a lehetőségek, amelyek negatívan befolyásolja a felhasználók számára a termelékenység. 

További tudnivalókért tanulmányozza [A Microsoft biztonságos pontszám](https://docs.microsoft.com/en-us/office365/securitycompliance/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>A levelek a kártevők elleni védelem szintjének emelése

Az Office 365 vagy Microsoft 365 környezetben a kártevők elleni védelem magában foglalja, de a védelem tovább növelhető, kártevő általánosan használt fájltípusok a mellékletek blokkolását. E-mailben a rosszindulatú programok elleni védekezés növelése:
  
1. Ugrás a [https://protection.office.com](https://protection.office.com) , és jelentkezzen be a rendszergazdai fiók hitelesítő adatait. 
    
2. Az Office 365 a &amp; Megfelelési központba, a bal oldali navigációs ablaktábla **fenyegetés kezelése**, válassza **a házirend** \> **Kártevőirtó**.
    
3. Kattintson duplán az alapértelmezett házirend a vállalati szintű házirendet kíván módosítani.
    
4. Kattintson a **Beállítások**gombra.
    
5. ** **Általános melléklet típusú szűrő**csoportban jelölje be.** A blokkolt fájltípusok közvetlenül alatt ez a vezérlő az ablakban jelennek meg.  Ellenőrizze, e fájl típusai:
   - ADE, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, modulok, isp, feladat, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif  <br/> Adjunk hozzá, vagy később, törölje a fájltípusok, szükség esetén.
    
6. Kattintson a **menteni.**
    
További információért lásd: [Anti-malware védelem](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409).
  
## <a name="protect-against-ransomware"></a>Ransomware elleni védelem

Ransomware korlátozza a hozzáférést a adatok által titkosított fájlok, vagy zárolni szeretné a számítógép képernyőjén. Majd megpróbálja extort a pénzt az áldozatok azzal, hogy "ransom," általában Bitcoin, mint cryptocurrencies cserébe adatokhoz való hozzáférés formájában. 
  
Ransomware elleni védekezésként egy vagy több levelezési folyamat szabályok (ezek kerültek a [mail a kártevők elleni védelem szintjének emelése](#raise-the-level-of-protection-against-malware-in-mail) lépés) ransomware általánosan használt fájlkiterjesztések le, vagy ezek kapó felhasználók figyelmeztetés létrehozása mellékletek, e-mailben.

Az előző lépésben blokkolt fájlok mellett tanácsos is makrókat tartalmazó Office fájl mellékletek megnyitása előtt figyelmeztesse a felhasználókat szabály létrehozásához. Ransomware belül, a makrók lehet elrejteni, azt fogja figyelmeztetni a felhasználókat a személyek nem tudják megnyitni ezeket a fájlokat.

Mail közlekedési szabály létrehozásához:
  
1. Ugrás az admin center <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> , és válassza a **Admin-centers** \> **Exchange**.
    
2. A **levelezés** kategóriában kattintson a **szabályok**gombra.
    
3. Kattintson a **+**, majd kattintson az **Új szabály létrehozása**.
    
4. Kattintson a **További beállítások** a párbeszédpanel alján tekintheti meg a beállítások teljes készletének. 
    
5. Az alábbi táblázat a szabályhoz tartozó beállításokat alkalmazza. A többi beállítást hagyja az alapértelmezett, kivéve, ha meg szeretnénk változtatni ezeket.
    
6. Kattintson a **Mentés** gombra.
    
|**Beállítás**|**A mellékletek az Office-fájlok megnyitása előtt figyelmeztesse a felhasználókat**||
|:-----|:-----|:-----|
|Name (Név)  <br/> |Anti-ransomware szabály: figyelmeztesse a felhasználókat  <br/>  |
|Ha a szabályt alkalmazni. . .  <br/> |Mellékletek. . . fájlkiterjesztés megfelel-e. . .  <br/> |
|Adja meg a szavak vagy kifejezések  <br/> |Ezek a fájltípusok hozzáadása:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm  <br/>|
|Tegye a következőket. . .  <br/> |Az üzenetet a címzett értesítés  <br/> |
|Adja meg az üzenet szövegét  <br/> |Ilyen típusú fájlokat nem tudja, mert a rosszindulatú kódot tartalmazó makrókat tartalmaz személyektől nem nyitható meg.  <br/> |
   
További információ:
  
- [Ransomware kezelése](https://go.microsoft.com/fwlink/?linkid=2016501&amp;clcid=0x409)
    
- [A OneDrive visszaállítása](https://support.office.com/article/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)
    


## <a name="stop-auto-forwarding-for-email"></a>E-mail automatikus továbbítását leállítása

Illetéktelen behatolóktól, akik hozzáférhetnek a felhasználói postafiók is ellophatják a levelek a szolgáltatással automatikusan továbbíthatja az e-mail postafiók megadásával. Ez akkor fordulhat elő, a felhasználói tudatosság nélkül is. Akkor is akadályozható ez mail Attribútumfolyam-szabály megadásával. 
  
Mail közlekedési szabály létrehozásához [a rövid](https://support.office.com/article/f9d693ba-5c78-47c0-b156-8e461e062aa7) videó, vagy kövesse az alábbi lépéseket:
  
1. A Microsoft 365 felügyeleti központban kattintson a **Admin-centers** \> **Exchange**.
    
2. A **levelezés** kategóriában kattintson a **szabályok**gombra.
    
3. Kattintson a **+**, majd kattintson az **Új szabály létrehozása**.
    
4. Kattintson a **További beállítások** a párbeszédpanel alján tekintheti meg a beállítások teljes készletének. 
    
5. Az alábbi táblázatban szereplő beállításokat alkalmazza. A többi beállítást hagyja az alapértelmezett, kivéve, ha meg szeretnénk változtatni ezeket.
    
6. Kattintson a **Mentés** gombra.
    
|**Beállítás**|**A mellékletek az Office-fájlok megnyitása előtt figyelmeztesse a felhasználókat**|
|:-----|:-----|
|Name (Név)  <br/> |E-mail automatikus továbbítását külső tartományokba megakadályozása  <br/> |
|Ha a szabály alkalmazása...  <br/> |A feladó. . . külső és belső. . . A szervezeten belül  <br/> |
|Feltétel hozzáadása  <br/> |Az üzenet tulajdonságai. . . az üzenet típusát tartalmazza. . . Automatikus továbbítás  <br/> |
|Tegye a következőket...  <br/> |Tiltsa le az üzenetet. . . el az üzenetet, és annak magyarázatát tartalmazza.  <br/> |
|Adja meg az üzenet szövegét  <br/> |A szervezeten kívüli automatikus továbbítási e-mail biztonsági okok miatt letiltja.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Az e-mail az adatlopási támadások elleni védelme

Ha egy vagy több egyéni tartományok beállítása az Office 365 vagy Microsoft 365 környezettől, beállíthatja a célzott adatlopás elleni védelem. ATP adatlopás elleni védelem, része az Office 365 speciális veszély védelmi, módszer segít megvédeni a szervezet a megszemélyesítés-alapú phishing rosszindulatú támadások és egyéb adathalászati célú támadások. Ha még nem konfigurált egyéni tartományban, nem szükséges ehhez.
  
Azt javasoljuk, hogy az első lépések megtétele a megjelölt védelemmel rendelkező védelme érdekében a legfontosabb felhasználók és az egyéni tartomány házirend létrehozásával. 

  
Az ATP adathalászat-házirend létrehozásához [a rövid videó képzés](https://support.office.com/article/86c425e1-1686-430a-9151-f7176cce4f2c)nézni, vagy hajtsa végre az alábbi lépéseket:
  
1. Nyissa meg a [https://protection.office.com](https://protection.office.com) lapot. 
    
2. Az Office 365 a &amp; Megfelelési központba, a bal oldali navigációs ablaktábla **fenyegetés kezelése**, válassza **a házirend**.
    
3. A **házirend** lapon válassza az **ATP adathalászat**.
    
4. Az **Adathalászat -** oldalon válassza az **+ létrehozása**. Elindul egy varázsló, amely végigvezeti az adathalászat-házirend meghatározása.
    
5. Adja meg a nevét, leírását és a javasolt az alábbi diagram zónáiba házirend beállításait. További részletekért lásd: [ATP adathalászat - házirend beállításaival kapcsolatos további tudnivalók](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409) . 
    
6. Miután elolvasta a beállításokat, válassza **a házirend létrehozása** és **mentése**, szükség szerint.
    

|**Beállítás, illetve az option**<br/>|**Javasolt beállítás** <br/>|
|:-----|:-----|
|Name (Név)  <br/> |Tartomány- és legértékesebb kampány személyzeti  <br/> |
|Leírás  <br/> |Legfontosabb személyzet és a tartományban vannak nem megszemélyesített biztosítása érdekében.  <br/> |
|A felhasználók hozzáadása  <br/> |Válassza **+ egy feltétel, a címzett hozzáadása**. Írja be a felhasználóneveket, vagy adja meg az e-mail címet, a jelölt, kampány-kezelő és egyéb fontos a személyzet tagjai. Megszemélyesítés védeni kívánt legfeljebb 20 külső és belső címeket adhat meg.  <br/> |
|Tartományok védelme  <br/> |Válassza ki a **+ Hozzáadás a feltétel, a címzett tartományhoz**. Ha egy adott Microsoft 365 előfizetése társított egyéni tartomány megadása Több tartományt is megadhat.  <br/> |
|Válassza a műveletek  <br/> |Ha egy megszemélyesített felhasználó által küldött e-mail: válassza a **Redirect üzenetet egy másik e-mail címet**, és írja be az e-mail címet, a biztonsági rendszergazda; például *Anna<span><span>@contoso.com*.          Ha e-mailben küld egy megszemélyesített tartomány: válassza ki a **Karantén üzenet**.  <br/> |
|Postaláda intelligencia  <br/> |Alapértelmezés szerint a postafiók intelligencia új adathalászat-házirend létrehozásakor van jelölve. Hagyja **ezt a beállítást a legjobb eredmény elérése érdekében** .  <br/> |
|Adja hozzá a megbízható feladók és tartományok  <br/> |Itt adhat meg a saját tartomány és a megbízható tartományokban.  <br/> |
|Alkalmazott  <br/> |Válassza ki **a címzett tartománya**. **Ezek**jelölje be a **választ**. Válassza ki a **+ Hozzáadás**. Jelölje be a jelölőnégyzetet az a tartomány nevét, például *contoso.<span> <span>com*, a listában, és válassza a **Hozzáadás**. Válassza ki a **kész**.  <br/> |
   
További információért lásd az [Office 365 ATP adathalászat - házirendek beállítása](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409).
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Ártalmas mellékleteket és ATP biztonságos mellékleteket tartalmazó fájlok elleni védelme

Személyek rendszeresen megküldik, kap, és ossza mellékletek, például a dokumentumok, bemutatók, számolótáblák és több. Nincs mindig állapítható meg, hogy e melléklet biztonságos vagy rosszindulatú e-mail üzenetet ránézésre csak egyszerű. Office 365 speciális veszély védelmi védelem ATP biztonságos mellékletet tartalmaz, de a védelem nincs alapértelmezés szerint bekapcsolva. Javasoljuk, hogy a védelem használatának megkezdéséhez új szabályt hoz létre. Ezt a védelmet fájlok a SharePoint, a OneDrive és a Microsoft Teams terjed.
  
Az ATP biztonságos melléklet házirend létrehozásához vagy [a rövid](https://support.office.com/article/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)videó, vagy hajtsa végre az alábbi lépéseket:
  
1. Ugrás a [https://protection.office.com](https://protection.office.com) , és jelentkezzen be a rendszergazdai fiók. 
    
2. Az Office 365 a &amp; Megfelelési központba, a bal oldali navigációs ablaktábla **fenyegetés kezelése**, válassza **a házirend**.
    
3. A házirend lapon válassza a **biztonságos mellékletek ATP**.
    
4. A biztonságos mellékletek lapon alkalmazni ezt a védelmet nagyjából **bekapcsolása a SharePoint, a OneDrive, és a Microsoft csapatok ATP** jelölőnégyzet bejelölésével. 
    
5. Válassza ki **+** hozzon létre egy új házirendet. 
    
6. Az alábbi táblázatban szereplő beállításokat alkalmazza. 
    
7. Miután elolvasta a beállításokat, válassza **a házirend létrehozása** és **mentése**, szükség szerint.
    

|**Beállítás, illetve az option**|**Javasolt beállítás** <br/>|
|:-----|:-----|
|Name (Név)  <br/> |Tiltsa le a jelenlegi és jövőbeli tartalmazó e-mailek észlelt kártevő.  <br/> |
|Leírás  <br/> |Jelenlegi és jövőbeli e-mailek és észlelt kártevő mellékletek blokkolása.  <br/> |
|Ismeretlen malware válasz mellékletek mentése  <br/> |Válassza a **blokk - a jelenlegi és jövőbeli e-mailek és az észlelt kártevő mellékletek blokkolása**.  <br/> |
|Melléklet a észlelési átirányítása  <br/> |Átirányítás engedélyezése (jelölje be a) adja meg a rendszergazda fiók, illetve a postaláda beállítása karantén.          A fenti kijelölést alkalmazza, ha a mellékletek keres malware időtúllépés vagy hiba lép fel (akkor válassza ezt a mezőt).  <br/> |
|Alkalmazott  <br/> |A címzett tartománya. . . Jelölje ki a tartományt.  <br/> |
   
További információért lásd az [Office 365 ATP adathalászat - házirendek beállítása](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409).
  


## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>ATP biztonságos hivatkozásokkal adathalászati célú támadások elleni védelem

A támadók néha elrejtése a hivatkozások e-mailben vagy más fájlok rosszindulatú webhelyek. Office 365 ATP biztonságos kapcsolatok (ATP biztonságos hivatkozások) része az Office 365 speciális veszély védelmi, védekezhet a szervezet azáltal, hogy a webcímeket (URL) ellenőrzése időt, kattintson az Office dokumentumok és e-mailek. Védelem ATP biztonságos kapcsolatok házirendeken keresztül történik.
  
Azt javasoljuk, hogy tegye a következőket:
  
- Módosítsa az alapértelmezett házirend növelhető.
    
- Adjunk hozzá egy új házirendet a tartomány összes címzett célzott.
    
ATP biztonságos kapcsolatok beállításához tekintse meg [a rövid videó képzés](https://support.office.com/article/61492713-53c2-47da-a6e7-fa97479e97fa), vagy hajtsa végre az alábbi lépéseket:
  
1. Ugrás a [https://protection.office.com](https://protection.office.com) , és jelentkezzen be a rendszergazdai fiók. 
    
2. Az Office 365 a &amp; Megfelelési központba, a bal oldali navigációs ablaktábla **fenyegetés kezelése**, válassza **a házirend**.
    
3. A házirend lapon válassza a **Biztonságos kapcsolatok ATP**.
    
Az alapértelmezett házirend módosítása:
  
1. **Az egész szervezetre érvényes házirendek**, a biztonságos kapcsolatok lapon jelölje be az **alapértelmezett** házirend. 
    
2. **Tartalom e-mail kivételével érvényes beállítások**csoportban jelölje be az **Office 365 ProPlus, iOS és Android**.
    
3. Kattintson a **Mentés** gombra. 
    
A tartomány összes címzett célzott új házirend létrehozása:
  
1. Kattintson a biztonságos kapcsolatok lap **, amely az egész szervezetre érvényes házirendek**, **+** hozzon létre egy új házirendet. 
    
2. A következő táblázatban felsorolt beállításokat alkalmazza.
    
3. Kattintson a **Mentés** gombra. 

|**Beállítás, illetve az option**|**Javasolt beállítás** <br/>|
|:-----|:-----|
|Name (Név)  <br/> |Biztonságos kapcsolatok csoportházirend a tartomány összes címzett  <br/> |
|Jelölje ki a műveletet ismeretlen potenciálisan rosszindulatú URL-címeket az üzenetek  <br/> |Válassza ki az **- URL-címek fog írni, és összeveti az ismert rosszindulatú hivatkozásokat, amikor a felhasználó a hivatkozásra kattint**.  <br/> |
|Biztonságos mellékletek segítségével letölthető tartalom beolvasása  <br/> |Jelölje be ezt a jelölőnégyzetet.  <br/> |
|Alkalmazott  <br/> |A címzett tartománya. . . Jelölje ki a tartományt.  <br/> |
   
További információ: az [Office 365 ATP biztonságos kapcsolatok](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409).

## <a name="go-to-intune-admin-center"></a>Ugrás az Intune admin center

1. [Borzas portal](https://portal.azure.com/)bejelentkezni.

2. Válassza ki **az összes szolgáltatás** és típus *Intune* a **Keresés mezőbe**.

3. Után az eredmények megjelenítéséhez kattintson a start **Microsoft Intune** teszi a kedvenc tovább és könnyen megjegyezhető.

Az admin center mellett Intune segítségével igényelhetnek, és a szervezet eszközök kezelése. További tudnivalókért lásd: [Windows eszközök tanúsítványigénylési módszer lehetőségeit](https://docs.microsoft.com/intune/enrollment-method-capabs) és a [beiktatási beállítások Intune által kezelt eszközök](https://docs.microsoft.com/intune/enrollment-options).

---
title: Növelje a Microsoft 365 Business fenyegetettség elleni védelmét
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
search.appverid:
- BCS160
- MET150
description: Állítsa be az Office 365 fejlett Fenyegetésvédelmet, és őrizzék meg a bizalmas adatokat.
ms.openlocfilehash: 00a40ceb6d51add2ebe8cc7ca4c299fe07a10b89
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/14/2019
ms.locfileid: "38320108"
---
# <a name="increase-threat-protection"></a>Növeli a fenyegetettséget

Ez a cikk segítséget nyújt a Microsoft 365-előfizetés védelmének növelésben az adathalászat, a rosszindulatú programok és egyéb fenyegetések elleni védekezéshez. Ezek az ajánlások alkalmasak a szervezetek fokozott biztonsági igény, mint a ügyvédi irodák és egészségügyi klinikák.

Mielőtt elkezdené, ellenőrizze az Office 365 biztonságos pontszámát. Hivatal 365 biztosít pont elemez-a Hivatal 365 szervezetek ' biztonság azon alapszik-a szabályos tevékenységek és biztonság elintézés, és átruház egy pont. Kezdje azzal, hogy tudomásul veszi a jelenlegi pontszám. -Hoz növekszik-a pont, kiegészít a tettek ajánlott ebben cikk. A cél nem az, hogy elérjék a maximális pontszámot, de tudatában kell lennie a lehetőségeket, hogy megvédjük a környezetet, amely nem befolyásolja hátrányosan a termelékenységet a felhasználók számára. 

További információt a [Microsoft biztonságos pontszám](https://docs.microsoft.com/office365/securitycompliance/microsoft-secure-score)című témakörben talál.

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>A rosszindulatú programok elleni védelem szintjének emelése a mail-ben

Az Office 365 vagy a Microsoft 365 környezet védelmet tartalmaz a rosszindulatú programok ellen. Ezt a védelmet növelheti a rosszindulatú programok által általánosan használt fájltípusokat tartalmazó mellékletek blokkolásával. A rosszindulatú szoftverek védelmének növelése az e-mailben:
  
1. Megy [https://protection.office.com](https://protection.office.com) és jel-ban-val-a admin számla megbízólevél. 
    
2. Az Office &amp; 365 biztonsági megfelelőségi központ bal oldali navigációs ablaktábláján a **fenyegetéskezelés**alatt válassza a **házirend** \> **anti-malware**.
    
3. A vállalati szintű házirend szerkesztéséhez kattintson duplán az alapértelmezett házirendra.
    
4. Válassza a **Settings (beállítások**)-t.
    
5. A **gyakori melléklettípusok szűrője**területen válassza **a**be-t. A letiltott fájltípusokat a közvetlenül a vezérlő alatt található ablak sorolja fel. Győződjön meg arról, hogy a következő fájltípusokat adja hozzá:
   - ade, ADP, Ani, BAS, bat, chm, cmd, com, cpl, CRT, hlp, HT, HTA, inf, ins, ISP, munka, js, JSE, lnk, MDA, mdb, MDE, mdz, MSC, MSI, MSP, MST, PCD, reg, SCR, SCT, SHS, URL, VB, VBE, vbs, wsc, wsf, WSH, exe, PIF  <br/> 
   
   Szükség esetén később is hozzáadhat és törölhet fájltípusokat.
    
6. Válassza a **Mentés.**
    
További információt a kártevők elleni [védelem](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409)című témakörben talál.
  
## <a name="protect-against-ransomware"></a>Elleni védelem ransomware

Ransomware korlátoz belépés-hoz adat mellett encrypting fájlokat vagy elzárás számítógép ernyőz. Ezt követően megpróbálja kicsikarni pénzt az áldozatok kérnek "váltságdíjat," általában a formájában cryptovaluták, mint a Bitcoin, cserébe az adatokhoz való hozzáférés. 
  
-Hoz megvéd ellen ransomware, teremt egy vagy több felad folyik szabályok-hoz fatuskó reszelő kiterjesztés amit van általában használt részére ransomware. (Ezeket a szabályokat a [rosszindulatú programok elleni védelem szintjének növelésében](#raise-the-level-of-protection-against-malware-in-mail) , az e-mail lépésben kell hozzáadni.) Figyelmeztetheti azokat a felhasználókat is, akik ezeket a mellékleteket megkapják e-mailben.

Az előző lépésben blokkolt fájlokon kívül célszerű létrehozni egy olyan szabályt, amely figyelmezteti a felhasználókat, mielőtt megnyitják az Office fájlmellékleteit, makrókat. Ransomware lehet elrejtve makrók, így figyelmezteti a felhasználókat, hogy ne nyissa meg ezeket a fájlokat az emberek nem tudják.

Levelezési átviteli szabály létrehozása:
  
1. Menj az Admin Center-on <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>, és válassza az **Admin Centers** \> **Exchange**.
    
2. A **levélforgalom** kategóriában válassza a **szabályok**kategóriát.
    
3. Válassza **+** a, majd **az új szabály létrehozása**-t.
    
4. Válassza a párbeszédpanel alján található **További beállítások** lehetőséget a teljes beállításkészlet megtekintéséhez. 
    
5. Alkalmazza a következő táblázatban található beállításokat a szabályhoz. A többi beállítás esetében használja az alapértelmezett értékeket, hacsak nem kívánja azokat megváltoztatni.
    
6. Válassza a **Mentés** lehetőséget.
    
|**Beállítás**|**A felhasználók figyelmeztetése az Office-fájlok mellékleteinek megnyitása előtt**||
|:-----|:-----|:-----|
|Name (Név)  <br/> |Anti-ransomware szabály: figyelmeztesse a felhasználók  <br/>  |
|Alkalmazza ezt a szabályt. . .  <br/> |Bármilyen mellékletet. . . fájlkiterjesztés megegyezik. . .  <br/> |
|Szavak vagy kifejezések megadása  <br/> |Adja hozzá ezeket a fájltípusokat:  <br/> dotm, docm, xlsm, sltm, xla, xlam, XLL, PPTM, potm, ppam, ppsm, sldm  <br/>|
|Tegye a következőt. . .  <br/> |Üzenet értesítése a címzettről  <br/> |
|Üzenetszöveg biztosítása  <br/> |Ne nyissa meg az ilyen típusú fájlokat olyan személyeknél, akiket nem ismer, mert olyan makrókat tartalmazhatnak, amelyek kártékony kódot tartalmaznak.  <br/> |
   
További információ:
  
- [Hogyan kezeljük a ransomware](https://go.microsoft.com/fwlink/?linkid=2016501&amp;clcid=0x409)
    
- [Visszaad-a OneDrive](https://support.office.com/article/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Automatikus továbbítás leállítása e-mailhez

Bárdok ki elnyer belépés-hoz egy használók ' postaláda tud lop felad mellett elintézés a postaláda-hoz gépiesen továbbít elektronikus levél. Ez történhet még a felhasználó figyelmének felkeltése nélkül is. Ennek elkerülésére állítson be egy levélfolyamszabályt. 
  
Levélátviteli szabály létrehozásához tekintse meg [ezt a rövid videót](https://support.office.com/article/f9d693ba-5c78-47c0-b156-8e461e062aa7) , vagy kövesse az alábbi lépéseket:
  
1. A Microsoft 365 Admin Center webhelyén válassza a **felügyeleti központok** \> **cseréje**parancsot.
    
2. A **levélforgalom** kategóriában válassza a **szabályok**kategóriát.
    
3. Válassza **+** a, majd **az új szabály létrehozása**-t.
    
4. Ha az összes beállítást meg szeretné nézni, válassza a párbeszédpanel alján található **További beállítások** lehetőséget. 
    
5. Alkalmazza a beállításokat a következő táblázatban. A többi beállítás esetében használja az alapértelmezett értékeket, hacsak nem kívánja azokat megváltoztatni.
    
6. Válassza a **Mentés** lehetőséget.
    
|**Beállítás**|**A felhasználók figyelmeztetése az Office-fájlok mellékleteinek megnyitása előtt**|
|:-----|:-----|
|Name (Név)  <br/> |E-mailek külső tartományokra történő automatikus továbbításának megakadályozása  <br/> |
|Alkalmazza ezt a szabályt, ha...  <br/> |A feladó. . . külső/belső. . . Szervezeten belül  <br/> |
|Feltételfeltétel hozzáadása  <br/> |Az üzenettulajdonságok. . . tartalmazza az üzenettípust. . . Automatikus továbbítás  <br/> |
|Tegye a következőt...  <br/> |Blokkolja az üzenetet. . . elutasíthatjuk az üzenetet, és magyarázatot is tartalmazniuk kell.  <br/> |
|Üzenetszöveg biztosítása  <br/> |E-mailek automatikus továbbítása a szervezeten kívülre nem biztonsági okokból akadályoztatva van.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Védje meg e-mail adathalász támadások

Ha egy vagy több egyéni tartományt konfigurál az Office 365 vagy a Microsoft 365 környezethez, beállíthatja a célzott adathalászat elleni védelmet. ATP anti-phishing védelem, része Hivatal 365 haladó fenyeget védelem, tud segít megvéd-a szervezet-ból kaján megszemélyesítés-kiindulópontul szolgáló phishing támadás és más phishing támadás. Ha nem konfigurálta az egyéni tartományt, akkor nem kell ezt megtennie.
  
Javasoljuk, hogy a védelem elkezdésével hozzon létre egy házirendet a legfontosabb felhasználók és az egyéni tartományok védelmének érdekében. 

Az ATP-ellenes irányelvek létrehozásához tekintse meg ezt a [rövid oktató videót](https://support.office.com/article/86c425e1-1686-430a-9151-f7176cce4f2c), vagy hajtsa végre az alábbi lépéseket:
  
1. Nyissa meg a [https://protection.office.com](https://protection.office.com) lapot. 
    
2. Az Office 365 biztonsági &amp; megfelelőségi központ bal oldali navigációs ablakában a **fenyegetéskezelés**területen válassza a **házirend**-t.
    
3. A **házirend** lapon válassza az **ATP-ellenes adathalászat**programot.
    
4. Az **adathalászat elleni** lapon válassza a **+ Létrehozás**. Egy varázsló indítja el az adathalászat-ellenes házirend definiálásához szükséges lépéseket.
    
5. Adja meg a házirend nevét, leírását és az ajánlott beállításokat az alábbi táblázatban. További információ: az [ATP-adathalászat elleni házirend-beállítások](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies#learn-about-atp-anti-phishing-policy-options)ismertetése. 
    
6. A beállítások felülvizsgálatát követően válassza **a Házirendlétrehozás** vagy a **Mentés**másként beállítást.
    

|**Beállítás vagy beállítás**<br/>|**Ajánlott beállítás** <br/>|
|:-----|:-----|
|Name (Név)  <br/> |Domainben és legértékesebb kampányában  <br/> |
|Leírás  <br/> |Biztosítani kell a legfontosabb személyzet és a mi domain nem megszemélyezett.  <br/> |
|Védjük a felhasználókat  <br/> |Select **+ feltétel hozzáadása, a címzett**. Írja be a felhasználóneveket, vagy írja be a pályázó, a kampányigazgató és más fontos munkatársak e-mail címét. Legfeljebb 20 olyan belső és külső címet adhat meg, amelyeket védeni szeretne a megszemélyesítésről.  <br/> |
|Tartományok hozzáadása a védelmhez  <br/> |Select **+ feltétel hozzáadása, a címzett tartománya**. Adja meg a Microsoft 365 előfizetéshez tartozó egyéni tartományt, ha definiált egyet. Egynél több tartományt is megadhat.  <br/> |
|Válasszon műveleteket!  <br/> |Ha az e-maileket egy megszemélyesítő felhasználó küldi: válassza az **üzenet átirányítása másik e-mail címre**lehetőséget, majd írja be a biztonsági rendszergazda e-mail címét; például *Alice<span><span>@contoso. com*. Ha az e-maileket egy megszemélyezett tartomány küldi: válassza a **karantén üzenet**lehetőséget.  <br/> |
|Postaláda-intelligencia  <br/> |Ha új adathalászat-ellenes házirendet hoz létre, a postaláda-intelligencia alapértelmezés szerint ki van választva. Hagyja ezt a **beállítást a** legjobb eredmény.  <br/> |
|Megbízható feladók és tartományok hozzáadása  <br/> |Itt adhatja hozzá saját tartományát vagy bármely más megbízható tartományt.  <br/> |
|Alkalmazva  <br/> |Jelölje ki **a címzetttartományt**. A **fentiek bármelyikén**válassza a **választ**. Válasszuk a **+ hozzáad** Jelölje be a tartomány neve melletti jelölőnégyzetet, például *contoso.<span> com <span>*,-ban oldalra dől, aztán kiválaszt **összead**. Válassza a **Done (kész**)-t.  <br/> |
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Védelmet nyújt a kártékony mellékletek és a fájlok az ATP biztonságos mellékletek

Az emberek rendszeresen küldhetnek, fogadhatnak és megoszthat mellékleteket, például dokumentumokat, bemutatókat, táblázatokat stb. Nem mindig könnyű megmondani, hogy egy mellékletet biztonságos vagy rosszindulatú pusztán megnézi az e-mail üzenetet. Hivatal 365 haladó fenyeget védelem beleértve ATP biztos egybefűzés védelem, de ez védelem van nem esztergált-ra mellett hiba. Ajánlott egy új szabályt létrehozni a védelem használatának megkezdéséhez. Ez a védelem kiterjed a SharePoint, az OneDrive és a Microsoft csapatok fájljaihoz is.
  
Az ATP-biztonságos mellékletre vonatkozó házirend létrehozásához tekintse meg [ezt a rövid videót](https://support.office.com/article/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), vagy hajtsa végre az alábbi lépéseket:
  
1. Menjen [https://protection.office.com](https://protection.office.com), és jelentkezzen be a rendszergazdai fiókkal. 
    
2. Az Office 365 biztonsági &amp; megfelelőségi központ bal oldali navigációs ablakában a **fenyegetéskezelés**területen válassza a **házirend**-t.
    
3. A házirend lapon válassza az **ATP-mellékleteket**.
    
4. A biztonságos mellékletek lapon ezt a védelmet nagyjából alkalmazza a **SharePoint, az OneDrive és a Microsoft csapatok esetén az ATP bekapcsolása** jelölőnégyzet bejelölésével. 
    
5. Bejelölésével **+** új házirendet hozhat létre. 
    
6. Alkalmazza a beállításokat a következő táblázatban. 
    
7. Miután áttekintette a beállításokat, válassza **a házirend létrehozása** vagy az adott esetben **Mentés**beállítást.
    

|**Beállítás vagy beállítás**|**Ajánlott beállítás** <br/>|
|:-----|:-----|
|Name (Név)  <br/> |Blokkolja a jelenlegi és a jövőbeli e-maileket észlelt malware.  <br/> |
|Leírás  <br/> |Fatuskó időszerű és jövő elektronikus levél és egybefűzés-val kinyomoz malware.  <br/> |
|Mellékletek mentése ismeretlen malware-válasz  <br/> |Kiválaszt **fatuskó-fatuskó a időszerű és jövő elektronikus levél és egybefűzés-val kinyomoz malware**.  <br/> |
|Az észlelést átirányító csatolás  <br/> |Átirányítás engedélyezése (jelölje be ezt a négyzetet) adja meg a rendszergazda fiókot, vagy egy postaláda-beállítást a karanténhoz.          Alkalmazza a fenti kiválasztási, ha malware fürkésző a mellékletek alkalommal, vagy hiba történik (jelölje be ezt a négyzetet).  <br/> |
|Alkalmazva  <br/> |A címzetttartomány. . . Válassza ki a tartományt.  <br/> |
   
További információ: az [Office 365 az ATP adathalászat elleni házirendek beállítása](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409).
  


## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Adathalász támadások elleni védelem az ATP-kompatibilis hivatkozásokkal

Bárdok néha eldug kaján websites-ban láncszemek-ban elektronikus levél vagy más fájlokat. Hivatal 365 ATP biztos láncszemek (ATP biztos láncszemek), része Hivatal 365 haladó fenyeget védelem, tud segít megvéd-a szervezet mellett felszerelt idő--ból-kettyenés beigazolódás-ból pókháló címek (URLs)-ban elektronikus levél üzenet és Hivatal okiratok. A védelem az ATP Safe Links irányelvei segítségével határozható meg.
  
A következő műveleteket javasoljuk:
  
- Módosítsa az alapértelmezett házirendet a védelem növeléséhez.
    
- Adjon hozzá egy új házirendet a tartomány összes címzettjének.
    
Az ATP-biztos hivatkozások beállításához tekintse meg [ezt a rövid oktató videót](https://support.office.com/article/61492713-53c2-47da-a6e7-fa97479e97fa), vagy hajtsa végre az alábbi lépéseket:
  
1. Menjen [https://protection.office.com](https://protection.office.com), és jelentkezzen be a rendszergazdai fiókkal. 
    
2. Az Office 365 biztonsági &amp; megfelelőségi központ bal oldali navigációs ablakában a **fenyegetéskezelés**területen válassza a **házirend**-t.
    
3. A házirend lapon válassza az **ATP-biztos hivatkozások**parancsát.
    
Az alapértelmezett házirend módosítása:
  
1. A biztonságos hivatkozások lapon a **teljes szervezetre vonatkozó házirendek**területen jelölje ki az **alapértelmezett** házirendet. 
    
2. Alatt **elintézés amit alkalmaz-hoz elégedett kivéve elektronikus levél**, kiválaszt **Hivatal 365 ProPlus, hivatal részére iOS és Android**.
    
3. Válassza a **Mentés** lehetőséget. 
    
A tartomány összes címzettjének tervezett új házirend létrehozása:
  
1. A biztonságos hivatkozások lapon a **teljes szervezetre vonatkozó házirendek**területen válassza ki **+** az új házirend létrehozását. 
    
2. Alkalmazza a következő táblázatban felsorolt beállításokat.
    
3. Válassza a **Mentés** lehetőséget. 

|**Beállítás vagy beállítás**|**Ajánlott beállítás** <br/>|
|:-----|:-----|
|Name (Név)  <br/> |A tartomány összes címzettjének biztonságos csatolásokra vonatkozó házirendje  <br/> |
|Az üzenetekben lévő ismeretlen potenciálisan kártékony URL-címekre vonatkozó művelet kiválasztása  <br/> |Select **on-URL-eket kell átírni, és ellenőrzik egy listát az ismert rosszindulatú linkek, amikor a felhasználó rákattint a linkre**.  <br/> |
|A biztonságos mellékletek használata letölthető tartalmak beolvasásához  <br/> |Jelölje be ezt a négyzetet.  <br/> |
|Alkalmazva  <br/> |A címzetttartomány. . . Válassza ki a tartományt.  <br/> |
   
További információ: [Office 365 ATP-biztos hivatkozások](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409).

## <a name="go-to-intune-admin-center"></a>Tovább az Intune admin Centerbe

1. Jelentkezzen be az [Azure portálra](https://portal.azure.com/).

2. Kiválaszt **minden szolgáltatás** és begépel *Intune* -ban **kutatás doboz**.

3. Egyszer a eredmények feltűnik, kiválaszt a Elkezd mellett **Mikroszkóp Intune** -hoz csinál ez egy kedvenc és könnyű-hoz talál később.

Az admin központ mellett az Intune segítségével is regisztrálhatja és kezelheti a szervezet eszközeit. További információt a Windows- [eszközök tanúsítványigénylési módszerével](https://docs.microsoft.com/intune/enrollment-method-capabs) és az [Intune által kezelt eszközök tanúsítványigénylési beállításaival](https://docs.microsoft.com/intune/enrollment-options)kapcsolatban a szolgáltatások című témakörben talál.

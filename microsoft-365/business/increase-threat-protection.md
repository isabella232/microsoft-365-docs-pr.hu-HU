---
title: A veszélyforrások elleni védelem növelése Microsoft 365 vállalati verzióban
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
description: Állítsa be a Microsoft Defendert Office 365 és megóvja a bizalmas adatokat az adathalászattal, a kártevővel és az egyéb fenyegetésekkel szemben.
ms.openlocfilehash: d5aad66642fc2b509ae40dc1277167deb53de6fbb0593a3dcd766062305fbd6a
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53831475"
---
# <a name="increase-threat-protection"></a>Veszélyforrások elleni védelem növelése

Ez a cikk segítséget nyújt az Microsoft 365 az adathalászat, a kártevők és más veszélyforrások elleni védelem érdekében. Ezek az ajánlások olyan szervezeteknek vannak megfelelőek, amelyekben nagyobb szükség van a biztonságra– ilyen például a jogi irodák és az egészségügyi rendelők.

Mielőtt hozzákezd, ellenőrizze a Office 365 pontszámát. Office 365 A Biztonsági pontszám elemzi a szervezet biztonságát a szokásos tevékenységek és biztonsági beállítások alapján, és egy pontszámot rendel hozzá. Először jegyezze fel az aktuális pontszámot. A pontszám növeléséhez a cikkben javasolt műveleteket kell végrehajtania. A cél nem a maximális pontszám elérése, hanem annak tudatában van, hogy milyen lehetőségek vannak a környezet védelmére, amelyek nem befolyásolják hátrányosan a felhasználók hatékonyságát.

További információ: [A Microsoft biztonsági pontszáma.](../security/defender/microsoft-secure-score.md)

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>A kártevők elleni védelem szintjének emelése a levelekben

Az Office 365 vagy Microsoft 365 környezet védelmet nyújt a kártevők ellen. Ezt a védelmet növelheti azzal, ha letiltja a mellékleteket a kártevők számára gyakran használt fájltípusokkal. A kártevők elleni védelem növelése az e-mailekben:

1. Jelentkezzen be a rendszergazdai fiók hitelesítő [https://protection.office.com](https://protection.office.com) adataival.

2. A Biztonsági megfelelőségi központ bal oldali navigációs ablakának Veszélyforrások kezelése területén válassza &amp; a   \> **Kártevők elleni házirend lehetőséget.**

3. Kattintson duplán az alapértelmezett házirendre a vállalati szintű házirend szerkesztéséhez.

4. Válassza a **Gépház** lehetőséget.

5. A **Gyakori melléklettípusok szűrője alatt válassza** a Be **lehetőséget.** A letiltott fájltípusok közvetlenül a vezérlő alatti ablakban listában szerepelnek. Győződjön meg arról, hogy az alábbi fájltípusokat adja hozzá:

   `ade, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, job, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif`

   Szükség esetén később is hozzáadhat vagy törölhet fájltípusokat.

6. Válassza a **Mentés gombot.**

További információ: Kártevők elleni védelem az [EOP-ban.](../security/office-365-security/anti-malware-protection.md)

## <a name="protect-against-ransomware"></a>Zsarolóvírusok elleni védelem

A zsarolóvírusok a fájlok titkosítása vagy a számítógép képernyőinek zárolása segítségével korlátozzák az adatokhoz való hozzáférést. Ezután megkísérli a pénz kitorzulása abból a kérdésből, hogy "zsarolójelet" kér, általában titkosítások, például a Bitcoin formájában, az adatokhoz való hozzáférésért cserébe.

A zsarolóvírusok elleni védelemhez hozzon létre egy vagy több e-mail-forgalomra vonatkozó szabályt a zsarolóvírusok által gyakran használt fájlkiterjesztések blokkolására. (Ezeket a szabályokat a kártevők elleni védelem szintjét a levelezési lépésben [emelte](#raise-the-level-of-protection-against-malware-in-mail) ki.) Figyelmeztetheti a mellékleteket e-mailben megkapó felhasználókat is.

Az előző lépésben letiltott fájlokon kívül azt is jó ötlet lehet szabályt létrehozni, amely figyelmezteti Office felhasználókat a makrókat használó fájlmellékletek megnyitása előtt. A zsarolóvírusok a makrókban is elrejtve vannak, ezért figyelmezteti a felhasználókat, hogy ne nyissák meg ezeket a fájlokat az őket nem kereső személyek elől.

Levelezési átviteli szabály létrehozása:

1. A felügyeleti központ megnyitásához válassza a Felügyeleti központok <https://admin.microsoft.com>  \> **lehetőséget Exchange.**

2. Az **e-mail-forgalom kategóriában** válassza a **szabályok lehetőséget.**

3. Válassza **+** a ot, majd **az Új szabály létrehozása lehetőséget.**

4. A **párbeszédpanel alján** a További beállítások lehetőséget választva az összes lehetőséget láthatja.

5. Alkalmazza a szabályra vonatkozó beállításokat az alábbi táblázatban. A többi beállításhoz használja az alapértelmezett értékeket, kivéve ha módosítani szeretné őket.

6. Válassza a **Mentés** elemet.

|Beállítás|Figyelmeztetést ad a felhasználóknak a fájlmellékletek Office megnyitása előtt|
|---|---|
|Name (Név)|Zsarolóvírusok elleni szabály: figyelmeztetést ad a felhasználóknak|
|Akkor alkalmazza ezt a szabályt, ha: . . .|Bármely melléklet. . . fájlkiterjesztés egyezéseket ad meg. . .|
|Szavak vagy kifejezések megadása|Adja meg az alábbi fájltípusokat:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm|
|Tegye a következőket. . .|A címzett értesítése egy üzenettel|
|Üzenetszöveg küldése|Az ilyen típusú fájlokat ne nyissa meg olyan személyektől, akiket nem ismer, mert azok kártékony kódot tartalmazó makrókat tartalmazhatnak.|

További információ:

- [Zsarolóvírusok: kockázat csökkentése](https://www.microsoft.com/security/blog/2020/04/28/ransomware-groups-continue-to-target-healthcare-critical-services-heres-how-to-reduce-risk/)

- [A saját OneDrive](https://support.microsoft.com/office/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Az e-mailek automatikus továbbításának leállítása

A felhasználók postaládájához hozzáféréssel hozzáférő támadók úgy ellophatják az e-maileket, hogy beják a postaládát az e-mailek automatikus továbbítására. Ez a felhasználó ismeretismeret nélkül is történhet. Ezt úgy előzheti meg, ha konfigurál egy e-mail-forgalom szabályát.

Levelezési átviteli szabály létrehozásához nézze meg ezt a [rövid](../business-video/stop-email-auto-forward.md) videót, vagy kövesse az alábbi lépéseket:

1. A csoportban Microsoft 365 Felügyeleti központ felügyeleti **központok lehetőséget, majd** \> **Exchange.**

2. Az **e-mail-forgalom kategóriában** válassza a **szabályok lehetőséget.**

3. Válassza **+** a ot, majd **az Új szabály létrehozása lehetőséget.**

4. Az összes lehetőség megjelenítéséhez válassza a További beállítások lehetőséget a párbeszédpanel alján. 

5. Alkalmazza az alábbi táblázatban található beállításokat. A többi beállításhoz használja az alapértelmezett értékeket, kivéve ha módosítani szeretné őket.

6. Válassza a **Mentés** elemet.

|Beállítás|Figyelmeztetést ad a felhasználóknak a fájlmellékletek Office megnyitása előtt|
|---|---|
|Name (Név)|Az e-mailek automatikus továbbításának megakadályozása külső tartományokba|
|Alkalmazza ezt a szabályt, ha...|A feladó. . . külső/belső. . . A szervezeten belül|
|Feltétel hozzáadása|Az üzenet tulajdonságai. . . üzenettípust is adja meg. . . Automatikus továbbítás|
|Tegye a következőket...|Az üzenet blokkolása. . . elutasíthatja az üzenetet, és magyarázatot is tartalmazhat.|
|Üzenetszöveg küldése|A szervezeten kívüli e-mailek automatikus továbbítása biztonsági okokból nem lehetséges.|


## <a name="protect-your-email-from-phishing-attacks"></a>Az e-mailek védelme az adathalászati támadások ellen

Ha egy vagy több egyéni tartományt konfigurált a Office 365 vagy Microsoft 365 környezetéhez, akkor beállíthatja az adathalászat elleni célzott védelmet. Az adathalászat elleni védelem, amely a Microsoft Defender a Office 365 programhoz része, segíthet megvédeni szervezetét a rosszindulatú megszemélyesítésen alapuló adathalász támadásoktól és az egyéb adathalász támadásoktól. Ha még nem konfigurált egyéni tartományt, nem kell ezt megtennie.

Azt javasoljuk, hogy ezt a védelmet a legfontosabb felhasználók és az egyéni tartomány védelmére vonatkozó házirend létrehozásával kezdje meg.

Ha adathalászat elleni házirendet hoz létre a Microsoft Defender Office 365, [nézze](../business-video/setup-anti-phishing.md)meg ezt a rövid oktatóvideónkat, vagy kövesse az alábbi lépéseket:

1. Nyissa meg a [https://protection.office.com](https://protection.office.com) lapot.

2. A Biztonsági megfelelőségi központ bal oldali navigációs ablakának Veszélyforrások kezelése területén válassza &amp; a Házirend **lehetőséget.** 

3. A Házirend **lapon** válassza az **Adathalászat elleni védelmet.**

4. Az **Adathalászat elleni lapon** válassza a **+ Létrehozás lehetőséget.** Egy varázsló elindítja ezt a lépést az adathalászat-házirend definiálása során.

5. Adja meg a házirend nevét, leírását és beállításait az alábbi táblázatban ajánlottak szerint. További információt a További információ az adathalászat elleni házirendről a [Microsoft Defenderben a](../security/office-365-security/set-up-anti-phishing-policies.md)Office 365 talál.

6. A beállítások áttekintése után válassza a Házirend létrehozása **vagy** a **Mentés** lehetőséget a megfelelő módon.

|Beállítás vagy beállítás|Ajánlott beállítás|
|---|---|
|Name (Név)|Domain and most valuable campaign staff|
|Leírás|Győződjön meg arról, hogy a legfontosabb munkatársakat és tartományunkat nem személyesülnek meg.|
|Felhasználók hozzáadása védelemhez|Válassza **a + Feltétel hozzáadása lehetőséget, a címzett pedig**. Írja be a felhasználóneveket, vagy adja meg a jelölt, a kampánymenedzser és más fontos személyzeti tagok e-mail-címét. Legfeljebb 20 belső és külső címet adhat hozzá, amelyek megszemélyesítéstől való védelmet kíván kitenni.|
|Tartományok hozzáadása védelemhez|Válassza **a + Feltétel hozzáadása, A címzett tartománya lehetőséget.** Ha definiált egy egyéni tartományt, Microsoft 365 előfizetéséhez társított egyéni tartományt. Egynél több tartományt is beírhat.|
|Műveletek kiválasztása|Ha egy megszemélyesített felhasználó küldi el az e-mailt: Válassza az Üzenet átirányítása másik e-mail címre **lehetőséget,** majd írja be a biztonsági rendszergazda e-mail-címét; például: *<span> <span> Zét @contoso.com.* Ha megszemélyesített tartomány küldi az e-mailt: Válassza a **Karantén üzenet lehetőséget.**|
|Postaláda-intelligencia|Új adathalászati házirend létrehozásakor alapértelmezés szerint a postaláda-intelligencia van kiválasztva. A legjobb eredmény érdekében hagyja **be a** beállítást.|
|Megbízható feladók és tartományok hozzáadása|Itt hozzáadhatja saját tartományát vagy bármely más megbízható tartományt.|
|Alkalmazva:|Válassza **A címzett tartománya lehetőséget.** A **Válasszon a beállítások közül alatt** válassza a **lehetőséget.** Válassza **a + Hozzáadás lehetőséget.** Jelölje be a tartomány neve melletti jelölőnégyzetet, például *contoso. <span> <span> com* gombra, majd válassza a Hozzáadás **lehetőséget.** Válassza a **Kész lehetőséget.**|

## <a name="protect-against-malicious-attachments-and-files-with-safe-attachments"></a>Kártékony mellékletek és fájlok elleni védelem Széf mellékletekkel

Rendszeresen küldhetnek, fogadhatnak és oszthatnak meg mellékleteket, például dokumentumokat, bemutatókat, számolótáblákat stb. Egy e-mail üzenetből nem mindig könnyű megmondani, hogy egy melléklet biztonságos vagy kártékony-e. A Microsoft Defender Office 365 biztonsági Széf, de ez a védelem alapértelmezés szerint nincs bekapcsolva. Azt javasoljuk, hogy hozzon létre egy új szabályt a védelem használatának megkezdéséhez. Ez a védelem kiterjed a fájlokra a SharePoint, OneDrive és Microsoft Teams.

Ha mellékletre vonatkozó Széf létre, [nézze](../business-video/safe-attachments.md)meg ezt a rövid videót, vagy kövesse az alábbi lépéseket:

1. A () [https://protection.office.com](https://protection.office.com) lapra lépve jelentkezzen be a rendszergazdai fiókjával.

2. A Biztonsági megfelelőségi központ bal oldali navigációs ablakának Veszélyforrások kezelése területén válassza &amp; a Házirend **lehetőséget.** 

3. A Házirend lapon válassza a **Mellékletek Széf lehetőséget.**

4. A Széf-mellékletek lapon ezt a védelmet széles körben alkalmazhatja aTp on **on ATP for SharePoint, a OneDrive** és a Microsoft Teams jelölőnégyzetet.

5. Válassza **+** ezt az új házirend létrehozásához.

6. Alkalmazza az alábbi táblázatban található beállításokat.

7. A beállítások áttekintése után válassza a Házirend **létrehozása** vagy a **Mentés** lehetőséget a megfelelő módon.

|Beállítás vagy beállítás|Ajánlott beállítás|
|---|---|
|Name (Név)|Az észlelt kártevők miatt blokkolhatja a jelenlegi és a jövőbeli e-maileket.|
|Leírás|Kártevőt észlelve blokkolhatja a jelenlegi és a jövőbeli e-maileket és mellékleteket.|
|Ismeretlen kártevő-válasz mentése a mellékletekbe|Válassza a Letiltás lehetőséget– A jelenlegi és a jövőben blokkolhatja az e-maileket és mellékleteket **az észlelt kártevők miatt.**|
|Melléklet átirányítása észlelésre|Átirányítás engedélyezése (válassza ezt a mezőt) Adja meg a rendszergazdai fiókot vagy egy postaláda-beállítást karanténként.          Akkor alkalmazza a fenti kijelölést, ha a kártevők a mellékletek időkorlokát vagy hibát keresnek (válassza ezt a mezőt).|
|Alkalmazva:|A címzett tartománya: . . . válassza ki a tartományt.|

További információt az Adathalászat elleni házirendek beállítása [a Microsoft Defender for Office 365.](../security/office-365-security/set-up-anti-phishing-policies.md)

## <a name="protect-against-phishing-attacks-with-safe-links"></a>Adathalászati támadások elleni védelem Széf hivatkozások segítségével

A támadók időnként elrejtik a kártékony webhelyeket az e-mailekben és más fájlokban található hivatkozásokban. Széf A Microsoft Defender for Office 365 webhelyre mutató hivatkozások az e-mailekben és a dokumentumokban található webcímek (URL-címek Office) kattintásra való ellenőrzésével segíthetnek szervezete védelmében. A védelem a csatolási házirendek Széf definiálva.

Azt javasoljuk, hogy tegye a következőket:

- A védelem növelése érdekében módosítsa az alapértelmezett házirendet.

- Vegyen fel egy új házirendet, amely a tartomány összes címzettjére lesz megcélzott.

A hivatkozások Széf tekintse meg [](../business-video/safe-links.md)ezt a rövid oktatóvideónkat, vagy kövesse az alábbi lépéseket:

1. A () [https://protection.office.com](https://protection.office.com) lapra lépve jelentkezzen be a rendszergazdai fiókjával.

2. A Biztonsági megfelelőségi központ bal oldali navigációs ablakának Veszélyforrások kezelése területén válassza &amp; a Házirend **lehetőséget.** 

3. A Házirend lapon válassza a Hivatkozások **Széf lehetőséget.**

Az alapértelmezett házirend módosítása:

1. A Széf lap Házirendek, amelyek a teljes szervezetre vonatkoznak területén válassza az Alapértelmezett **házirend** lehetőséget.

2. Az **Gépház tartalomra vonatkozó** beállítások között válassza az **iOS és az Android Nagyvállalati Microsoft 365-alkalmazások,** Office lehetőséget.

3. Válassza a **Mentés** elemet.

Új házirend létrehozása a tartomány összes címzettjéhez:

1. A Széf lap Házirendek, amelyek a teljes szervezetre területén válassza az új házirend **+** létrehozásához lehetőséget.

2. Alkalmazza az alábbi táblázatban felsorolt beállításokat.

3. Válassza a **Mentés** elemet.

|Beállítás vagy beállítás|Ajánlott beállítás|
|---|---|
|Name (Név)|Széf tartomány összes címzettjének hivatkozási házirendje|
|Az ismeretlen rosszindulatú URL-címek műveletének kiválasztása az üzenetekben|Válassza a Be – Az URL-címeket a rendszer újra fogja írni és ellenőrzi az ismert kártékony hivatkozások listájában, amikor a felhasználó a **hivatkozásra kattint.**|
|Letölthető Széf beolvasása a mellékletek használatával|Jelölje ki ezt a mezőt.|
|Alkalmazva:|A címzett tartománya: . . . válassza ki a tartományt.|

További információt a Hivatkozások [Széf témakörben.](../security/office-365-security/safe-links.md)

## <a name="go-to-intune-admin-center"></a>Az Intune Felügyeleti központ elérése

1. Jelentkezzen be az [Azure Portalba.](https://portal.azure.com/)

2. Válassza **a Minden szolgáltatás lehetőséget,** és írja be az *Intune-t* a **keresőmezőbe.**

3. Miután megjelentek az eredmények,  válassza a kezdő Microsoft Intune, hogy kedvencként és később könnyen megtalálható legyen.

A felügyeleti központban kívül az Intune-nal regisztrálhatja és kezelheti a szervezet eszközeit. További információért lásd: Funkciók regisztrálási [módszerrel](/intune/enrollment/enrollment-method-capab) az Windows és Az Intune által kezelt eszközök regisztrációs [beállításai.](/intune/enrollment-options)

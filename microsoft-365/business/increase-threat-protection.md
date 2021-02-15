---
title: Veszélyforrások elleni védelem növelése a Microsoft 365 Vállalati verzióban
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
description: Állítsa be a Microsoft Defendert az Office 365-hez, és megóvja a bizalmas adatokat az adathalászat, a kártevők és más fenyegetések ellen.
ms.openlocfilehash: 2f1a26b5a2c5678871502d441b6ba64c9b011e1c
ms.sourcegitcommit: 815229e39a0f905d9f06717f00dc82e2a028fa7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48842256"
---
# <a name="increase-threat-protection"></a>Veszélyforrások elleni védelem növelése

Ez a cikk segítséget nyújt a Microsoft 365-előfizetés védelmének növelésében az adathalászat, a kártevők és más fenyegetések elleni védelem érdekében. Ezek az ajánlások a biztonságra fokozottan szükség van, például a jogi irodák és az egészségügyi rendelők számára ajánlottak.

Mielőtt nekikezd, ellenőrizze az Office 365 biztonsági pontszámát. Az Office 365 Biztonsági pontszám elemzi a szervezet biztonságát a szokásos tevékenységek és biztonsági beállítások alapján, és hozzárendel egy pontszámot. Először jegyezze fel az aktuális pontszámot. A pontszám növeléséhez a cikkben ajánlott műveleteket kell végrehajtania. A cél nem a maximális pontszám elérése, hanem a környezet védelmére vonatkozó lehetőségek, amelyek nem befolyásolják hátrányosan a felhasználók hatékonyságát.

További információt a [Microsoft biztonsági pontszáma tartalmaz.](https://docs.microsoft.com/microsoft-365/security/mtp/microsoft-secure-score)

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>A kártevők elleni védelem szintjének emelése a levelekben

Office 365- vagy Microsoft 365-környezete védelmet nyújt a kártevők ellen. Ezt a védelmet növelheti, ha letiltja a mellékleteket a kártevők gyakran használt fájltípusokkal. A kártevők elleni védelem növelése az e-mailekben:

1. Jelentkezzen be a rendszergazdai fiók hitelesítő [https://protection.office.com](https://protection.office.com) adataival.

2. A Biztonsági megfelelőségi központ bal oldali navigációs ablakának Veszélyforrások kezelése területén válassza a Kártevők elleni házirend &amp;   \> **lehetőséget.**

3. Kattintson duplán az alapértelmezett házirendre a vállalati szintű házirend szerkesztéséhez.

4. Válassza a **Beállítások lehetőséget.**

5. A **Gyakori melléklettípusok szűrő alatt válassza** a Be **lehetőséget.** A letiltott fájltípusok közvetlenül a vezérlő alatti ablakban listában szerepelnek. Győződjön meg arról, hogy az alábbi fájltípusokat adja hozzá:

   `ade, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, job, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif`

   Szükség esetén később is hozzáadhat vagy törölhet fájltípusokat.

6. Válassza a **Mentés gombot.**

További információt az [EOP kártevővédelemmel kapcsolatos.](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-malware-protection)

## <a name="protect-against-ransomware"></a>Zsarolóvírusok elleni védelem

A zsarolóvírusok a fájlok titkosítása vagy a számítógép képernyőinek zárolása segítségével korlátozzák az adatokhoz való hozzáférést. Ezután megkísérli zsarolni a pénzüket a zsarolásból, általában cryptocurrencies, például a Bitcoin formájában, az adatokhoz való hozzáférésért cserébe.

A zsarolóvírusok elleni védelem érdekében hozzon létre egy vagy több levelezési szabályt a zsarolóvírusok által gyakran használt fájlkiterjesztések blokkolására. (Ezeket a szabályokat a kártevők elleni védelem szintjét a levelezési lépésben [emelje](#raise-the-level-of-protection-against-malware-in-mail) fel.) Figyelmeztetheti a mellékleteket e-mailben megkapó felhasználókat is.

Az előző lépésben letiltott fájlokon kívül a makrókat is magukban foglaló Office-fájlmellékletek megnyitása előtt létrehozhat egy szabályt, amely figyelmezteti a felhasználókat. A zsarolóvírusok a makrókban elrejtve is el vannak rejtve, ezért figyelmezteti a felhasználókat, hogy ne nyissák meg ezeket a fájlokat az olyan személyek elől, akiket nem ismernek.

Levelezési átviteli szabály létrehozása:

1. A felügyeleti központ megnyitásához válassza az <https://admin.microsoft.com> Exchange **felügyeleti központok** \> **lehetőséget.**

2. Az **e-mail-forgalom kategóriájában** válassza ki a **szabályokat.**

3. Jelölje **+** ki, majd válassza **az Új szabály létrehozása lehetőséget.**

4. Válassza **a párbeszédpanel** alján a További beállítások lehetőséget a beállítások teljes listájának megjelenítéséhez.

5. Alkalmazza a szabályra vonatkozó beállításokat az alábbi táblázatban. A többi beállításhoz használja az alapértelmezett értékeket, hacsak nem szeretné módosítani őket.

6. Válassza a **Mentés** elemet.

|Beállítás|Figyelmeztetést ad a felhasználóknak az Office-fájlok mellékletének megnyitása előtt||
|---|---|---|
|Name (Név)|Zsarolóvírusok elleni szabály: figyelmeztetés a felhasználóknak|
|Alkalmazza ezt a szabályt, ha. . .|Bármely melléklet. . . fájlkiterjesztés egyezik. . .|
|Szavak vagy kifejezések megadása|Adja meg az alábbi fájltípusokat:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm|
|Tegye a következőket. . .|A címzett értesítése üzenettel|
|Üzenetszöveg küldése|Ne nyissa meg az ilyen típusú fájlokat olyan személyektől, akiket nem ismer, mert kártékony kódot tartalmazó makrókat tartalmazhatnak.|

További információ:

- [Zsarolóvírusok: a kockázatok csökkentése](https://www.microsoft.com/security/blog/2020/04/28/ransomware-groups-continue-to-target-healthcare-critical-services-heres-how-to-reduce-risk/)

- [A OneDrive visszaállítása](https://support.microsoft.com/office/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Az e-mailek automatikus továbbításának leállítása

A felhasználók postaládájához hozzáféréssel hozzáférő támadók úgy is ellophatják az e-maileket, hogy a postaládát az e-mailek automatikus továbbítására ják. Ez a felhasználó tájékoztatása nélkül is előfordulhat. Ennek elkerüléséhez konfigurálja az e-mail-forgalom szabályát.

Levelezési átviteli szabály létrehozásához nézze meg ezt a rövid videót, [vagy](https://support.microsoft.com/office/f9d693ba-5c78-47c0-b156-8e461e062aa7) kövesse az alábbi lépéseket:

1. A Microsoft 365 Felügyeleti központban válassza az Exchange **felügyeleti központok** \> **lehetőséget.**

2. Az **e-mail-forgalom kategóriájában** válassza ki a **szabályokat.**

3. Jelölje **+** ki, majd válassza **az Új szabály létrehozása lehetőséget.**

4. Az összes beállítás megjelenítéséhez válassza a További beállítások lehetőséget a párbeszédpanel alján. 

5. Alkalmazza az alábbi táblázatban található beállításokat. A többi beállításhoz használja az alapértelmezett értékeket, hacsak nem szeretné módosítani őket.

6. Válassza a **Mentés** elemet.

|Beállítás|Figyelmeztetést ad a felhasználóknak az Office-fájlok mellékletének megnyitása előtt|
|---|---|
|Name (Név)|Az e-mailek automatikus továbbításának megakadályozása külső tartományokba|
|Alkalmazza ezt a szabályt, ha...|A feladó. . . külső/belső. . . A szervezeten belül|
|Feltétel hozzáadása|Az üzenet tulajdonságai. . . adja meg az üzenet típusát. . . Automatikus továbbítás|
|Tegye a következőket...|Az üzenet blokkolása. . . elutasíthatja az üzenetet, és magyarázatot is tartalmazhat.|
|Üzenetszöveg küldése|A szervezeten kívüli e-mailek automatikus továbbítása biztonsági okokból nem lehetséges.|


## <a name="protect-your-email-from-phishing-attacks"></a>Az e-mailek védelme az adathalász támadások ellen

Ha konfigurált egy vagy több egyéni tartományt az Office 365- vagy a Microsoft 365-környezetben, konfigurálhatja az adathalászat elleni célzott védelmet. Az Adathalászat elleni védelem, amely az Office 365- ös Microsoft Defender része, segíthet megvédeni szervezetét a rosszindulatú, megszemélyesítésen alapuló adathalász támadásoktól és más adathalászati támadásoktól. Ha még nem konfigurált egyéni tartományt, nem kell ezt megtennie.

Azt javasoljuk, hogy ezt a védelmet a legfontosabb felhasználók és az egyéni tartomány védelmére vonatkozó házirend létrehozásával kezdje meg.

Ha az Office 365-hez készült Microsoft [](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)Defenderben adathalászati házirendet hoz létre, nézze meg ezt a rövid oktatóvideónkat, vagy kövesse az alábbi lépéseket:

1. Nyissa meg a [https://protection.office.com](https://protection.office.com) lapot.

2. A Biztonsági megfelelőségi központ bal oldali navigációs ablakának &amp; **Veszélyforrások kezelése** területén válassza a Házirend **lehetőséget.**

3. A Házirend **lapon** válassza az **Adathalászat elleni védelmet.**

4. Az **Adathalászat elleni lapon** válassza a **+ Létrehozás gombot.** Egy varázsló elindítja a lépéseket az adathalászat-csökkentő házirend definiálása során.

5. Adja meg a házirend nevét, leírását és beállításait az alábbi táblázatban ajánlottak szerint. További információt az Adathalászat elleni védelemről az [Office 365-nek a Microsoft Defenderben](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies)talál.

6. A beállítások áttekintése után válassza  a Házirend létrehozása vagy a **Mentés** lehetőséget a megfelelő módon.

|Beállítás vagy beállítás|Ajánlott beállítás|
|---|---|
|Name (Név)|Domain and most valuable campaign staff|
|Leírás|Gondoskodjon arról, hogy a legfontosabb munkatársakat és tartományunkat ne személyeskedje meg.|
|Felhasználók hozzáadása védelemhez|Select **+ Add a condition, The recipient is**. Írja be a felhasználóneveket, vagy adja meg a jelölt, a kampánymenedzser és a többi fontos alkalmazott e-mail-címét. Legfeljebb 20 belső és külső címet adhat hozzá a megszemélyesítéstől védeni kívánt címekhez.|
|Tartományok hozzáadása védelemhez|Select **+ Add a condition, The recipient domain is**. Ha definiált egyet, adja meg a Microsoft 365-előfizetéséhez társított egyéni tartományt. Egynél több tartományt is beírhat.|
|Műveletek kiválasztása|Ha egy megszemélyesített felhasználó küldte az e-mailt: Válassza az Üzenet átirányítása másik e-mail címre **lehetőséget,** majd írja be a biztonsági rendszergazda e-mail-címét; például: *Tamak <span> <span> @contoso.com*. Ha egy megszemélyesített tartomány küldi az e-maileket: Válassza a **Karantén üzenet lehetőséget.**|
|Postaláda-intelligencia|Új adathalászat-házirend létrehozásakor alapértelmezés szerint a postaláda-intelligencia van kiválasztva. A legjobb eredmény érdekében hagyja **be** ezt a beállítást.|
|Megbízható feladók és tartományok hozzáadása|Itt hozzáadhatja saját tartományát vagy bármely más megbízható tartományt.|
|Alkalmazva|Jelölje **ki a címzett tartományát.** A **választható beállítások bármelyike** alatt válassza a **Choose (Választás) lehetőséget.** Válassza **a + Hozzáadás gombot.** Jelölje be a tartomány neve (például contoso) melletti *jelölőnégyzetet. <span> <span> com* listában, majd válassza a **Hozzáadás gombot.** Válassza **a Kész gombot.**|

## <a name="protect-against-malicious-attachments-and-files-with-safe-attachments"></a>A kártékony mellékletek és fájlok elleni védelem a Biztonságos mellékletekkel

A személyek rendszeresen küldenek, fogadnak és osztnak meg mellékleteket, például dokumentumokat, bemutatókat, számolótáblákat stb. Az e-mailekből nem mindig könnyű megmondani, hogy a mellékletek biztonságosak vagy kártékonyak-e. Az Office 365-hez microsoft defender biztonságos mellékletek elleni védelmet is nyújt, de ez a védelem alapértelmezés szerint nincs bekapcsolva. Azt javasoljuk, hogy hozzon létre egy új szabályt a védelem használatának megkezdéséhez. Ez a védelem a SharePointban, a OneDrive-ban és a Microsoft Teamsben tárolt fájlokra is kiterjed.

Biztonságos mellékletre vonatkozó házirend létrehozásához nézze meg ezt a rövid [videót,](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)vagy kövesse az alábbi lépéseket:

1. Jelentkezzen be [https://protection.office.com](https://protection.office.com) a rendszergazdai fiókjával.

2. A Biztonsági megfelelőségi központ bal oldali navigációs ablakának &amp; **Veszélyforrások kezelése** területén válassza a Házirend **lehetőséget.**

3. A Házirend lapon válassza a **Biztonságos mellékletek lehetőséget.**

4. A Biztonságos mellékletek lapon széles körben alkalmazhatja ezt a védelmet a **SharePoint, a OneDrive** és a Microsoft Teams szolgáltatásban bekapcsolt ATP bekapcsolás jelölőnégyzetével.

5. Válassza **+** ezt az új házirend létrehozásához.

6. Alkalmazza az alábbi táblázatban található beállításokat.

7. Miután átnézte a beállításokat, válassza a Házirend létrehozása vagy **a Mentés** lehetőséget a megfelelő módon. 

|Beállítás vagy beállítás|Ajánlott beállítás|
|---|---|
|Name (Név)|Blokkolhatja a kártevőket észlelő aktuális és jövőbeli e-maileket.|
|Leírás|Az észlelt kártevők letiltják a jelenlegi és a jövőbeli e-maileket és mellékleteket.|
|Ismeretlen kártevő-válasz mellékletek mentése|Válassza a Letiltás lehetőséget – A jelenlegi és a jövőbeli e-mailek és **mellékletek blokkolása észlelt kártevővel.**|
|Melléklet átirányítása észlelés után|Engedélyezze az átirányítást (jelölje be ezt a jelölőnégyzetet) Adja meg a rendszergazdai fiókot vagy a postaláda karanténba való beállítását.          A fenti kijelölés alkalmazása, ha a kártevők a mellékletek időkorlok vagy hiba esetén keresnek (jelölje be ezt a jelölőnégyzetet).|
|Alkalmazva|A címzett tartománya. . . válassza ki a tartományát.|

További információt az Adathalászat-elleni házirendek beállítása az [Office 365-hez szükséges Microsoft Defenderben.](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies)

## <a name="protect-against-phishing-attacks-with-safe-links"></a>Az adathalászati támadások elleni védelem biztonságos hivatkozásokkal

A támadók időnként elrejtik a kártékony webhelyeket az e-mailekben vagy más fájlokban található hivatkozásokban. Az Office 365- ös Microsoft Defender biztonságos hivatkozások szolgáltatása az e-mailekben és Az Office-dokumentumokban található webcímek (URL-címek) kattintásra ellenőrzésével segíthet a szervezet védelmében. A biztonságos hivatkozásokra vonatkozó házirendek határozzák meg a védelmet.

Azt javasoljuk, hogy a következőket tegye:

- A védelem növelése érdekében módosítsa az alapértelmezett házirendet.

- Vegyen fel egy új házirendet, amely a tartomány összes címzettjének meg van célva.

A Biztonságos hivatkozások beállításhoz nézze meg ezt a rövid [oktatóvideónkat,](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)vagy kövesse az alábbi lépéseket:

1. Jelentkezzen be [https://protection.office.com](https://protection.office.com) a rendszergazdai fiókjával.

2. A Biztonsági megfelelőségi központ bal oldali navigációs ablakának &amp; **Veszélyforrások kezelése** területén válassza a Házirend **lehetőséget.**

3. A Házirend lapon válassza a **Biztonságos hivatkozások lehetőséget.**

Az alapértelmezett házirend módosítása:

1. A Biztonságos hivatkozások lap Házirendek területén, amelyek a **teljes** szervezetre vonatkoznak, válassza az Alapértelmezett **házirendet.**

2. Az **e-mailek kivételével** a tartalomra vonatkozó beállítások csoportban válassza a **Nagyvállalati Microsoft 365-appok, az iOS És az Android Office** lehetőséget.

3. Válassza a **Mentés** elemet.

Új házirend létrehozása a tartomány összes címzettje számára:

1. A Biztonságos hivatkozások lap Házirendek területén, amelyek a teljes szervezetre vonatkoznak, válassza ki, hogy **+** új házirendet hoz létre.

2. Alkalmazza az alábbi táblázatban felsorolt beállításokat.

3. Válassza a **Mentés** elemet.

|Beállítás vagy beállítás|Ajánlott beállítás|
|---|---|
|Name (Név)|Biztonságos hivatkozásokra vonatkozó házirend a tartomány összes címzettje számára|
|Az ismeretlen, potenciálisan kártékony URL-címek műveletének kiválasztása az üzenetekben|Válassza **a Be lehetőséget–** Az URL-címeket a rendszer újra fogja írni és ellenőrzi az ismert kártékony hivatkozások listájában, amikor a felhasználó a hivatkozásra kattint.|
|Letölthető tartalom beolvasása biztonságos mellékletek használatával|Jelölje ki ezt a jelölőnégyzetet.|
|Alkalmazva|A címzett tartománya. . . válassza ki a tartományát.|

További információt a Biztonságos [hivatkozások témakörben található.](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links)

## <a name="go-to-intune-admin-center"></a>Az Intune Felügyeleti központ elérése

1. Jelentkezzen be az [Azure Portalba.](https://portal.azure.com/)

2. Válassza **az Összes szolgáltatás lehetőséget,** és írja be az *Intune-t* **a keresőmezőbe.**

3. Miután megjelentek az eredmények, válassza a **Microsoft Intune** melletti indítást, hogy kedvencként és később könnyen megtalálható legyen.

A Felügyeleti központon kívül az Intune-nal regisztrálhatja és kezelheti a szervezet eszközeit. További információt a [Funkciók regisztrálási módszerrel](https://docs.microsoft.com/intune/enrollment/enrollment-method-capab) Windows-eszközökhöz és az [Intune](https://docs.microsoft.com/intune/enrollment-options)által kezelt eszközök regisztrációs beállításairól.

---
title: A Microsoft 365 vállalati verzió veszélyforrásai elleni védelem növelése
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
description: Az Office 365 speciális veszélyforrásai elleni védelem beállítása és a bizalmas adatok védelme az adathalászat, a kártevők és más fenyegetések ellen.
ms.openlocfilehash: d56a5371bc5fc4da22f4625024769cc0325a25ca
ms.sourcegitcommit: dffb9b72acd2e0bd286ff7e79c251e7ec6e8ecae
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/17/2020
ms.locfileid: "47948588"
---
# <a name="increase-threat-protection"></a>Veszélyforrások elleni védelem növelése

Ez a cikk segít növelni a Microsoft 365-előfizetés védelmét az adathalászat, a kártevők és az egyéb fenyegetések elleni védekezéshez. Ezek az ajánlások olyan szervezetek számára megfelelőek, amelyeknek nagyobb biztonságra van szükségük, például ügyvédi irodák és egészségügyi klinikák.

Mielőtt elkezdené, ellenőrizze az Office 365 biztonsági pontszámát. Az Office 365 biztonságos pontszáma a szervezeti biztonságot a szokásos tevékenységek és biztonsági beállítások alapján elemzi, és egy pontszámot rendel el. Először vegye figyelembe a jelenlegi pontszámát. A pontszám növeléséhez végezze el a jelen cikkben javasolt műveleteket. A cél nem a maximális pontszám elérése, hanem a környezet védelmére szolgáló lehetőségek ismerete, amelyek nem befolyásolják negatívan a felhasználók hatékonyságát.

További információt a [Microsoft biztonsági pontszáma](https://docs.microsoft.com/microsoft-365/security/mtp/microsoft-secure-score)című témakörben talál.

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>A kártevők elleni védelem szintjének növelése a levelekben

Office 365-vagy Microsoft 365-környezete védelmet nyújt a kártevők ellen. Ezt a védelmet úgy növelheti, hogy a kártevők számára általánosan használt fájltípusokkal blokkolja a mellékleteket. A kártevők elleni védelem növelése az e-mailekben:

1. Nyissa meg a [https://protection.office.com](https://protection.office.com) rendszergazdai fiókja hitelesítő adatait, és lépjen be a fiókjába.

2. A biztonsági &amp; megfelelőségi központban a bal oldali navigációs ablaktábla **veszélyforrások kezelése**csoportjában válassza a **házirend-** \> **ellenes kártevő**lehetőséget.

3. Kattintson duplán az alapértelmezett házirendre a vállalati szintű házirend szerkesztéséhez.

4. Válassza a **Beállítások**lehetőséget.

5. A **gyakori melléklet típusú szűrők**csoportban válassza **a be**lehetőséget. A letiltott fájltípusok közvetlenül a vezérlő alatt jelennek meg az ablakban. Ellenőrizze, hogy a következő fájltípusokat adja-e hozzá:

   `ade, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, job, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif`

   Szükség esetén később is hozzáadhat és törölhet fájltípusokat.

6. Válassza a **Mentés lehetőséget.**

További információ: [kártevők elleni védelem a EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-malware-protection).

## <a name="protect-against-ransomware"></a>Ransomware elleni védelem

A ransomware a fájlok titkosításával vagy a számítógép-képernyők zárolásával korlátozza az adathozzáférést. Ezután megkísérel pénzt keresni az áldozatoktól a "váltságdíjat" kifejezésre, általában cryptocurrencies (például Bitcoin) formájában, az adathozzáférés iránti cserében.

A ransomware elleni védekezéshez hozzon létre egy vagy több e-mail-flow-szabályt, hogy letiltsa a ransomware leggyakrabban használt fájlkiterjesztések használatát. (Ezeket a szabályokat a " [kártevők elleni védelem szintje a posta](#raise-the-level-of-protection-against-malware-in-mail) lépésben" című részen vette fel.) Arra is lehetősége van, hogy figyelmeztesse azokat a felhasználókat, akik e-mail-mellékleteket kapnak.

Az előző lépésben blokkolt fájlok mellett célszerű lehet szabályt létrehozni, hogy figyelmeztesse a felhasználókat, mielőtt megnyitná az Office-mellékletek makrókat tartalmazó fájljait. A ransomware elrejtheti a makrókat, így figyelmeztetheti a felhasználókat, hogy ne tudják megnyitni ezeket a fájlokat a nem ismert személyektől.

Levelezési átviteli szabály létrehozása:

1. Nyissa meg a felügyeleti központot <https://admin.microsoft.com> , és válassza a **felügyeleti központok** \> **Exchange**lehetőséget.

2. Az **e-mail-forgalom** kategóriájában válassza a **szabályok**lehetőséget.

3. Válassza a elemet **+** , majd **az új szabály létrehozása**lehetőséget.

4. A párbeszédpanel alján a **További beállítások** elemre koppintva megtekintheti a teljes beállításokat.

5. Alkalmazza a szabályt az alábbi táblázat beállításaival. Használja a többi beállítás alapértelmezett értékét, kivéve, ha módosítani szeretné őket.

6. Válassza a **Mentés** elemet.

|Beállítás|A felhasználók figyelmeztetése az Office-fájlok mellékleteinek megnyitása előtt||
|---|---|---|
|Name (Név)|Anti-ransomware szabály: felhasználók figyelmeztetése|
|Ezt a szabályt akkor alkalmazza, ha. . .|Bármely melléklet. . . a fájlkiterjesztés-találatok. . .|
|Szavak vagy kifejezések megadása|Adja hozzá az alábbi fájltípusokat:  <br/> dotm, docm, xlsm, sltm, xla, xlam, XLL, PPTM, potm, ppam, ppsm, sldm|
|Végezze el az alábbi műveleteket. . .|Üzenet bejelentése a címzettről|
|Üzenet szövegének megadása|Ne nyissa meg ezeket a fájlokat a nem ismert személyektől, mert kártékony kódot tartalmazó makrókat tartalmazhatnak.|

További információ:

- [Ransomware: a kockázatok csökkentése](https://www.microsoft.com/security/blog/2020/04/28/ransomware-groups-continue-to-target-healthcare-critical-services-heres-how-to-reduce-risk/)

- [A OneDrive visszaállítása](https://support.microsoft.com/office/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Automatikus átirányítás leállítása e-mailekhez

A felhasználók postaládájához hozzáféréssel rendelkező hackerek e-mailek automatikus továbbítására való beállításával a postaládát megadhatják. Ez a funkció a felhasználó figyelmének felhívása nélkül is megtörténhet. Ennek elkerüléséhez állítsa be az e-mail-forgalom szabályát.

Ha levelezési átviteli szabályt szeretne létrehozni, nézze meg [ezt a rövid videót](https://support.microsoft.com/office/f9d693ba-5c78-47c0-b156-8e461e062aa7) , vagy kövesse az alábbi lépéseket:

1. A Microsoft 365 felügyeleti központban válassza a **felügyeleti központok** \> **Exchange**lehetőséget.

2. Az **e-mail-forgalom** kategóriájában válassza a **szabályok**lehetőséget.

3. Válassza a elemet **+** , majd **az új szabály létrehozása**lehetőséget.

4. Az összes beállítás megtekintéséhez válassza a **További beállítások** lehetőséget a párbeszédpanel alján.

5. Alkalmazza az alábbi táblázatban szereplő beállításokat. Használja a többi beállítás alapértelmezett értékét, kivéve, ha módosítani szeretné őket.

6. Válassza a **Mentés** elemet.

|Beállítás|A felhasználók figyelmeztetése az Office-fájlok mellékleteinek megnyitása előtt|
|---|---|
|Name (Név)|E-mailek automatikus továbbításának megakadályozása külső tartományokban|
|Ezt a szabályt akkor alkalmazza, ha...|A feladót. . . külső/belső. . . A szervezeten belül|
|Feltétel hozzáadása|Az üzenet tulajdonságai. . . adja meg az üzenetet. . . Automatikus továbbítás|
|Végezze el az alábbi műveleteket...|Tiltsa le az üzenetet. . . utasítsa el az üzenetet, és adja meg a magyarázatot.|
|Üzenet szövegének megadása|A szervezeten kívüli e-mailek automatikus továbbítása nem akadályozza meg a biztonsági megfontolásokat.|


## <a name="protect-your-email-from-phishing-attacks"></a>E-mailek védelme az adathalász támadások ellen

Ha egy vagy több egyéni tartományt konfigurált az Office 365-vagy Microsoft 365-környezetéhez, beállíthatja a célzott adathalászat elleni védelmet. Az ATP-adathalászat elleni védelem, az Office 365 Advanced Threat Protection része segíthet a szervezet védelmében a rosszindulatú megszemélyesítési alapú adathalász támadások és más adathalász támadások ellen. Ha még nem állított be egyéni tartományt, erre nincs szükség.

Azt javasoljuk, hogy kezdje el ezt a védelmet a fontos felhasználók és az egyéni tartomány védelmére szolgáló házirend létrehozásával.

Ha ATP-adathalászati házirendet szeretne létrehozni, nézze meg  [ezt a rövid oktatóprogramot](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c), vagy végezze el az alábbi lépéseket:

1. Nyissa meg a [https://protection.office.com](https://protection.office.com) lapot.

2. A biztonsági &amp; megfelelőségi központban, a bal oldali navigációs ablak **veszélyforrások kezelése**csoportjában válassza a **házirend**lehetőséget.

3. A **házirend** lapon válassza az **ATP-adathalászat**lehetőséget.

4. Az **anti-phishing** lapon válassza a **+ create (létrehozás**) lehetőséget. A varázsló bemutatja, hogy milyen lépéseket kell tennie az adathalászati adathalászat-házirend meghatározásához.

5. Adja meg a házirend nevét, leírását és beállításait az alábbi táblázatban javasolt módon. További részletekért olvassa el az [ATP-adathalászatról szóló házirend-beállítások](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies)ismertetése című témakört.

6. A beállítások átnézése után válassza a **házirend létrehozása** vagy a megfelelő **mentése**lehetőséget.

|Beállítás vagy beállítás|Ajánlott beállítás|
|---|---|
|Name (Név)|A tartomány és a legértékesebb kampány oktatói|
|Leírás|Ügyeljen arra, hogy a legfontosabb munkatársak és a tartományuk ne legyen megszemélyesítve.|
|Felhasználók hozzáadása a védelemhez|Válassza **a + feltétel hozzáadása lehetőséget, a címzett**. Írja be a felhasználóneveket, vagy írja be a pályázó, a kampány kezelőjé és a többi fontos oktató e-mail-címét. Legfeljebb 20 belső és külső címet adhat hozzá, amelyeket a megszemélyesítéstől védeni szeretne.|
|Tartományok hozzáadása a védelemhez|Válassza **a + feltétel hozzáadása lehetőséget, a címzett tartomány**lehetőséget. Adja meg a Microsoft 365-előfizetéséhez társított egyéni tartományt, ha definiált egyet. Több tartományt is beírhat.|
|A műveletek elem választása|Ha a rendszer megszemélyesített felhasználó által küldi el az e-mailt, válassza az **üzenet átirányítása másik e-mail-címre**lehetőséget, majd írja be a biztonsági rendszergazda e-mail-címét. például *Alice <span> <span> @contoso. com*. Ha egy megszemélyesített tartomány küldi el az e-mailt: válassza a **karantén üzenet**lehetőséget.|
|Postaláda-intelligencia|A postaláda-intelligencia alapértelmezés szerint ki van jelölve, amikor új adathalászati házirendet hoz létre. A legjobb eredmény érdekében hagyja ezt **a** beállítást.|
|Megbízható feladók és tartományok hozzáadása|Itt adhatja meg saját tartományát vagy más megbízható tartományokat.|
|Alkalmazva|Válassza ki **a címzett tartományát**. A **bármelyik**csoportban válassza a **kiválasztás**gombot. Válassza a **+ Hozzáadás**gombot. Jelölje be a tartomány neve melletti jelölőnégyzetet, például: *contoso. <span> <span> com*, a listában, és válassza a **Hozzáadás**gombot. Válassza a **kész**lehetőséget.|

## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Ártalmas mellékletek és fájlok elleni védelem az ATP-Safe-mellékletekkel

A személyek rendszeresen küldenek, fogadhatnak és oszthatnak meg mellékleteket (például dokumentumokat, bemutatókat, számolótáblákat stb.). Nem mindig könnyű megállapítani, hogy egy melléklet biztonságos vagy rosszindulatú-e egy e-mail-üzenetben. Az Office 365 Advanced Threat Protection az ATP Safe Attachment Protectiont is támogatja, de ez a védelem alapértelmezés szerint nincs bekapcsolva. Azt javasoljuk, hogy hozzon létre egy új szabályt a védelem használatának megkezdéséhez. Ez a védelem kiterjed a SharePoint, a OneDrive és a Microsoft Teams fájljaira.

Az ATP-biztonsággal kapcsolatos házirend létrehozásához nézze meg [ezt a rövid videót](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), vagy végezze el az alábbi lépéseket:

1. Nyissa meg a [https://protection.office.com](https://protection.office.com) rendszergazdai fiókját, és lépjen be a fiókjába.

2. A biztonsági &amp; megfelelőségi központban, a bal oldali navigációs ablak **veszélyforrások kezelése**csoportjában válassza a **házirend**lehetőséget.

3. A házirend lapon válassza az **ATP Safe mellékletek**elemet.

4. A biztonságos mellékletek lapon széles körben alkalmazza ezt a védelmet az **ATP bekapcsolása a sharepointhoz, a OneDrive és a Microsoft Teams** jelölőnégyzet bejelölésével.

5. **+** Új házirend létrehozásához válassza a elemet.

6. Alkalmazza az alábbi táblázatban szereplő beállításokat.

7. A beállítások átnézése után válassza a **házirend létrehozása** vagy a megfelelő **mentése**lehetőséget.

|Beállítás vagy beállítás|Ajánlott beállítás|
|---|---|
|Name (Név)|Az észlelt kártevőket tartalmazó jelenlegi és jövőbeli e-mailek blokkolása.|
|Leírás|Letilthatja a jelenlegi és a jövőbeli e-maileket és mellékleteket az észlelt kártevővel.|
|A mellékletek ismeretlen kártevő-válasz mentése|Válassza **a blokkolás – blokkolhatja a jelenlegi és a jövőbeli e-maileket és mellékleteket az észlelt kártevővel**.|
|Melléklet átirányítása az észleléshez|Átirányítás engedélyezése (jelölje be ezt a jelölőnégyzetet) a rendszergazdai fiók vagy a karanténba helyezett postaláda-beállítás megadásához.          A fenti kijelölés alkalmazása, ha a kártevők beolvasása a mellékletek időtúllépése vagy a hiba történik (jelölje be a jelölőnégyzetet).|
|Alkalmazva|A címzett tartománya. . . Válassza ki a tartományt.|

További információt az [Office 365 ATP-adathalászati házirendek beállítása](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies)című témakörben talál.

## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Adathalász támadások elleni védelem az ATP-Safe-hivatkozásokkal

A hackerek időnként kártékony webhelyeket rejtenek el az e-mailek vagy más fájlok hivatkozásaiban. Office 365 ATP Safe Links (ATP Safe Links), az Office 365 Advanced Threat Protection része segíthet a szervezet védelmében azáltal, hogy időpontos ellenőrzéssel rendelkezik az e-mailekben és az Office-dokumentumokban lévő webcímekről. A védelem az ATP Safe Links-házirendjeivel van meghatározva.

Azt javasoljuk, hogy tegye az alábbiakat:

- Módosítsa az alapértelmezett házirendet a védelem növeléséhez.

- Vegyen fel egy új házirendet a tartomány összes címzettjének.

Az ATP-Safe-kapcsolatok beállításához nézze meg [ezt a rövid oktatóprogramot](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), vagy végezze el az alábbi lépéseket:

1. Nyissa meg a [https://protection.office.com](https://protection.office.com) rendszergazdai fiókját, és lépjen be a fiókjába.

2. A biztonsági &amp; megfelelőségi központban, a bal oldali navigációs ablak **veszélyforrások kezelése**csoportjában válassza a **házirend**lehetőséget.

3. A házirend lapon válassza az **ATP-megbízható hivatkozások**lehetőséget.

Az alapértelmezett házirend módosítása:

1. A megbízható hivatkozások lapon, az **egész szervezetre érvényes házirendek**csoportban válassza ki az **alapértelmezett** házirendet.

2. Az **e-mailek kivételével a tartalomra vonatkozó beállítások**csoportban válassza **a Microsoft 365-alkalmazások nagyvállalatoknak, iOS-és Android-Office**lehetőséget.

3. Válassza a **Mentés** elemet.

Új házirend létrehozása a tartomány összes címzettjének:

1. A megbízható hivatkozások lapon, **az egész szervezetre érvényes házirendek**csoportban válassza **+** a lehetőséget új házirend létrehozásához.

2. Alkalmazza az alábbi táblázatban felsorolt beállításokat.

3. Válassza a **Mentés** elemet.

|Beállítás vagy beállítás|Ajánlott beállítás|
|---|---|
|Name (Név)|A megbízható hivatkozások házirendje a tartomány összes címzettjének|
|Az ismeretlen, esetleg kártékony URL-címekre vonatkozó műveletek kijelölése az üzenetekben|**Ha a felhasználó a hivatkozásra kattint, a beérkező URL-címeket a program felülírja és ellenőrzi az ismert rosszindulatú hivatkozások listájával**.|
|Letölthető tartalmak beolvasása biztonságos mellékletekkel|Jelölje be a jelölőnégyzetet.|
|Alkalmazva|A címzett tartománya. . . Válassza ki a tartományt.|

További információt az [Office 365 ATP Safe Links](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links)című témakörben találhat.

## <a name="go-to-intune-admin-center"></a>Nyissa meg az Intune felügyeleti központot.

1. Bejelentkezés az [Azure portálra](https://portal.azure.com/)

2. Jelölje ki az **összes szolgáltatást** , és írja be az *Intune* **kifejezést a keresőmezőbe**.

3. Ha megjelentek a találatok, válassza a Start gombot a **Microsoft Intune** elem mellett, hogy kedvencként és könnyebben megtaláljon később.

A felügyeleti központban kívül a Intune segítségével is beírhatja és kezelheti szervezete eszközeit. További információért olvassa el a [Windows rendszerű eszközökre vonatkozó beiktatási módszer](https://docs.microsoft.com/intune/enrollment/enrollment-method-capab) , valamint [az Intune által felügyelt eszközök tanúsítványigénylési lehetőségei](https://docs.microsoft.com/intune/enrollment-options)című témakört.

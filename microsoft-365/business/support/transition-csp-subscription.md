---
title: Microsoft 365 Vállalati csp-előfizetés váltása 
description: Megtudhatja, hogy miként válthat át a Microsoft 365 Vállalati alapú csp-előfizetéselőnézetről általános rendelkezésre állásra (GA).
author: jasongroce
f1.keywords:
- NOCSH
ms.custom:
- seo-marvel-mar
ms.author: jasgro
ms.topic: article 
ms.prod: microsoft-365-business
localization_priority: Normal
audience: microsoft-business 
keywords: Microsoft 365 Vállalati verzió, Microsoft 365, SMB, átmeneti CSP-előfizetés
ms.date: 11/01/2017
ms.openlocfilehash: 77b7b474a5ad17db58e283ea61b074c959905d1b
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/07/2020
ms.locfileid: "42560780"
---
# <a name="transition-a-microsoft-365-business-csp-subscription"></a>Microsoft 365 Vállalati csp-előfizetés váltása

Ha Microsoft 365 Vállalati előzetes verziós kripta-előfizetéssel rendelkezik, az alábbi útmutatóból megtudhatja, hogyan válthat át meglévő előzetes előfizetését a Microsoft 365 Vállalati vállalati verzióra (általános elérhetőség).

**Az előzetes verziójú előfizetés ga-ra váltása**

1. Jelentkezzen be a <a href="https://partnercenter.microsoft.com" target="_blank">Partnerközpontba</a>.
2. Az irányítópulton válassza az **Ügyfelek**lehetőséget, majd keresse meg és válassza ki a vállalat nevét.

    A vállalat előfizetései fel lesznek sorolva.

    ![Az ügyfél előfizetései a Partnerközpontban](../../media/pc_customer_subscriptions_1.png)
    
3. A vállalat **Előfizetések** lapján válassza az **Előfizetés hozzáadása**lehetőséget.
4. Az **Új előfizetés** lapon válassza a **Kisvállalkozás** lehetőséget, majd a Listából válassza a **Microsoft 365 Business** lehetőséget.
5. Adja meg a licencek számát, majd válassza a **Tovább: Véleményezés lehetőséget** az előfizetés áttekintéséhez, majd válassza a **Küldés**lehetőséget.

    ![Tekintse át a Microsoft 365 Business új előfizetését](../../media/pc_customer_reviewnewsubscription.png)

    A **licencalapú előfizetések** a **Microsoft 365 Business Preview** és a Microsoft **365 Business**előzetes verziót jelenítik meg. Ezután felfüggeszti az előzetes verziós előfizetést.

6. Válassza a **Microsoft 365 Üzleti előzetes verzió**lehetőséget.
7. A **Microsoft 365 Üzleti előzetes verzió** lapján válassza a **Felfüggesztett** lehetőséget az előzetes verziós előfizetés felfüggesztéséhez.

    ![A Microsoft 365 Business Preview előfizetés felfüggesztése](../../media/pc_customer_m365bpreview_suspend.png)

8. Válassza a **Megerősítés beküldése** lehetőséget.

    Az **Előfizetések** lapon ellenőrizze, hogy a **Microsoft 365 Vállalati előzetes verzió** állapota **felfüggesztés.**

    ![Az előzetes verzióelőfizetés állapotának felfüggesztése](../../media/pc_customer_m365bpreview_suspend_confirm.png)

9. Szükség esetén érvényesítheti a licencszerződést is. Ehhez kövesse az alábbi lépéseket:
    1. Válassza a **Felhasználók és licencek** lehetőséget a vállalat **Előfizetések** lapján.
    2. A **Felhasználók és licencek** lapon jelöljön ki egy felhasználót.
    3. A felhasználó oldalán ellenőrizze a **Licencek hozzárendelése** szakaszt, és ellenőrizze, hogy a **Microsoft 365 Vállalati verzió látható-e.**

        ![Annak ellenőrzése, hogy a Microsoft 365 Vállalati verzió licenc hozzá van rendelve a felhasználóhoz](../../media/pc_customer_userslicenses_m365b_validate.png)

## <a name="impact-to-customers-and-users-during-and-after-transition"></a>Az ügyfelekre és a felhasználókra gyakorolt hatás az átmenet alatt és után

Az átállás és a felhasználók nincshatással az ügyfelekre és a felhasználókra az átállás és a bejegyzés során.

## <a name="impact-to-customers-who-dont-transition"></a>Hatással van az ügyfelekre, akik nem váltanak át

Az alábbi táblázat azokat az ügyfeleket foglalja össze, akik nem váltanak át Microsoft 365 Business Preview-előfizetésről Microsoft 365 Vállalati verziós előfizetésre.

|       | T-0-tól T+30-ig     | T+30 és T+60 között | T+60 és T+120 között | T+120-on túl  |
|-------|-----------------|--------------|---------------|---------------|
| **Állami** | Türelmi időszakban | Lejárt      | Tiltva      | Megszüntetés |
| **A szolgáltatásra gyakorolt hatások**                                                        |
| **Microsoft 365 Vállalati verzió felügyeleti portálja** | Nincs hatással a funkcionalitásra | Nincs hatással a funkcionalitásra | Felhasználókat adhat hozzá/törölhet, előfizetéseket vásárolhat.</br> Nem lehet licenceket rendelni/visszavonni. | Az ügyfél előfizetése és minden adat törlődik. A rendszergazda más fizetős előfizetéseket is kezelhet. |
| **Office-alkalmazások**                         | Nincs végfelhasználói hatás | Nincs végfelhasználói hatás | Az Office csökkentett üzemmódba lép.</br> A felhasználók csak fájlokat tekinthetnek meg. | Az Office csökkentett üzemmódba lép.</br> A felhasználók csak fájlokat tekinthetnek meg. |
| **Felhőszolgáltatások (SharePoint Online, Exchange Online, Skype, Teams stb.)** | Nincs végfelhasználói hatás | Nincs végfelhasználói hatás | A végfelhasználók és a rendszergazdák nem férnek hozzá a felhőben lévő adatokhoz. | Az ügyfél előfizetése és minden adat törlődik. |
| **EM+S alkatrészek** | Nincs rendszergazdai hatás</br> Nincs végfelhasználói hatás | Nincs rendszergazdai hatás</br> Nincs végfelhasználói hatás | A képesség már nem érvényesíthető.</br> További információ: [A mobileszközök relevancia az előfizetés lejáratakor](#mobile-device-impacts-upon-subscription-expiration) és a [Windows 10-es számítógépek relevancia az előfizetés lejáratakor.](#windows-10-pc-impacts-upon-subscription-expiration) | A képesség már nem érvényesíthető.</br> További információ: [A mobileszközök relevancia az előfizetés lejáratakor](#mobile-device-impacts-upon-subscription-expiration) és a [Windows 10-es számítógépek relevancia az előfizetés lejáratakor.](#windows-10-pc-impacts-upon-subscription-expiration) |
| **Windows 10 Vállalati verzió** | Nincs rendszergazdai hatás</br> Nincs végfelhasználói hatás | Nincs rendszergazdai hatás</br> Nincs végfelhasználói hatás | A képesség már nem érvényesíthető.</br> További információ: [A mobileszközök relevancia az előfizetés lejáratakor](#mobile-device-impacts-upon-subscription-expiration) és a [Windows 10-es számítógépek relevancia az előfizetés lejáratakor.](#windows-10-pc-impacts-upon-subscription-expiration) | A képesség már nem érvényesíthető.</br> További információ: [A mobileszközök relevancia az előfizetés lejáratakor](#mobile-device-impacts-upon-subscription-expiration) és a [Windows 10-es számítógépek relevancia az előfizetés lejáratakor.](#windows-10-pc-impacts-upon-subscription-expiration) |
| **Azure AD bejelentkezés Windows 10-es számítógépre** | Nincs rendszergazdai hatás</br> Nincs végfelhasználói hatás | Nincs rendszergazdai hatás</br> Nincs végfelhasználói hatás | Nincs rendszergazdai hatás</br> Nincs végfelhasználói hatás | A bérlő törlése után a felhasználó csak helyi hitelesítő adatokkal jelentkezhet be. Ha nincs enek helyi hitelesítő adatok, képezd át újra az eszközt. |

## <a name="mobile-device-impacts-upon-subscription-expiration"></a>A mobileszköz hatással van az előfizetés lejáratára

Az alábbi táblázat összefoglalja az alkalmazáskezelési szabályzatokra gyakorolt hatást a mobileszközökön.

|                            | Teljes körű licenccel rendelkező élmény                      | T+60 nappal a lejárat után          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Munkafájlok törlése inaktív eszközről** | A munkafájlok a kijelölt napok után törlődnek | A munkahelyi fájlok a felhasználó személyes eszközein maradnak |
| **A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió** | A munkahelyi fájlok csak a OneDrive Vállalati verzióba menthetők | A munkahelyi fájlok at bárhol menthetik |
| **Munkahelyi fájlok titkosítása** | A munkahelyi fájlok titkosítva vannak | A munkahelyi fájlok már nincsenek titkosítva.</br> A rendszer eltávolítja a biztonsági házirendeket, és eltávolítja az alkalmazások Office-adatait. |
| **PIN-kód vagy ujjlenyomat megkövetelése az Office-alkalmazások eléréséhez** | Korlátozott hozzáférés az alkalmazásokhoz | Nincs alkalmazásszintű hozzáférési korlátozás |
| **PIN-kód alaphelyzetbe állítása, ha a bejelentkezés sikertelen** | Korlátozott hozzáférés az alkalmazásokhoz | Nincs alkalmazásszintű hozzáférési korlátozás |
| **Az Office-alkalmazások tétlensége után a felhasználók tól újra be kell jelentkezniük** | Bejelentkezés szükséges | Nincs szükség bejelentkezésre |
| **Munkahelyi fájlokhoz való hozzáférés letiltása függetlenített vagy feltört eszközökön** | A munkahelyi fájlok nem érhetők el feltört/gyökeres eszközökön | A munkahelyi fájlok jailbroken/gyökeres eszközökön érhetők el |
| **Tartalom másolásának engedélyezése a felhasználóknak az Office-alkalmazásokból a személyes alkalmazásokba** | Másolás/beillesztés a Microsoft 365 Business-előfizetés részeként elérhető alkalmazásokra korlátozva | Az összes alkalmazás másolása/beillesztése |

## <a name="windows-10-pc-impacts-upon-subscription-expiration"></a>A Windows 10 PC hatással van az előfizetés lejáratára

Az alábbi táblázat összefoglalja a Windows 10-es eszközkonfigurációs házirendek hatását.

|                            | Teljes körű licenccel rendelkező élmény                      | T+60 nappal a lejárat után          |
|----------------------------|------------------------------------------------|------------------------------------|
| **A Windows Defender segítségével megvédheti a számítógépeket a fenyegetésektől** | A be- és kikapcsolás kívül esik a felhasználói vezérlőn | A felhasználó be- és kikapcsolhatja a Windows Defender t a Windows 10-es pc-n |
| **PC-k védelme a webes fenyegetésekkel szemben a Microsoft Edge böngészőben** | Számítógép-védelem a Microsoft Edge-ben | A felhasználó be- és kikapcsolhatja a számítógép védelmét a Microsoft Edge-ben |
| **Az eszköz képernyőjének kikapcsolása tétlen állapotban** | A rendszergazda határozza meg a képernyő időintervallum-házirendjét | A képernyő időkorlátját a végfelhasználó konfigurálhatja |
| **A felhasználók letölthetnek appokat innen: Microsoft Áruház** | A rendszergazda határozza meg, hogy a felhasználó le tudja-e tölteni az alkalmazásokat a Microsoft Store-ból | A felhasználó bármikor letölthet alkalmazásokat a Microsoft Store-ból |
| **A felhasználók igénybe vehetik Cortana segítségét** | A rendszergazda határozza meg a Cortanához való felhasználói hozzáférésre vonatkozó szabályzatot | Cortana be- és kikapcsolásához használható felhasználói eszközök |
| **Tippek és hirdetések fogadásának engedélyezése a felhasználóknak a Microsofttól** | A rendszergazda határozza meg a felhasználókra vonatkozó irányelveket, amelyek tippeket és hirdetéseket kapnak a Microsofttól | A felhasználó be- és kikapcsolhatja a Microsoft tippjeit és hirdetéseit |
| **A felhasználók másolhatnak tartalmakat az Office-appokból személyes appokba** | A rendszergazda határozza meg a Windows 10-es eszközök naprakészen tartására vonatkozó házirendet | A felhasználók eldönthetik, hogy mikor frissítsék a Windows rendszert |

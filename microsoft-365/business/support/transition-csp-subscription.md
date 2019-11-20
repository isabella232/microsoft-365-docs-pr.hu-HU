---
title: Microsoft 365 Business CSP-előfizetés át, 
description: Megtudhatja, hogyan lehet a Microsoft 365 Business CSP előfizetését GA-ra átmenni. 
author: jasongroce
ms.author: jasgro
ms.topic: article 
ms.prod: microsoft-365-business
localization_priority: Normal
audience: microsoft-business 
keywords: Microsoft 365 Business, Microsoft 365, SMB, átmeneti CSP-előfizetés
ms.date: 11/01/2017
ms.openlocfilehash: 72e620df69a425ca7e5c41c5a6651bc0f7f533de
ms.sourcegitcommit: b535fe233234fd25146cfe15478e20d954f71e03
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/20/2019
ms.locfileid: "38748341"
---
# <a name="transition-a-microsoft-365-business-csp-subscription"></a>Microsoft 365 Business CSP-előfizetés át,

Ha rendelkezik Microsoft 365 Business Preview CSP előfizetéssel, akkor kövesse az alábbi útmutatót, hogy megtudja, hogyan lehet áttérni a meglévő előnézet-előfizetést a Microsoft 365 Business GA szoftverbe (általános elérhetőség).

**Hogyan átmenet egy előnézet előfizetés GA**

1. Jelentkezzen be a <a href="https://partnercenter.microsoft.com" target="_blank">Partnerközpontba</a>.
2. Az irányítópulton válassza a **vevők**, majd keresse meg és jelölje ki a vállalatnevet.

    Megjelennek a vállalat előfizetései.

    ![Ügyfél-előfizetések a Partnerközpontban](images/pc_customer_subscriptions_1.png)
    
3. A vállalat **előfizetések** lapján jelölje be az **előfizetés hozzáadása**választógombot.
4. Az **új előfizetés** lapon válassza ki a **Small Business** és válassza a **Microsoft 365 Business** listaoldalt.
5. Adja meg a licencek számát, majd kattintson a **Tovább: Review (ellenőrzés** ) lehetőségre az előfizetés áttekintéséhez, majd válassza a **Küldés**-t.

    ![Tekintse át a Microsoft 365 Business új előfizetését.](images/pc_customer_reviewnewsubscription.png)

    A **engedély-kiindulópontul szolgáló előfizetések** akarat mutat **Mikroszkóp 365 teendő sajtóbemutató** és **Mikroszkóp 365 teendő**. Ezután felfüggeszti az előfizetés előnézetét.

6. Válassza a **Microsoft 365 Business Preview**-t.
7. -On **mikroszkóp 365 teendő sajtóbemutató** oldal, kiválaszt **felfüggesztett** -hoz felfüggeszt a sajtóbemutató aláírás.

    ![A Microsoft 365 Business Preview előfizetésének felfüggesztése](images/pc_customer_m365bpreview_suspend.png)

8. Jóváhagyásához válassza a **Küldés** -t.

    -On **előfizetések** oldal, igazol amit a **Mikroszkóp 365 teendő sajtóbemutató** helyzet mutat **felfüggesztett**.

    ![Nyugtázza az előfizetés-előnézetet állapot felfüggesztése](images/pc_customer_m365bpreview_suspend_confirm.png)

9. Szükség esetén a licencszerződést is érvényesítheti. Ehhez kövesse az alábbi lépéseket:
    1. Válassza ki a **felhasználókat és licenceket** a vállalat **előfizetések** oldalán.
    2. A **felhasználók és licencek** lapon jelöljön ki egy felhasználót.
    3. -On használók ' oldal, ellenőriz a **átruház engedélyez** rész és igazol amit ez mutat **Mikroszkóp 365 teendő**.

        ![Erősítse meg a Microsoft 365 üzleti licenc hozzárendelését a felhasználóhoz](images/pc_customer_userslicenses_m365b_validate.png)

## <a name="impact-to-customers-and-users-during-and-after-transition"></a>Az ügyfeleknek és a felhasználóknak átmenet közben és után gyakorolt hatása

Nincs hatása az ügyfelek és a felhasználók az átmenet során, és utáni átmenet.

## <a name="impact-to-customers-who-dont-transition"></a>Hatással vannak az olyan vásárlvevőknek, akik nem átmennek

Az alábbi táblázat összefoglalja azokat a vevőket, akik nem a Microsoft 365 Business Preview előfizetését Microsoft 365 Business előfizetésre átírták.

|       | T-0-T + 30     | T + 30-T + 60 | T + 60-T + 120 | Beyond T + 120  |
|-------|-----------------|--------------|---------------|---------------|
| **Állami** | Türelmi időszakban | Lejárt      | Tiltva      | Deprovisioned |
| **A szolgáltatás hatásai**                                                        |
| **Microsoft 365 üzleti adminisztrátori portál** | Nincs hatással a funkcionalitás | Nincs hatással a funkcionalitás | Felvehet/törölhet felhasználókat, vásárolhat előfizetéseket.</br> Nem lehet hozzárendelni/visszavonni a licenceket. | Az ügyfél előfizetése és minden adat törlődik. Admin tudja kezelni a többi fizetett előfizetések. |
| **Office-alkalmazások**                         | Nincs végfelhasználói ütközés | Nincs végfelhasználói ütközés | Az Office csökkentett szolgáltatáskészletet nyújtó üzemmódba lép.</br> Használók tud kilátás fájlokat egyetlen. | Az Office csökkentett szolgáltatáskészletet nyújtó üzemmódba lép.</br> Használók tud kilátás fájlokat egyetlen. |
| **Felhőalapú szolgáltatások (SharePoint Online, Exchange Online, Skype, csapatok és egyéb)** | Nincs végfelhasználói ütközés | Nincs végfelhasználói ütközés | A végfelhasználók és az adminisztrátorok nem férhetnek hozzá az adatokhoz a felhőben. | Az ügyfél előfizetése és minden adat törlésre kerül. |
| **EM + S komponensek** | Nincs admin hatása</br> Nincs végfelhasználói ütközés | Nincs admin hatása</br> Nincs végfelhasználói ütközés | A képességek már nem érvényesíthetők.</br> Lát [mozgatható berendezés ütközés azon aláírás kipárolgás](#mobile-device-impacts-upon-subscription-expiration) és [Windows 10 PC ütközés azon aláírás lejárat](#windows-10-pc-impacts-upon-subscription-expiration) többért értesít. | A képességek már nem érvényesíthetők.</br> Lát [mozgatható berendezés ütközés azon aláírás kipárolgás](#mobile-device-impacts-upon-subscription-expiration) és [Windows 10 PC ütközés azon aláírás lejárat](#windows-10-pc-impacts-upon-subscription-expiration) többért értesít. |
| **Windows 10 üzleti** | Nincs admin hatása</br> Nincs végfelhasználói ütközés | Nincs admin hatása</br> Nincs végfelhasználói ütközés | A képességek már nem érvényesíthetők.</br> Lát [mozgatható berendezés ütközés azon aláírás kipárolgás](#mobile-device-impacts-upon-subscription-expiration) és [Windows 10 PC ütközés azon aláírás lejárat](#windows-10-pc-impacts-upon-subscription-expiration) többért értesít. | A képességek már nem érvényesíthetők.</br> Lát [mozgatható berendezés ütközés azon aláírás kipárolgás](#mobile-device-impacts-upon-subscription-expiration) és [Windows 10 PC ütközés azon aláírás lejárat](#windows-10-pc-impacts-upon-subscription-expiration) többért értesít. |
| **Azúrkék AD logika-hoz egy Windows 10 PC** | Nincs admin hatása</br> Nincs végfelhasználói ütközés | Nincs admin hatása</br> Nincs végfelhasználói ütközés | Nincs admin hatása</br> Nincs végfelhasználói ütközés | A bérlő törlését követően a felhasználó csak helyi hitelesítő adatokkal tud bejelentkezni. Ha nincsenek helyi hitelesítő adatok, az eszköz ismételt képe |

## <a name="mobile-device-impacts-upon-subscription-expiration"></a>Mobileszköz-hatások az előfizetés lejártakor

Az alábbi táblázat összefoglalja, hogy az Alkalmazáskezelési házirendek milyen hatással vannak a mobileszközökre.

|                            | Teljesen licenszelt tapasztalat                      | T + 60 nap utáni lejárati          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Munkafájlok törlése egy inaktív eszközről** | A munkafájlok törlődnek a kijelölt napok után | A munkahelyi fájlok megmaradnak a felhasználó személyi eszközén |
| **A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió** | Munka fájlokat tud egyetlen lenni megtakarított-hoz OneDrive részére teendő | A munkahelyi fájlokat bárhol elmenthető |
| **Munkahelyi fájlok titkosítása** | A munkafájlok titkosítva vannak | A munka fájljai már nem titkosítottak.</br> A biztonsági házirendek törlődnek, az alkalmazások Office-adatai pedig törlődnek. |
| **A PIN-vagy ujjlenyomat-hozzáférés megkövetelése az Office-alkalmazásokhoz** | Az alkalmazásokhoz való hozzáférés korlátozása | Nincs app szintű hozzáférés-korlátozás |
| **A PIN visszaállítása a bejelentkezés sikertelensége esetén** | Az alkalmazásokhoz való hozzáférés korlátozása | Nincs app szintű hozzáférés-korlátozás |
| **A felhasználók bejelentkezése az Office alkalmazások üresjárata után** | Bejelentkezés szükséges | Nincs szükség bejelentkezelemre |
| **Munkahelyi fájlokhoz való hozzáférés letiltása függetlenített vagy feltört eszközökön** | A munka fájlok nem érhetők el jailbroken/gyökeres eszközökön | Dolgozik fájlokat lehet kitört-ra jailbroken/begyökerezett berendezés |
| **Az Office-alkalmazásokból származó tartalmak másolása a felhasználók személyes alkalmazásába** | Másol/tészta behatárolt-hoz apps elérhető részeként Mikroszkóp 365 teendő aláírás | Másolás/beillesztés az összes alkalmazás számára |

## <a name="windows-10-pc-impacts-upon-subscription-expiration"></a>Windows 10 PC hatása után előfizetés lejárata

Az alábbi táblázat összefoglalja a Windows 10 eszközkonfigurációs házirendjeit.

|                            | Teljesen licenszelt tapasztalat                      | T + 60 nap utáni lejárati          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Megvédheti a számítógépeket a fenyegetésektől a Windows Defender segítségével** | A be-/kikapcsolás nincs a felhasználó vezérlőn | A felhasználó be-/kikapcsolható a Windows Defender a Windows 10 PC |
| **PC-k védelme a webes fenyegetésekkel szemben a Microsoft Edge böngészőben** | PC védelem a Microsoft Edge-ben | Felhasználó tud megereszt/távoli PC védelem-ban Mikroszkóp él |
| **Az eszköz képernyőjének üresjáratban történő kikapcsolása** | A képernyő időtúllépési házirendjének adminisztrálja | A képernyő időtúllépését a végfelhasználó konfigurálhatja |
| **A felhasználók letölthetnek appokat innen: Microsoft Áruház** | Az adminisztrátor meghatározza, hogy a felhasználó letölthet-e alkalmazásokat a Microsoft Store webhelyéről | Felhasználó tud letölt apps-ból Mikroszkóp készlet bármikor |
| **A felhasználók igénybe vehetik Cortana segítségét** | Az admin a Cortana-hoz való felhasználói hozzáférés politikáját határozza meg | A Cortana ki-/bekapcsolható felhasználói eszközei |
| **A Microsofttól származó tippek és hirdetések fogadásának engedélyezése a felhasználók számára** | Admin határozza meg a házirendet a felhasználó tippeket és hirdetéseket a Microsoft | Felhasználó tud fordít-ra/távoli porkoláb és hirdetés-ból Mikroszkóp |
| **A felhasználók másolhatnak tartalmakat az Office-appokból személyes appokba** | Az admin meghatározza a Windows 10-eszközök naprakészen tartapolitikáját | A felhasználók eldönthetik, hogy mikor frissítsék a Windows rendszert |

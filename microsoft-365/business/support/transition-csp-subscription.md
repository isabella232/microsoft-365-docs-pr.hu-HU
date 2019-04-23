---
title: Az átmenet egy Microsoft 365 üzleti CSP-előfizetés 
description: Megtudhatja, hogyan is átléphet egy Microsoft 365 üzleti CSP előfizetés preview GA 
author: jasongroce
ms.author: jasgro
ms.topic: article 
ms.prod: microsoft-365-business
localization_priority: Normal
audience: microsoft-business 
keywords: Microsoft 365 Business, Microsoft 365, SMB, átmenet CSP-előfizetés
ms.date: 11/01/2017
ms.openlocfilehash: 8109c0b00f06a15c12bbccf89e7f49dc3fa4b34a
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32286244"
---
# <a name="transition-a-microsoft-365-business-csp-subscription"></a>Az átmenet egy Microsoft 365 üzleti CSP-előfizetés

Ha rendelkezünk Microsoft 365 üzleti előnézet kriptográfiai Szolgáltató előfizetés, kövesse az útmutatóban megtudhatja, hogyan is átléphet a meglévő minta-előfizetés Microsoft 365 üzleti GA (általános elérhetőség).

**Hogyan átmenet egy előnézet GA-előfizetés**

1. Jelentkezzen be a <a href="https://partnercenter.microsoft.com" target="_blank">Partner Center</a>.
2. Irányítópultról jelölje ki a **Vevők**, és ezután keressük meg és jelölje ki a vállalat nevét.

    A vállalat az előfizetések jelenik meg.

    ![A Partner Center vevő előfizetések](images/pc_customer_subscriptions_1.png)
    
3. A vállalat **az előfizetések** lapon jelölje be a **Hozzáadás előfizetés**.
4. Az **Új előfizetés** lapon jelölje be a **Small business** , és a listából válassza ki **A Microsoft 365 Business** .
5. Adja hozzá a licencek számát, és válassza a **Tovább: tekintse át a** tekintse át az előfizetés, és válassza a **Küldés**.

    ![Tekintse át az új Microsoft 365 üzleti előfizetés](images/pc_customer_reviewnewsubscription.png)

    A **licenc alapú előfizetések** **Microsoft 365 üzleti kép** és **Microsoft 365 üzleti**jelennek meg. Szüksége lesz az előnézeti előfizetés következő felfüggeszti.

6. Válassza ki a **Microsoft üzleti 365 előnézet**.
7. A **Microsoft 365 üzleti előnézet** lapon jelölje ki a **Suspended** felfüggeszti az előnézet előfizetés.

    ![A Microsoft 365 üzleti előnézet előfizetés felfüggesztése](images/pc_customer_m365bpreview_suspend.png)

8. Jelölje be a **Küldés** megerősítéséhez.

    Az **előfizetések** lapon győződjön meg arról, hogy a **Microsoft 365 üzleti előnézet** állapota **Suspended**.

    ![Erősítse meg a kép előfizetés állapotának fel van függesztve](images/pc_customer_m365bpreview_suspend_confirm.png)

9. Másik lehetőségként is ellenőrizheti a licencszerződést. Ehhez kövesse az alábbi lépéseket:
    1. Jelölje ki a **felhasználók és a licencek** a vállalat **előfizetések** lapról.
    2. A **felhasználók és a licencek** lapon válasszon ki egy felhasználót.
    3. A felhasználó lapon a **licencek hozzárendelése** szakaszban ellenőrizze, és győződjön meg arról, hogy **Microsoft 365 üzleti**mutatja.

        ![Erősítse meg a felhasználóhoz rendelt Microsoft 365 üzleti licenc](images/pc_customer_userslicenses_m365b_validate.png)

## <a name="impact-to-customers-and-users-during-and-after-transition"></a>Ügyfelek és felhasználók alatt és után átmeneti hatás

Nincs nincs hatással az ügyfelek és a felhasználók átmenet és átmenet feladása során.

## <a name="impact-to-customers-who-dont-transition"></a>A felhasználók, akik nem az átmenet hatása

Az alábbi táblázat összefoglalja a felhasználók számára nem Microsoft 365 üzleti előfizetés Microsoft 365 üzleti előnézet előfizetésből átmenet hatása.

|       | T + 30 T-0     | T + 30 T + 60 | T + 60 T + 120 | T + 120 túl  |
|-------|-----------------|--------------|---------------|---------------|
| **Állam** | A türelmi időszak | Lejárt      | Letiltva      | Deprovisioned |
| **Szolgáltatás hatások**                                                        |
| **A Microsoft Business-365 rendszergazdai portál** | Nincs hatással a funkció | Nincs hatással a funkció | Segítségével a felhasználók hozzáadása, törlése, beszerzési előfizetések.</br> Nem hozzárendelése/revoke licenceket. | Vevő előfizetés és minden adat törlődik. Admin más fizetett előfizetések kezelése. |
| **Office-alkalmazások**                         | Nincs végfelhasználói hatása | Nincs végfelhasználói hatása | Office csökkentett szolgáltatáskészletet nyújtó üzemmódba lép.</br> A felhasználók megtekinthetik a fájlokat csak. | Office csökkentett szolgáltatáskészletet nyújtó üzemmódba lép.</br> A felhasználók megtekinthetik a fájlokat csak. |
| **Felhő szolgáltatások (SharePoint Online, Exchange Online, Skype, csoportok, és több)** | Nincs végfelhasználói hatása | Nincs végfelhasználói hatása | A végfelhasználók és a rendszergazdák ne férjenek hozzá adatokat a felhőben. | Vevő előfizetés és minden adat törlődik. |
| **EM + S összetevők** | Nincs admin hatása</br> Nincs végfelhasználói hatása | Nincs admin hatása</br> Nincs végfelhasználói hatása | Képesség megszűnik hajtják végre.</br> További információért lásd a [előfizetés lejártakor hatások mobil eszköz](#mobile-device-impacts-upon-subscription-expiration) és a [Windows 10 PC hatások előfizetés lejártakor](#windows-10-pc-impacts-upon-subscription-expiration) . | Képesség megszűnik hajtják végre.</br> További információért lásd a [előfizetés lejártakor hatások mobil eszköz](#mobile-device-impacts-upon-subscription-expiration) és a [Windows 10 PC hatások előfizetés lejártakor](#windows-10-pc-impacts-upon-subscription-expiration) . |
| **Windows 10 üzleti** | Nincs admin hatása</br> Nincs végfelhasználói hatása | Nincs admin hatása</br> Nincs végfelhasználói hatása | Képesség megszűnik hajtják végre.</br> További információért lásd a [előfizetés lejártakor hatások mobil eszköz](#mobile-device-impacts-upon-subscription-expiration) és a [Windows 10 PC hatások előfizetés lejártakor](#windows-10-pc-impacts-upon-subscription-expiration) . | Képesség megszűnik hajtják végre.</br> További információért lásd a [előfizetés lejártakor hatások mobil eszköz](#mobile-device-impacts-upon-subscription-expiration) és a [Windows 10 PC hatások előfizetés lejártakor](#windows-10-pc-impacts-upon-subscription-expiration) . |
| **10 személyi számítógéphez Windows Azure AD bejelentkezés** | Nincs admin hatása</br> Nincs végfelhasználói hatása | Nincs admin hatása</br> Nincs végfelhasználói hatása | Nincs admin hatása</br> Nincs végfelhasználói hatása | A bérlő a törölt felhasználó csak helyi hitelesítő adatokkal lehet bejelentkezni. Az eszközt újra kép, ha nincs helyi hitelesítő adatokkal. |

## <a name="mobile-device-impacts-upon-subscription-expiration"></a>Mobil eszköz hatások előfizetés lejártakor

A followint táblázat foglalja össze a mobileszközök app adatkezelési házirendeket gyakorolt hatásuk.

|                            | Teljes mértékben licencelt tapasztalat                      | T + 60 nap utáni lejárati          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Munka fájlokat töröl az inaktív eszközök** | Munkafájlok kijelölt nap után törlődnek. | Munka fájlok maradnak a felhasználó személyes eszközök |
| **A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió** | Munkafájlok csak menthetők az üzleti OneDrive | Munkafájlok bárhol lehet menteni |
| **Munkahelyi fájlok titkosítása** | Munka fájlok titkosítottak. | Munka fájlok nem titkosítottak.</br> Biztonsági házirendek törlődik, és az Office alkalmazások adatai törlődik. |
| **Szükséges PIN-kód vagy az ujjlenyomat-Office-alkalmazások eléréséhez** | Korlátozott hozzáférést apps | Nincs alkalmazás szintű hozzáférés-korlátozás |
| **PIN-kód visszaállítása sikertelen bejelentkezés esetén** | Korlátozott hozzáférést apps | Nincs alkalmazás szintű hozzáférés-korlátozás |
| **A felhasználónak újból bejelentkezni után az Office alkalmazások üresjáratban** | -Bejelentkezés szükséges | Nincs bejelentkezés alkalmazások eléréséhez szükséges |
| **Munkahelyi fájlokhoz való hozzáférés letiltása függetlenített vagy feltört eszközökön** | Munkafájlok jailbroken/gyökeres eszköz nem érhető el | Munkafájlok jailbroken/gyökeres eszközökön érhető el |
| **Engedélyezése a felhasználók számára az Office alkalmazások tartalmának másolása személyes apps** | Másolás/beillesztés korlátozott apps elérhető Microsoft 365 üzleti előfizetés részeként | Másolás/beillesztés az összes apps elérhető |

## <a name="windows-10-pc-impacts-upon-subscription-expiration"></a>Előfizetés lejártakor Windows 10 PC hatások

Az alábbi táblázat összefoglalja a Windows 10 eszköz konfigurációs politikák hatása.

|                            | Teljes mértékben licencelt tapasztalat                      | T + 60 nap utáni lejárati          |
|----------------------------|------------------------------------------------|------------------------------------|
| **A Windows Defender használata fenyegetések PC védelme** | Felhasználói vezérlő kívül esik következik be-és kikapcsolása | Felhasználó is kapcsolja be-és kikapcsolása a Windows Defender a Windows 10 PC-n |
| **PC-k védelme a webes fenyegetésekkel szemben a Microsoft Edge böngészőben** | PC védelem a Microsoft Edge | Felhasználó lehet, hogy a/PC védelem kikapcsolása a Microsoft Edge |
| **Kapcsolja ki a kijelzőnek üresjáratban** | Admin képernyőn időtúllépési intervallum házirend határozza meg. | A felhasználó konfigurálhatja képernyő időkorlát |
| **A felhasználók letölthetnek appokat innen: Microsoft Áruház** | Admin határozza meg, hogy a felhasználó apps letölthető Microsoft Store | Felhasználó letölthető alkalmazások Microsoft Store bármikor |
| **A felhasználók igénybe vehetik Cortana segítségét** | Felügyeleti házirend határozza meg, Cortana felhasználói hozzáférés | Felhasználói eszközök be- és kikapcsolás Cortana |
| **Felhasználók tippek és hirdetéseket kapni a Microsofttól** | Felügyeleti házirend határozza meg, felhasználói tippek és hirdetéseket kapni a Microsofttól | Felhasználó kikapcsolhatja a/tippek és hirdetések a Microsofttól |
| **A felhasználók másolhatnak tartalmakat az Office-appokból személyes appokba** | Felügyeleti eszközök Windows 10 naprakészen házirend definiálása | A felhasználók dönthetjük el, mikor a Windows frissítése |





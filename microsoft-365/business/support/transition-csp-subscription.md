---
title: Áttérés a Microsoft 365 Vállalati verziós felhőszolgáltatói előfizetésre
description: Ismerje meg, hogyan lehet áttűnni a Microsoft 365 Vállalati verzió felhőszolgáltatói előfizetését az előzetes verzióról az általános elérhetőségre.
author: jasongroce
f1.keywords:
- NOCSH
ms.custom:
- seo-marvel-mar
- AdminSurgePortfolio
ms.author: jasgro
ms.topic: article 
ms.prod: microsoft-365-business
localization_priority: Normal
audience: microsoft-business 
keywords: Microsoft 365 Vállalati verzió, Microsoft 365, SMB, áttérés felhőszolgáltatói előfizetés
ms.date: 11/01/2017
ms.openlocfilehash: 5fc532b4a59d8e94068e7e1bae99bf8edac75abb
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403430"
---
# <a name="transition-a-microsoft-365-business-csp-subscription"></a>Áttérés a Microsoft 365 Vállalati verziós felhőszolgáltatói előfizetésre

Ha Microsoft 365 Vállalati előzetes verziós felhőszolgáltatói előfizetéssel rendelkezik, az alábbi útmutatóból kiderítheti, hogy miként áttűnhet a meglévő előzetes verziós előfizetése a Microsoft 365 Vállalati verzióra (általános elérhetőség).

**Az előzetes verziós előfizetések átváltása a Ga szolgáltatásra**

1. Jelentkezzen be a <a href="https://partnercenter.microsoft.com" target="_blank">Partnerközpontba.</a>
2. Az irányítópulton válassza a **Vevők** lehetőséget, majd keresse meg és jelölje ki a cég nevét.

    A vállalat előfizetései fel lesznek sorolva.

    ![Ügyfél előfizetései a Partnerközpontban](../../media/pc_customer_subscriptions_1.png)
    
3. A vállalat Előfizetések **lapján** válassza az **Előfizetés hozzáadása lehetőséget.**
4. Az Új **előfizetés lapon** válassza a **Kisvállalati** verzió lehetőséget, majd a listában válassza a **Microsoft 365 Vállalati** verzió lehetőséget.
5. Adja meg a licencek számát, majd válassza a **Tovább: Tekintse** át az előfizetés áttekintéséhez, majd válassza a **Küldés gombot.**

    ![A Microsoft 365 Vállalati verzió új előfizetésének áttekintése](../../media/pc_customer_reviewnewsubscription.png)

    A **licencalapú előfizetések között** megjelenik a **Microsoft 365 Vállalati előzetes verzió és** a Microsoft **365 Vállalati verzió.** Ezután felfüggeszti az előzetes verziós előfizetést.

6. Válassza a **Microsoft 365 Vállalati előzetes verzió lehetőséget.**
7. A **Microsoft 365 Vállalati** verzió előzetes verzió lapján válassza a **Felfüggesztve** lehetőséget az előzetes verziós előfizetés felfüggesztéséhez.

    ![A Microsoft 365 Vállalati előzetes verzió előfizetésének felfüggesztése](../../media/pc_customer_m365bpreview_suspend.png)

8. A **megerősítéshez válassza** a Küldés gombot.

    Az **Előfizetések lapon** győződjön meg arról, hogy a **Microsoft 365 Vállalati** verzió előzetes verziójának állapota Fel van **függesztve.**

    ![Az előzetes verziós előfizetés állapotának ellenőrzése](../../media/pc_customer_m365bpreview_suspend_confirm.png)

9. Szükség esetén a licencszerződést is érvényesítheti. Ehhez hajtsa végre a következő lépéseket:
    1. Válassza **a Felhasználók és licencek** lehetőséget a vállalat **Előfizetések lapján.**
    2. A Felhasználók **és licencek lapon** jelöljön ki egy felhasználót.
    3. A felhasználó lapján ellenőrizze a  Licencek hozzárendelése szakaszt, és győződjön meg arról, hogy a **Microsoft 365 Vállalati** verzió látható rajta.

        ![Erősítse meg, hogy a Microsoft 365 Vállalati verzió licence hozzá van rendelve a felhasználóhoz](../../media/pc_customer_userslicenses_m365b_validate.png)

## <a name="impact-to-customers-and-users-during-and-after-transition"></a>Az áttérés során és után az ügyfelekre és a felhasználókra gyakorolt hatás

Az áttérés és a utáni áttűnés során nincs hatással az ügyfelekre és a felhasználókra.

## <a name="impact-to-customers-who-dont-transition"></a>Hatás az áttűnésen nem áttűnő ügyfelekre

Az alábbi táblázat összefoglalja azokat az ügyfeleket, akik nem lépnek át Microsoft 365 Vállalati előzetes verziós előfizetésről Microsoft 365 Vállalati verziós előfizetésre.

|       | T-0 –T+30     | T+30 – T+60 | T+60 – T+120 | A T+120-nál több  |
|-------|-----------------|--------------|---------------|---------------|
| **Állam** | Türelmi időszakban | Lejárt      | Letiltva      | Leépítve |
| **A szolgáltatás hatásai**                                                        |
| **A Microsoft 365 Vállalati verzió felügyeleti portálja** | Nincs hatással a működésre | Nincs hatással a működésre | Felvehet és törölhet felhasználókat, előfizetéseket vásárolhat.</br> Nem lehet licenceket hozzárendelni vagy visszavonni. | Az ügyfél előfizetése és az összes adat törlődik. A rendszergazda más fizetős előfizetéseket is kezelhet. |
| **Office-appok**                         | Nincs hatással a végfelhasználókra | Nincs hatással a végfelhasználókra | Az Office csökkentett szolgáltatáskészletű üzemmódba vált.</br> A felhasználók csak a fájlokat megtekinthetik. | Az Office csökkentett szolgáltatáskészletű üzemmódba vált.</br> A felhasználók csak a fájlokat megtekinthetik. |
| **Felhőszolgáltatások (SharePoint Online, Exchange Online, Skype, Teams és egyéb szolgáltatások)** | Nincs hatással a végfelhasználókra | Nincs hatással a végfelhasználókra | A végfelhasználók és a rendszergazdák nem férnek hozzá a felhőbeli adatokhoz. | Az ügyfél előfizetése és minden adata törlődik. |
| **EM+S összetevők** | Nincs hatással a rendszergazdákra</br> Nincs hatással a végfelhasználókra | Nincs hatása a rendszergazdának</br> Nincs hatással a végfelhasználókra | A funkció már nincs kényszerítve.</br> További [információért tekintse](#mobile-device-impacts-upon-subscription-expiration) meg, hogy a mobileszköz milyen hatással van az előfizetés lejáratára, illetve a [Windows 10-es PC-re](#windows-10-pc-impacts-upon-subscription-expiration) az előfizetés lejártakor. | A funkció már nincs kényszerítve.</br> További [információért tekintse](#mobile-device-impacts-upon-subscription-expiration) meg, hogy a mobileszköz milyen hatással van az előfizetés lejáratára, illetve a [Windows 10-es PC-re](#windows-10-pc-impacts-upon-subscription-expiration) az előfizetés lejártakor. |
| **Windows 10 Business** | Nincs hatással a rendszergazdákra</br> Nincs hatással a végfelhasználókra | Nincs hatással a rendszergazdákra</br> Nincs hatással a végfelhasználókra | A funkció már nincs kényszerítve.</br> További [információért tekintse](#mobile-device-impacts-upon-subscription-expiration) meg, hogy a mobileszköz milyen hatással van az előfizetés lejáratára, illetve a [Windows 10-es PC-re](#windows-10-pc-impacts-upon-subscription-expiration) az előfizetés lejártakor. | A funkció már nincs kényszerítve.</br> További [információért tekintse](#mobile-device-impacts-upon-subscription-expiration) meg, hogy a mobileszköz milyen hatással van az előfizetés lejáratára, illetve a [Windows 10-es PC-re](#windows-10-pc-impacts-upon-subscription-expiration) az előfizetés lejártakor. |
| **Azure AD-bejelentkezés Windows 10-es PC-re** | Nincs hatással a rendszergazdákra</br> Nincs hatással a végfelhasználókra | Nincs hatással a rendszergazdákra</br> Nincs hatással a végfelhasználókra | Nincs hatással a rendszergazdákra</br> Nincs hatással a végfelhasználókra | A bérlő törlése után a felhasználók csak helyi hitelesítő adatokkal tudnak bejelentkezni. Ha nincsenek helyi hitelesítő adatok, akkor képpel tegye újra az eszközt. |

## <a name="mobile-device-impacts-upon-subscription-expiration"></a>Az előfizetés lejáratakor a mobileszközre gyakorolt hatás

Az alábbi táblázat összefoglalja, hogy milyen hatása van az appkezelési házirendek mobileszközön való használatának.

|                            | Teljesen licencelt élmény                      | T+60 nap a lejárat után          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Munkahelyi fájlok törlése inaktív eszközről** | A munkafájlok a kijelölt napok után törlődnek | A munkahelyi fájlok a felhasználó személyes eszközein maradnak |
| **A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió** | A munkahelyi fájlok csak a OneDrive Vállalati verzióba menthetők | A munkahelyi fájlok bárhová menthetők |
| **Munkahelyi fájlok titkosítása** | A munkahelyi fájlok titkosítva vannak | A munkahelyi fájlokat a továbbiakban nem titkosítja a rendszer.</br> A rendszer eltávolítja a biztonsági házirendeket, az Office-adatokat pedig az appokban. |
| **PIN-kód vagy ujjlenyomat megkövetelve az Office-appok eléréséhez** | Alkalmazásokhoz való korlátozott hozzáférés | Nincs appszintű hozzáférési korlátozás |
| **A PIN-kód alaphelyzetbe állítása sikertelen bejelentkezéskor** | Alkalmazásokhoz való korlátozott hozzáférés | Nincs appszintű hozzáférési korlátozás |
| **A felhasználók újra be kell jelentkezniük, miután az Office-appok inaktívak voltak** | Bejelentkezés szükséges | Nincs szükség bejelentkezésre |
| **Munkahelyi fájlokhoz való hozzáférés letiltása függetlenített vagy feltört eszközökön** | A munkahelyi fájlok nem érhetők el feltört/rootolt eszközökön | A munkahelyi fájlok feltört/rootolt eszközökön is elérhetők |
| **Tartalom másolásának engedélyezése a felhasználóknak az Office-appok személyes appokba** | A Microsoft 365-előfizetés részeként elérhető alkalmazásokra korlátozott másolás/beillesztés | A másolás/beillesztés minden alkalmazás számára elérhető |

## <a name="windows-10-pc-impacts-upon-subscription-expiration"></a>A Windows 10-es PC hatással van az előfizetés lejáratára

Az alábbi táblázat összefoglalja a Windows 10-es eszközkonfigurációs házirendek hatását.

|                            | Teljesen licencelt élmény                      | T+60 nap a lejárat után          |
|----------------------------|------------------------------------------------|------------------------------------|
| **PC-k védelme a fenyegetésekkel szemben a Windows Defender használatával** | A be- és kikapcsolása nem felhasználói vezérlőelem | A felhasználó be- és kikapcsolhatja a Windows Defendert a Windows 10-es PC-n |
| **PC-k védelme a webes fenyegetésekkel szemben a Microsoft Edge böngészőben** | PC-védelem a Microsoft Edge-ben | A felhasználó be- és kikapcsolhatja a PC védelmét a Microsoft Edge-ben |
| **Az eszköz képernyőjének kikapcsolása inaktív üzemmódban** | A rendszergazda időkorlát-időkorlát-házirendet ad meg a képernyőn | A képernyő-időkorlátot a végfelhasználó konfigurálhatja |
| **A felhasználók letölthetnek appokat innen: Microsoft Áruház** | A rendszergazda azt határozza meg, hogy egy felhasználó letölthet-e alkalmazásokat a Microsoft Store-ból | A felhasználó bármikor letölthet alkalmazásokat a Microsoft Store-ból |
| **A felhasználók igénybe vehetik Cortana segítségét** | A rendszergazda házirendet határoz meg a Cortanához való felhasználói hozzáférésről | Felhasználói eszközök Cortana be- és kikapcsolt használatához |
| **Tippek és hirdetések fogadásának engedélyezése a Felhasználóknak a Microsofttól** | A rendszergazda házirendet határoz meg a Microsofttól kapott felhasználói tippekre és hirdetésekre | A felhasználó be- és kikapcsolhatja a Microsofttól származó tippeket és hirdetéseket |
| **A felhasználók másolhatnak tartalmakat az Office-appokból személyes appokba** | A rendszergazda olyan házirendet határoz meg, amely naprakészen tartja a Windows 10-es eszközöket | A felhasználók dönthetik el, hogy mikor frissítsék a Windowst |

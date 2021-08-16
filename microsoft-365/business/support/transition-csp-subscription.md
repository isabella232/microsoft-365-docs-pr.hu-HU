---
title: Áttérés vállalati Microsoft 365-előfizetésre
description: Ismerje meg, hogy miként áttűnhet az Microsoft 365 Vállalati verziós csp-előfizetés előzetes verzióról általános elérhetőségre.
author: jasongroce
f1.keywords:
- NOCSH
ms.custom:
- seo-marvel-mar
- AdminSurgePortfolio
ms.author: jasongroce
ms.topic: article
manager: jasonh
ms.prod: microsoft-365-business
localization_priority: Normal
audience: microsoft-business
keywords: Microsoft 365 Vállalati, Microsoft 365, SMB, áttérés a csp-előfizetésre
ms.date: 11/01/2017
ms.openlocfilehash: c35cb3b78c4fe2cebc8308b34ceef3decd346b3db298ce5fb56abc8cf205e69d
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53867123"
---
# <a name="transition-a-microsoft-365-business-csp-subscription"></a>Áttérés vállalati Microsoft 365-előfizetésre

Ha rendelkezik Microsoft 365 Vállalati előzetes verziós csp-előfizetéssel, ebből az útmutatóból azt tudhatja meg, hogy miként áttűnés meglévő előzetes előfizetését a Microsoft 365 Business GA szolgáltatásra (általános elérhetőség).

**Előnézeti előfizetések átváltása az ga.ga szolgáltatásra**

1. Jelentkezzen be a <a href="https://partnercenter.microsoft.com" target="_blank">Partnerközpontba.</a>
2. Az irányítópulton válassza **az** Ügyfelek lehetőséget, majd keresse meg és válassza ki a vállalat nevét.

    A vállalat előfizetései fel lesznek sorolva.

    ![Az ügyfél előfizetései a Partnerközpontban](../../media/pc_customer_subscriptions_1.png)
    
3. A vállalat Előfizetések **lapján** válassza az **Előfizetés hozzáadása lehetőséget.**
4. Az Új **előfizetés lapon** válassza a **Kisvállalati** verzió lehetőséget, majd Microsoft 365 **a** listában a Vállalati verzió lehetőséget.
5. Adja meg a licencek számát, majd válassza a **Tovább: Áttekintés lehetőséget** az előfizetés áttekintéséhez, majd válassza a Küldés **lehetőséget.**

    ![A Vállalati verzió új előfizetésének Microsoft 365 áttekintése](../../media/pc_customer_reviewnewsubscription.png)

    A **Licencalapú előfizetések között** megjelenik a **Microsoft 365 Business Preview** és a **Microsoft 365 neve.** Ezután felfüggeszti az előzetes verziós előfizetést.

6. Válassza **Microsoft 365 üzleti előzetes verzió lehetőséget.**
7. A Microsoft 365 **Előzetes verzió lapon a** Felfüggesztve lehetőséget választva függesztheti fel az előzetes verziós előfizetést. 

    ![A Microsoft 365 Előzetes verzió előfizetésének felfüggesztése](../../media/pc_customer_m365bpreview_suspend.png)

8. A **megerősítéshez válassza** a Küldés gombot.

    Az **Előfizetések lapon győződjön** meg arról, hogy a **Microsoft 365 Üzleti előzetes verzió** állapota Fel van **függesztve.**

    ![Az előfizetés előnézeti állapotának ellenőrzése](../../media/pc_customer_m365bpreview_suspend_confirm.png)

9. Szükség esetén ellenőrizheti a licencszerződést is. Ehhez hajtsa végre a következő lépéseket:
    1. Válassza **a Felhasználók és licencek** lehetőséget a vállalat **Előfizetések lapján.**
    2. A Felhasználók **és licencek lapon** jelöljön ki egy felhasználót.
    3. A felhasználó lapján jelölje be  a Licencek hozzárendelése szakaszt, és győződjön meg arról, hogy a "Licencek hozzárendelése Microsoft 365 **megjelenik.**

        ![Erősítse meg Microsoft 365 hogy a Microsoft 365 Vállalati verzió licenc hozzá van rendelve a felhasználóhoz](../../media/pc_customer_userslicenses_m365b_validate.png)

## <a name="impact-to-customers-and-users-during-and-after-transition"></a>Hatás az ügyfelekre és a felhasználókra az áttérés során és után

Az áttérés és az azt követő felhasználók számára nincsenek hatással a felhasználók és az ügyfelek.

## <a name="impact-to-customers-who-dont-transition"></a>Hatás az áttűnésen nem áttűnő ügyfelekre

Az alábbi táblázat összefoglalja, hogy milyen hatása van az olyan ügyfeleinknek, akik nem áttérésre Microsoft 365 Vállalati előzetes verziós előfizetésről vállalati Microsoft 365 előfizetésre.

|       | T-0 – T+30     | T+30 – T+60 | T+60 – T+120 | A T+120-on túl  |
|-------|-----------------|--------------|---------------|---------------|
| **State (Állam)** | Türelmi időszakban | Lejárt      | Letiltva      | Leépítve |
| **A szolgáltatás hatásai**                                                        |
| **Microsoft 365 Felügyeleti központ** | Nincs hatással a működésre | Nincs hatással a működésre | Felvehet vagy törölhet felhasználókat, előfizetéseket vásárolhat.</br> Nem rendelhet hozzá és nem vonhat vissza licenceket. | Az ügyfél előfizetése és minden adata törlődik. A rendszergazda más fizetős előfizetéseket is kezelhet. |
| **Office alkalmazások**                         | Nincs hatással a végfelhasználókra | Nincs hatással a végfelhasználókra | Office csökkentett szolgáltatáskészletű üzemmódba lép.</br> A felhasználók csak megtekinthetik a fájlokat. | Office csökkentett szolgáltatáskészletű üzemmódba lép.</br> A felhasználók csak megtekinthetik a fájlokat. |
| **Felhőszolgáltatások (SharePoint Online, Exchange Online, Skype, Teams és sok más)** | Nincs hatással a végfelhasználókra | Nincs hatással a végfelhasználókra | A végfelhasználók és a rendszergazdák nem férnek hozzá a felhőbeli adatokhoz. | Az ügyfél előfizetése és minden adata törlődik. |
| **EM+S-összetevők** | Nincs hatása a rendszergazdáknak</br> Nincs hatással a végfelhasználókra | Nincs hatása a rendszergazdáknak</br> Nincs hatással a végfelhasználókra | A képesség már nincs kényszerítve.</br> További információért lásd: A mobileszköz milyen hatással van az előfizetés [lejártakor,](#mobile-device-impacts-upon-subscription-expiration) Windows 10 pc milyen hatással van [az előfizetés lejártakor.](#windows-10-pc-impacts-upon-subscription-expiration) | A képesség már nincs kényszerítve.</br> További információért lásd: A mobileszköz milyen hatással van az előfizetés [lejártakor,](#mobile-device-impacts-upon-subscription-expiration) Windows 10 pc milyen hatással van [az előfizetés lejártakor.](#windows-10-pc-impacts-upon-subscription-expiration) |
| **Windows 10 Business** | Nincs hatása a rendszergazdáknak</br> Nincs hatással a végfelhasználókra | Nincs hatása a rendszergazdáknak</br> Nincs hatással a végfelhasználókra | A képesség már nincs kényszerítve.</br> További információért lásd: A mobileszköz milyen hatással van az előfizetés [lejártakor,](#mobile-device-impacts-upon-subscription-expiration) Windows 10 pc milyen hatással van [az előfizetés lejártakor.](#windows-10-pc-impacts-upon-subscription-expiration) | A képesség már nincs kényszerítve.</br> További információért lásd: A mobileszköz milyen hatással van az előfizetés [lejártakor,](#mobile-device-impacts-upon-subscription-expiration) Windows 10 pc milyen hatással van [az előfizetés lejártakor.](#windows-10-pc-impacts-upon-subscription-expiration) |
| **Azure AD-bejelentkezés egy Windows 10 pc-re** | Nincs hatása a rendszergazdáknak</br> Nincs hatással a végfelhasználókra | Nincs hatása a rendszergazdáknak</br> Nincs hatással a végfelhasználókra | Nincs hatása a rendszergazdáknak</br> Nincs hatással a végfelhasználókra | A bérlő törlése után a felhasználók csak helyi hitelesítő adatokkal tudnak bejelentkezni. Ha nincsenek helyi hitelesítő adatok, lemezképet az eszközről. |

## <a name="mobile-device-impacts-upon-subscription-expiration"></a>A mobileszköz hatással van az előfizetés lejáratakor

Az alábbi táblázat összefoglalja, hogy milyen hatása van az appkezelési házirendek mobileszközön való használatának.

|                            | Teljes licencelt élmény                      | T+60 nap lejárat után          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Munkahelyi fájlok törlése inaktív eszközről** | A munkahelyi fájlok a kijelölt napok után törlődnek | A munkahelyi fájlok a felhasználó személyes eszközein maradnak |
| **A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió** | A munkahelyi fájlok csak a OneDrive Vállalati verzió | A munkahelyi fájlok bárhová menthetők |
| **Munkahelyi fájlok titkosítása** | A munkahelyi fájlok titkosítva vannak | A munkahelyi fájlok a továbbiakban nem titkosítottak.</br> A rendszer eltávolítja a biztonsági házirendeket, Office az appokban használt adatokat. |
| **PIN-kód vagy ujjlenyomat megkövetelve az Office eléréséhez** | Alkalmazások korlátozott elérése | Nincs alkalmazásszintű hozzáférési korlátozás |
| **PIN-kód alaphelyzetbe állítása sikertelen bejelentkezés esetén** | Alkalmazások korlátozott elérése | Nincs alkalmazásszintű hozzáférési korlátozás |
| **A felhasználók újra be kell jelentkezniük, miután Office alkalmazások inaktívak voltak** | Bejelentkezés szükséges | Nincs szükség bejelentkezésre |
| **Munkahelyi fájlokhoz való hozzáférés letiltása függetlenített vagy feltört eszközökön** | A munkahelyi fájlok nem érhetők el a feltört/rootolt eszközökön | A munkahelyi fájlok a feltört/rootolt eszközökön érhetők el |
| **Tartalom másolásának engedélyezése a felhasználók Office alkalmazásokból a személyes alkalmazásokba** | Az előfizetés részeként elérhető alkalmazásokra korlátozott másolási/beillesztési Microsoft 365 | Minden alkalmazás számára elérhető másolás/beillesztés |

## <a name="windows-10-pc-impacts-upon-subscription-expiration"></a>Windows 10 A PC hatással van az előfizetés lejáratakor

Az alábbi táblázat összefoglalja az eszközkonfigurációs házirendek Windows 10 hatását.

|                            | Teljes licencelt élmény                      | T+60 nap lejárat után          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Számítógépek védelme a számítógépekkel szembeni Windows Defender** | A ki- és bekapcsolás nem része a felhasználói vezérlőelemnek | A felhasználó be- és kikapcsolhatja a Windows Defender a Windows 10 PC-n |
| **PC-k védelme a webes fenyegetésekkel szemben a Microsoft Edge böngészőben** | PC-védelem a Microsoft Edge | A felhasználó be- és kikapcsolhatja a PC védelmét a Microsoft Edge |
| **Az eszköz képernyőjének kikapcsolása inaktív állapotban** | A rendszergazda meghatároz egy időkorlát-időkorlát-házirendet | A használati időkorlátot a végfelhasználó konfigurálhatja |
| **A felhasználók letölthetnek appokat innen: Microsoft Áruház** | A rendszergazda azt határozza meg, hogy a felhasználó letölthet-e alkalmazásokat a Microsoft Store | A felhasználó bármikor letölthet alkalmazásokat a Microsoft Store-ból |
| **A felhasználók igénybe vehetik Cortana segítségét** | A rendszergazda házirendet határoz meg a felhasználók hozzáférését Cortana | Felhasználói eszközök a fiók be- és Cortana |
| **Tippek és hirdetések fogadásának engedélyezése a Microsofttól** | A rendszergazda házirendet határoz meg a Microsofttól kapott tippekre és hirdetésekre vonatkozó felhasználói tippekre és hirdetésekre | A felhasználó be- és kikapcsolhatja a Microsoft által közzétett tippeket és hirdetéseket |
| **A felhasználók másolhatnak tartalmakat az Office-appokból személyes appokba** | A rendszergazda házirendet ad Windows 10 eszköz naprakészentartásához | A felhasználók dönthetik el, hogy mikor frissítsék a Windows |

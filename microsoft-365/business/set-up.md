---
title: A Microsoft 365 Business beállítása
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- TRN_SMB
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Útmutató a Microsoft 365 Business beállításához.
ms.openlocfilehash: 7ab6ae095ae30f8ceb74be69fcee20f31977ae21
ms.sourcegitcommit: 8fda7852b2a5baa92b8a365865b014ea6d100bbc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/03/2019
ms.locfileid: "39818917"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>A Microsoft 365 Business beállítása a telepítővarázslóban

Tekintse meg a Microsoft 365 Business beállítását ismertető videót.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Ha Ön alapít ez video segíteni kész, kijelenti magát a [kiegészít képzés sor részére kicsi teendő és azok új-hoz mikroszkóp 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

## <a name="add-your-domain-users-and-set-up-policies"></a>A tartomány, a felhasználók és a házirendek beállítása

[![A megjelenő címke figyelmeztet a felügyeleti központ változásaira, további részleteket itt talál: aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Amikor vagy megvásárol Mikroszkóp 365 teendő, Önnek van a választás-ból használ egy birtok Ön saját, vagy buying egy közben a [jel-megjelöl](sign-up.md).

- Ha a feliratkozáskor új tartományt vásárolt, akkor a tartománya be van állítva, és segítségével [felhasználókat vehet fel és licenceket rendelhet](#add-users-and-assign-licenses)hozzá.

### <a name="add-your-domain-to-personalize-sign-in"></a>Saját tartomány felvétele a bejelentkezés személyre szabásához

1. Jelentkezzen be a [Microsoft 365 felügyeleti központba](https://admin.microsoft.com) a globális rendszergazdai hitelesítő adatok használatával. 

2. A varázsló elindításához válassza a **mehet beállítást** .

    ![Válassza az Ugrás a telepítéshez beállítást.](media/gotosetupinadmincenter.png)

3. Az **Office alkalmazások telepítése** lapon tetszés szerint telepítheti az alkalmazásokat a saját számítógépére.
    
4. A **tartomány hozzáadása** lépésben adja meg a használni kívánt tartománynevet (például contoso.com).

    > [!IMPORTANT]
    > Ha a regisztráció során tartományt vásárolt, akkor itt nem jelenik meg **a domainlépés hozzáadása** . Tovább a [felhasználók hozzáadásához](#add-users-and-assign-licenses) helyette.

    ![Ernyőz-ból megszemélyesít-a jel--ban oldal.](media/adddomain.png)

    
4. A varázsló lépéseit követve [hozzon létre DNS-rekordokat az Office 365 olyan DNS-](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) szolgáltatójánál, amely igazolja, hogy Ön a tartomány tulajdonosa. Ha ismeri a domainnevét, akkor tekintse meg a [gazdagép utasításait](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)is.

    Ha a tárhely szolgáltató GoDaddy vagy más Host engedélyezve [domain Connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), a folyamat egyszerű, és akkor automatikusan felkérték, hogy jelentkezzen be, és hagyja, hogy a Microsoft hitelesít az Ön nevében.

    ![-Ra GoDaddy igazol belépés oldal, kiválaszt engedélyez.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Felhasználók felvétele és licencek hozzárendelése

Felhasználókat felvehet a varázslóba, de később az admin központban is [hozzáadhat felhasználókat](add-users-m365b.md) . Ezenkívül, ha van helyi tartományvezérlője, hozzáadhat felhasználókat a [Azure ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)segítségével.

#### <a name="add-users-in-the-wizard"></a>Felhasználók hozzáadása a varázslóhoz

A varázslóban hozzáadott felhasználók automatikusan Microsoft 365 üzleti licencet kapnak.

![Az új felhasználók hozzáadása lap képernyőképe a varázslóban](media/addnewuserspage.png)

1. Ha a Microsoft 365 üzleti előfizetés már meglévő felhasználókkal rendelkezik (például, ha a Azure AD Connect szolgáltatást használta), akkor most lehetősége van licencek kiosztésére. Nyugodtan felvehet licenceket hozzájuk is.

2. A felhasználók hozzáadása után lehetőség van a hitelesítő adatok megosztására is az új felhasználókkal. Ezeket kinyomtathatja, elküldheti e-mailben, vagy pedig letöltheti.

### <a name="connect-your-domain"></a>Tartomány csatlakoztatása

> [!NOTE]
> Ha az. onmicrosoft tartomány használata mellett döntött, vagy a felhasználók beállításához a Azure AD Connect szolgáltatást használja, akkor ezt a lépést nem fogja látni.
  
A szolgáltatások beállításához frissítenie kell bizonyos rekordokat a DNS-szolgáltatónál vagy a tartományregisztrálónál.
  
1. A beállítási varázsló általában felismeri a regisztrálóját, és részletes útmutatást jelenít meg arról, hogy miként frissítheti a névkiszolgálói rekordokat a regisztráló webhelyén. Ha nem, [módosítsa a névszervereket az Office 365 beállításához bármely tartományregisztrálóval](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Ha vannak meglévő DNS-rekordjai, például egy meglévő webhely, de a DNS-állomás a tartományhoz történő [kapcsolódáshoz](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)engedélyezve van, válassza **a saját rekord hozzáadása**lehetőséget. Az **online szolgáltatások kiválasztása** lapon fogadja el az összes alapértelmezett beállításokat, majd kattintson a **Tovább gombra**, és válassza az engedélyezés a DNS-állomás oldalán **engedélyt** .
    - Ha van meglévő DNS-rekordja más DNS-állomásokkal (nincs engedélyezve a tartomány csatlakoztatásához), saját DNS-rekordokat kell kezelnie annak érdekében, hogy a meglévő szolgáltatások ne maradjanak kapcsolatban. További információ a [tartomány alapjai](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) című témakörben található.

        ![A rekordok oldal aktiválása.](media/activaterecords.png)

2. Kövesse a varázsló lépéseit, és az e-mail és egyéb szolgáltatások lesznek beállítva az Ön számára.

### <a name="protect-your-organization"></a>A szervezet védelme 

A varázslóban beállított házirendek automatikusan alkalmazásra kerülnek a *minden felhasználó*nevű [biztonsági csoportra](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) . További csoportokat is létrehozhat, ha házirendeket rendel az admin Centerhez.

1. A **növekedés elleni védelem a fejlett számítógépes fenyegetések**, ajánlott, hogy fogadja el az alapértelmezett, hogy hagyja [Office 365 Advance fenyegetés védelem](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) Scan fájlokat és linkeket az Office alkalmazásokban.

    ![Ernyőz-ból növekszik védelem oldal.](media/increasetreatprotection.png)


2. -On **megakadályoz átereszt-ból érzékeny adat** oldal, elfogad a hiba-hoz megereszt Hivatal 365 adat elvesztés megakadályozás (DLP)-hoz nyom érzékeny adat-ban Hivatal apps és megakadályoz a esetleges cserépdarab-ból ezek külső rész-a szervezet.

3. Az **Office mobileszközre szánt adatok védelme** lapon hagyja meg a mobilalkalmazás-kezelés beállítást, bontsa ki a beállításokat, és tekintse át őket, majd válassza a **mobilalkalmazás-kezelési házirend létrehozása**beállítást.

    ![Ernyőz-ból megvéd adat-ban hivatal részére mozgatható oldal.](media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Biztonságos Windows 10 PC-k

-On bal NAV, kiválaszt **beállít** aztán, alatt **énekel--ban és biztonság**, választ **biztosít-a Windows 10 számítógépek**. A **megtekintéshez** válassza a nézet-t. A [Windows 10 rendszerű számítógép biztonságossá tétele](secure-win-10-pcs.md) teljes körű utasításokért lásd:

## <a name="deploy-office-365-client-apps"></a>Az Office 365 ügyfélalkalmazások telepítése

Ha úgy dönt, hogy telepítéskor automatikusan telepíti az Office-alkalmazásokat, az alkalmazások a Windows 10 eszközökre fognak telepíteni, amint a felhasználók a Azure AD rendszerbe be vannak jelentkezve a saját felhasználói hitelesítő adataik segítségével.

Az Office mobil iOS vagy Android eszközökre történő telepítéséhez tekintse meg [a mobileszközök beállítása a Microsoft 365 üzleti felhasználók számára](set-up-mobile-devices.md)című témakört.

Az Office programot egyenként is telepíthetjük. Útmutatás: az [Office telepítése PC vagy Mac számítógépre](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) .

## <a name="see-also"></a>See also

[Microsoft 365 üzleti képzési videók](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)

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
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Útmutató a Microsoft 365 Business beállításához.
ms.openlocfilehash: dbd2e740c85f52d3f43e6cd3d6ce45c478a9b1a9
ms.sourcegitcommit: 7690c8bfdea6e6d245cfa7c5b09b913b092cde0a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/23/2019
ms.locfileid: "37121318"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>A Microsoft 365 Business beállítása a telepítővarázslóban

## <a name="add-your-domain-users-and-set-up-policies"></a>A tartomány, a felhasználók és a házirendek beállítása

[![Label, hogy tudd, az admin központ változik, és találsz további részleteket a aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Amikor vagy megvásárol Mikroszkóp 365 teendő, Önnek van a választás-ból használ egy birtok Ön saját, vagy buying egy közben a [jel-megjelöl](sign-up.md).

- Ha a feliratkozáskor új tartományt vásárolt, akkor a tartománya be van állítva, és segítségével [felhasználókat vehet fel és licenceket rendelhet](#add-users-and-assign-licenses)hozzá.

### <a name="add-your-domain-to-personalize-sign-in"></a>Saját tartomány felvétele a bejelentkezés személyre szabásához

1. Jelentkezzen be a [Microsoft 365 felügyeleti központba](https://admin.microsoft.com) a globális rendszergazdai hitelesítő adatok használatával. 

2. Válassza a **tartomány hozzáadása** vagy a **felhasználók hozzáadása** a varázsló elindításához.
    > [!IMPORTANT]
    > Ha a regisztráció során tartományt vásárolt, akkor itt nem jelenik meg **a domainlépés hozzáadása** . Tovább a [felhasználók hozzáadásához](#add-users-and-assign-licenses) helyette.

    ![Válassza a tartomány hozzáadása-t.](media/addadomainadmincenter.png)
    
3. A varázslóban adja meg a használni kívánt tartománynevet (például contoso.com).


    ![Ernyőz-ból megszemélyesít-a jel--ban oldal.](media/personalizesignin.png)

    
4. A varázsló lépéseit követve [hozzon létre DNS-rekordokat az Office 365 olyan DNS-](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) szolgáltatójánál, amely igazolja, hogy Ön a tartomány tulajdonosa. Ha ismeri a domainnevét, akkor tekintse meg a [gazdagép utasításait](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)is.

    Ha-a ellenséges eltartó van GoDaddy, vagy másik házigazda lehetővé tett-val [birtok összeköt](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), a folyamat van könnyű és lesz lenni keresztül keresztül-hoz jel-ban és enged Mikroszkóp hitelesít-ra-a nevében:

    ![-Ra GoDaddy igazol belépés oldal, kiválaszt engedélyez.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Felhasználók felvétele és licencek hozzárendelése

Felhasználókat felvehet a varázslóba, de később az admin központban is [hozzáadhat felhasználókat](add-users-m365b.md) . Ezenkívül, ha van helyi tartományvezérlője, hozzáadhat felhasználókat a [Azure ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)segítségével.

#### <a name="add-users-in-the-wizard"></a>Felhasználók hozzáadása a varázslóhoz

A varázslóban hozzáadott felhasználók automatikusan Microsoft 365 üzleti licencet kapnak.

![Az új felhasználók hozzáadása lap képernyőképe a varázslóban](media/addnewuserspage.png)

1. Ha a Microsoft 365 üzleti előfizetés már meglévő felhasználókkal rendelkezik (például, ha a Azure AD Connect szolgáltatást használta), akkor most lehetősége van licencek kiosztésére. Nyugodtan felvehet licenceket hozzájuk is.

3. A felhasználók hozzáadása után lehetősége van a hitelesítő adatok megosztására az új felhasználóknál is. Ezeket kinyomtathatja, elküldheti e-mailben, vagy pedig letöltheti.

4. Hagyja ki az e-mail-üzenetek áttelepítését, és kattintson a **Tovább** gombra az **E-mail-üzenetek áttelepítése** lapon. 

    Ha egy másik e-mail szolgáltatótól költözik, és később át kívánja másolni az adatokat, akkor [áttelepítheti az e-maileket és a névjegyeket az Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).


### <a name="connect-your-domain"></a>Tartomány csatlakoztatása

> [!NOTE]
> Ha az. onmicrosoft tartomány használata mellett döntött, vagy a felhasználók beállításához a Azure AD Connect szolgáltatást használja, akkor ezt a lépést nem fogja látni.
  
A szolgáltatások beállításához frissítenie kell bizonyos rekordokat a DNS-szolgáltatónál vagy a tartományregisztrálónál.
  
1. A beállítási varázsló általában felismeri a regisztrálóját, és részletes útmutatást jelenít meg arról, hogy miként frissítheti a névkiszolgálói rekordokat a regisztráló webhelyén. Ha nem, [módosítsa a névszervereket az Office 365 beállításához bármely tartományregisztrálóval](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Ha vannak meglévő DNS-rekordjai, például egy meglévő webhely, de a DNS-állomás a tartományhoz történő [kapcsolódáshoz](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)engedélyezve van, válassza **a saját rekord hozzáadása**lehetőséget. 
    - Ha van meglévő DNS-rekordja más DNS-állomásokkal (nincs engedélyezve a tartomány csatlakoztatásához), saját DNS-rekordokat kell kezelnie annak érdekében, hogy a meglévő szolgáltatások ne maradjanak kapcsolatban. További információ a [tartomány alapjai](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) című témakörben található.

        ![Összeköt-a birtok oldal-val én ' kezel az én-m saját DNS hanglemezek.](media/connectyourdomainpage.png)

2. Kövesse a varázsló lépéseit, és az e-mail és egyéb szolgáltatások lesznek beállítva az Ön számára.

### <a name="set-up-security-policies-and-device-configurations"></a>Biztonsági házirendek és eszközkonfigurációk beállítása 

A varázslóban beállított házirendek automatikusan alkalmazásra kerülnek a *minden felhasználó*nevű [biztonsági csoportra](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) . További csoportokat is létrehozhat, ha házirendeket rendel az admin Centerhez.

1. -Ra a **megvéd-a dolgozik fájlokat-ra mozgatható berendezés** a választás **megvéd dolgozik fájlokat mikor berendezés van elveszett vagy lopott** van válogatott mellett hiba. Lehetősége van bekapcsolni annak **kezelését, hogy a felhasználók hogyan férhessék hozzá az Office-fájlokat a mobileszközökön**, és ez ajánlott.

    ![Ernyőz-ból megvéd dolgozik fájlokat-ra mozgatható berendezés oldal.](media/protectworkfilesondevices.png)

     - Az [alapértelmezett értékek](protect-work-files-on-lost-or-stolen-device.md)megjelenítéséhez bontsa ki a **fájlvédelem a munkahelyi fájlokat, ha az eszköz elvész vagy ellopják** :

        ![Képernyőkép az alapértelmezett értékekről az elveszett eszközökön lévő fájlok védelméhez.](media/protectworkfilesondevicesdefault.png)

    - Válassza a **kezelés, hogy a felhasználók hogyan férhetnek hozzá az Office-fájlokhoz a mobileszközökön** , és bontsa ki azt az [alapértelmezett értékek](manage-user-access-on-mobile-devices.md)megjelenítéséhez. Javasoljuk, hogy a telepítés során fogadja el az alapértelmezett értékeket, hogy az összes felhasználóra érvényes Android, iOS és Windows 10 alkalmazások házirendjeit hozza létre. A telepítés után további házirendeket is létrehozhat majd.

        ![A mobil Office-fájlokhoz tartozó védelmi beállítások képernyőképe.](media/useraccessonmobile.png)

2. Az adatok és eszközök védelmének utolsó lépése lehetővé teszi a házirendek beállítására a Windows 10 eszközök biztonságossá tétele érdekében. Ezeket a beállításokat a rendszer automatikusan alkalmazza, amikor a felhasználó Windows 10-e csatlakozik a szervezethez. A **biztonságos Windows 10 eszközöket** kibonthatja az [alapértelmezett értékek](secure-windows-10-devices.md)megtekintéséhez és módosításához.
3. Azt is választhatja, hogy [automatikusan telepíti az Office](install-office-on-windows-10-during-setup.md) -t a Windows 10 eszközén.

    ![Képernyőkép beállítása a Windows 10 eszköz konfigurációs lapjáról.](media/setwin10config.png)



## <a name="deploy-office-365-client-apps"></a>Az Office 365 ügyfélalkalmazások telepítése

Ha úgy dönt, hogy a telepítés során automatikusan telepíti az Office-alkalmazásokat, az alkalmazások a Windows 10 eszközén telepíthetnek, amint a felhasználók az azúrkék HIRDETÉSRE be lettek jelentkezve a saját munkájukat hitelesítő adataikkal.
Az Office mobil iOS vagy Android eszközökre történő telepítéséhez tekintse meg [a mobileszközök beállítása a Microsoft 365 üzleti felhasználók számára](set-up-mobile-devices.md)című témakört.

Az Office programot egyenként is telepíthetjük. Útmutatás: az [Office telepítése PC vagy Mac számítógépre](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) .

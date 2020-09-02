---
title: A Microsoft 365 vállalati prémium verzió beállítása
f1.keywords:
- NOCSH
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
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Ismerje meg a Microsoft 365 vállalati prémium verzió beállítási lépéseit, például a tartomány és a felhasználók hozzáadását, a biztonsági házirendek beállítását és sok mást.
ms.openlocfilehash: cc20637d7a78bd34ecb61a4ed46eb06d564d63df
ms.sourcegitcommit: 25afc0c34edc7f8a5eb389d8c701175256c58ec8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/01/2020
ms.locfileid: "47324496"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a>A Microsoft 365 vállalati prémium verzió beállítása a beállítási varázslóban

Ebből a videóból áttekintést kaphat a Microsoft 365 vállalati prémium verzió telepítéséről.<br><br>

## <a name="add-your-domain-users-and-set-up-policies"></a>A tartomány, a felhasználók és a házirendek beállítása

Amikor megvásárolja a Microsoft 365 Business Premiumot, lehetősége van a saját tartomány használatára, vagy a [regisztráció](sign-up.md)során egyet vásárolni.

- Ha regisztrációkor új tartományt vásárolt, a tartománya minden beállítása, és áthelyezheti a [felhasználók hozzáadását és a licencek hozzárendelését](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Saját tartomány hozzáadása a bejelentkezés személyre szabásához

1. A [Microsoft 365 felügyeleti központba](https://admin.microsoft.com) a globális rendszergazdai hitelesítő adataival jelentkezhet be. 

2. A varázsló indításához válassza az **Ugrás a beállításra** lehetőséget.

    ![Kattintson az Ugrás a beállításra elemre.](../media/gotosetupinadmincenter.png)

3. Az **Office-alkalmazások telepítése** lapon igény szerint telepítheti az alkalmazásokat saját számítógépére.
    
4. A **tartomány hozzáadása** lépésben adja meg a használni kívánt tartománynevet (például contoso.com).

    > [!IMPORTANT]
    > Ha a regisztráció során megvásárolt egy tartományt, itt nem jelenik meg **a tartomány felvétele** lépés. Nyissa meg a [felhasználók felvétele](#add-users-and-assign-licenses) helyet.

    ![Képernyőkép: a bejelentkezési lap személyre szabása.](../media/adddomain.png)

    
4. A varázsló lépéseit követve [hozzon létre DNS-rekordokat bármely DNS-szolgáltatónál a Microsoft 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) , amely igazolja, hogy Ön a tartomány tulajdonosa. Ha ismeri a tartomány szolgáltatóját, olvassa el a [Host-specifikus utasítások](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)című témakört is.

    Ha szolgáltatójánál a GoDaddy vagy egy másik állomás engedélyezve van a [tartomány csatlakozásakor](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), a folyamat egyszerű, és automatikusan kéri a bejelentkezést, és hagyja, hogy a Microsoft hitelesítse az Ön nevében.

    ![A GoDaddy hozzáférés megerősítése lapon válassza az Engedélyezés lehetőséget.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Felhasználók felvétele és licencek hozzárendelése

Hozzáadhat felhasználókat a varázslóban, de [később is hozzáadhat felhasználókat](add-users-m365b.md) a felügyeleti központban. Ha helyi tartományvezérlőt használ, akkor az [Azure ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)segítségével felhasználókat vehet fel.

#### <a name="add-users-in-the-wizard"></a>Felhasználók hozzáadása a varázslóban

A varázslóban hozzáadott minden felhasználó automatikusan hozzárendeli a Microsoft 365 vállalati prémium verzió licencét.

![Képernyőkép a varázsló új felhasználók hozzáadása lapjáról](../media/addnewuserspage.png)

1. Ha a Microsoft 365 vállalati prémium verzióra szóló előfizetése meglévő felhasználókkal rendelkezik (például az Azure AD Connectt használta), akkor lehetősége van arra, hogy most rendelje hozzá a licenceket. Nyugodtan felvehet licenceket hozzájuk is.

2. Miután hozzáadta a felhasználókat, megoszthatja a hitelesítő adatokat a hozzáadott új felhasználókkal. Ezeket kinyomtathatja, elküldheti e-mailben, vagy pedig letöltheti.

### <a name="connect-your-domain"></a>Tartomány csatlakoztatása

> [!NOTE]
> Ha az. onmicrosoft tartomány használatát választotta, vagy az Azure AD Connectt használja a felhasználók beállításához, akkor nem fogja látni ezt a lépést.
  
A szolgáltatások beállításához frissítenie kell bizonyos rekordokat a DNS-szolgáltatónál vagy a tartományregisztrálónál.
  
1. A beállítási varázsló általában felismeri a regisztrálóját, és részletes útmutatást jelenít meg arról, hogy miként frissítheti a névkiszolgálói rekordokat a regisztráló webhelyén. Ha nem, [módosítsa a névkiszolgálók beállítást a Microsoft 365 bármely tartományregisztrálónál való beállításához](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar). 

    - Ha van meglévő DNS-rekordja (például egy meglévő webhely), de a DNS-szolgáltatója engedélyezve van a [tartomány csatlakoztatása](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)beállításnál, válassza a saját **rekordok hozzáadása**lehetőséget. Az **online szolgáltatások kiválasztása** lapon fogadja el az összes alapértelmezett elemet, és válassza a **tovább**gombot, és válassza a DNS-szolgáltatója lapon az **Engedélyezés** lehetőséget.
    - Ha meglévő DNS-rekordjait más DNS-szolgáltatókkal (nem engedélyezett a tartományhoz való csatlakozáskor) szeretné használni, kezelje saját DNS-rekordjait, és ellenőrizze, hogy a meglévő szolgáltatások maradnak-e csatlakoztatva. További információt a [tartomány alapjai](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) című témakörben találhat.

        ![A rekordok aktiválása lap](../media/activaterecords.png)

2. Kövesse a varázsló lépéseit, és az e-mailek és más szolgáltatások beállításra kerülnek.

### <a name="protect-your-organization"></a>A szervezet védelme 

A varázslóban beállított házirendeket a rendszer automatikusan alkalmazza az *összes felhasználó*nevű [biztonsági csoportba](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) . Létrehozhat további csoportokat is, amelyekkel a felügyeleti központban megadhatja a házirendeket.

1. A **speciális Cyber-fenyegetések elleni védelem fokozása**érdekében ajánlott elfogadnia az alapértelmezett beállításokat, hogy az [Office 365 előzetes veszélyforrásokkal védett](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) fájlok és hivatkozások legyenek az Office-alkalmazásokban.

    ![Képernyőkép a védelem növelése lapról.](../media/increasetreatprotection.png)


2. A **bizalmas adatok szivárgásának megakadályozása** lapon fogadja el az alapértelmezett adatokat az Office 365 adatvesztés-megelőzés (DLP) bekapcsolásához az Office-alkalmazásokban lévő bizalmas adatok nyomon követéséhez és a szervezeten kívüli adatok véletlenszerű megosztásához.

3. Az **Adatvédelem az Office Mobile-ban** lapon hagyja meg a mobil app-kezelés lehetőséget, bontsa ki a beállításokat, és tekintse át őket, és válassza a **mobil app-kezelési házirend létrehozása**lehetőséget.

    ![Képernyőkép az adatvédelemről az Office for Mobile lapon.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Windows 10-es számítógépek biztonságossá tétele

A bal oldali navigációs sávon válassza a **Setup (beállítás** ) lehetőséget, majd a **Bejelentkezés és biztonság**csoportban válassza **a Windows 10-es számítógépek biztonságossá tétele**lehetőséget. A kezdéshez válassza a **nézet** lehetőséget. A teljes körű útmutatásért olvassa el a [Windows 10-es számítógépek biztonságossá tétele](secure-win-10-pcs.md) című témakört.

## <a name="deploy-office-365-client-apps"></a>Az Office 365 ügyfélalkalmazás központi telepítése

Ha a telepítés során úgy döntött, hogy automatikusan telepíti az Office-alkalmazásokat, az alkalmazások a Windows 10-es eszközökön fognak megjelenni, amint a felhasználók a Windows-eszközökről bejelentkeznek az Azure AD szolgáltatásba, a munkahelyi hitelesítő adataikkal.

Ha az Office-t mobil iOS-vagy Android-eszközön szeretné telepíteni, olvassa el a [mobileszközök beállítása a Microsoft 365 vállalati prémium verzió felhasználóinak](set-up-mobile-devices.md)című témakört.

Az Office-t külön is telepítheti. További információt az [Office telepítése PC-re vagy Mac gépre](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) című témakörben találhat.

## <a name="see-also"></a>Lásd még

[Microsoft 365 vállalati verziós képzési videók](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)

---
title: A Microsoft 365 Vállalati prémium verzió beállítása
f1.keywords:
- NOCSH
ms.author: kwekua
author: kwekua
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
description: Megismerheti a fiókkal kapcsolatos Microsoft 365 Vállalati prémium verzió, például tartomány és felhasználók felvételét, biztonsági házirendek beállítását és sok minden más.
ms.openlocfilehash: 37607b483686fc12ac6253ae9f693ec86c073c4e
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52245044"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a>A Microsoft 365 Vállalati prémium verzió beállítása a beállítási varázslóban

Ez a videó áttekintést nyújt a Microsoft 365 Vállalati prémium verzió beállításról.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a>Tartomány, felhasználók hozzáadása és házirendek beállítása

A (Microsoft 365 Vállalati prémium verzió vásárlásakor lehetősége van saját tartományt használni, illetve a regisztráció során vásárolni [egyet.](sign-up.md)

- Ha a feliratkozáskor új tartományt vásárolt, akkor a tartománya be van állítva, és a Felhasználók hozzáadása és licencek hozzárendelése gombra kell [lépnie.](#add-users-and-assign-licenses)

### <a name="add-your-domain-to-personalize-sign-in"></a>Tartomány hozzáadása a bejelentkezés személyre szabása

1. Jelentkezzen be [Microsoft 365 felügyeleti központba](https://admin.microsoft.com) globális rendszergazdai hitelesítő adataival. 

2. A **varázslót az Ugrás** a beállításra gombra állítva indítsa el.

    ![Válassza az Ugrás a beállításra lehetőséget.](../media/gotosetupinadmincenter.png)

3. A **Saját appok Office lapján** tetszés szerint telepítheti az alkalmazásokat a saját számítógépén.
    
4. A **Tartomány hozzáadása lépésben** adja meg a használni kívánt tartománynevet (például contoso.com).

    > [!IMPORTANT]
    > Ha a regisztráció során tartományt vásárolt, itt nem fogja látni **a** Tartomány hozzáadása lépést. Ehelyett a [Felhasználók hozzáadása gombra](#add-users-and-assign-licenses) kell azt felvennie.

    ![Képernyőkép a Bejelentkezési lap személyre szabása lapról.](../media/adddomain.png)

    
4. A varázsló lépéseit követve hozza létre a DNS-rekordokat bármely [DNS-szolgáltatónál](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) annak Microsoft 365, hogy Öné a tartomány. Ha ismeri a tartományát, olvassa el a [szolgáltatóra vonatkozó utasításokat is.](/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)

    Ha az Ön tárhelyszolgáltatója a GoDaddy vagy más szolgáltató, amely támogatja a tartomány [csatlakoztatását,](/office365/admin/get-help-with-domains/domain-connect)a folyamat egyszerű, és a rendszer automatikusan kérni fogja, hogy jelentkezzen be, és a Microsoft hitelesítse magát az Ön nevében.

    ![A GoDaddy Confirm Access (Hozzáférés megerősítése) lapon válassza a Authorize (Engedély) lehetőséget.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Felhasználók felvétele és licencek hozzárendelése

Felvehet felhasználókat a varázslóba, de [](../admin/add-users/add-users.md) később a Felügyeleti központban is. Ha pedig helyi tartományvezérlője van, felhasználókat is felvehet az [Azure AD Csatlakozás.](/azure/active-directory/hybrid/how-to-connect-install-express)

#### <a name="add-users-in-the-wizard"></a>Felhasználók hozzáadása a varázslóban

A varázslóban hozzáadt minden felhasználóhoz automatikusan hozzárendel egy Microsoft 365 Vállalati prémium verzió licencet.

![Képernyőkép a varázsló Új felhasználók hozzáadása lapról](../media/addnewuserspage.png)

1. Ha az Microsoft 365 Vállalati prémium verzió-előfizetéséhez vannak meglévő felhasználók (például ha az Azure AD Csatlakozás-t használta), akkor most lehetősége van licenceket rendelni hozzájuk. Nyugodtan felvehet licenceket hozzájuk is.

2. A felhasználók hozzáadása után a hitelesítő adatokat is megoszthatja a felvett új felhasználókkal. Ezeket kinyomtathatja, elküldheti e-mailben, vagy pedig letöltheti.

### <a name="connect-your-domain"></a>Tartomány csatlakoztatása

> [!NOTE]
> Ha az .onmicrosoft tartományt választotta, vagy az Azure AD Csatlakozás segítségével beállította a felhasználókat, ez a lépés nem látható.
  
A szolgáltatások beállításához frissítenie kell bizonyos rekordokat a DNS-szolgáltatónál vagy a tartományregisztrálónál.
  
1. A beállítási varázsló általában felismeri a regisztrálóját, és részletes útmutatást jelenít meg arról, hogy miként frissítheti a névkiszolgálói rekordokat a regisztráló webhelyén. Ha nem így van, módosítsa a névkiszolgálói rekordokat úgy, hogy Microsoft 365 [tartományregisztrálónál beállítsa a rekordokat.](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md) 

    - Ha van meglévő DNS-rekordja, például egy meglévő webhelye, de a DNS-szolgáltató engedélyezve van a [tartományhoz](/office365/admin/get-help-with-domains/domain-connect)való csatlakozáshoz, válassza a Rekordok hozzáadása **lehetőséget.** A Choose **your online services (Online szolgáltatások kiválasztása)** lapon fogadja el az összes alapértelmezett beállítást, és válassza a **Tovább**, majd az **Authorize** (Engedély) lehetőséget a DNS-szolgáltatója lapján.
    - Ha más DNS-szolgáltatónál már van DNS-rekordja (a tartomány csatlakoztatása nem engedélyezett), akkor saját DNS-rekordjait kell kezelnie, hogy a meglévő szolgáltatások kapcsolatban maradjanak. További [információt a tartományokkal kapcsolatos alapismeretek](/office365/admin/get-help-with-domains/dns-basics) között található.

        ![Rekordok aktiválása lap.](../media/activaterecords.png)

2. Kövesse a varázsló lépéseit, és állítsa be Önnek a levelezést és más szolgáltatásokat.

### <a name="protect-your-organization"></a>A szervezet védelme 

A varázslóban beállított házirendek automatikusan vonatkoznak a Minden [felhasználó](/office365/admin/create-groups/compare-groups#security-groups) nevű biztonsági *csoportra.* További csoportokat is létrehozhat, amelyekhez házirendeket rendelhet hozzá a Felügyeleti központban.

1. A speciális **kiberfenyegetések** elleni védelem növelése érdekében javasoljuk, hogy fogadja el az alapértelmezett értékeket, hogy a Office 365 [Komplex](../security/office-365-security/defender-for-office-365.md) veszélyforrások elleni védelem megvizsgálja a fájlokat és hivatkozásokat az Office alkalmazásokban.

    ![Képernyőkép a Védelem növelése lapról](../media/increasetreatprotection.png)


2. A  Bizalmas adatok kiszivárgásának megakadályozása lapon fogadja el az Office 365 Adatveszteség-megelőzés (DLP) alapértelmezett beállítását a bizalmas adatok nyomon követéséhez az Office-appokban, valamint annak érdekében, hogy megakadályozza ezeknek a szervezeten kívüli véletlen megosztását.

3. Az **Adatok védelme a mobileszközök Office** lapon hagyja be a mobilapp felügyeletét, bontsa ki a beállításokat, és tekintse át őket, majd válassza a Mobilappkezelési házirend **létrehozása lehetőséget.**

    ![Képernyőkép a Mobileszközök Office adatokat lapról.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Pc Windows 10 biztonságossá

A bal oldali  navigációs sávon válassza a Beállítás lehetőséget, majd a Bejelentkezés és biztonság alatt válassza A számítógép **Windows 10 lehetőséget.** Első **lépésekhez** válassza a Nézet lehetőséget. Részletes [útmutatást a számítógépei Windows 10 el.](secure-win-10-pcs.md)

## <a name="deploy-office-365-client-apps"></a>Ügyfélalkalmazások Office 365 telepítése

Ha a telepítés során az Office-appok automatikus telepítését választotta, az alkalmazások az Windows 10-eszközökre fognak telepíteni, miután a felhasználók bejelentkeztek az Azure AD-be az Windows-eszközükről a munkahelyi hitelesítő adataik használatával.

Az iOS Office Android rendszerű mobileszközökön való telepítéséhez lásd: Mobileszközök beállítása az összes [Microsoft 365 Vállalati prémium verzió számára.](set-up-mobile-devices.md)

A frissítéseket egyenként Office is. Útmutatásért [Office PC-re](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) vagy Mac gépre való telepítéséről.

## <a name="see-also"></a>Lásd még

[Microsoft 365 vállalati verziós oktatóvideók](../business-video/index.yml)

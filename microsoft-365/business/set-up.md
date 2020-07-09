---
title: A Microsoft 365 Vállalati Prémium verzió beállítása
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
description: Ismerje meg a Microsoft 365 Business Premium beállítási lépéseit, beleértve a tartomány és a felhasználók hozzáadását, a biztonsági házirendek beállítását és egyebeket.
ms.openlocfilehash: efa7934ece0dfeac3c4b20daa37da6f1160901e7
ms.sourcegitcommit: 5b769f74bcc76ac8d38aad815d1728824783cd9f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081902"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a>A Microsoft 365 Vállalati Prémium verzió beállítása a beállítási varázslóban

Ebből a videóból megtudhatja, hogy miként tekintheti meg a Microsoft 365 Business Premium beállítását.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Ha hasznosnak találta ezt a videót, tekintse meg a [teljes tanfolyamok kisvállalatoknak és Microsoft 365-újoncoknak](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) című cikket.

## <a name="add-your-domain-users-and-set-up-policies"></a>Tartomány, felhasználók hozzáadása és házirendek beállítása

A Microsoft 365 Business Premium megvásárlásakor lehetősége van arra, hogy saját tartományt használjon, vagy a [regisztráció](sign-up.md)során megvásárolja.

- Ha a regisztrált tartományban új tartományt vásárolt, a tartomány be van állítva, és áthelyezheti a Felhasználók hozzáadása és [a licencek hozzárendelése lehetőséget.](#add-users-and-assign-licenses)

### <a name="add-your-domain-to-personalize-sign-in"></a>A tartomány hozzáadása a bejelentkezés személyre szabásához

1. Jelentkezzen be a [Microsoft 365 Felügyeleti központba](https://admin.microsoft.com) a globális rendszergazdai hitelesítő adatok használatával. 

2. A varázsló elindításához válassza **az Ugrás gombot** a beállításhoz.

    ![Válassza az Ugrás a beállításhoz lehetőséget.](../media/gotosetupinadmincenter.png)

3. Az **Office-alkalmazások telepítése** lapon igény szerint telepítheti az alkalmazásokat a saját számítógépére.
    
4. A **Tartomány hozzáadása** lépésben adja meg a használni kívánt tartománynevet (például contoso.com).

    > [!IMPORTANT]
    > Ha a regisztráció során vásárolt egy tartományt, itt nem jelenik meg **a Tartomány hozzáadása** lépés. Nyissa meg a [Felhasználók hozzáadása](#add-users-and-assign-licenses) lehetőséget.

    ![Képernyőkép a Bejelentkezés testreszabása lapról.](../media/adddomain.png)

    
4. Kövesse a varázsló lépéseit a [DNS-rekordok létrehozásához bármely Olyan Microsoft 365-alapú DNS-szolgáltatónál,](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) amely ellenőrzi a tartomány ön általi tulajdonát. Ha ismeri a tartományi állomást, olvassa el a [gazdagépspecifikus utasításokat](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)is.

    Ha a tárhelyszolgáltatója A GoDaddy vagy a [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)egy másik állomása, a folyamat egyszerű, és a rendszer automatikusan kéri, hogy jelentkezzen be, és hagyja, hogy a Microsoft hitelesítse magát az Ön nevében.

    ![A GoDaddy Hozzáférés megerősítése lapján válassza az Engedélyezés lehetőséget.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Felhasználók felvétele és licencek hozzárendelése

A varázslóban hozzáadhat felhasználókat, de később a felügyeleti központban is [hozzáadhat felhasználókat.](add-users-m365b.md) Továbbá, ha rendelkezik egy helyi tartományvezérlővel, hozzáadhat felhasználókat az [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)használatával.

#### <a name="add-users-in-the-wizard"></a>Felhasználók felvétele a varázslóba

A varázslóban hozzáadott felhasználók automatikusan Microsoft 365 Business Premium licencet kapnak.

![Képernyőkép a varázsló Új felhasználók hozzáadása lapjáról](../media/addnewuserspage.png)

1. Ha a Microsoft 365 Business Premium-előfizetése meglévő felhasználókkal rendelkezik (például ha az Azure AD Connectet használta), most lehetősége van licenceket rendelni hozzájuk. Nyugodtan felvehet licenceket hozzájuk is.

2. Miután hozzáadta a felhasználókat, lehetősége van a hitelesítő adatok megosztására a hozzáadott új felhasználókkal. Ezeket kinyomtathatja, elküldheti e-mailben, vagy pedig letöltheti.

### <a name="connect-your-domain"></a>Tartomány csatlakoztatása

> [!NOTE]
> Ha az .onmicrosoft tartomány t választotta, vagy az Azure AD Connect használatával állította be a felhasználókat, akkor ez a lépés nem jelenik meg.
  
A szolgáltatások beállításához frissítenie kell bizonyos rekordokat a DNS-szolgáltatónál vagy a tartományregisztrálónál.
  
1. A beállítási varázsló általában felismeri a regisztrálóját, és részletes útmutatást jelenít meg arról, hogy miként frissítheti a névkiszolgálói rekordokat a regisztráló webhelyén. Ha nem, módosítsa a [névkiszolgálókat, hogy a Microsoft 365-öt bármely tartományregisztrálóval állítsa be.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar) 

    - Ha már rendelkezik meglévő DNS-rekordokkal, például egy meglévő webwebhelytel, de a DNS-szolgáltatója engedélyezve van a [tartománycsatlakozáshoz,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)válassza **a Rekordok hozzáadása nekem**lehetőséget. Az **Online szolgáltatások kiválasztása** lapon fogadja el az összes alapértelmezést, és válassza a **Tovább**gombot, és válassza a DNS-szolgáltató lapján az **Engedélyezés** lehetőséget.
    - Ha más DNS-állomásokkal is rendelkezik DNS-rekordokkal (nincs engedélyezve a tartománycsatlakozáshoz), akkor a meglévő szolgáltatások kapcsolatának biztosítása érdekében saját DNS-rekordjait kell kezelnie. További információ a [tartományokkal kapcsolatos alapvető tudnivalókról.](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics)

        ![Rekordok aktiválása lap.](../media/activaterecords.png)

2. Kövesse a varázsló lépéseit, és az e-mail és egyéb szolgáltatások be lesznek állítva.

### <a name="protect-your-organization"></a>A szervezet védelme 

A varázslóban beállított házirendek automatikusan érvénybe lépnek a Minden felhasználó nevű [biztonsági](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) *csoportra.* A felügyeleti központban további csoportokat is létrehozhat, amelyekhez házirendeket rendelhet.

1. A Fokozott védelem növelése a **fejlett kiberfenyegetésekkel**szembeni védelem beállításnál ajánlott elfogadni azokat az alapértelmezett beállításokat, amelyek lehetővé teszik, hogy az [Office 365 Előzetes veszélyforrások elleni védelem](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) fájlokat és hivatkozásokat késebősebben az Office-alkalmazásokban.

    ![Képernyőkép: Védelem növelése lap.](../media/increasetreatprotection.png)


2. A **Bizalmas adatok kiszivárgásának megelőzése** lapon fogadja el az Office 365 adatveszteség-megelőzési (DLP) bekapcsolását a bizalmas adatok Office-alkalmazásokban való nyomon követéséhez és a szervezeten kívüli véletlen megosztás megakadályozásához.

3. Az Adatok védelme az **Office mobilszolgáltatásban** lapon hagyja bekapcsolva a mobilalkalmazás-kezelést, bontsa ki a beállításokat, és tekintse át őket, majd válassza **a Mobilalkalmazás-kezelési szabályzat létrehozása lehetőséget.**

    ![Képernyőkép: Adatok védelme az Office mobilon alkalmazásban lapról.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Biztonságos Windows 10-es számítógépek

A bal oldali navigációs sávon válassza a **Telepítés** lehetőséget, majd a Bejelentkezés és biztonság csoportban válassza **a Windows 10-es számítógépek védelme**lehetőséget. **Sign-in and security** A kezdéshez válassza a **Nézet** lehetőséget. A teljes körű útmutatásért tekintse meg [a Windows 10-es számítógépek biztonságossá](secure-win-10-pcs.md) tétele.

## <a name="deploy-office-365-client-apps"></a>Office 365-ügyfélalkalmazások telepítése

Ha úgy döntött, hogy a telepítés során automatikusan telepíti az Office-alkalmazásokat, az alkalmazások akkor települnek a Windows 10-es eszközökre, amikor a felhasználók bejelentkeztek az Azure AD-be a Windows-eszközeikről, a munkahelyi hitelesítő adataik használatával.

Az Office mobilos iOS- vagy Android-eszközökre való telepítéséről a [Mobileszközök beállítása Microsoft 365 Vállalati Prémium verziófelhasználói számára című](set-up-mobile-devices.md)témakörben található.

Az Office-t külön is telepítheti. További információt [az Office telepítése PC-re vagy Mac gépre](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) című témakörben talál.

## <a name="see-also"></a>Lásd még

[Microsoft 365 üzleti oktatóvideók](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)

---
title: A Microsoft 365 Business beállítása
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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Fedezze fel a Microsoft 365 Vállalati verzió beállítási lépéseit, beleértve a tartomány és a felhasználók hozzáadását, a biztonsági házirendek beállítását stb.
ms.openlocfilehash: 4535a32b579b91b6c2bb0e64ec95904be6c08fce
ms.sourcegitcommit: d6c871bf3f94d9299d22695f5dbaf25dc1bd6ff9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42417296"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>A Microsoft 365 Business beállítása a telepítővarázslóban

Ebből a videóból megtudhatja, hogy mik a Microsoft 365 Vállalati verzió beállítása.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Ha hasznosnak találta ezt a videót, tekintse meg a [teljes tanfolyamok kisvállalatoknak és Microsoft 365-újoncoknak](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) című témakört.

## <a name="add-your-domain-users-and-set-up-policies"></a>Tartomány, felhasználók hozzáadása és házirendek beállítása

[![A megjelenő címke figyelmeztet a felügyeleti központ változásaira, további részleteket itt talál: aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

A Microsoft 365 Business megvásárlásakor lehetősége van arra, hogy a saját tartományát használja, vagy a [regisztráció](sign-up.md)során vásároljon egyet.

- Ha regisztrált, új tartományt vásárolt, a tartomány teljesen be van állítva, és áthelyezheti a [Felhasználók hozzáadása és a licencek hozzárendelése](#add-users-and-assign-licenses)elemre.

### <a name="add-your-domain-to-personalize-sign-in"></a>A tartomány hozzáadása a bejelentkezés személyre szabásához

1. Jelentkezzen be a [Microsoft 365 Felügyeleti központba](https://admin.microsoft.com) a globális rendszergazdai hitelesítő adatok használatával. 

2. A varázsló elindításához válassza az **Ugrás a beállításhoz** lehetőséget.

    ![Válassza az Ugrás a beállításhoz lehetőséget.](../media/gotosetupinadmincenter.png)

3. Az **Office-alkalmazások telepítése** lapon igény szerint telepítheti az alkalmazásokat a saját számítógépére.
    
4. A **Tartomány hozzáadása** lépésben adja meg a használni kívánt tartománynevet (például contoso.com).

    > [!IMPORTANT]
    > Ha a regisztráció során vásárolt tartományt, itt nem jelenik meg a **Tartomány hozzáadása** lépés. Nyissa meg inkább a [Felhasználók hozzáadása](#add-users-and-assign-licenses) lehetőséget.

    ![Képernyőkép a Bejelentkezési oldal személyre szabása lapról.](../media/adddomain.png)

    
4. A varázsló lépéseit [követve dns-rekordokat hozhat létre bármely Olyan OFFICE 365-ös DNS-szolgáltatónál,](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) amely ellenőrzi, hogy Ön a tartomány tulajdonosa.Follow the steps in the wizard to Create DNS records at any DNS hosting provider for Office 365 that verifies you own the domain. Ha ismeri a tartományi állomást, olvassa el a [gazdagép specifikus utasításait.](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)

    Ha a tárhelyszolgáltató godaddy vagy más, [tartományi kapcsolattal](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)rendelkező gazdagép, a folyamat egyszerű, és a rendszer automatikusan megkéri, hogy jelentkezzen be, és hagyja, hogy a Microsoft hitelesítse magát az Ön nevében.

    ![A GoDaddy Access megerősítése lapon válassza az Engedélyezés lehetőséget.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Felhasználók felvétele és licencek hozzárendelése

A varázslóban felhasználókat is felvehet, de később is [felvehet felhasználókat](add-users-m365b.md) a felügyeleti központban. Ha helyi tartományvezérlővel is rendelkezik, hozzáadhat felhasználókat az [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)szolgáltatással.

#### <a name="add-users-in-the-wizard"></a>Felhasználók hozzáadása a varázslóban

A varázslóban hozzáadott felhasználók automatikusan Microsoft 365 Vállalati licencet kapnak.

![Képernyőkép az Új felhasználók hozzáadása lapról a varázslóban](../media/addnewuserspage.png)

1. Ha a Microsoft 365 Business-előfizetése meglévő felhasználókkal rendelkezik (például ha az Azure AD Connectet használta), most lehetősége van licencek hozzárendelésére. Nyugodtan felvehet licenceket hozzájuk is.

2. Miután felvette a felhasználókat, lehetőséget kap arra is, hogy megossza a hitelesítő adatokat a hozzáadott új felhasználókkal. Ezeket kinyomtathatja, elküldheti e-mailben, vagy pedig letöltheti.

### <a name="connect-your-domain"></a>Tartomány csatlakoztatása

> [!NOTE]
> Ha az .onmicrosoft tartomány t használja, vagy az Azure AD Connectet használta a felhasználók beállításához, akkor ez a lépés nem jelenik meg.
  
A szolgáltatások beállításához frissítenie kell bizonyos rekordokat a DNS-szolgáltatónál vagy a tartományregisztrálónál.
  
1. A beállítási varázsló általában felismeri a regisztrálóját, és részletes útmutatást jelenít meg arról, hogy miként frissítheti a névkiszolgálói rekordokat a regisztráló webhelyén. Ha nem, módosítsa a [névkiszolgálókat, hogy az Office 365-öt bármely tartományregisztrálóval](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2)beállítsák. 

    - Ha meglévő DNS-rekordokkal rendelkezik, például egy meglévő webhely, de a DNS-szolgáltató engedélyezve van a [tartománycsatlakozáshoz,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)válassza **a Rekordok hozzáadása számomra**lehetőséget. Az **Online szolgáltatások kiválasztása** lapon fogadja el az összes alapértelmezést, és válassza a **Tovább**gombot, és válassza a DNS-szolgáltató lapján az **Engedélyezés** lehetőséget.
    - Ha már rendelkezik DNS-rekordokkal más DNS-állomásokkal (nincs engedélyezve a tartománycsatlakozáshoz), akkor a meglévő szolgáltatások kapcsolatának biztosítása érdekében kezelje a saját DNS-rekordjait. További információ a [tartomány alapjaiban.](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics)

        ![Rekordok aktiválása lap.](../media/activaterecords.png)

2. Kövesse a varázsló lépéseit, és az e-mailek és egyéb szolgáltatások beállítva lesznek.

### <a name="protect-your-organization"></a>A szervezet védelme 

A varázslóban beállított házirendek automatikusan érvénybe lépnek a *Minden felhasználó*nevű [biztonsági csoportra.](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) További csoportokat is létrehozhat, amelyekhez házirendeket rendelhet a felügyeleti központban.

1. A **Fokozott védelem a fejlett kiberfenyegetésekkel kapcsolatban**ajánlott elfogadni az alapértelmezett beállításokat, hogy az [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) beszana fájlokat és hivatkozásokat az Office-alkalmazásokban.

    ![Képernyőkép: Védelem növelése lap.](../media/increasetreatprotection.png)


2. A **Bizalmas adatok szivárgásának megakadályozása** lapon fogadja el az Office 365 adatveszteség-megelőzési (DLP) beállításának alapértelmezett beállításait a bizalmas adatok nyomon követéséhez az Office-alkalmazásokban, és megakadályozza ezek véletlen megosztását a szervezeten kívül.

3. Az **Adatok védelme mobiloffice-ban** lapon hagyja bekapcsolva a mobilalkalmazás-felügyeletet, bontsa ki a beállításokat és tekintse át őket, majd válassza a **Mobilalkalmazás-kezelési szabályzat létrehozása**lehetőséget.

    ![Képernyőkép: Adatok védelme a mobiloffice-ban lapon.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Windows 10-es számítógépek biztonságossá tétele

A bal oldali navigációs sávon válassza a **Telepítés** lehetőséget, majd a **Sin-in és a Biztonság**csoportban válassza a Windows **10-es számítógépek biztonsága**lehetőséget. A kezdéshez válassza a **Nézet** lehetőséget. A teljes útmutatóban a [Windows 10-es számítógépek biztonsága](secure-win-10-pcs.md) látható.

## <a name="deploy-office-365-client-apps"></a>Az Office 365 ügyfélalkalmazásának telepítése

Ha úgy dönt, hogy a telepítés során automatikusan telepíti az Office-alkalmazásokat, az alkalmazások a Windows 10-es eszközökre települnek, miután a felhasználók bejelentkeztek az Azure AD-be a munkahelyi hitelesítő adataik használatával.

Az Office mobiliOS vagy Android rendszerű eszközökre való telepítéséhez olvassa el [a Mobileszközök beállítása a Microsoft 365 Vállalati verzió felhasználói számára](set-up-mobile-devices.md)című témakört.

Az Office-t külön is telepítheti. Az [Office telepítése PC-re vagy Mac gépre](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) című témakörben talál további információt.

## <a name="see-also"></a>Lásd még

[Microsoft 365 Vállalati verziós oktatóvideók](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)

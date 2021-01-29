---
title: A Microsoft 365 Vállalati prémium verzió beállítása
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
description: Megismerheti a Microsoft 365 Vállalati prémium verzió beállítási lépéseit, például tartomány és felhasználók hozzáadását, biztonsági házirendek beállítását és sok más lépést.
ms.openlocfilehash: e7ebe179c67077dc71ae4873b0711d0e810c701a
ms.sourcegitcommit: 1b30ac6e05906c8a014b1fed33fc71e1821f6ad2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/29/2021
ms.locfileid: "50044730"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a>A Microsoft 365 Vállalati prémium verzió beállítása a beállítási varázslóban

Ebből a videóból áttekintheti a Microsoft 365 Vállalati prémium verzió beállítását.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a>Tartomány, felhasználók hozzáadása és házirendek beállítása

A Microsoft 365 Vállalati prémium verzió megvásárlásakor lehetősége van saját tartományt használni, vagy a regisztráció során vásárolni [egyet.](sign-up.md)

- Ha a feliratkozáskor új tartományt vásárolt, a tartománya be van állítva, és áthelyezheti a Felhasználók hozzáadása és licencek [hozzárendelése gombra.](#add-users-and-assign-licenses)

### <a name="add-your-domain-to-personalize-sign-in"></a>Tartomány hozzáadása a bejelentkezés személyre szabása

1. Jelentkezzen be a [Microsoft 365](https://admin.microsoft.com) Felügyeleti központba a globális rendszergazdai hitelesítő adataival. 

2. A **varázslót az Ugrás** a beállításhoz gombra állítva indítsa el.

    ![Válassza az Ugrás a beállításhoz lehetőséget.](../media/gotosetupinadmincenter.png)

3. Az **Office-alkalmazások telepítése** lapon tetszés szerint telepítheti az appokat a saját számítógépére.
    
4. A Tartomány **hozzáadása lépésben** adja meg a használni kívánt tartománynevet (például contoso.com).

    > [!IMPORTANT]
    > Ha a regisztráció során tartományt vásárolt, itt nem látható a Tartomány **hozzáadása** lépés. Ehelyett a [Felhasználók hozzáadása gombra.](#add-users-and-assign-licenses)

    ![Képernyőkép a Bejelentkezési lap személyre szabása lapról.](../media/adddomain.png)

    
4. A varázsló lépéseit követve hozza létre a DNS-rekordokat a [Microsoft 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) bármely OLYAN DNS-szolgáltatójánál, amely igazolja, hogy Öné a tartomány. Ha ismeri a tartománygazdát, olvassa el a [szolgáltatóra vonatkozó utasításokat is.](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)

    Ha tárhelyszolgáltatója a GoDaddy vagy egy tartomány-csatlakozással engedélyezett másik [szolgáltató,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)a folyamat egyszerű, és a rendszer automatikusan kérni fogja, hogy jelentkezzen be, és hagyja, hogy a Microsoft hitelesítse magát az Ön nevében.

    ![On GoDaddy Confirm Access page, select Authorize.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Felhasználók felvétele és licencek hozzárendelése

Felvehet felhasználókat a varázslóba, de [](add-users-m365b.md) később a Felügyeleti központban is felvehet felhasználókat. Ha pedig helyi tartományvezérlője van, felhasználókat is felvehet az [Azure AD Connect használatával.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

#### <a name="add-users-in-the-wizard"></a>Felhasználók hozzáadása a varázslóban

A varázslóban hozzáadt felhasználók automatikusan hozzárendelnek egy Microsoft 365 Vállalati prémium verziós licencet.

![Képernyőkép a varázsló Új felhasználók hozzáadása lapról](../media/addnewuserspage.png)

1. Ha Microsoft 365 Vállalati prémium verziós előfizetése meglévő felhasználókkal rendelkezik (például ha az Azure AD Connectet használta), akkor most lehetősége van licenceket rendelni hozzájuk. Nyugodtan felvehet licenceket hozzájuk is.

2. A felhasználók hozzáadása után a hitelesítő adatokat is megoszthatja a felvett új felhasználókkal. Ezeket kinyomtathatja, elküldheti e-mailben, vagy pedig letöltheti.

### <a name="connect-your-domain"></a>Tartomány csatlakoztatása

> [!NOTE]
> Ha az .onmicrosoft tartományt választotta, vagy az Azure AD Connectet használta a felhasználók beállítására, ez a lépés nem látható.
  
A szolgáltatások beállításához frissítenie kell bizonyos rekordokat a DNS-szolgáltatónál vagy a tartományregisztrálónál.
  
1. A beállítási varázsló általában felismeri a regisztrálóját, és részletes útmutatást jelenít meg arról, hogy miként frissítheti a névkiszolgálói rekordokat a regisztráló webhelyén. Ha nem, módosítsa a névkiszolgálókat úgy, hogy a [Microsoft 365-öt bármely tartományregisztrálónál beállítsa.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar) 

    - Ha már van DNS-rekordja, például egy meglévő webhelye, [](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)de a DNS-szolgáltató engedélyezte a tartományhoz való csatlakozást, válassza a Rekordok hozzáadása **lehetőséget.** Az Online **szolgáltatások kiválasztása** lapon fogadja el az összes alapértelmezett beállítást, válassza a Tovább **gombot,** és válassza az **Authorize** (Engedély) lehetőséget a DNS-szolgáltató lapján.
    - Ha már van DNS-rekordja más DNS-szolgáltatónál (a tartományhoz való csatlakozáshoz nincs engedélyezve), akkor saját DNS-rekordokat kell kezelnie, hogy a meglévő szolgáltatások kapcsolatban maradjanak. További [információt a tartományi alapismeretek](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) között láthat.

        ![Rekordok aktiválása lap.](../media/activaterecords.png)

2. Kövesse a varázsló lépéseit, és állítsa be Önnek a levelezést és más szolgáltatásokat.

### <a name="protect-your-organization"></a>A szervezet védelme 

A varázslóban beállított házirendeket [a](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) program automatikusan alkalmazza a Minden felhasználó nevű biztonsági *csoportra.* A felügyeleti központban további csoportokat is létrehozhat, amelyekhez házirendeket rendelhet hozzá.

1. A **speciális** kiberfenyegetések elleni védelem növelése érdekében javasoljuk, hogy hagyja, hogy az [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) átolvassa az Office-appokban lévő fájlokat és hivatkozásokat.

    ![Képernyőkép a Védelem növelése lapról](../media/increasetreatprotection.png)


2. A  bizalmas adatok kiszivárgásának megelőzése lapon fogadja el az Office 365 Adatveszteség-megelőzés (DLP) alapértelmezett beállítását a bizalmas adatok nyomon követéséhez az Office-appokban, és megakadályozza, hogy a szervezeten kívüli adatok véletlenül meg is oszthatóak.

3. Az **Office** mobileszközökre vonatkozó adatainak védelme lapon hagyja be a mobilappok kezelését, bontsa ki a beállításokat, és tekintse át őket, majd válassza a Mobilappkezelési házirend **létrehozása lehetőséget.**

    ![Képernyőkép az Adatok védelme lapról a Mobil Office-ban.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Windows 10-es PC-k biztonságossá teve

A bal oldali navigációs sávon válassza a **Beállítás** lehetőséget, majd a Bejelentkezés és biztonság alatt válassza a **Windows 10-es számítógépek biztonságának biztosítása lehetőséget.** Első **lépésekhez** válassza a Nézet lehetőséget. A [teljes útmutatást a Windows 10-es](secure-win-10-pcs.md) számítógépek biztonságának biztosítása érdekében olvassa el.

## <a name="deploy-office-365-client-apps"></a>Office 365-ügyfélalkalmazások telepítése

Ha a telepítés során úgy döntött, hogy automatikusan telepíti az Office-appokat, az appok a Windows 10-es eszközökre fognak telepíteni, miután a felhasználók bejelentkeztek az Azure AD-be a windowsos eszközükről a munkahelyi hitelesítő adataik használatával.

Az Office mobilos iOS- vagy Android-eszközökre való telepítéséhez lásd: Mobileszközök beállítása [a Microsoft 365 Vállalati prémium verzió felhasználóinak.](set-up-mobile-devices.md)

Az Office-t külön is telepítheti. Útmutatásért [olvassa el az Office telepítése PC-re](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) vagy Mac gépre.

## <a name="see-also"></a>Lásd még

[Microsoft 365 Vállalati verziós oktatóvideók](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)

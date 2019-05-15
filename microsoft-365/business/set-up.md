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
description: Útmutató a Microsoft 365 üzleti beállítása.
ms.openlocfilehash: 42a35810531b6abd5b22e5fdbce2c0cfea57b8d7
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/15/2019
ms.locfileid: "34074590"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>A telepítővarázsló a Microsoft 365 üzleti beállítása

## <a name="add-your-domain-users-and-set-up-policies"></a>Adja hozzá a tartományi felhasználók és a házirendek beállítása

![Mutató transzparens https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

Microsoft 365 üzleti beszerzése esetén a saját tartomány használata, vagy a vásárlás során lehetőség van az [Internet-előfizetési](sign-up.md).

- Ha új tartomány létrehozása során vásárolt, a tartomány összes fel, és Ugrás [felhasználók hozzáadása és a licencek hozzárendelése](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Az egyéni bejelentkezési tartomány hozzáadása

1. Jelentkezzen be a [Microsoft 365 felügyeleti központ](https://admin.microsoft.com) a globális rendszergazdai hitelesítő adatok használatával. 

2. Kattintson a **Hozzáadás a tartományhoz** vagy a **felhasználók hozzáadása** varázsló elindításához.
    > [!IMPORTANT]
    > Ha a regisztráció során vásárolt egy tartomány, a program nem lásd: **tartomány hozzáadása** lépés itt. Ugrás a [felhasználók hozzáadása](#add-users-and-assign-licenses) helyett.

    ![Jelölje be a tartomány hozzáadása.](media/addadomainadmincenter.png)
    
3. A varázslóban adja meg a tartomány nevét (például contoso.com) használni kívánt.


    ![Képernyőkép a személyre szabás Bejelentkezés lapon.](media/personalizesignin.png)

    
4. Ellenőrzi a saját tartomány [létrehozása DNS-rekordokat az Office 365 bármely DNS-szolgáltatójánál,](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) kövesse a varázsló utasításait. Ha ismeri a tartományi állomás, lásd még: [állomás konkrét utasításokat](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Ha a videotár-szolgáltató GoDaddy, a folyamat egyszerű és program automatikusan kéri, jelentkezzen be, és hagyja, hogy a nevünkben hitelesíti a Microsoft:

    ![GoDaddy megerősítése adatelérési lapon jelölje be az engedélyezés.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Felhasználók felvétele és licencek hozzárendelése

A varázslóban hozzáadhat felhasználókat, de is [újabb felhasználók hozzáadása](add-users-m365b.md) a felügyeleti központban. Ezenkívül ha a helyi tartományvezérlő, hozzáadhat [Azure AD csatlakozás](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)rendelkező felhasználók.

#### <a name="add-users-in-the-wizard"></a>Felhasználók hozzáadása varázsló

A varázsló felvett felhasználóknak Microsoft 365 üzleti licenc beszerzése automatikusan.

![Képernyőkép a Hozzáadás új felhasználó lapon a varázsló](media/addnewuserspage.png)

1. Ha a Microsoft 365 üzleti előfizetés (például, ha Azure AD csatlakozás) a meglévő felhasználók, licencek hozzárendelése őket most lehetőséget kap. Nyugodtan felvehet licenceket hozzájuk is.

3. Miután hozzáadta a felhasználók, a hozzáadott új felhasználók hitelesítő adatok megosztása lehetőséget is fog kapni. Ezeket kinyomtathatja, elküldheti e-mailben, vagy pedig letöltheti.

4. Hagyja ki az e-mail-üzenetek áttelepítését, és kattintson a **Tovább** gombra az **E-mail-üzenetek áttelepítése** lapon. 

    Ha áthelyezni egy másik e-mail szolgáltatójától, és később az adatok másolásához, akkor [e-mail áttelepítése és az Office 365 ügyfeleket](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).


### <a name="connect-your-domain"></a>Tartomány csatlakoztatása

> [!NOTE]
> Ha a .onmicrosoft tartomány használata mellett, vagy Azure AD csatlakozás segítségével a felhasználók beállítása, ez a lépés nem jelenik meg.
  
A szolgáltatások beállításához frissítenie kell bizonyos rekordokat a DNS-szolgáltatónál vagy a tartományregisztrálónál.
  
1. A beállítási varázsló általában felismeri a regisztrálóját, és részletes útmutatást jelenít meg arról, hogy miként frissítheti a névkiszolgálói rekordokat a regisztráló webhelyén. Ha nem, [Módosítás nameservers beállítása az Office 365 bármely tartomány tartományneveket regisztráló szervezetnél](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Ha meglévő DNS-rekordok, például egy létező webhelyen, érdemes kapcsolattartásra a meglévő szolgáltatások biztosításához a saját DNS-rekordok kezeléséhez. További információ a [tartomány alapjai](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) témakörben talál.

        ![Csatlakozás a tartomány lap i. fogja kezelni a saját DNS-rekordokat.](media/connectyourdomainpage.png)

2. Kövesse a varázsló utasításait, és e-mail és egyéb szolgáltatások hoznak létre meg.

### <a name="set-up-security-policies-and-device-configurations"></a>Állítsa be a biztonsági házirendek és az eszközök konfigurációja 

A házirendek beállítása varázsló automatikusan alkalmazni *Minden felhasználó*létrehoz egy [biztonsági csoportot](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) . A felügyeleti központ házirendek hozzárendelése további csoportokat is létrehozhat.

1. A **mobil eszközökön a munka fájlok védelme** a beállítás **védelme Munkafájlok, ha elveszett vagy ellopott eszköz** alapértelmezés szerint van jelölve. Akkor **kezelheti, hogy a felhasználók miként férhetnek hozzá a mobil eszközökön tárolt Office fájlokhoz**bekapcsolása lehetőséget, és ez ajánlott.

    ![Munkafájlok védelme Képernyőkép a mobileszközök lapon.](media/protectworkfilesondevices.png)

     - Bontsa ki az [alapértelmezett értékek](protect-work-files-on-lost-or-stolen-device.md)megjelenítése **védelme Munkafájlok, ha elveszett vagy ellopott eszközök** :

        ![Képernyőkép a elveszett eszköz fájlok védelme alapértelmezett értékeit.](media/protectworkfilesondevicesdefault.png)

    - Jelölje ki a **kezelni, hogy a felhasználók miként férhetnek hozzá a mobil eszközökön található Office-fájlokat** , és bontsa ki az [alapértelmezett értékeinek](manage-user-access-on-mobile-devices.md)megjelenítése. Azt javasoljuk, hogy elfogadja az alapértelmezett értékeket, Android, iOS és a Windows 10 alkalmazás-házirendek létrehozásához a telepítés során, amelyek minden felhasználóra vonatkoznak. A telepítés után további házirendeket is létrehozhat majd.

        ![Képernyőkép a védelmi beállításait a hordozható Office-fájlokat.](media/useraccessonmobile.png)

2. Az utolsó lépés az adatok védelmét és az eszköz lehetővé teszi a házirendek beállítása Windows 10 eszközök biztonságos. Ezek a beállítások automatikusan érvényesek, ha a felhasználó Windows 10 csatlakozik a szervezet. Kibonthatja a **biztonságos Windows 10 eszközök** és az [alapértelmezett értékek](secure-windows-10-devices.md)módosíthatók.
3. Választhatja azt is, [automatikus telepítése az Office](install-office-on-windows-10-during-setup.md) eszközök a Windows 10.

    ![Képernyőkép a Windows 10 eszköz konfigurációs lapon állítsa be.](media/setwin10config.png)



## <a name="deploy-office-365-client-apps"></a>Telepítse az Office 365 ügyfélalkalmazások

Ha azt választotta, hogy automatikusan telepíti az Office-alkalmazások a telepítéskor ki, az apps telepíti a Windows 10 eszközök után a felhasználó bejelentkezett az Azure AD a munka hitelesítő adatokkal a Windows eszközök.
Office telepítése mobil iOS vagy Android-eszköz, lásd: [állítsa be a mobil eszközök Microsoft 365 üzleti felhasználók számára](set-up-mobile-devices.md).

Office külön-külön is telepíthető. Lásd: [PC vagy Mac Office telepítéséhez](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) további útmutatást.

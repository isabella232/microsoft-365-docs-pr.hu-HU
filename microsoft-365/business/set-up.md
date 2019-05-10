---
title: A Microsoft 365 Business beállítása
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
ms.openlocfilehash: e635b828609fc47cd8b92bb179a25bcc43cb0a1a
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660809"
---
# <a name="set-up-microsoft-365-business"></a>A Microsoft 365 Business beállítása

Mielőtt elkezdené, előfizetési információt [Kaphat a Microsoft 365 üzleti](get-microsoft-365-business.md) talál.

Tekintse meg egy [rövid videó a Microsoft 365 üzleti beállítása](https://support.office.com/article/38003e30-9d10-44cf-b596-f1b5f662bfa1) a készlet varázsló, és ha nem rendelkezünk a helyszíni Active Directory használatával
  

## <a name="overview"></a>Áttekintés

Lépéseket beállítása a legtöbb elvégezhető a telepítő varázsló, de az egyéb beállítások is szerepelnek.

1. [A tartomány hozzáadása](#add-your-domain-to-personalize-sign-in) (a domain [regisztráció](sign-up.md)során vásárolt, ha ez a lépés már megtörtént.)
2. Felhasználók hozzáadása. Ez a három módokon teheti meg:
    - A [telepítő varázsló](#add-users-in-the-wizard).
    - Ha a helyszíni Active directory [Azure AD csatlakozás segítségével a felhasználók](#add-users-by-using-azure-ad-connect) hozzáadása a címtárszinkronizálás használata
    - Is [újabb felhasználók hozzáadása](add-users-m365b.md) a felügyeleti központban.
3. Biztonsági házirendek beállítása, és eszközök konfigurálása. Ez a három módokon teheti meg:
    - A [telepítő varázsló](#set-up-policies-in-the-wizard).  
    - A [felügyeleti központ](#modify-or-add-policies-in-the-admin-center).
    - A [felügyeleti központ Intune](https://docs.microsoft.com/intune/what-is-device-management).
4. Állítsa be és Eszközkezelés Windows 10.

    Azure ad WIndows 10 eszköz csatlakoztatásakor a házirendeket a rendszer alkalmazza azt.
    - A [telepítő varázsló](#set-up-policies-in-the-wizard)a Windows 10 eszköz konfigurációjának beállítása.
    - Borzas AD egy [új Windows 10 eszköz](set-up-windows-devices.md#for-a-brand-new-or-newly-upgraded-windows-10-pro-device) csatlakoztatása.
    - Borzas AD egy [meglévő Windows 10 eszköz](set-up-windows-devices.md#for-a-device-already-set-up-and-running-windows-10-pro) csatlakoztatása.
1. Telepítse az Office 365 üzleti.
    - A [telepítő varázsló](#set-up-policies-in-the-wizard)segítségével a Windows-eszközök automatikusan telepíthető Office.
    - Automatikusan [az Office telepítése](auto-install-or-uninstall-office.md) az admin center.
    - Lehetővé teszik a felhasználók [Office alkalmazások telepítése](https://docs.microsoft.com/office365/admin/setup/install-applications) a Windows és az eszközök.
     
1. További biztonsági beállítása.
    - A telepítő varázsló az eszközök biztonságos házirendeket ad, de azt is kihasználhatják a [további biztonsági](#additional-security-settings) szolgáltatásainak segítségével biztonságos segít az adatok, partnerek és e-mailek. 

## <a name="add-your-domain-users-and-set-up-policies"></a>Adja hozzá a tartományi felhasználók és a házirendek beállítása

![Mutató transzparens https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

Microsoft 365 üzleti beszerzése esetén a saját tartomány használata, vagy a vásárlás során lehetőség van az [Internet-előfizetési](sign-up.md).

- Ha új tartomány létrehozása során vásárolt, a tartomány összes fel, és Ugrás [felhasználók hozzáadása és a licencek hozzárendelése](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Az egyéni bejelentkezési tartomány hozzáadása

1. Jelentkezzen be a [Microsoft 365 felügyeleti központ](https://admin.microsoft.com) a globális rendszergazdai hitelesítő adatok használatával. 

2. Válassza ki **a tartomány hozzáadása** varázsló elindításához.

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
Ha tartomány tartományvezérlőjét, és az Active Directory használata, lásd: [ddd felhasználók Azure AD csatlakozás segítségével](#add-users-by-using-azure-ad-connect).

![Képernyőkép a Hozzáadás új felhasználó lapon a varázsló](media/addnewuserspage.png)

1. Ha az Microsoft 365 Business-előfizetéshez tartoznak meglévő felhasználók (például ha az Azure AD Connect szolgáltatást használta), akkor itt lehetősége lesz licenceket rendelheti hozzájuk. Nyugodtan felvehet licenceket hozzájuk is.

3. Miután hozzáadta a felhasználók, a hozzáadott új felhasználók hitelesítő adatok megosztása lehetőséget is fog kapni. Ezeket kinyomtathatja, elküldheti e-mailben, vagy pedig letöltheti.

4. Hagyja ki az e-mail-üzenetek áttelepítését, és kattintson a **Tovább** gombra az **E-mail-üzenetek áttelepítése** lapon. 

    Ha áthelyezni egy másik e-mail szolgáltatójától, és később az adatok másolásához, akkor [e-mail áttelepítése és az Office 365 ügyfeleket](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).

#### <a name="add-users-by-using-azure-ad-connect"></a>Borzas AD csatlakozás segítségével a felhasználók hozzáadása

 Ha az Active Directory tartomány tartományvezérlőjét, a felhasználók és szinkronizálása Microsoft 365 üzleti [Azure AD csatlakozás](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)segítségével. Végezze el ezt a telepítő varázsló elindítása előtt. A felügyeleti központ letölthető:

- Keresse fel **a felhasználók** \> **aktív felhasználók**, az oldal tetején található az ellipszisek válassza, majd **a címtárszinkronizálás** Azure AD csatlakozás letöltése.

    ![Az aktív felhasználók lapján válassza ki az ellipszisek > könyvtár snchronization.](media/setupdirsync.png)

    > [!IMPORTANT]
    > Ha ezzel a módszerrel hoz létre a felhasználók, még akkor rendelhet licenceket azokat a felügyeleti központ.

##### <a name="continue-to-access-domain-joined-apps-and-devices"></a>Továbbra is elérhető a tartományhoz tartozó alkalmazások és eszközök

Ha továbbra is elérhető a tartományhoz tartozó alkalmazások és eszközök, olvassa el az alábbi cikkekből, amelyek lehetővé teszik, hogy két különböző módon:
  
- [A tartományhoz csatlakoztatott Windows 10-es eszközök kezelésének engedélyezése a Microsoft 365 Vállalati verzió számára](manage-windows-devices.md)
    - Ez az ajánlott módja.

- [Hozzáférés a helyi erőforrások egy Azure AD csatlakozott eszközről a Microsoft 365 Business](access-resources.md)

### <a name="connect-your-domain"></a>Tartomány csatlakoztatása

> [!NOTE]
> Ha a .onmicrosoft tartomány használata mellett, vagy Azure AD csatlakozás segítségével a felhasználók beállítása, ez a lépés nem jelenik meg.
  
A szolgáltatások beállításához frissítenie kell bizonyos rekordokat a DNS-szolgáltatónál vagy a tartományregisztrálónál.
  
1. A beállítási varázsló általában felismeri a regisztrálóját, és részletes útmutatást jelenít meg arról, hogy miként frissítheti a névkiszolgálói rekordokat a regisztráló webhelyén. Ha nem, [Módosítás nameservers beállítása az Office 365 bármely tartomány tartományneveket regisztráló szervezetnél](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Ha meglévő DNS-rekordok, például egy létező webhelyen, érdemes kapcsolattartásra a meglévő szolgáltatások biztosításához a saját DNS-rekordok kezeléséhez. További információ a [tartomány alapjai](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) témakörben talál.

        ![Csatlakozás a tartomány lap i. fogja kezelni a saját DNS-rekordokat.](media/connectyourdomainpage.png)

2. Kövesse a varázsló utasításait, és e-mail és egyéb szolgáltatások hoznak létre meg.

### <a name="set-up-security-policies-and-device-configurations"></a>Állítsa be a biztonsági házirendek és az eszközök konfigurációja 

Ezek a házirendek vonatkoznak minden felhasználó adhat a licencet, vagy a felhasználók egy csoportja, ha úgy dönt, hogy a felhasználók egy csoportja különböző házirendek hozzárendelése.

#### <a name="set-up-policies-in-the-wizard"></a>A varázsló házirendek beállítása

A házirendek beállítása varázsló automatikusan alkalmazni *Minden felhasználó*létrehoz egy [biztonsági csoportot](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) .

1. A **mobil eszközökön a munka fájlok védelme** a beállítás **védelme Munkafájlok, ha elveszett vagy ellopott eszköz** alapértelmezés szerint van jelölve. Akkor **kezelheti, hogy a felhasználók miként férhetnek hozzá a mobil eszközökön tárolt Office fájlokhoz**bekapcsolása lehetőséget, és ez ajánlott.

    ![Munkafájlok védelme Képernyőkép a mobileszközök lapon.](media/protectworkfilesondevices.png)

     - Bontsa ki a **védelem Munkafájlok, ha az eszköz elveszett vagy ellopott**, ha az [alapértelmezett értékek](protect-work-files-on-lost-or-stolen-device.md) előre kiválasztott:

        ![Képernyőkép a elveszett eszköz fájlok védelme alapértelmezett értékeit.](media/protectworkfilesondevicesdefault.png)

    - Ha bejelöli a **kezelése, hogy a felhasználók miként férhetnek hozzá a mobil eszközökön található Office-fájlok** kibontásához, az [alapértelmezett értékek](manage-user-access-on-mobile-devices.md) jelennek meg. Azt javasoljuk, hogy a telepítés során fogadja el azokat az alapértelmezett értékeket, amelyekkel minden felhasználóra vonatkozó alkalmazásházirendeket hozhat létre Android, iOS és Windows 10 rendszerekre. A telepítés után további házirendeket is létrehozhat majd.

        ![Képernyőkép a védelmi beállításait a hordozható Office-fájlokat.](media/useraccessonmobile.png)

2. Az utolsó lépés az adatok védelmét és az eszköz lehetővé teszi a házirendek beállítása Windows 10 eszközök biztonságos. Ezek a beállítások automatikusan érvényesek, ha a felhasználó Windows 10 csatlakozik a szervezet. Kibonthatja a **biztonságos Windows 10 eszközök** és az [alapértelmezett értékek](secure-windows-10-devices.md)módosíthatók.
3. Választhatja azt is, [automatikus telepítése az Office](install-office-on-windows-10-during-setup.md) eszközök a Windows 10.

    ![Képernyőkép a Windows 10 eszköz konfigurációs lapon állítsa be.](media/setwin10config.png)

#### <a name="modify-or-add-policies-in-the-admin-center"></a>Módosítsa vagy adja hozzá a házirendek a felügyeleti központ

Lásd a [Microsoft 365 tevékenység kezelésére](manage.md) vonatkozó házirendek hogyan lehet megtekinteni és módosítani az eszköz-és app témakörökre mutató hivatkozásokat, és hogyan adatainak eltávolítása vagy visszaállítása a felhasználói eszközök.

## <a name="deploy-and-manage-windows-10"></a>Telepítését és kezelését a Windows 10
Manuális csatlakoztatása Azure AD, vagy új számítógépek, illetve a meglévő számítógépek bejelentkezési profil módosításával a telepítés során a [Microsoft 365 üzleti felhasználók számára a Windows-eszközök beállítása](set-up-windows-devices.md) témakörben található. 

### <a name="use-autopilot-to-set-up-new-devices"></a>Automata segítségével állítsa be az új eszközök

[Windows automata](add-autopilot-devices-and-profile.md) segítségével automatikusan előre konfigurálja egy felhasználó **Új** Windows 10 eszközök, de lehet egyszerűbben, egy [partner](https://www.microsoft.com/solution-providers/search) , aki teheti meg. Ugrás a [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) is, és kérje meg a felhő technológia szakértői vásárol meg az új eszközök beállítása.

### <a name="access-on-premises-resources"></a>Helyi erőforrások eléréséhez.

Ha a szervezet használja a Windows Server Active Directory helyszíni, állíthat be Microsoft 365 üzleti védelme érdekében a Windows 10 eszközök továbbra is fenntartva helyi hitelesítést igénylő helyszíni erőforrásokhoz való hozzáférést. Kövesse a [Microsoft 365 üzleti által kezelt tartományhoz tartozó Windows 10 eszközök engedélyezése](manage-windows-devices.md) meg. Ez a javasolt módszer és eszközök ebben az állapotban úgynevezett hibrid Azure AD eszközöket csatlakozott.

Ha a vállalatnál a helyi Active Directory, amely tartalmazza az egyes helyi erőforrásokat (például fájlmegosztásokat és nyomtatókat), a Borzas AD csatlakoztatott eszközök hozzáférést biztosíthat a forrásokhoz való lépések itt: [Access helyszíni erőforrásokat egy 365 üzleti Microsoft Azure AD csatlakozott eszköz](access-resources.md).

## <a name="deploy-office-365-client-apps"></a>Telepítse az Office 365 ügyfélalkalmazások

Ha azt választotta, hogy automatikusan telepíti az Office-alkalmazások a telepítéskor ki, az apps telepíti a Windows 10 eszközök után a felhasználó bejelentkezett az Azure AD a munka hitelesítő adatokkal a Windows eszközök.
Office telepítése mobil iOS vagy Android-eszköz, lásd: [állítsa be a mobil eszközök Microsoft 365 üzleti felhasználók számára](set-up-mobile-devices.md).

Office külön-külön is telepíthető. Lásd: [PC vagy Mac Office telepítéséhez](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) további útmutatást.

## <a name="additional-security-settings"></a>További biztonsági beállítások

A biztonsági és kompatibilitási beállítást a telepítő varázsló mellett a következő további beállításokat is meg lehet:
  
- **E-mail rosszindulatú programok elleni védekezés**
- **Speciális veszély védelmi (ATP) biztonságos mellékletek**
- **ATP ajánlott hivatkozások**
- **APT adatlopás**
- **Exchange Online Archiválás**
- **Adatvesztés megelőzése (DLP)**
- **Borzas információk védelméről** (1 terv)
- **Intune portál elérhetősége**

Get elindítani a [Speciális biztonsági házirendek beállítása](set-up-advanced-security.md)című témakörben talál.

Lásd még: [365 a Microsoft üzleti biztonságos felső 10 mód](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) a legjobb biztonsági gyakorlatok ütemterv.
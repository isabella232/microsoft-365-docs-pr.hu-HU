---
title: A Microsoft 365 Business beállítása a beállítási varázslóval
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
description: Útmutató a Microsoft 365 üzleti beállítása négy lépés végrehajtásával.
ms.openlocfilehash: a1c8a41c3e291983276280a063248bdd10a7f85a
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32283911"
---
# <a name="set-up-microsoft-365-business-by-using-the-setup-wizard"></a>A Microsoft 365 Business beállítása a beállítási varázslóval

Hajtsa végre az alábbi 1 – 4.
  
### <a name="set-up-microsoft-365-business"></a>A Microsoft 365 Business beállítása

Ha helyszíni Active Directory nincs Microsoft 365 üzleti beállítása a videó megtekintése:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/0705c337-f3e8-4d28-bb6c-530cd28e99f2?autoplay=false]
  
A beállítási lépéseket a telepítéshez, amely tartalmazza a helyi Active Directory információkat tartalmazza. Ha továbbra is elérhető a tartományhoz csatlakoztatott eszközök, olvassa el az alábbi cikkekből, amelyek lehetővé teszik, hogy két különböző módon, és hajtsa végre a varázsló futtatása előtt:
  
- [A tartományhoz csatlakoztatott Windows 10-es eszközök kezelésének engedélyezése a Microsoft 365 Vállalati verzió számára](manage-windows-devices.md)
    
    -Ez az ajánlott módja.
    
- [Hozzáférés a helyi erőforrások egy Azure AD csatlakozott eszközről a Microsoft 365 Business](access-resources.md)
    
### <a name="step-1-personalize-sign-in"></a>1. lépés: A bejelentkezés testreszabása

1. Jelentkezzen be a [Microsoft 365 Business](https://portal.microsoft.com) szolgáltatásba a globális rendszergazdai hitelesítő adataival. A **Felügyelet** csempét választva lépjen a felügyeleti központba. 
    
2. Válassza a **Beállítás indítása** lehetőséget (az állapotától függően előfordulhat, hogy ehelyett a **Beállítás folytatása** elem látható) a felügyeleti központban a varázsló elindításához. 
    
3. Adja meg a használni kívánt tartomány nevét (például contoso.com).
    
    Nyugodtan megadhatja a tartományt akkor is, ha már ellenőrizte például az Azure AD Connect használata során. A következő két lépést nem vonatkoznak, ha Azure AD csatlakozás segítségével ellenőrizze a tartomány.
    
4. Ellenőrzi a saját tartomány [létrehozása DNS-rekordokat az Office 365 bármely DNS-szolgáltatójánál,](https://support.office.com/article/7b7b075d-79f9-4e37-8a9e-fb60c1d95166) kövesse a varázsló utasításait. 
    
    Megtekintheti egy példa videó [Videó: telepítés Office 365 az új Admin központban](https://support.office.com/article/a8c2002a-34bc-4ab3-93d8-9b5156c48bf8). Fontos megjegyezni, hogy a videóban nem szerepelnek az Microsoft 365 Business adatvédelmi lépései.
    
    ![Screenshot of the Business Cloud Suite setup wizard.](media/3c4fd40c-2de1-4a87-8ee0-78d3928c7bb7.png)
  
### <a name="step-2-add-users-and-assign-licenses"></a>2. lépés: Felhasználók hozzáadása és a licencek hozzárendelése

1. A felhasználókat felveheti itt, vagy [később is](add-users-m365b.md) a felügyeleti központban. 
    
    A rendszer minden felvett felhasználóhoz automatikusan hozzárendel egy Microsoft 365 Business-licencet.
    
2. Ha az Microsoft 365 Business-előfizetéshez tartoznak meglévő felhasználók (például ha az Azure AD Connect szolgáltatást használta), akkor itt lehetősége lesz licenceket rendelheti hozzájuk. Nyugodtan felvehet licenceket hozzájuk is.
    
3. Emellett arra is lesz lehetősége, hogy megossza a hitelesítő adatokat a felvett új felhasználókkal. Ezeket kinyomtathatja, elküldheti e-mailben, vagy pedig letöltheti.
    
4. Hagyja ki az e-mail-üzenetek áttelepítését, és kattintson a **Tovább** gombra az **E-mail-üzenetek áttelepítése** lapon. 
    
    Ha áthelyezni egy másik e-mail szolgáltatójától, és később az adatok másolásához, akkor [e-mail áttelepítése és az Office 365 ügyfeleket](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).
    
    ![Screenshot of two new users added in the setup wizard](media/8f729967-5c65-4ceb-b737-18119db40564.png)
  
### <a name="step-3-connect-your-domain"></a>3. lépés: Csatlakozás a tartomány

> [!NOTE]
> Ha a .onmicrosoft tartomány használata mellett, vagy Azure AD csatlakozás használt, ez a lépés nem jelenik meg. 
  
A szolgáltatások beállításához frissítenie kell bizonyos rekordokat a DNS-szolgáltatónál vagy a tartományregisztrálónál.
  
1. A beállítási varázsló általában felismeri a regisztrálóját, és részletes útmutatást jelenít meg arról, hogy miként frissítheti a névkiszolgálói rekordokat a regisztráló webhelyén. Ha nem, [Módosítás nameservers beállítása az Office 365 bármely tartomány tartományneveket regisztráló szervezetnél](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).
    
2. A levelezési és egyéb szolgáltatásokat a rendszer beállítja Önnek
    
### <a name="step-4-manage-devices-and-work-files"></a>4. lépés: Eszközök kezelése és fájlok használata

1. A **Munkafájlok védelme a mobileszközök** lap beállítása **védelme Munkafájlok, ha elveszett vagy ellopott eszközök** és a beállítások **kezelése, hogy a felhasználók miként férhetnek hozzá a mobil eszközökön tárolt Office fájlokhoz** **a**. Minden rész beállításra kattintva minden beállítás a chevron is elérhető.
  
  A licenccel rendelkező felhasználók munka fájlokat most védett iOS és Android-eszköz, azokat a lehető leghamarabb [telepítse az Office alkalmazások](set-up-mobile-devices.md) (és azok Microsoft 365 üzleti hitelesítő adatokkal hitelesítik). 
  
  ![Screenshot of protect work files on your mobile devices page](media/3139a9aa-6228-4e74-8166-c6a886d7319f.PNG)
  
2. A **Windows 10 beállítása eszköz konfigurációs** lapon állítsa be a **Windows 10 eszközök biztonságos** **meg**.
  
   Minden rész beállítás mellett a francia idézőjelre kattintva is elérheti.
  
3. Állítsa be az **Office telepítése Windows 10 eszközök** **Igen** Ha minden felhasználó Windows 10 számítógéppel rendelkezik, és telepíti vagy nem létező Office vagy Office-telepítések való kattintásra. Ha nem ez a helyzet, ez a beállítás **nem**értékre. Lehetőség van [automatikus telepítése az Office](auto-install-or-uninstall-office.md) újabb admin közepétől már rendelkezésre állnak a felhasználó számítógépére. Útmutatásért lásd: az [Office ügyfél telepítésének előkészítéséhez](prepare-for-office-client-deployment.md).
  
    Munkafájlok licenccel rendelkező felhasználók a Windows 10 eszközök, amint azok tervezett fog [csatlakozni a Windows 10 eszköz](set-up-windows-devices.md) Microsoft 365 Business Azure AD tartomány vagy [Windows 10 új számítógépre telepíti](https://support.office.com/article/c654bd23-d256-4ac7-8fba-0c993bf5a771.aspx) a Microsoft 365 egyidejűleg csatlakozó Üzleti Azure Active Directory-tartománynak. 
  
4. Kattintson a **Tovább** gombra, és a telepítő befejezte. 
  
    Kérjük visszajelzés nekünk ennél a lépésnél segítheti a tapasztalat.
  
    ![Screenshot of Prepare Windows 10 devices page](media/bff701c1-48a3-44f4-aa95-9d959d57c85b.PNG)
  
## <a name="additional-security-settings"></a>További biztonsági beállítások

A biztonsági és kompatibilitási beállítást a telepítő varázsló mellett a következő további beállításokat is meg lehet:
  
- Állítsa be a nem biztonságos mellékletek elleni védelem. **Speciális veszély védelmi** (ATP) azonosítja a rosszindulatú tartalmat, és adathalászó sémák és ransomware fertőzések elleni védelme, majd blokkolja a nem biztonságos mellékletek, szállítás. Melléklet védelem aktiválása, lásd: [Office 365 ATP biztonságos mellékletek házirendek beállítása](https://support.office.com/article/078eb946-819a-4e13-8673-fe0c0ad3a775#setpolicy).
    
- A környezet védelme, amikor a felhasználó a rosszindulatú hivatkozások kattint. ATP megvizsgálja e-mailben található hivatkozásokra, amikor a felhasználó rájuk kattint. Ha a kapcsolat nem biztonságos, a felhasználó figyelmeztetést arról, hogy nem a webhelyen vagy tájékoztatták, hogy a hely le van tiltva. Ez segít az adatlopás elleni védelem. [Office 365 ATP biztonságos csatolások házirendek beállítása](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#reveddefaultscc) , vagy [Office 365 ATP biztonságos csatolások házirendek beállítása](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#addemailpolscc).
    
- Minden postaláda tartalom, beleértve a törölt elemek helyezi a felhasználó teljes postaláda **peres eljárás tartsa**megőrizhető. Útmutatásért lásd: 
- [E-mail adatmegőrzési az Exchange Online archiválás beállítása](security-features.md#set-up-email-retention-with-exchange-online-archiving).
    
- Állítsa be egyéni **adatmegőrzési szabályok**, például egy bizonyos meghatározott ideig megőrizni és tartalom véglegesen törli a birtokon tartási időszak végén. Engedélyezheti az értékpapírok és a Megfelelési központba, keresse fel az **adatok kormányzás** egyéni adatmegőrzési \> **fenntartását**, és kövesse a varázsló utasításait. További [adatmegőrzési szabályok – áttekintés](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423)című témakörben talál.
    
## <a name="next-steps"></a>Következő lépések

A licencekkel már rendelkező felhasználóknak következő lépésként be kell állítaniuk az eszközeiket.<br/> Lásd: [Windows rendszerű eszközök beállítása a Microsoft 365 Business felhasználóinak](set-up-windows-devices.md) és [Mobileszközök beállítása a Microsoft 365 Business felhasználóinak](set-up-mobile-devices.md). <br/>[A Microsoft 365 Business kezelése](manage.md) című témakörben olyan hivatkozásokat talál, amelyekre kattintva az eszköz és az appvédelmi házirendek beállításával és az adatok felhasználói eszközökről történő eltávolításával foglalkozó cikkek érhetők el. 
  



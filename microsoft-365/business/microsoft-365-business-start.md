---
title: A Microsoft 365 Business használatbavétele
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Ismerje meg, hogyan állítsa be a Microsoft 365 Business.
ms.openlocfilehash: d309700761ee48ef66a8cd3886fd416c79463ed5
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/15/2019
ms.locfileid: "34074300"
---
# <a name="get-started-with-microsoft-365-business"></a>A Microsoft 365 Business használatbavétele

## <a name="what-is-microsoft-365-business"></a>Mi a Microsoft 365 Vállalati verzió?

A Microsoft 365 Vállalati verzió a vállalati hatékonyságot és együttműködést elősegítő eszközök átfogó gyűjteménye, amely például olyan termékeket tartalmaz, mint az Outlook, a Word, az Excel és egyéb Office-termékek, amelyek mindig naprakészek. Az egyszerűen kezelhető, nagyvállalati szintű biztonsági funkciókkal minden iOS, Android és Windows 10 rendszerű eszközén megvédheti a munkahelyi fájljait.
  
A Microsoft 365 Business legfeljebb 300 licenccel való használatra készült. Ha ennél több licencre van szüksége, további információért olvassa el a [Microsoft 365 Nagyvállalati verzió](https://go.microsoft.com/fwlink/p/?linkid=860986) dokumentációját. 
  
## <a name="get-microsoft-365-business"></a>A Microsoft 365 Vállalati verzió beszerzése

- Ha van partnere, az illető meg fogja kapni a Microsoft 365 Businesst: [A Microsoft 365 Vállalati verzió beszerzése a Microsoft Partnerközpontban](get-microsoft-365-business.md).
    
- Ha nincs partnere, és meg szeretné vásárolni a Microsoft 365 Businesst, [itt megteheti](https://www.microsoft.com/en-us/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>A Microsoft 365 Vállalati verzió beállítása

 **Microsoft 365 Business Suite beállítása – áttekintés**
  
A következő ábra bemutatja, hogyan lehet a rendszergazdák a Microsoft 365 üzleti beállítani. Ezenkívül a Windows rendszerű PC-k Microsoft 365 Business használatára való előkészítésének lépéseit is tartalmazza. Új eszközöket is felvehet a Microsoft 365 Business Felügyeleti központban a [Windows AutoPilot](add-autopilot-devices-and-profile.md) segítségével. Ha az AutoPilot segítségével előre beállítja és konfigurálja az eszközöket, a felhasználók hatékonyan használhatják őket, amint bejelentkeznek a Microsoft 365 Business szolgáltatásban érvényes hitelesítő adataikkal.
  
![A diagram that shows the setup and management flow for admins, and also for a user](media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)
  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: Microsoft 365 Business (Admin) beállítása

Jelentkezzen be a [Microsoft 365 Vállalati verzió Felügyeleti központba](https://portal.office.com/adminportal/home) globális rendszergazdai hitelesítő adataival, majd a Microsoft 365 Business beállításához kövesse az alábbi lépéseket. 
  
1. [A Microsoft 365 Vállalati verziót tartalmazó eszközök adatvédelmének előfeltételei](pre-requisites-for-data-protection.md)
    
    Az eszközök kompatibilitásának ellenőrzéséhez elsőként olvassa el a Microsoft 365 Business előfeltételeit.
    
2. [A Microsoft 365 Vállalati verzió beállítása a beállítási varázslóval](set-up.md)
    
    Ha **véglegesen áthelyezése a helyi Active Directory a felhő**, vagy kézzel adhatók hozzá a felhasználók a Microsoft 365 üzleti felügyeleti központ a telepítő varázsló segítségével, vagy egy egyszeri szinkronizálás Azure AD csatlakozás a is elvégezheti. Ehhez két lehetőség közül választhat: 
    
  - Ha egy Exchange 2010, Exchange 2013 vagy Exchange 2016 kiszolgáló is rendelkezik, [Használata minimális hibrid gyors áttelepítése az Office 365 Exchange postaládákat](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef)is. A hibrid minimumkonfiguráció lépései részeként egyszeri szinkronizálást kell végeznie a felhasználókon az Azure AD-vel, valamint a helyszíni kiszolgálóról a felhőbe kell migrálnia az e-maileket. Ha ezt a módszert alkalmazza, az e-mail-migrálás befejeztével a program automatikusan kikapcsolja a címtár-szinkronizálást.
    
  - Az Office 365 címtár-szinkronizálási varázslójával szinkronizálhatja a felhasználókat a felhőbe. Ezt a [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) című cikk lépéseit követve végezheti el. Miután szinkronizálta a felhasználókat a felhőbe, [Turn off directory synchronization for Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Az ily módon felvett felhasználóknak ezenkívül a Microsoft 365 Vállalati verzióra szóló licencet kell adnia. Ehhez a [telepítő varázsló](set-up.md), vagy a [felhasználóknak az Office 365 rendszerben üzleti licencek hozzárendelése](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC).
    
### <a name="2-prepare-mobile-devices"></a>2: mobil eszközök előkészítése

Kövesse a lépéseket a[mobil eszközök Microsoft 365 üzleti felhasználók számára létrehozott](set-up-mobile-devices.md) Office-alkalmazások telepítéséhez eszközök, és ellenőrizzük, hogy a Microsoft 365 üzleti védettek legyenek. 
  
### <a name="3-prepare-pcs"></a>3: személyi számítógépek előkészítése

Rendszergazdák előre választhat új eszközök Windows 10 PC-k [Windows automata](add-autopilot-devices-and-profile.md)segítségével. A felhasználók ebben a témakörben leírt lépéseket követve állíthatja a meglévő vagy új Windows 10 eszközök: [állítsa be a Windows PC-k Microsoft 365 üzleti felhasználók számára](set-up-windows-devices.md). A meglévő eszközök felhasználók is **tetszés szerint**a[fájlok kerüljenek át az üzleti OneDrive](move-files-to-onedrive.md). Külső eszközök segítségével azok is OneDrive a Windows profilhoz társított fájlok áthelyezése.
  
Ha a szervezet használja a Windows Server Active Directory helyszíni, állíthat be Microsoft 365 üzleti védelme érdekében a Windows 10 eszközök továbbra is fenntartva helyi hitelesítést igénylő helyszíni erőforrásokhoz való hozzáférést. Kövesse a [Microsoft 365 üzleti által kezelt tartományhoz tartozó Windows 10 eszközök engedélyezése](manage-windows-devices.md) meg. Ez a javasolt módszer és eszközök ebben az állapotban a **hibrid Azure AD csatlakozott eszközök**nevezzük. 
  
Ha megőrzi a helyi Active Directory, amely tartalmazza az egyes helyi erőforrásokat (például fájlmegosztásokat és nyomtatókat), a **Borzas AD csatlakoztatott eszközök** hozzáférést biztosíthat a forrásokhoz való lépések itt: [Access helyszíni erőforrásokat egy 365 üzleti Microsoft Azure AD csatlakozott eszköz](access-resources.md).
  
10 PC-k Windows telepítése után [automatikusan telepíti az Office](auto-install-or-uninstall-office.md) eszközök is. 
  
## <a name="contact-support"></a>Lépjen kapcsolatba a támogatási szolgálattal.

 **Ha kapcsolatba szeretne lépni az ügyfélszolgálattal:**
  
- Forduljon a partneréhez.
    
- Ügyfélszolgálati csoportunkhoz, [kérjen segítséget a támogatási üzleti termékek - Admin súgó](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b) **hozzáféréssel rendelkezünk egy Microsoft 365 üzleti rendszergazdaként**
    
## <a name="related-topics"></a>Kapcsolódó témakörök
[A Microsoft 365 Vállalati verzióval kapcsolatos dokumentáció és források](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[A Microsoft 365 Vállalati verzió kezelése](manage.md)[Áttelepítés a Microsoft 365 Vállalati verzióba](migrate-to-microsoft-365-business.md)
  


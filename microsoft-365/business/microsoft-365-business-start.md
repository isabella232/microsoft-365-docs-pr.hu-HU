---
title: A Microsoft 365 Business használatbavétele
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: overview
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
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
ms.openlocfilehash: 1c4adc64f62f7d4ae5038603804aa10e48d8a6e1
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983795"
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
  
A következő ábra bemutatja, hogyan lehet a rendszergazdák a Microsoft 365 üzleti beállítani. Előkészítése a Windows PC-k Microsoft 365 üzleti lépéseket is ismerteti. Új eszközök a [Windows automata](add-autopilot-devices-and-profile.md)a Microsoft 365 üzleti admin közepén is hozzáadhat. Automata segítségével és felkészülés azok hatékony használata, amint a bejelentkezés hitelesítő adataikat a Microsoft 365 üzleti be előre beállítani új eszközöket.
  
![A diagram that shows the setup and management flow for admins, and also for a user](media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)
  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: Microsoft 365 Business (Admin) beállítása

Jelentkezzen be a [Microsoft 365 Vállalati verzió Felügyeleti központba](https://portal.office.com/adminportal/home) globális rendszergazdai hitelesítő adataival, majd a Microsoft 365 Business beállításához kövesse az alábbi lépéseket. 
  
1. [A Microsoft 365 Vállalati verziót tartalmazó eszközök adatvédelmének előfeltételei](pre-requisites-for-data-protection.md)
    
    Az eszközök kompatibilitásának ellenőrzéséhez elsőként olvassa el a Microsoft 365 Business előfeltételeit.
    
2. [A Microsoft 365 Vállalati verzió beállítása a beállítási varázslóval](set-up.md)
    
    Ha **véglegesen áthelyezése a helyi Active Directory a felhő**, vagy kézzel adhatók hozzá a felhasználók a Microsoft 365 üzleti felügyeleti központ a telepítő varázsló segítségével, vagy egy egyszeri szinkronizálás Azure AD csatlakozás a is elvégezheti. Ennek két módja van: 
    
  - Ha egy Exchange 2010, Exchange 2013 vagy Exchange 2016 kiszolgáló is rendelkezik, [Használata minimális hibrid gyors áttelepítése az Office 365 Exchange postaládákat](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef)is. A minimális hibrid lépéseket tartalmaz egy egyszeri szinkronizálás Azure ad a felhasználók, valamint e-mail helyszíni áttérés a felhő. Az e-mail áttelepítés befejezése után a címtár-szinkronizálás automatikusan ki van kapcsolva ez a módszer használata esetén.
    
  - Az Office 365 címtár-szinkronizálási varázslójával szinkronizálhatja a felhasználókat a felhőbe. Ezt a [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) című cikk lépéseit követve végezheti el. Miután szinkronizálta a felhasználókat a felhőbe, [Turn off directory synchronization for Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Minden felhasználó Microsoft 365 üzleti licenc így hozzáadott is lesz. Ehhez a [telepítő varázsló](set-up.md), vagy a [felhasználóknak az Office 365 rendszerben üzleti licencek hozzárendelése](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC).
    
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
[A Microsoft 365 Business dokumentációja és forrásai](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[A Microsoft 365 Vállalati verzió kezelése](manage.md)[Áttelepítés a Microsoft 365 Vállalati verzióba](migrate-to-microsoft-365-business.md)
  


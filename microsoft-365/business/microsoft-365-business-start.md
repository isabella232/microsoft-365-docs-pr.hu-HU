---
title: Első lépések a Microsoft 365 vállalati verzióban
f1.keywords:
- NOCSH
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
- TRN_SMB
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Megtudhatja, hogy miként állíthatja be a Microsoft 365 vállalati verzióját, hogyan állíthatja be és hogyan készítheti el a felhasználói eszközöket és a számítógépeket, hogy védve legyenek a Microsoft 365 vállalati verziójában.
ms.openlocfilehash: ec50036f589cfd8497b0e7e9af6519b30d25dcd3
ms.sourcegitcommit: 555d756c69ac9031d1fb928f2e1f9750beede066
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/29/2020
ms.locfileid: "47306489"
---
# <a name="get-started-with-microsoft-365-for-business"></a>Első lépések a Microsoft 365 vállalati verzióban

## <a name="what-is-microsoft-365-for-business"></a>Mi a Microsoft 365 vállalati verzió?

A Microsoft 365 vállalati verzió a vállalati hatékonyságnövelő és együttműködési eszközök (például az Outlook, a Word, az Excel és más Office-termékek) átfogó készlete, amelyek mindig naprakészek. A munkahelyi fájlokat az iOS, az Android és a Windows 10 rendszerű eszközökön is megvédheti, így egyszerűen kezelhető nagyvállalati szintű biztonság.

Ebből a videóból megnézheti a Microsoft 365 vállalati verziójának gyors áttekintését.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
A Microsoft 365 vállalati verzió a 300-licencek esetében jelent meg. Ha ennél több licencre van szüksége, további információért olvassa el a [Microsoft 365 Nagyvállalati verzió](https://go.microsoft.com/fwlink/p/?linkid=860986) dokumentációját. 
  
## <a name="get-microsoft-365-for-business"></a>A Microsoft 365 vállalati verziójának beszerzése

- Ha van partnere, a Microsoft 365 vállalati verziójának [beszerzése: a microsoft 365 vállalati verzió beszerzése a Microsoft partner központból](get-microsoft-365-business.md).
    
- Ha nincs partnere, és szeretné beszerezni a Microsoft 365 vállalati verziót, [itt megvásárolhatja](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-for-business"></a>A Microsoft 365 vállalati verzió beállítása

 **A Microsoft 365 for Business Suite beállítása – áttekintés**
  
Az alábbi ábra azt ismerteti, hogy a rendszergazdák hogyan állíthatják be a Microsoft 365 vállalati verziót. Ismerteti a Windows PC-k Microsoft 365 vállalati verzióra való felkészülésének lépéseit is. Új eszközöket a Microsoft 365 felügyeleti központban, a [Windows Autopilot](add-autopilot-devices-and-profile.md)segítségével is hozzáadhat. Az Autopilot segítségével beállíthatja és előre beállíthatja az új eszközöket úgy, hogy készen álljanak a hatékony használatra, amint a felhasználó bejelentkezik a Microsoft 365 vállalati verziós hitelesítő adataival.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

Ebből a videóból megtekintheti a Microsoft 365 vállalati verzió beállítását.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Ha hasznosnak találta ezt a videót, tekintse meg a [teljes tanfolyamok kisvállalatoknak és Microsoft 365-újoncoknak](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) című cikket.

  
### <a name="1-set-up-microsoft-365-for-business-admin"></a>1: a Microsoft 365 vállalati verzió beállítása (rendszergazda)

A Microsoft [365 felügyeleti központba](https://portal.office.com/adminportal/home) a globális rendszergazdai hitelesítő adataival jelentkezhet be, és az alábbi lépéseket követve beállíthatja a Microsoft 365 vállalati verziót. 
  
1. [A Microsoft 365 vállalati verzióval rendelkező eszközökön tárolt adatok védelmének előfeltételei](pre-requisites-for-data-protection.md)
    
    Először olvassa el az előfeltételeit, és győződjön meg arról, hogy az eszközök készen állnak a Microsoft 365 vállalati verzióra.
    
2. [A Microsoft 365 vállalati verzió beállítása a beállítási varázslóval](set-up.md)
    
    Ha **véglegesen egy helyi Active Directory-címtárból a felhőbe**lép, a Microsoft 365 felügyeleti központját használhatja, és a beállítási varázslóval manuálisan is felveheti a felhasználókat, vagy az Azure ad Connect segítségével egyszer szinkronizálhatja őket. Ehhez két lehetőség közül választhat: 
    
    - Ha Exchange 2010-, Exchange 2013-vagy Exchange 2016-kiszolgálóval is rendelkezik, az [Exchange-postaládák gyors áttelepítése a Microsoft 365-be minimális hibrid](https://docs.microsoft.com/Exchange/mailbox-migration/use-minimal-hybrid-to-quickly-migrate)lehet. A minimális hibrid lépések közé tartozik a felhasználók egyszeri szinkronizálása az Azure AD-ba, és a helyszíni e-mailek áttelepítése a felhőbe. Az áttelepítés befejeződése után a rendszer automatikusan kikapcsolja a címtár-szinkronizálást, ha ezt a módszert használja.
    
    - A címtár-szinkronizálás varázslóval szinkronizálhatja a felhasználókat a felhőben. A folyamat végrehajtásához kövesse a [címtár-szinkronizálás beállítása a Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) -hoz című témakör lépéseit. Miután szinkronizálta a felhasználókat a felhőbe, [ki kell kapcsolnia a címtár-szinkronizálást a Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/turn-off-directory-synchronization)-hoz.
    
    Azt is megteheti, hogy a Microsoft 365 vállalati verzió licence által felvett minden felhasználónak meg kell adnia a licencet. Ezt megteheti a [beállítási varázslóban](set-up.md) , vagy [licenceket rendelhet a felhasználókhoz](../admin/manage/assign-licenses-to-users.md).
    
### <a name="2-prepare-mobile-devices"></a>2: mobileszközök előkészítése

Kövesse a következő témakör lépéseit: [mobileszközök beállítása a Microsoft 365 vállalati verzió felhasználói](set-up-mobile-devices.md) számára az Office-alkalmazások eszközön való telepítéséhez és a Microsoft 365 vállalati verzió által védettnek kell lennie. 
  
### <a name="3-prepare-pcs"></a>3: PC-k előkészítése

A rendszergazdák az új Windows 10-es PC-k beállítását előre is megadhatják a [Windows Autopilot](add-autopilot-devices-and-profile.md)segítségével. A felhasználók a meglévő vagy új Windows 10-es eszközeiket az ebben a témakörben ismertetett lépésekkel hozhatják létre: [Windows-PC-k beállítása a Microsoft 365 vállalati verzió felhasználói](set-up-windows-devices.md)számára. A meglévő eszközök esetében a felhasználók **tetszés szerint** [át tudják helyezni a fájlokat a OneDrive vállalati](move-files-to-onedrive.md)verzióba. Harmadik féltől származó eszközöket is használhatnak a Windows-profilokkal társított fájlok áthelyezéséhez a OneDrive.
  
Ha a szervezete a Windows Server Active Directoryt használja helyszíniként, beállíthatja a Microsoft 365 vállalati verzióját a Windows 10-es eszközök védelmére, miközben továbbra is megőrizheti a helyi hitelesítéshez szükséges helyszíni erőforrásokhoz való hozzáférést. Kövesse a [tartományhoz csatlakoztatott Windows 10-es eszközök kezelésének engedélyezése a Microsoft 365 vállalati](manage-windows-devices.md) verzióban című témakör lépéseit. Ezt a módszert részesíti előnyben, és az ebben az állapotban lévő eszközöket **hibrid Azure ad-összekapcsolt eszközöknek**nevezzük. 
  
Ha megőrzi a helyszíni erőforrásokat (például fájlmegosztás és nyomtató) tartalmazó helyi Active Directoryt, az **Azure ad-inaktív eszközökhöz** való hozzáférést az alábbi lépésekkel érheti el: [hozzáférés a helyszíni erőforrásokhoz a Microsoft 365 vállalati](access-resources.md)verziójában.
  
  
## <a name="contact-support"></a>Ügyfélszolgálat

 **Ha kapcsolatba szeretne lépni az ügyfélszolgálattal:**
  
- Forduljon a partneréhez.
    
- Microsoft 365 vállalati verziós rendszergazdaként hozzáférése van az ügyfélszolgálati csapathoz: ** [Kapcsolatfelvétel az üzleti termékek támogatási csoportjával – rendszergazdai Súgó](https://docs.microsoft.com/microsoft-365/admin/contact-support-for-business-products)**
    
## <a name="see-also"></a>Lásd még

[A Microsoft 365 vállalati verzió dokumentációja és erőforrásai](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
A [microsoft 365 vállalati](manage.md)verzióba való[áttérés kezelése a Microsoft 365 vállalati](migrate-to-microsoft-365-business.md) verzióba

[Microsoft 365 vállalati verziós képzési videók](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) 

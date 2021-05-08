---
title: Első lépések a Microsoft 365 vállalati verzióban
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: Tudnivalók a Microsoft 365 vállalati verzióról, a beállításról, valamint arról, hogy miként készítheti fel a felhasználók eszközeit és számítógépeit a vállalati Microsoft 365 védelmére.
ms.openlocfilehash: cc54147e75a27fbb93255d6f706b4f9044c75858
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52245124"
---
# <a name="get-started-with-microsoft-365-for-business"></a>Első lépések a Microsoft 365 vállalati verzióban

## <a name="what-is-microsoft-365-for-business"></a>A vállalati Microsoft 365

Microsoft 365 vállalati verzió az üzleti hatékonyságot és együttműködési eszközöket (például Outlook, Word, Excel és más Office-termékek) átfogó készlete, amely mindig naprakész. A nagyvállalati szintű, egyszerűen kezelhető, nagyvállalati szintű biztonsági megoldásokkal minden iOS, Android és Windows 10 eszközén megvédheti a munkahelyi fájljait.

Ebből a videóból gyorsan áttekintheti a vállalati Microsoft 365 áttekintését.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
Microsoft 365 vállalati verzió legfeljebb 300 licenccel rendelkezik. Ha ennél több licencre van szüksége, további információért olvassa el a [Microsoft 365 Nagyvállalati verzió](../enterprise/index.yml) dokumentációját. 
  
## <a name="get-microsoft-365-for-business"></a>A Microsoft 365 vállalati verzió

- Ha van partnere, a következőt fogja kapni a Microsoft 365 számára: Vállalati verziós Microsoft 365 a [Microsoft Partnerközpontban.](get-microsoft-365-business.md)
    
- Ha nincs partnere, és meg szeretné vásárolni Microsoft 365 vállalati verzióhoz, meg [is vásárolhatja itt.](https://www.microsoft.com/microsoft-365/business)
    
## <a name="set-up-microsoft-365-for-business"></a>A vállalati Microsoft 365 beállítása

 **A vállalati Microsoft 365 csomag beállításának áttekintése**
  
Az alábbi diagram bemutatja, hogy a rendszergazdák hogyan Microsoft 365 vállalati verzióban. A cikk a számítógépekkel való Windows a vállalati Microsoft 365 lépéseket is ismerteti. Az [AutoPilot](add-autopilot-devices-and-profile.md)segítségével új eszközöket is Microsoft 365 Felügyeleti központban Windows. Az AutoPilot segítségével beállíthatja és előre konfigurálhatja az új eszközöket, így azonnal készen állnak a hatékony használatra, amint a felhasználó bejelentkezik az Microsoft 365 vállalati hitelesítő adataival.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

Ebből a videóból áttekintheti a vállalati Microsoft 365 beállításokat.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Ha hasznosnak találta ezt a videót, tekintse meg a [teljes tanfolyamok kisvállalatoknak és Microsoft 365-újoncoknak](../business-video/index.yml) című cikket.

  
### <a name="1-set-up-microsoft-365-for-business-admin"></a>1: A vállalati Microsoft 365 beállítása (rendszergazda)

Jelentkezzen be [Microsoft 365](https://portal.office.com/adminportal/home) felügyeleti központba a globális rendszergazdai hitelesítő adataival, és az alábbi lépéseket követve állítsa be Microsoft 365 vállalati verzióban. 
  
1. [Az adatok vállalati Microsoft 365 védelmének előfeltételei](pre-requisites-for-data-protection.md)
    
    Először olvassa el az előfeltételeket, és győződjön meg arról, hogy eszközei készen állnak Microsoft 365 vállalati használatra.
    
2. [A vállalati verzió beállítása a Microsoft 365 varázslóval](set-up.md)
    
    Ha egy helyi **Active Directoryról** véglegesen a felhőbe szeretne áttérni, a Microsoft 365 Felügyeleti központba lépve manuálisan felveheti a felhasználókat a beállítási varázslóval, vagy egy egyszer szinkronizálhat az Azure AD-címtárral Csatlakozás. Ehhez két lehetőség közül választhat: 
    
    - Ha Exchange, Exchange 2013 vagy Exchange 2016-kiszolgálóval is van, a hibrid minimumkontraszt használatával gyorsan át Exchange postaládákat a [Microsoft 365.](/Exchange/mailbox-migration/use-minimal-hybrid-to-quickly-migrate) A minimális hibrid lépések közé tartozik a felhasználók egyszeres szinkronizálása az Azure AD-be, valamint a levelezés áttelepítése a helyszíni környezetből a felhőbe. A levelezés áttelepítése után a rendszer automatikusan kikapcsolja a címtár-szinkronizálást, amikor ezt a módszert használja.
    
    - A címtár-szinkronizálási varázslóval szinkronizálja a felhasználókat a felhőbe. A folyamat befejezéséhez kövesse [A](../enterprise/set-up-directory-synchronization.md) címtár-szinkronizálás beállítása Microsoft 365 lépéseit. Miután szinkronizálta a felhasználókat a felhőbe, ki kell kapcsolnia a címtár-szinkronizálást a [Microsoft 365.](../enterprise/turn-off-directory-synchronization.md)
    
    Ezenkívül az ily módon felvett felhasználóknak licencet kell adni Microsoft 365 vállalati verzióhoz. Ezt a beállítási [varázslóban](set-up.md) vagy a Licencek hozzárendelése [felhasználókhoz adhatja meg.](../admin/manage/assign-licenses-to-users.md)
    
### <a name="2-prepare-mobile-devices"></a>2: Mobileszközök előkészítése

A Mobileszközök beállítása a [Microsoft 365](set-up-mobile-devices.md) Vállalati verzió felhasználóinak Office-appok telepítéséhez és a vállalati verziós Microsoft 365 védjük őket. 
  
### <a name="3-prepare-pcs"></a>3: Pc-k előkészítése

A rendszergazdák előre kiválaszthatják az új és az Windows 10 beállításait az [AutoPilot](add-autopilot-devices-and-profile.md)Windows használatával. A felhasználók a következő témakörben található lépéseket követve állíthatják be meglévő vagy új Windows 10 eszközüket: Windows pc-k beállítása vállalati Microsoft 365 [felhasználóknak.](set-up-windows-devices.md) Meglévő eszközök esetén  a felhasználók tetszés szerint áthelyezheti a fájlokat a [OneDrive Vállalati verzió.](move-files-to-onedrive.md) Emellett külső eszközökkel is áthelyezhet Windows profilhoz társított fájlokat OneDrive.
  
Ha szervezete helyszíni Windows Server Active Directoryt használ, beállíthatja a Microsoft 365 Vállalati verziót az Windows 10-eszközök védelmére, miközben továbbra is hozzáfér a helyi hitelesítést igénylő helyszíni erőforrásokhoz. A beállítás beállításához kövesse A tartományhoz Windows 10 eszközök vállalati verzió által kezelhető [Microsoft 365 lépéseket.](manage-windows-devices.md) Ezt a módszert előnyben részesítik, az ebben az állapotban használt eszközöket pedig hibrid Azure AD-hez csatlakozású **eszközöknek nevezzük.** 
  
Ha megőriz egy olyan helyi Active Directory-címtárat, amely helyszíni erőforrásokat (például fájlmegosztásokat és nyomtatókat) tartalmaz, az alábbi lépéseket követve hozzáférést adhat Azure **AD-hez** eszközének ezekhez az erőforrásokhoz: Az Microsoft 365 Vállalati verzióban az [Azure AD-hez](access-resources.md)csatlakozott eszköz helyszíni erőforrásainak elérése.
  
  
## <a name="contact-support"></a>Ügyfélszolgálat

 **Ha kapcsolatba szeretne lépni az ügyfélszolgálattal:**
  
- Forduljon a partneréhez.
    
- Vállalati Microsoft 365 rendszergazdáként hozzáférhet ügyfélszolgálati csapatunkhoz: Kapcsolatfelvétel az ügyfélszolgálattal üzleti termékekhez **[– rendszergazdai súgó](../admin/contact-support-for-business-products.md)**
    
## <a name="related-content"></a>Kapcsolódó tartalom

[Microsoft 365 vállalati verzió dokumentációja és forrásai](./index.yml)
  
[Vállalati Microsoft 365 kezelése](manage.md)Áttelepítés Microsoft 365[vállalati verzióba](migrate-to-microsoft-365-business.md)

[Microsoft 365 vállalati verziós oktatóvideók](../business-video/index.yml)
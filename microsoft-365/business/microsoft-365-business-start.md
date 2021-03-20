---
title: A Microsoft 365 Vállalati verzió első lépések
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
description: Tudnivalók a Microsoft 365 Vállalati verzióról, a beállításról, valamint arról, hogy miként készítheti fel felhasználói eszközeit és SZÁMÍTÓGÉPeit a Microsoft 365 Vállalati verzió védelmére.
ms.openlocfilehash: 9430dc7aa637be3fdb833150b83e96caacc82170
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912962"
---
# <a name="get-started-with-microsoft-365-for-business"></a>A Microsoft 365 Vállalati verzió első lépések

## <a name="what-is-microsoft-365-for-business"></a>Mi a Microsoft 365 Vállalati verzió?

A Microsoft 365 Vállalati verzió olyan üzleti hatékonyságnövelő és együttműködési eszközök átfogó készlete, mint például az Outlook, a Word, az Excel és más Office-termékek, amelyek mindig naprakészek. Az egyszerűen kezelhető, nagyvállalati szintű biztonsági megoldásokkal minden iOS, Android és Windows 10 rendszerű eszközén megvédheti a munkahelyi fájljait.

Ez a videó rövid áttekintést nyújt a Microsoft 365 Vállalati verzióról.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
A Microsoft 365 Vállalati verzió legfeljebb 300 licenccel rendelkezik. Ha ennél több licencre van szüksége, további információért olvassa el a [Microsoft 365 Nagyvállalati verzió](../enterprise/index.yml) dokumentációját. 
  
## <a name="get-microsoft-365-for-business"></a>A Microsoft 365 Vállalati verzió 365-ről

- Ha van partnere, a microsoft 365 Vállalati verzióhoz jut hozzá: A Microsoft 365 Vállalati verzió a [Microsoft Partnerközpontból.](get-microsoft-365-business.md)
    
- Ha nincs partnere, és meg szeretné vásárolni a Microsoft 365 Vállalati verziót, meg [is vásárolhatja itt.](https://www.microsoft.com/microsoft-365/business)
    
## <a name="set-up-microsoft-365-for-business"></a>A Microsoft 365 Vállalati verzió beállítása

 **A Microsoft 365 Vállalati verzió beállítása – áttekintés**
  
Az alábbi diagram bemutatja, hogy a rendszergazdák hogyan állíthatják be a Microsoft 365 Vállalati verziót. A cikk a Windows rendszerű PC-k Microsoft 365 Vállalati verzióra való előkészítésének lépéseit is ismerteti. A Windows AutoPilot segítségével új eszközöket is felvehet a Microsoft 365 [Felügyeleti központban.](add-autopilot-devices-and-profile.md) Az AutoPilot segítségével beállíthatja és előre konfigurálhatja az új eszközöket, így azonnal készen állnak a hatékony használatra, amint a felhasználó bejelentkezik a Microsoft 365 Vállalati verziós hitelesítő adataival.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

Ebből a videóból áttekintheti a Microsoft 365 Vállalati verzió beállítását.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Ha hasznosnak találta ezt a videót, tekintse meg a [teljes tanfolyamok kisvállalatoknak és Microsoft 365-újoncoknak](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) című cikket.

  
### <a name="1-set-up-microsoft-365-for-business-admin"></a>1: A Microsoft 365 Vállalati verzió beállítása (rendszergazda)

Jelentkezzen be a [Microsoft 365](https://portal.office.com/adminportal/home) Felügyeleti központba globális rendszergazdai hitelesítő adataival, és az alábbi lépéseket követve állítsa be a Microsoft 365 Vállalati verziót. 
  
1. [Az eszközökön a Microsoft 365 Vállalati verzióval való adatvédelem előfeltételei](pre-requisites-for-data-protection.md)
    
    Először olvassa el az előfeltételeket, és győződjön meg arról, hogy eszközei készen állnak a Microsoft 365 Vállalati verzió használatára.
    
2. [A Microsoft 365 Vállalati verzió beállítása a beállítási varázslóval](set-up.md)
    
    Ha egy helyi **Active Directoryról** véglegesen a felhőbe szeretne áttérni, a Microsoft 365 Felügyeleti központba lépve manuálisan felveheti a felhasználókat a beállítási varázslóval, vagy az Azure AD Connect segítségével is szinkronizálhat egy egyszeres szinkronizálást. Ehhez két lehetőség közül választhat: 
    
    - Ha Exchange 2010-, Exchange 2013- vagy Exchange 2016-kiszolgálóval is van, akkor a Hibrid minimumkontraszttal gyorsan át lehet miolni az Exchange-postaládákat a [Microsoft 365-be.](/Exchange/mailbox-migration/use-minimal-hybrid-to-quickly-migrate) A minimális hibrid lépések közé tartozik a felhasználók egyszeres szinkronizálása az Azure AD-be, valamint a levelezés áttelepítése a helyszíni környezetből a felhőbe. A levelezés áttelepítése után a rendszer automatikusan kikapcsolja a címtár-szinkronizálást, amikor ezt a módszert használja.
    
    - A címtár-szinkronizálási varázslóval szinkronizálja a felhasználókat a felhőbe. A folyamat befejezéséhez kövesse A Címtár-szinkronizálás beállítása a Microsoft 365-bencímtár-szinkronizálástcímtárban található lépéseket. [](../enterprise/set-up-directory-synchronization.md) Miután szinkronizálta a felhasználókat a felhőbe, ki kell kapcsolnia a [címtár-szinkronizálást a Microsoft 365-ben.](../enterprise/turn-off-directory-synchronization.md)
    
    Ezenkívül az ily módon felvett felhasználóknak licencet kell adni a Microsoft 365 Vállalati verzióhoz. Ezt a beállítási [varázslóban](set-up.md) vagy a Licencek hozzárendelése [felhasználókhoz adhatja meg.](../admin/manage/assign-licenses-to-users.md)
    
### <a name="2-prepare-mobile-devices"></a>2: Mobileszközök előkészítése

A Mobileszközök beállítása a [Microsoft 365](set-up-mobile-devices.md) Vállalati verzió felhasználóinak lépéseit követve telepítse az Office-appokat az eszközökre, és győződjön meg arról, hogy a Microsoft 365 Vállalati verzió védelmet nyújt nekik. 
  
### <a name="3-prepare-pcs"></a>3: Pc-k előkészítése

A rendszergazdák előre kiválaszthatják az új Windows 10-es PC-k beállításait a [Windows AutoPilot használatával.](add-autopilot-devices-and-profile.md) A felhasználók a következő témakörben található lépéseket követve állíthatják be meglévő vagy új Windows 10-es eszközeiket: Windows rendszerű PC-k beállítása a [Microsoft 365 Vállalati verzió felhasználóinak.](set-up-windows-devices.md) Meglévő eszközök esetén  a felhasználók tetszés szerint áthelyezhet fájlokat a [OneDrive Vállalati verzióba.](move-files-to-onedrive.md) Emellett külső eszközökkel is áthelyezheti a Windows-profilhoz társított fájlokat a OneDrive-ra.
  
Ha szervezete helyszíni Windows Server Active Directoryt használ, beállíthatja a Microsoft 365 Vállalati verziót a Windows 10-es eszközök védelmére, miközben továbbra is hozzáfér a helyi hitelesítést igénylő helyszíni erőforrásokhoz. A beállítás beállításához kövesse A tartományhoz csatlakozott [Windows 10-es eszközök Microsoft 365](manage-windows-devices.md) Vállalati verzió által történő kezelése. Ezt a módszert előnyben részesítik, az ebben az állapotban használt eszközöket pedig hibrid Azure AD-hez csatlakozású **eszközöknek nevezzük.** 
  
Ha megőriz egy olyan helyi Active Directory-címtárat, amely helyszíni erőforrásokat (például fájlmegosztásokat és nyomtatókat) tartalmaz, az alábbi lépéseket követve hozzáférést adhat Azure **AD-hez** eszközének ezekhez az erőforrásokhoz: Hozzáférés helyszíni erőforrásokhoz a Microsoft 365 Vállalati verzió [Azure AD-csatlakozású eszközéről.](access-resources.md)
  
  
## <a name="contact-support"></a>Ügyfélszolgálat

 **Ha kapcsolatba szeretne lépni az ügyfélszolgálattal:**
  
- Forduljon a partneréhez.
    
- A Microsoft 365 Vállalati verzió rendszergazdájaként kapcsolatba léphet ügyfélszolgálati csapatunkkal: Kapcsolatfelvétel az ügyfélszolgálattal vállalati termékek **[esetében – rendszergazdai súgó](../admin/contact-support-for-business-products.md)**
    
## <a name="see-also"></a>Lásd még

[A Microsoft 365 Vállalati verzió dokumentációja és forrásai](./index.yml)
  
[A Microsoft 365 Vállalati verzió kezelése](manage.md)[Áttelepítés a Microsoft 365 Vállalati verzióba](migrate-to-microsoft-365-business.md)

[Microsoft 365 Vállalati verzió – oktatóvideók](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
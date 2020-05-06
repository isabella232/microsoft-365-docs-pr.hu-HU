---
title: Ismerkedés a Microsoft 365 vállalati verzióval
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
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Ismerje meg a Microsoft 365 vállalati verziót, a beállításmódját, valamint azt, hogy miként készítheti fel a felhasználók eszközeit és számítógépeit a Microsoft 365 vállalati verzió általi védelemre.
ms.openlocfilehash: 8754c470cb6369f0814f953288be130fa49cea86
ms.sourcegitcommit: 5476c2578400894640ae74bfe8e93c3319f685bd
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/06/2020
ms.locfileid: "44048085"
---
# <a name="get-started-with-microsoft-365-for-business"></a>Ismerkedés a Microsoft 365 vállalati verzióval

## <a name="what-is-microsoft-365-for-business"></a>Mi a Microsoft 365 vállalati verzió

A Microsoft 365 vállalati verzió az üzleti hatékonyságnövelő és együttműködési eszközök, például az Outlook, a Word, az Excel és más Office-termékek átfogó készlete, amelyek mindig naprakészek. A munkahelyi fájlokat az összes iOS, Android és Windows 10-es eszközén megvédheti a nagyvállalati szintű, egyszerűen kezelhető biztonsággal.

Ebből a videóból gyors áttekintést kaphat a Microsoft 365 vállalati verzióról.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
A Microsoft 365 vállalati verzió akár 300 licencre is alkalmas. Ha ennél több licencre van szüksége, további információért olvassa el a [Microsoft 365 Nagyvállalati verzió](https://go.microsoft.com/fwlink/p/?linkid=860986) dokumentációját. 
  
## <a name="get-microsoft-365-for-business"></a>A Microsoft 365 vállalati verzió beszereznie

- Ha van partnere, akkor a Microsoft 365 vállalati verzió: [A Microsoft 365 vállalati verzió ta-](get-microsoft-365-business.md)
    
- Ha nincs partnere, és szeretné, hogy a Microsoft 365 üzleti, [megvásárolhatja itt](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-for-business"></a>A Microsoft 365 vállalati verzió beállítása

 **A Microsoft 365 vállalati verziócsomag beállítása**
  
Az alábbi ábra azt ismerteti, hogy a rendszergazdák hogyan állították be a Microsoft 365 vállalati verziót. Ismerteti továbbá a Windows-számítógépek Microsoft 365 vállalati verzióra való előkészítésének lépéseit is. Új eszközöket is hozzáadhat a Microsoft 365 felügyeleti központban a [Windows AutoPilot](add-autopilot-devices-and-profile.md)segítségével. Az AutoPilot segítségével beállíthatja és előre konfigurálhatja az új eszközöket, hogy azok készen álljanak a hatékony használatra, amint a felhasználó bejelentkezik a Microsoft 365 üzleti hitelesítő adataival.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

Ebből a videóból megtudhatja, hogy miként tekintheti meg a Microsoft 365 vállalati beállításokat.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Ha hasznosnak találta ezt a videót, tekintse meg a [teljes tanfolyamok kisvállalatoknak és Microsoft 365-újoncoknak](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) című cikket.

  
### <a name="1-set-up-microsoft-365-for-business-admin"></a>1: A Microsoft 365 vállalati verzió (rendszergazda) beállítása

Jelentkezzen be a [Microsoft 365 Felügyeleti központba](https://portal.office.com/adminportal/home) globális rendszergazdai hitelesítő adataival, és hajtsa végre az alábbi lépéseket a Microsoft 365 vállalati verzió beállításához. 
  
1. [Az eszközökön lévő adatok védelmének előfeltételei a Microsoft 365 vállalati verzióval](pre-requisites-for-data-protection.md)
    
    Először olvassa el az előfeltételeket, és győződjön meg arról, hogy az eszközök készen állnak a Microsoft 365 vállalati verzióra.
    
2. [A Beállítás varázsló használata a Microsoft 365 vállalati verzió beállításához](set-up.md)
    
    Ha **véglegesen a helyi Active Directoryról a felhőbe költözik,** nyissa meg a Microsoft 365 felügyeleti központot, és a beállítási varázsló segítségével manuálisan adja hozzá a felhasználókat, vagy egyszeri szinkronizálást hajthat elő az Azure AD Connecttel. Ehhez két lehetőség közül választhat: 
    
    - Ha Exchange 2010-es, Exchange 2013- vagy Exchange 2016-kiszolgálóval is rendelkezik, [a Minimal Hybrid használatával gyorsan áttelepítheti az Exchange-postaládákat az Office 365-be.](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef) A minimális hibrid lépések közé tartozik a felhasználók egyszeri szinkronizálása az Azure AD-vel, és e-mailes áttelepítés a helyszíni felhőbe. Az e-mailek áttelepítése után a címtár-szinkronizálás automatikusan kikapcsol, ha ezt a módszert használja.
    
    - A címtár-szinkronizálási varázsló segítségével szinkronizálja a felhasználókat a felhővel. A folyamat végrehajtásához kövesse a [Címtár-szinkronizálás beállítása a Microsoft 365-höz](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) című részben leírt lépéseket. Miután szinkronizálta a felhasználókat a felhővel, ki kell [kapcsolnia az Office 365 címtár-szinkronizálását.](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d)
    
    Azt is meg kell adnia minden felhasználónak, hogy a hozzáadott így egy licencet a Microsoft 365 vállalati verzióhoz. Ezt megteheti a [telepítővarázslóban,](set-up.md) vagy licenceket rendelhet a [Microsoft 365 vállalati verzió felhasználóihoz.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)
    
### <a name="2-prepare-mobile-devices"></a>2: Mobileszközök előkészítése

Kövesse a [Mobileszközök beállítása az üzleti felhasználók számára című, A mobileszközök beállítása üzleti felhasználók számára](set-up-mobile-devices.md) című témakör lépéseit, amelyek segítségével telepítheti az Office-alkalmazásokat az eszközökre, és meggyőződhet arról, hogy azokat a Microsoft 365 vállalati verzió védi. 
  
### <a name="3-prepare-pcs"></a>3: Pc-k előkészítése

A rendszergazdák előre kiválaszthatják az új Windows 10-es számítógépek beállításait a [Windows AutoPilot](add-autopilot-devices-and-profile.md)segítségével. A felhasználók a jelen témakörben leírt lépések végrehajtásával állíthatják be meglévő vagy új Windows 10-eszközeiket: [Windows-számítógépek beállítása Microsoft 365-höz üzleti felhasználók számára](set-up-windows-devices.md). Meglévő eszközök esetén a felhasználók **tetszés szerint** [fájlokat helyezhetnek át a OneDrive Vállalati verzióba.](move-files-to-onedrive.md) Külső eszközökkel is áthelyezhetik a Windows-profilhoz társított fájlokat a OneDrive-ra.
  
Ha a szervezet a helyszíni Windows Server Active Directoryt használja, beállíthatja a Microsoft 365 vállalati verziót a Windows 10-es eszközök védelmére, miközben továbbra is hozzáférhet a helyi hitelesítést igénylő helyszíni erőforrásokhoz. Kövesse a [Tartományhoz csatlakozó Windows 10-es eszközök microsoft 365 vállalati verziós rendszerének engedélyezése](manage-windows-devices.md) című, ezt bekövetkező lépéseit. Ez a módszer előnyös, és az ilyen állapotú eszközök nevezzük **hibrid Azure AD-hez csatlakozó eszközök.** 
  
Ha megtart egy helyi Active Directoryt, amely néhány helyszíni erőforrást (például fájlmegosztásokat és nyomtatókat) tartalmaz, az **Azure AD-hez csatlakoztatott eszközöknek** hozzáférést adhat ezekhez az erőforrásokhoz az alábbi lépések végrehajtásával: [Helyszíni erőforrások elérése egy Azure AD-hez csatlakoztatott eszközről a Microsoft 365 vállalati verzióban.](access-resources.md)
  
  
## <a name="contact-support"></a>Ügyfélszolgálat

 **Ha kapcsolatba szeretne lépni az ügyfélszolgálattal:**
  
- Forduljon a partneréhez.
    
- Microsoft 365 vállalati rendszergazdaként hozzáférhet ügyfélszolgálatunkhoz: ** [Vegye fel a kapcsolatot az üzleti termékekkel foglalkozó ügyfélszolgálattal – Rendszergazdai súgó](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b)**
    
## <a name="see-also"></a>Lásd még

[Microsoft 365 üzleti dokumentációés források](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[A Microsoft 365 vállalati verzió kezelése](manage.md)[Áttelepítés a Microsoft 365 vállalati verzióra](migrate-to-microsoft-365-business.md)

[Microsoft 365 üzleti oktatóvideók](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) 

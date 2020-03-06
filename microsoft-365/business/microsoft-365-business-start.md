---
title: A Microsoft 365 Business használatbavétele
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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Ismerje meg a Microsoft 365 Vállalati verziót, a beállításmódját, valamint a felhasználói eszközök és számítógépek előkészítését annak érdekében, hogy a Microsoft 365 Business védje őket.
ms.openlocfilehash: f6fd73762c0b57777c19d32886f758875e2e7e6a
ms.sourcegitcommit: 41c0bc5cf50f4ca63b4286d1ea0f58ab82984b7a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42547731"
---
# <a name="get-started-with-microsoft-365-business"></a>A Microsoft 365 Business használatbavétele

## <a name="what-is-microsoft-365-business"></a>Mi a Microsoft 365 Vállalati verzió?

A Microsoft 365 Business az üzleti hatékonyság és az együttműködés olyan eszközeinek átfogó készlete, mint például az Outlook, a Word, az Excel és más Office-termékek, amelyek mindig naprakészek. A munkahelyi fájlokat minden iOS, Android és Windows 10 rendszerű eszközén megvédheti az egyszerű kezelhető nagyvállalati szintű biztonsággal.

Ebből a videóból gyorsan áttekintheti a Microsoft 365 Vállalati verziót.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
A Microsoft 365 Business legfeljebb 300 licenchez szól. Ha további licencre van szüksége, további információt a [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986) dokumentációjában talál. 
  
## <a name="get-microsoft-365-business"></a>A Microsoft 365 Vállalati verzió beszerzése

- Ha van partnere, a Microsoft 365 Vállalati verzió: [A Microsoft 365 Vállalati verzió beszerezheti a Microsoft Partner Center programból.](get-microsoft-365-business.md)
    
- Ha nincs partnere, és meg szeretné vásárolni a Microsoft 365 Businesst, [itt megteheti](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>A Microsoft 365 Vállalati verzió beállítása

 **A Microsoft 365 Business Suite beállításának áttekintése**
  
Az alábbi ábra azt ismerteti, hogy a rendszergazdák hogyan állították be a Microsoft 365 Business t. Ezenkívül a Windows rendszerű PC-k Microsoft 365 Business használatára való előkészítésének lépéseit is tartalmazza. Új eszközöket is hozzáadhat a Microsoft 365 Vállalati felügyeleti központban a [Windows AutoPilot](add-autopilot-devices-and-profile.md)segítségével. Az AutoPilot segítségével új eszközöket állíthat be és konfigurálhat előre, hogy azok készen álljanak a hatékony használatra, amint a felhasználó bejelentkezik a Microsoft 365 Vállalati hitelesítő adataikkal.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

Ebből a videóból megtudhatja, hogy mik a Microsoft 365 Vállalati verzió beállítása.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Ha hasznosnak találta ezt a videót, tekintse meg a [teljes tanfolyamok kisvállalatoknak és Microsoft 365-újoncoknak](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) című témakört.

  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: A Microsoft 365 Vállalati verzió beállítása (rendszergazda)

Jelentkezzen be a [Microsoft 365 Vállalati felügyeleti központba](https://portal.office.com/adminportal/home) a globális rendszergazdai hitelesítő adatokkal, és hajtsa végre az alábbi lépéseket a Microsoft 365 Vállalati verzió beállításához. 
  
1. [Az adatok védelmének előfeltételei az eszközökön a Microsoft 365 Business segítségével](pre-requisites-for-data-protection.md)
    
    Először olvassa el az előfeltételeket, és győződjön meg arról, hogy eszközei készen állnak a Microsoft 365 Business szolgáltatásra.
    
2. [A Microsoft 365 Vállalati verzió beállítása a telepítővarázslóval](set-up.md)
    
    Ha **véglegesen áthelyez egy helyi Active Directoryból a felhőbe,** lépjen a Microsoft 365 Vállalati felügyeleti központba, és a telepítővarázslóval manuálisan vegye fel a felhasználókat, vagy egyszeri szinkronizálást hajtson le az Azure AD Connectszolgáltatással. Ehhez két lehetőség közül választhat: 
    
    - Ha Exchange 2010, Exchange 2013 vagy Exchange 2016 kiszolgálóis, a [Minimal Hybrid segítségével gyorsan áttelepítheti az Exchange-postaládákat az Office 365-be.](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef) A minimális hibrid lépések közé tartozik a felhasználók egyszeri szinkronizálása az Azure AD-vel, és az e-mailek áttelepítése a helyszíni felhőbe. Az e-mailek áttelepítése után a címtár-szinkronizálás automatikusan kikapcsol, amikor ezt a módszert használja.
    
    - Az Office 365 címtárszinkronizálási varázslójával szinkronizálhatja a felhasználókat a felhővel. Ezt a [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) című cikk lépéseit követve végezheti el. Miután szinkronizálta a felhasználókat a felhővel, ki kell [kapcsolnia az Office 365 címtár-szinkronizálását.](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d)
    
    A Microsoft 365 Business számára licencet kell adnia minden hozzáadott felhasználónak is. Ezt megteheti a [telepítővarázslóban,](set-up.md) vagy licenceket rendelhet a [felhasználókhoz az Office 365 vállalati verzióban.](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC)
    
### <a name="2-prepare-mobile-devices"></a>2: Mobileszközök előkészítése

Kövesse a [Mobileszközök beállítása a Microsoft 365 Vállalati verzió felhasználói számára,](set-up-mobile-devices.md) hogy Office-alkalmazásokat telepítsen az eszközökre, és győződjön meg arról, hogy a Microsoft 365 Business védi őket. 
  
### <a name="3-prepare-pcs"></a>3: Pc-k előkészítése

A rendszergazdák előre kiválaszthatják az új Windows 10-es számítógépek beállításait a [Windows AutoPilot](add-autopilot-devices-and-profile.md)használatával. A felhasználók a jelen témakör lépéseivel állíthatják be meglévő vagy új Windows 10-es eszközeiket: [Windows-számítógépek beállítása a Microsoft 365 Vállalati verzió felhasználói számára.](set-up-windows-devices.md) Meglévő eszközök esetén a felhasználók **tetszés szerint** [áthelyezhetnek fájlokat a OneDrive Vállalati verzióba.](move-files-to-onedrive.md) Külső gyártótól származó eszközökkel is áthelyezhetik a Windows-profilhoz társított fájlokat a OneDrive-ra.
  
Ha szervezete a helyszínen használja a Windows Server Active Directoryt, beállíthatja a Microsoft 365 Business alkalmazást a Windows 10-es eszközök védelmére, miközben továbbra is hozzáférhet a helyi hitelesítést igénylő helyszíni erőforrásokhoz. Kövesse a [Microsoft 365 Business által felügyelt tartományhoz csatlakozó Windows 10-eszközök engedélyezése](manage-windows-devices.md) című részt. Ez a módszer ajánlott, és az ebben az állapotban lévő eszközöket **hibrid Azure AD-csatlakozású eszközöknek**nevezzük. 
  
Ha megtart egy helyi Active Directoryt, amely tartalmaz néhány helyszíni erőforrást (például fájlmegosztásokat és nyomtatókat), az **Azure AD-hez csatlakozott eszközeinek** hozzáférést biztosíthat ezekhez az erőforrásokhoz az alábbi lépéseket követve: [Helyszíni erőforrások elérése egy Azure AD-hez csatlakozó eszközről a Microsoft 365 Business](access-resources.md)programban.
  
  
## <a name="contact-support"></a>Ügyfélszolgálat

 **Ha kapcsolatba szeretne lépni az ügyfélszolgálattal:**
  
- Forduljon a partneréhez.
    
- Microsoft 365 Vállalati verzió rendszergazdájaként hozzáférhet ügyfélszolgálati csapatunkhoz: Lépjen kapcsolatba az ** [üzleti termékek ügyfélszolgálatával – Rendszergazdai súgó](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b)**
    
## <a name="see-also"></a>Lásd még

[A Microsoft 365 Vállalati verzióval kapcsolatos dokumentáció és források](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[A Microsoft 365 Vállalati verzió kezelése](manage.md)[Áttelepítés a Microsoft 365 Vállalati verzióba](migrate-to-microsoft-365-business.md)

[Microsoft 365 Vállalati verziós oktatóvideók](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) 

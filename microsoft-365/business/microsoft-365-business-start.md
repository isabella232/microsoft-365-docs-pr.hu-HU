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
description: Tudnivalók a Microsoft 365 Vállalati verzióról, a beállításról, valamint a felhasználói eszközök és PC-k felkészít arról, hogy a Microsoft 365 Vállalati verzió védelmet nyújt nekik.
ms.openlocfilehash: ec50036f589cfd8497b0e7e9af6519b30d25dcd3
ms.sourcegitcommit: 555d756c69ac9031d1fb928f2e1f9750beede066
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/29/2020
ms.locfileid: "47306489"
---
# <a name="get-started-with-microsoft-365-for-business"></a>A Microsoft 365 Vállalati verzió első lépések

## <a name="what-is-microsoft-365-for-business"></a>Mi a Microsoft 365 Vállalati verzió?

A Microsoft 365 Vállalati verzió az üzleti hatékonyságot és együttműködési eszközöket (például Outlook, Word, Excel és más Office-termékek) átfogó készlete, amely mindig naprakész. A nagyvállalati szintű, egyszerűen kezelhető, nagyvállalati szintű biztonsági megoldásokkal minden iOS-, Android- és Windows 10-es eszközén megvédheti a munkahelyi fájljait.

Ez a videó rövid áttekintést nyújt a Microsoft 365 Vállalati verzióról.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
A Microsoft 365 Vállalati verzió legfeljebb 300 licenccel rendelkezik. Ha ennél több licencre van szüksége, további információért olvassa el a [Microsoft 365 Nagyvállalati verzió](https://go.microsoft.com/fwlink/p/?linkid=860986) dokumentációját. 
  
## <a name="get-microsoft-365-for-business"></a>A Microsoft 365 Vállalati verzió lekérte

- Ha van partnere, a microsoftos 365 Vállalati verzióhoz jut hozzá: A [Microsoft 365 Vállalati](get-microsoft-365-business.md)verzió lekérte a Microsoft Partnerközpontból.
    
- Ha nincs partnere, és meg szeretné vásárolni a Microsoft 365 Vállalati verziós microsoftos verziójára vonatkozót, megvásárolhatja [itt.](https://www.microsoft.com/microsoft-365/business)
    
## <a name="set-up-microsoft-365-for-business"></a>A Microsoft 365 Vállalati verzió beállítása

 **A Microsoft 365 Vállalati verzió beállítása – áttekintés**
  
Az alábbi diagram bemutatja, hogy a rendszergazdák hogyan állíthatják be a Microsoft 365 Vállalati verziót. Ismerteti azokat a lépéseket is, amelyek a Windows rendszerű PC-ket felkészítik a Microsoft 365 Vállalati verzióra. Új eszközöket is felvehet a Microsoft 365 Felügyeleti központban a [Windows AutoPilottal.](add-autopilot-devices-and-profile.md) Az AutoPilot segítségével beállíthatja és előre konfigurálhatja az új eszközöket, hogy azok azonnal használatra készek legyenek, amint a felhasználó bejelentkezik a Microsoft 365 Vállalati verziós hitelesítő adataival.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

Ebből a videóból áttekintheti a Microsoft 365 Vállalati verzió beállítását.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Ha hasznosnak találta ezt a videót, tekintse meg a [teljes tanfolyamok kisvállalatoknak és Microsoft 365-újoncoknak](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) című cikket.

  
### <a name="1-set-up-microsoft-365-for-business-admin"></a>1: A Microsoft 365 Vállalati verzió beállítása (rendszergazda)

Jelentkezzen be a [Microsoft 365](https://portal.office.com/adminportal/home) Felügyeleti központba globális rendszergazdai hitelesítő adataival, és az alábbi lépéseket követve állítsa be a Microsoft 365 Vállalati verziót. 
  
1. [A Microsoft 365 Vállalati verziós eszközök adatainak védelmére vonatkozó előfeltételek](pre-requisites-for-data-protection.md)
    
    Először olvassa el az előfeltételeket, és győződjön meg arról, hogy eszközei készen állnak a Microsoft 365 Vállalati verzió használatára.
    
2. [A Microsoft 365 Vállalati verzió beállítása a beállítási varázslóval](set-up.md)
    
    Ha egy helyi **Active Directoryból** véglegesen a felhőbe szeretne áttérni, lépjen a Microsoft 365 Felügyeleti központba, és a beállítási varázslóval manuálisan vegye fel a felhasználókat, vagy egy alkalommal szinkronizálja az Azure AD Connectet. Ehhez két lehetőség közül választhat: 
    
    - Ha Exchange 2010-, Exchange 2013- vagy Exchange 2016-kiszolgálója is van, akkor a hibrid minimumkontraszttal gyorsan át lehet miolni az Exchange-postaládákat a [Microsoft 365-be.](https://docs.microsoft.com/Exchange/mailbox-migration/use-minimal-hybrid-to-quickly-migrate) A minimális hibrid lépések közé tartozik a felhasználók egy alkalommal való szinkronizálása az Azure AD-be, és a levelezés áttelepítése a helyszíni környezetből a felhőbe. A levelezés áttelepítése után a címtár-szinkronizálás automatikusan kikapcsol, amikor ezt a módszert használja.
    
    - A címtár-szinkronizálási varázslóval szinkronizálhatja a felhasználókat a felhőbe. A folyamat befejezéséhez kövesse a Címtár-szinkronizálás beállítása [a Microsoft 365-ben](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) lépéseit. Miután szinkronizálta a felhasználókat a felhőbe, ki kell kapcsolnia a címtár-szinkronizálást a [Microsoft 365-ben.](https://docs.microsoft.com/microsoft-365/enterprise/turn-off-directory-synchronization)
    
    Ezenkívül minden ilyen módon hozzáadott felhasználónak licencet kell adni a Microsoft 365 Vállalati verzióhoz. Ezt a beállítási [varázslóban](set-up.md) vagy a felhasználókhoz [is hozzárendelheti.](../admin/manage/assign-licenses-to-users.md)
    
### <a name="2-prepare-mobile-devices"></a>2: A mobileszközök előkészítése

A Mobileszközök beállítása a [Microsoft 365](set-up-mobile-devices.md) Vállalati verzió felhasználóinak lépéseit követve telepítse az Office-appokat az eszközökre, és győződjön meg arról, hogy a Microsoft 365 Vállalati verzió védi őket. 
  
### <a name="3-prepare-pcs"></a>3: PC-k előkészítése

A rendszergazdák előre kiválaszthatják az új Windows 10-es PC-k beállításait a [Windows AutoPilottal.](add-autopilot-devices-and-profile.md) A felhasználók a következő témakörben található lépéseket követve állíthatják be meglévő vagy új Windows 10-es eszközeiket: Windows rendszerű PC-k beállítása a [Microsoft 365 Vállalati verzió felhasználóinak.](set-up-windows-devices.md) Meglévő eszközök esetén  a felhasználók tetszés szerint áthelyezhet fájlokat a [OneDrive Vállalati verzióba.](move-files-to-onedrive.md) Külső eszközökkel is áthelyezheti a Windows-profillal társított fájlokat a OneDrive-ra.
  
Ha szervezete helyszíni Windows Server Active Directoryt használ, beállíthatja a Microsoft 365 Vállalati verziót a Windows 10-es eszközök védelmére, miközben továbbra is hozzáfér a helyi hitelesítést igénylő helyszíni erőforrásokhoz. A beállítás beállításához kövesse az [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 for business](manage-windows-devices.md) (Tartományhoz csatlakozott Windows 10-es eszközök engedélyezése) beállítás lépéseit. Ez a módszer előnyben részesített, és az ebben az állapotban használt eszközöket hibrid **Azure AD-hez csatlakozott eszközöknek nevezzük.** 
  
Ha olyan helyi Active Directoryt őriz meg, amely helyszíni erőforrásokat (például fájlmegosztásokat és nyomtatókat) tartalmaz, az alábbi lépéseket követve hozzáférést adhat az **Azure AD-hez** csatlakozott eszközöknek: A [Microsoft 365](access-resources.md)Vállalati verzió helyszíni erőforrásainak elérése Azure AD-hez csatlakozott eszközről.
  
  
## <a name="contact-support"></a>Ügyfélszolgálat

 **Ha kapcsolatba szeretne lépni az ügyfélszolgálattal:**
  
- Forduljon a partneréhez.
    
- A Microsoft 365 Vállalati verzió rendszergazdájaként hozzáférhet ügyfélszolgálati csapatunkhoz: Kapcsolatfelvétel a vállalati termékek **[ügyfélszolgálatával – rendszergazdai súgó](https://docs.microsoft.com/microsoft-365/admin/contact-support-for-business-products)**
    
## <a name="see-also"></a>Lásd még

[A Microsoft 365 Vállalati verzió dokumentációja és forrásai](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[A Microsoft 365 Vállalati](manage.md)verzió áttelepítése a[Microsoft 365 Vállalati verzióba](migrate-to-microsoft-365-business.md)

[Microsoft 365 Vállalati verziós oktatóvideók](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) 

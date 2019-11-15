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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Ismerje meg, hogy hozzanak létre a Microsoft 365 Business.
ms.openlocfilehash: 5986e3fb7786ebb3fa7bcf42b34345be98af44a2
ms.sourcegitcommit: 9a057e70637dcfe06d4f729a96c02be989cf9e25
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/14/2019
ms.locfileid: "38633429"
---
# <a name="get-started-with-microsoft-365-business"></a>A Microsoft 365 Business használatbavétele

## <a name="what-is-microsoft-365-business"></a>Mi a Microsoft 365 Vállalati verzió?

A Microsoft 365 Business egy átfogó üzleti termelékenységi és együttműködési eszköz, például az Outlook, a Word, az Excel és más Office termékek, amelyek mindig naprakész. Tudod megvéd-a dolgozik fájlokat-ra minden-a iOS, Android, és Windows 10 berendezés-val vállalat-osztályoz biztonság ez minden egyszerű-hoz kezel.
  
Mikroszkóp 365 teendő van tervezett részére valameddig 300 engedélyez. Ha további licencekre van szüksége, további információért olvassa el a [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986) dokumentációjában található tudnivalókat. 
  
## <a name="get-microsoft-365-business"></a>A Microsoft 365 Vállalati verzió beszerzése

- Ha önnek van egy társ, ők ' kap Mikroszkóp 365 teendő: [kap mikroszkóp 365 teendő-bólMikroszkóp társ központ](get-microsoft-365-business.md).
    
- Ha nincs partnere, és meg szeretné vásárolni a Microsoft 365 Businesst, [itt megteheti](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>A Microsoft 365 Vállalati verzió beállítása

 **A Microsoft 365 Business Suite programcsomag áttekintése**
  
A következő ábra leírja, hogyan kell beállítani a Microsoft 365 Business az adminok. Ezenkívül a Windows rendszerű PC-k Microsoft 365 Business használatára való előkészítésének lépéseit is tartalmazza. Új eszközöket is hozzáadhat a Microsoft 365 Business admin Centerhez a [Windows robotpilóta](add-autopilot-devices-and-profile.md)segítségével. A robotpilóta segítségével beállíthat és konfigurálhat új eszközöket, hogy azok készen állnak a hatékony használatra, amint a felhasználó bejelentkezik a Microsoft 365 Business hitelesítő adataival.
  
![A diagram that shows the setup and management flow for admins, and also for a user](media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)
  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: állítsa be a Microsoft 365 Business (admin)

Jelentkezzen be a [microsoft 365 Business Admin Center](https://portal.office.com/adminportal/home) webhelyére a globális rendszergazdai hitelesítő adataival, majd a Microsoft 365 Business beállításához hajtsa végre az alábbi lépéseket. 
  
1. [A Microsoft 365 Business és egy eszköz adatvédelmének előfeltételei](pre-requisites-for-data-protection.md)
    
    Először olvassa el az előfeltételeket, hogy megbizonyosodjon arról, hogy az eszközök készen állnak a Microsoft 365 Business.
    
2. [A telepítővarázsló segítségével állítsa be a Microsoft 365 Business](set-up.md)
    
    Ha **véglegesen áthelyezi a helyi Active Directory címtárat a felhőbe**, látogasson el a Microsoft 365 Business Admin Center webhelyére, és használja a telepítővarázslót a felhasználók manuális hozzáadásához, vagy egy egyszeri szinkronizálást az Azure ad Connect segítségével. Ehhez két lehetőség közül választhat: 
    
    - Ha rendelkezik Exchange 2010, Exchange 2013 vagy Exchange 2016 kiszolgálóval is, akkor [a minimális hibrid használatával gyorsan áttelepítheti az Exchange-postaládákat az Office 365](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef)kiszolgálóra. A minimális hibrid lépések közé tartozik egy egyszeri szinkronizálás a felhasználók Azure AD, és az e-mail migráció helyszíni a felhő. Az e-mailek áttelepítése után a címtár-szinkronizálás automatikusan kikapcsol, ha ezt a módszert használja.
    
    - Az Office 365 címtár-szinkronizáló varázsló segítségével szinkronizálja a felhasználókat a felhővel. Ezt a [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) című cikk lépéseit követve végezheti el. Miután a felhasználókat szinkronizálja a felhővel, [ki kell kapcsolnia az Office 365 címtár-szinkronizálást](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Youll ' is kell ad mindegyik felhasználó amit volt hozzáadott így egy engedély-hoz Mikroszkóp 365 teendő. Ezt megteheti a [telepítővarázslóban](set-up.md) , de az [Office 365 for Business felhasználói számára is rendelhet licenceket](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC).
    
### <a name="2-prepare-mobile-devices"></a>2: mobileszközök előkészítése

Kövessük a [microsoft 365. üzleti felhasználók számára a mobil eszközök beállítása](set-up-mobile-devices.md) című témakört, és telepítsük az Office alkalmazásokat az eszközökre, és győződjünk meg arról, hogy a Microsoft 365 Business védi őket. 
  
### <a name="3-prepare-pcs"></a>3: készítsünk PC-k

Admins tud előre kiválaszt elintézés részére új Windows 10 PCs mellett használ [Windows robotpilóta](add-autopilot-devices-and-profile.md). A felhasználók a jelen témakörben ismertetett lépések végrehajtásával beállhatják meglévő vagy új Windows 10 eszközeiket: a [Windows PC-k Microsoft 365 üzleti felhasználók számára történő beállításához](set-up-windows-devices.md). Részére létező berendezés, használók tud **tetszés szerint** [mozog fájlokat-hoz onedrive részére teendő](move-files-to-onedrive.md). Ők tud is használ harmadik-csapat szerszámok-hoz mozog fájlokat társult-val Windows arcél-hoz OneDrive.
  
Ha a szervezet helyi Windows Server Active Directoryt használ, beállíthatja a Microsoft 365 Business rendszert, hogy védje a Windows 10 eszközeit, miközben továbbra is fenntartja az intézményi erőforrásokhoz való hozzáférést, amelyekhez szükség van lokális hitelesítésre. Hajtsa végre a [Microsoft 365 Business által felügyelt, tartományhoz csatlakoztatott Windows 10 eszközök engedélyezésére](manage-windows-devices.md) vonatkozó lépéseket. Ezt a módszert kell előnyben részesíteni, és az ilyen állapotú eszközöket **hibrid azúrkék hirdetési eszközöknek**is nevezzük. 
  
Ha olyan helyi Active Directoryt tart fenn, amely az intézményi erőforrásokat (például a fájlmegosztásokat vagy a nyomtatókat) tartalmazza, az **azúrkék ad-illesztett eszközök** a következő lépések végrehajtásával férhetnek hozzá ezekhez az erőforrásokhoz: a [Microsoft 365 Business-ben található Azure Active Directory-eszköz intézményi erőforrásainak elérése](access-resources.md).
  
A Windows 10 PC-k beállítása után az [Office automatikusan telepíthető](auto-install-or-uninstall-office.md) az eszközökre. 
  
## <a name="contact-support"></a>Lépjen kapcsolatba a támogatási szolgálattal.

 **Ha kapcsolatba szeretne lépni az ügyfélszolgálattal:**
  
- Forduljon a partneréhez.
    
- Mint a Microsoft 365 Business admin, akkor hozzáférhet az ügyfélszolgálati Csoport: ** [Kapcsolatfelvétel üzleti termékek támogatása-admin Súgó](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b)**
    
## <a name="related-topics"></a>Kapcsolódó témakörök
[A Microsoft 365 Vállalati verzióval kapcsolatos dokumentáció és források](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[A Microsoft 365 Vállalati verzió kezelése](manage.md)[Áttelepítés a Microsoft 365 Vállalati verzióba](migrate-to-microsoft-365-business.md)
  


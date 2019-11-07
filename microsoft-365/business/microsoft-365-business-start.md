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
ms.openlocfilehash: 4c744d6a900dba3c11ee51e75602a430268e15bb
ms.sourcegitcommit: 70e920f76526f47fc849df615de4569e0ac2f4be
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/07/2019
ms.locfileid: "38029104"
---
# <a name="get-started-with-microsoft-365-business"></a>A Microsoft 365 Business használatbavétele

## <a name="what-is-microsoft-365-business"></a>Mi a Microsoft 365 Vállalati verzió?

A Microsoft 365 Vállalati verzió a vállalati hatékonyságot és együttműködést elősegítő eszközök átfogó gyűjteménye, amely például olyan termékeket tartalmaz, mint az Outlook, a Word, az Excel és egyéb Office-termékek, amelyek mindig naprakészek. Az egyszerűen kezelhető, nagyvállalati szintű biztonsági funkciókkal minden iOS, Android és Windows 10 rendszerű eszközén megvédheti a munkahelyi fájljait.
  
A Microsoft 365 Business legfeljebb 300 licenccel való használatra készült. Ha ennél több licencre van szüksége, további információért olvassa el a [Microsoft 365 Nagyvállalati verzió](https://go.microsoft.com/fwlink/p/?linkid=860986) dokumentációját. 
  
## <a name="get-microsoft-365-business"></a>A Microsoft 365 Vállalati verzió beszerzése

- Ha van partnere, az illető meg fogja kapni a Microsoft 365 Businesst: [A Microsoft 365 Vállalati verzió beszerzése a Microsoft Partnerközpontban](get-microsoft-365-business.md).
    
- Ha nincs partnere, és meg szeretné vásárolni a Microsoft 365 Businesst, [itt megteheti](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>A Microsoft 365 Vállalati verzió beállítása

 **A Microsoft 365 Business Suite programcsomag áttekintése**
  
A következő ábra leírja, hogyan kell beállítani a Microsoft 365 Business az adminok. Ezenkívül a Windows rendszerű PC-k Microsoft 365 Business használatára való előkészítésének lépéseit is tartalmazza. Új eszközöket is felvehet a Microsoft 365 Business Felügyeleti központban a [Windows AutoPilot](add-autopilot-devices-and-profile.md) segítségével. Ha az AutoPilot segítségével előre beállítja és konfigurálja az eszközöket, a felhasználók hatékonyan használhatják őket, amint bejelentkeznek a Microsoft 365 Business szolgáltatásban érvényes hitelesítő adataikkal.
  
![A diagram that shows the setup and management flow for admins, and also for a user](media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)
  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: állítsa be a Microsoft 365 Business (admin)

Jelentkezzen be a [Microsoft 365 Vállalati verzió Felügyeleti központba](https://portal.office.com/adminportal/home) globális rendszergazdai hitelesítő adataival, majd a Microsoft 365 Business beállításához kövesse az alábbi lépéseket. 
  
1. [A Microsoft 365 Vállalati verziót tartalmazó eszközök adatvédelmének előfeltételei](pre-requisites-for-data-protection.md)
    
    Az eszközök kompatibilitásának ellenőrzéséhez elsőként olvassa el a Microsoft 365 Business előfeltételeit.
    
2. [A Microsoft 365 Vállalati verzió beállítása a beállítási varázslóval](set-up.md)
    
    Ha **véglegesen áthelyezi a helyi Active Directory címtárat a felhőbe**, a felhasználók manuálisan hozzáadhatók a Microsoft 365 Business admin Centerhez a telepítővarázslóval, de egyszeri szinkronizálás is történhet az Azure ad Connect alkalmazással. Ehhez két lehetőség közül választhat: 
    
  - Ha rendelkezik Exchange 2010, Exchange 2013 vagy Exchange 2016 kiszolgálóval is, akkor [a minimális hibrid használatával gyorsan áttelepítheti az Exchange-postaládákat az Office 365](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef)kiszolgálóra. A hibrid minimumkonfiguráció lépései részeként egyszeri szinkronizálást kell végeznie a felhasználókon az Azure AD-vel, valamint a helyszíni kiszolgálóról a felhőbe kell migrálnia az e-maileket. Ha ezt a módszert alkalmazza, az e-mail-migrálás befejeztével a program automatikusan kikapcsolja a címtár-szinkronizálást.
    
  - Az Office 365 címtár-szinkronizálási varázslójával szinkronizálhatja a felhasználókat a felhőbe. Ezt a [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) című cikk lépéseit követve végezheti el. Miután szinkronizálta a felhasználókat a felhőbe, [Turn off directory synchronization for Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Az ily módon felvett felhasználóknak ezenkívül a Microsoft 365 Vállalati verzióra szóló licencet kell adnia. Ezt megteheti a [telepítővarázslóban](set-up.md)vagy a [licencek hozzárendelése az Office 365 az üzleti életben felhasználók](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC)számára.
    
### <a name="2-prepare-mobile-devices"></a>2: mobileszközök előkészítése

Kövessük a[microsoft 365. üzleti felhasználóknak szánt mobil eszközök beállítása](set-up-mobile-devices.md) című részt, hogy telepítsenek Office alkalmazásokat az eszközökre, és megbizonyosodjunk arról, hogy a Microsoft 365 Business védi őket. 
  
### <a name="3-prepare-pcs"></a>3: készítsünk PC-k

Admins tud előre kiválaszt elintézés részére új berendezés Windows 10 PCs mellett használ [Windows robotpilóta](add-autopilot-devices-and-profile.md). A felhasználók a jelen témakörben ismertetett lépések végrehajtásával beállhatják meglévő vagy új Windows 10 eszközeiket: a [Windows PC-k Microsoft 365 üzleti felhasználók számára történő beállításához](set-up-windows-devices.md). Részére létező berendezés használók tud is **tetszés szerint**[mozog fájlokat-hoz onedrive részére teendő](move-files-to-onedrive.md). Ők tud is használ harmadik-csapat szerszámok-hoz mozog fájlokat társult-val Windows arcél-hoz OneDrive.
  
Ha a szervezet helyi Windows Server Active Directoryt használ, beállíthatja a Microsoft 365 Business rendszert, hogy védje a Windows 10 eszközeit, miközben továbbra is fenntartja az intézményi erőforrásokhoz való hozzáférést, amelyekhez szükség van lokális hitelesítésre. Hajtsa végre a [Microsoft 365 Business által felügyelt, tartományhoz csatlakoztatott Windows 10 eszközök engedélyezésére](manage-windows-devices.md) vonatkozó lépéseket. Ez az adott állapotú módszer és eszközök az úgynevezett **hibrid Azure egyesített eszközök**. 
  
Ha olyan helyi Active Directoryt tart fenn, amely az intézményi erőforrásokat (például a fájlmegosztásokat vagy a nyomtatókat) tartalmazza, az **azúrkék ad-illesztett eszközök** a következő lépések végrehajtásával férhetnek hozzá ezekhez az erőforrásokhoz: az [intézményi erőforrások elérése egy Azúrkék hirdetés-összekapcsolt berendezés-ban Mikroszkóp 365 teendő](access-resources.md).
  
A Windows 10 PC-k beállítása után az [Office automatikusan telepíthető](auto-install-or-uninstall-office.md) az eszközökre. 
  
## <a name="contact-support"></a>Lépjen kapcsolatba a támogatási szolgálattal.

 **Ha kapcsolatba szeretne lépni az ügyfélszolgálattal:**
  
- Forduljon a partneréhez.
    
- Mint a Microsoft 365 Business admin, akkor hozzáférhet az ügyfélszolgálati csapatunk, ** [forduljon támogatás üzleti termékek-admin Súgó](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b)**
    
## <a name="related-topics"></a>Kapcsolódó témakörök
[A Microsoft 365 Vállalati verzióval kapcsolatos dokumentáció és források](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[A Microsoft 365 Vállalati verzió kezelése](manage.md)[Áttelepítés a Microsoft 365 Vállalati verzióba](migrate-to-microsoft-365-business.md)
  


---
title: A tartományhoz csatlakoztatott Windows 10-es eszközök kezelésének engedélyezése a Microsoft 365 Vállalati verzió számára
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Útmutató a Microsoft 365 védelmének engedélyezése helyi AD Windows 10 eszközök csatlakozott.
ms.openlocfilehash: d61b3bf6be50d6b21e7b883774567bb63995e60e
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32278077"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>A tartományhoz csatlakoztatott Windows 10-es eszközök kezelésének engedélyezése a Microsoft 365 Vállalati verzió számára

Ha a szervezet használja a Windows Server Active Directory helyszíni, állíthat be Microsoft 365 üzleti védelme érdekében a Windows 10 eszközök továbbra is fenntartva helyi hitelesítést igénylő helyszíni erőforrásokhoz való hozzáférést. Beállíthatja a által első szinkronizálása az Active Directory Azure Active Directory regisztrálja a Windows 10 eszközök Azure AD, majd azokat igénylése Microsoft 365 üzleti mobil eszköz kezelésére.
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a>Microsoft 365 üzleti által kezelt tartományhoz csatlakoztatott eszközök beállítása

Tartományhoz csatlakoztatott eszközök a szervezet beállítása a Azure Active Directory mellett helyszíni Active Directory nyújtotta lehetőségeket élvezhessék, megvalósítható **hibrid Azure AD eszközöket csatlakozott**. Ezek olyan eszközök, amelyek mind a helyszíni Active Directory és az Azure Active Directory tartományhoz. Hibrid csatlakozott Azure AD eszközöket védett, és kezeli a Microsoft 365 Business... 
  
Hajtsa végre az alábbi lépéseket a Windows 10 eszközök hibrid Azure AD a tartományhoz, és kezeli a Microsoft 365 Business.
  
1. A felhasználók, csoportok és a helyi Active Directory ügyfelek Active Directory Azure szinkronizálásához futtassa a címtár-szinkronizálás varázsló és Azure Active Directory csatlakozás az [Office 365 címtár-szinkronizálás beállítása](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
    > [!NOTE]
    > A lépések azonosak, pontosan 365 üzleti Microsoft. 
  
2. 3. lépést ahhoz, hogy Windows 10 eszközök hibrid Azure AD a tartományhoz kell, meg kell győződjön meg arról, hogy teljesülnek a következő előfeltételek:
    
   - Borzas AD a legújabb verzióját futtatja csatlakozni.
    
   - Borzas AD csatlakozás van szinkronizálva legyen hibrid Azure AD csatlakozott az eszközök számítógép-objektumok. Ha a számítógép-objektumok adott szervezeti egység (OU) tartozó, majd állítsuk a szervezeti egységek az Azure Active Directory szinkronizálási kapcsolatot, valamint.
    
3. Meglévő tartományhoz tartozó Windows 10 eszközök Azure AD Joined hibrid és Intune (Microsoft 365 Business) mobil eszköz kezelésére őket igényelni regisztrálása:
    
4. [Hibrid Azure Active Directory tartományhoz eszközök konfigurálása](https://go.microsoft.com/fwlink/p/?linkid=872870)lépésről lépésre kövesse. Ez lehetővé teszi a helyi Active Directory szinkronizálása Windows 10 számítógépek tartományhoz, és azokat a felhő kész.
    
5. Annak érdekében, hogy egy mobil eszköz kezelése Windows 10 eszköz igényléséhez utasításokat [igényelni egy Intune a csoportházirend segítségével Windows 10 eszközt](https://go.microsoft.com/fwlink/p/?linkid=872871) talál. Beállíthatja a csoportházirend egy olyan helyi számítógép szinten, vagy a tömeges műveletek esetében a tartomány vezérlő-kiszolgálón hozhat létre a csoportházirend-beállítás. 
    


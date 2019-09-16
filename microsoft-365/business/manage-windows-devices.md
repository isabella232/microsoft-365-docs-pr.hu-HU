---
title: A tartományhoz csatlakoztatott Windows 10-es eszközök kezelésének engedélyezése a Microsoft 365 Vállalati verzió számára
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
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
description: Útmutató a Microsoft 365 a helyi AD-hez csatlakozott Windows 10-eszközök védelmének engedélyezéséhez.
ms.openlocfilehash: 5cce4bc53f118560e31ad7e6048e4efcb49d662e
ms.sourcegitcommit: c0f769244d05ad019ea2307c38d5543d7b1e5afd
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992229"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>A tartományhoz csatlakoztatott Windows 10-es eszközök kezelésének engedélyezése a Microsoft 365 Vállalati verzió számára

Ha a szervezet helyi Windows Server Active Directoryt használ, beállíthatja a Microsoft 365 Business rendszert, hogy védje a Windows 10 eszközeit, miközben továbbra is fenntartja az intézményi erőforrásokhoz való hozzáférést, amelyekhez szükség van lokális hitelesítésre. Ezt úgy állíthatja be, hogy először a Azure Active Directoryval szinkronizálja az Active Directory címtárat, majd regisztrálja a Windows 10 eszközöket az azúrkék HIRDETÉSRE, és a Microsoft 365 Business mobileszköz-kezelést végez.
A következő videó részletesen ismerteti, hogy hogyan lehet ezt beállítani a leggyakoribb forgatókönyvhöz.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a>A Microsoft 365 Business által kezelhető, tartományhoz csatlakoztatott eszközök beállítása

Ahhoz, hogy a szervezet tartományhoz csatlakoztatott eszközeit úgy állítsa be, hogy a helyszíni Active Directory címtáron kívül az Azure Active Directory által nyújtott szolgáltatások előnyeit is élvezheti, a **hibrid Azure beépített eszközöket**is implementálja. Ezek olyan eszközök, amelyek mind a helyi Active Directory címtárba, mind a Azure Active Directoryba csatlakoztak. A Hybrid Azure egyesített eszközök a Microsoft 365 Business által védhetők és kezelhetők. 
  
Hajtsa végre az alábbi lépéseket a Microsoft 365 Business által a Hybrid Azure AD által egyesített és kezelt Windows 10-eszközök elérhetővé tétele érdekében.
  
1. A felhasználók, csoportok és kapcsolattartók helyi Active Directoryból Azure Active Directoryba történő szinkronizálásához futtassa a címtár-szinkronizálás varázslót és az Azure Active Directory csatlakozási szolgáltatást az [Office 365 címtár-szinkronizálás beállítása](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)című témakörben leírtak szerint.
    
    > [!NOTE]
    > A lép van pontosan ugyanaz részére Mikroszkóp 365 teendő. 
  
2. A 3. lépés elvégzése előtt ahhoz, hogy a Windows 10 eszközök Hybrid Azure AD csatlakozhatók legyenek, a következő előfeltételeknek kell eleget tennie:

   - A legújabb verziójú Azure AD Connect-et futtatja.

   - Azúrkék AD összeköt birtokol szinkronizál minden a számítógép tárgy-ból berendezés ön akar-hoz lenni hibrid Azure AD összekapcsolt. Ha a számítógép-objektumok meghatározott szervezeti egységekhez tartoznak, akkor győződjön meg arról, hogy ezek a szervezeti egységek szinkronizálásra vannak beállítva a Azure AD Connect-ben is.
    
3. Regisztrálja a meglévő, tartományhoz csatlakoztatott Windows 10-eszközöket a hibrid Azure AD-hez, és igényelje azokat az Intune (Microsoft 365 Business) mobil eszközkezelésére:
    
4. Kövesse lépésről lépésre, [Hogyan állítsuk be a hibrid Azure Active Directory egyesített eszközeit](https://go.microsoft.com/fwlink/p/?linkid=872870). Ez lehetővé teszi az intézményi Active Directory-nak a Windows 10 számítógépekhez való szinkronizálását, és készen áll a felhőre.
    
5. A Windows 10 eszköz mobil eszközkezelés céljából történő igényléséhez tekintse meg a [Windows 10 eszköznek az Intune szolgáltatással történő igénylésével](https://go.microsoft.com/fwlink/p/?linkid=872871) kapcsolatos utasításokat a csoportházirend segítségével. A csoportházirendet beállíthatja helyi számítógépszinten vagy tömeges műveleteknél, ezt a csoportházirend-beállítást létrehozhatja a tartományvezérlő-kiszolgálón is.
---
title: Tartományfelhasználók szinkronizálása a Microsoft 365-be
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
description: Szinkronizálja a tartományvezérelt felhasználókat a Microsoft 365 Vállalati verzióval.
ms.openlocfilehash: b40a995a1723808d2fd171c534e9131a891840ba
ms.sourcegitcommit: e56894917d2aae05705c3b9447388d10e2156183
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48841359"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a>Tartományfelhasználók szinkronizálása a Microsoft 365-be

## <a name="1-prepare-for-directory-synchronization"></a>1. Felkészülés a címtár-szinkronizálásra 

Mielőtt szinkronizálja a felhasználókat és a számítógépeket a helyi Active Directory-tartományból, tekintse át a Felkészülés a Címtár-szinkronizálásra a [Microsoft 365-ben.](https://docs.microsoft.com/microsoft-365/enterprise/prepare-for-directory-synchronization) Különösen:

   - Győződjön meg arról, hogy a címtárban nincsenek ismétlődő attribútumok a következő attribútumok esetén: **mail,** **proxyAddresses** és **userPrincipalName.** Ezeknek az értékeknek egyedinek kell lennie, az ismétlődő értékeket pedig el kell távolítani.
   
   - Azt javasoljuk, hogy állítsa be a **userPrincipalName** (UPN) attribútumot az egyes helyi felhasználói fiókokhoz úgy, hogy megegyeznek a licencelt Microsoft 365-felhasználónak megfelelő elsődleges e-mail-címmel. Például: *mary.shelley@contoso.com* a *mary@contoso.local helyett*
   
   - Ha az Active Directory-tartomány egy nem átirányítható utótaggal (például *.local* vagy *.lan)* végződik egy internetes átirányítható utótag (például *.com* vagy *.org)* helyett, először módosítsa a helyi felhasználói fiókok UPN-utótagját a Nem átirányítható tartomány előkészítése [címtár-szinkronizálásra](https://docs.microsoft.com/microsoft-365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization)leírásának megfelelően. 

Az alábbi, 4. lépésben lefutott **IdFix** futtatása azt is meg fogja győződni arról, hogy a helyszíni Active Directory készen áll a címtár-szinkronizálásra.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Az Azure AD Connect telepítése és konfigurálása

Ha szinkronizálni szeretné a felhasználókat, csoportokat és névjegyeket a helyi Active Directoryból az Azure Active Directoryba, telepítse az Azure Active Directory Connectet, és állítsa be a címtár-szinkronizálást. 

 1. A Felügyeleti [központban válassza](https://go.microsoft.com/fwlink/p/?linkid=2024339)a **bal** oldali navigációs sávOn a Beállítás lehetőséget.

 2. A **Bejelentkezés és biztonság** csoportban válassza a **Nézet** lehetőséget a Felhasználók szinkronizálása csoportban a szervezet **címtárában.**

 3. A felhasználók **szinkronizálása a** szervezet címtárlapján válassza az **Első lépések lehetőséget.**

 4. Az első lépésben futtassa az IdFix eszközt a címtár-szinkronizálás előkészítéséhez.

 5. A varázsló lépéseit követve töltse le az Azure AD Connectet, és ezzel szinkronizálja a tartományvezérelt felhasználókat a Microsoft 365-be.


További [információ: Címtár-szinkronizálás beállítása a Microsoft 365-ben.](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization)

Az Azure AD Connect beállításainak konfigurálásakor azt javasoljuk, hogy engedélyezze a  jelszó-szinkronizálást, a zökkenőmentes egyszeri bejelentkezést és a jelszóvisszaírási funkciót, amelyet a Microsoft 365 Vállalati verzió is támogat. 

> [!NOTE]
> Az Azure AD Connect jelölőnégyzete után további lépésekkel is visszaírhatja a jelszavakat. További információt a ["How-to: configure password writeback" (Jelszóvisszaírás konfigurálása)](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback) 

Ha a tartományhoz csatlakozott Windows 10-es eszközöket is kezelni szeretné, a Tartományhoz csatlakozott [Windows 10-es](manage-windows-devices.md) eszközök kezelése a Microsoft 365 Vállalati prémium verzióval a hibrid Azure AD Join beállításához. 
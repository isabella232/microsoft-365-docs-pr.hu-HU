---
title: A tartományi felhasználók szinkronizálása a Microsoft 365
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
description: Tartomány által felügyelt felhasználók szinkronizálása a Microsoft 365 vállalati verzióval.
ms.openlocfilehash: b40a995a1723808d2fd171c534e9131a891840ba
ms.sourcegitcommit: e56894917d2aae05705c3b9447388d10e2156183
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48841359"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a>A tartományi felhasználók szinkronizálása a Microsoft 365

## <a name="1-prepare-for-directory-synchronization"></a>1. Felkészülés a címtár-szinkronizálásra 

Mielőtt szinkronizálni szeretné a felhasználókat és a számítógépeket a helyi Active Directory-tartományból, tanulmányozza a [címtár-szinkronizálás előkészítése a Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/prepare-for-directory-synchronization)-ra című részt. Különösen:

   - Győződjön meg arról, hogy a címtárban nincsenek ismétlődések a következő attribútumok esetében: **posta** , **ProxyAddresses** és **userPrincipalName**. Ezeknek az értékeknek egyedinek kell lenniük, és minden ismétlődést el kell távolítani.
   
   - Azt javasoljuk, hogy állítsa be az **userPrincipalName** (UPN) attribútumot mindegyik helyi felhasználói fiókhoz, hogy megegyezzen a licenccel rendelkező Microsoft 365-felhasználóhoz tartozó elsődleges e-mail-címmel. Például: *Mary.Shelley@contoso.com* helyett *Mary@contoso. local*
   
   - Ha az Active Directory-tartomány nem átirányítható (például. com vagy *. org* ) (például. *com* vagy. org) végződésű útválasztással *végződik, a* helyi felhasználói fiókokhoz tartozó UPN-utótagot a [címtár-szinkronizáláshoz nem útválasztásos tartomány](https://docs.microsoft.com/microsoft-365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization)létrehozása című témakörben leírtak szerint állítsa *be.* 

A **Futtatás IdFix** az alábbi négy lépésben (4) az alábbi lépésekkel gondoskodhat arról is, hogy a helyszíni Active Directory készen áll a címtár-szinkronizálásra.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. az Azure AD Connect telepítése és beállítása

Ha a helyi Active Directoryból szeretné szinkronizálni a felhasználókat, a csoportokat és a névjegyeket az Azure Active Directoryhoz, telepítse az Azure Active Directory Connect alkalmazást, és állítsa be a címtár-szinkronizálást. 

 1. A [felügyeleti központban](https://go.microsoft.com/fwlink/p/?linkid=2024339)válassza a **Setup (beállítás** ) lehetőséget a bal oldali navigációs sávon.

 2. A **Bejelentkezés és biztonság** csoportban válassza **a szervezet címtárában lévő felhasználók szinkronizálása** csoportban a **nézet** lehetőséget.

 3. A **felhasználók szinkronizálása a szervezeti címtárból** lapon válassza az első **lépések** elemet.

 4. Az első lépésben futtassa a IdFix eszközt a címtár-szinkronizálásra való felkészüléshez.

 5. Kövesse a varázsló lépéseit az Azure AD Connect letöltéséhez, és használja azt a tartományba tartozó felhasználók szinkronizálásához a Microsoft 365-ban.


További információt a [címtár-szinkronizálás beállítása a Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) -hoz című témakörben talál.

Az Azure AD Connect beállításainak beállításakor javasoljuk, hogy engedélyezze a **Jelszó-szinkronizálást** , a **zökkenőmentes egyszeri bejelentkezést** és a jelszó- **writeback** szolgáltatást, amelyet a Microsoft 365 vállalati verzió is támogat.

> [!NOTE]
> Az Azure AD Connect writeback kívül további lépéseket is találhat a jelszavakkal kapcsolatos további lépésekhez. További információt a [jelszó-writeback beállítása](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback)című témakörben talál. 

Ha a tartományhoz csatlakoztatott Windows 10-es eszközök kezelését is szeretné használni, olvassa el a [tartományhoz csatlakoztatott Windows 10-es eszközök kezelésének engedélyezése a Microsoft 365 vállalati prémium](manage-windows-devices.md) verzióban című témakört a hibrid Azure ad-illesztések beállításához. 
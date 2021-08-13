---
title: Tartományfelhasználók szinkronizálása a Microsoft 365
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: Szinkronizálja a tartomány által vezérelt felhasználókat a Microsoft 365 Vállalati verzióval.
ms.openlocfilehash: 468fa943df55b12573f0a4f595294e39a146b1850f3c430ac2088a30991c0e60
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53809312"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a>Tartományfelhasználók szinkronizálása a Microsoft 365

## <a name="1-prepare-for-directory-synchronization"></a>1. Felkészülés a címtár-szinkronizálásra 

Mielőtt szinkronizálja a felhasználókat és a számítógépeket a helyi Active Directory-tartományból, olvassa el a Felkészülés a [címtár-szinkronizálásra](../enterprise/prepare-for-directory-synchronization.md)a Microsoft 365. Különösen:

   - Győződjön meg arról, hogy a címtárban nem léteznek ismétlődő attribútumok a **következő** attribútumok esetén: mail , **proxyAddresses** és **userPrincipalName.** Ezeknek az értékeknek egyedinek kell lennie, és az ismétlődéseket el kell távolítani.
   
   - Azt javasoljuk, hogy az egyes helyi felhasználói fiókok **userPrincipalName** (UPN) attribútumát úgy konfigurálja, hogy megegyezzon a licencelt felhasználónak Microsoft 365 e-mail-címével. Például: *mary.shelley@contoso.com.local* mary@contoso *helyett*
   
   - Ha az Active Directory-tartomány egy nem átirányítható utótaggal végződik , például *.local* vagy *.lan*, internetes átirányítható utótag (például *.com* vagy *.org)* helyett, módosítsa a helyi felhasználói fiókok UPN-utótagját a Nem átirányítható tartomány előkészítése a [címtár-szinkronizáláshoz](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md)leírt módon. 

Az **idFix futtatása** az alábbi negyedik lépésben (4) azt is meg kell győződni arról, hogy a helyszíni Active Directory készen áll-e a címtár-szinkronizálásra.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Telepítse és konfigurálja az Azure AD-Csatlakozás

Ha szinkronizálni szeretné a felhasználókat, csoportokat és névjegyeket a helyi Active Directoryból a Azure Active Directory, telepítse Azure Active Directory Csatlakozás és állítsa be a címtár-szinkronizálást. 

 1. A Felügyeleti [központban válassza](https://go.microsoft.com/fwlink/p/?linkid=2024339)a bal oldali navigációs **sávon** a Beállítás lehetőséget.

 2. A **Bejelentkezés és biztonság csoportban** válassza a Megtekintés lehetőséget a Felhasználók szinkronizálása a szervezet **címtárában csoportban.** 

 3. A Felhasználók **szinkronizálása a szervezeti** címtárból lapon válassza az Első **lépések lehetőséget.**

 4. Az első lépésben futtassa az IdFix eszközt a címtár-szinkronizálásra való felkészüléshez.

 5. A varázsló lépéseit követve töltse le az Azure AD-Csatlakozás, és ezzel szinkronizálja a tartomány által szabályozott felhasználókat a Microsoft 365.


További [információ: Címtár-szinkronizálás beállítása Microsoft 365](../enterprise/set-up-directory-synchronization.md) számára.

Az Azure AD Csatlakozás beállításainak konfigurálásakor azt javasoljuk, hogy engedélyezze a Jelszó-szinkronizálást, a Zökkenőmentes egyszeri bejelentkezést és a jelszóvisszaírási funkciót, amelyet az Microsoft 365 Vállalati verzió is támogat. 

> [!NOTE]
> Az Azure AD szolgáltatásban található jelölőnégyzeten túl további lépéseket is végre kell Csatlakozás. További információért lásd: [Hogyan: jelszóvisszaírás konfigurálása](/azure/active-directory/authentication/howto-sspr-writeback). 

Ha a tartományhoz csatlakozott Windows 10-eszközöket is szeretné kezelni, A tartományhoz csatlakozott [Windows 10-eszközök](manage-windows-devices.md) kezelése az Microsoft 365 Vállalati prémium verzió számára a hibrid Azure AD Join beállításához.
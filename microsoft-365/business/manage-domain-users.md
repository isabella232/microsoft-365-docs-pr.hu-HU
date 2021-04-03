---
title: Tartományfelhasználók szinkronizálása a Microsoft 365-be
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
ms.openlocfilehash: b477b8a1f35a790d6c49937c973c141ad9f90ad4
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578407"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a>Tartományfelhasználók szinkronizálása a Microsoft 365-be

## <a name="1-prepare-for-directory-synchronization"></a>1. Felkészülés a címtár-szinkronizálásra 

Mielőtt szinkronizálja a felhasználókat és a számítógépeket a helyi Active Directory-tartományból, tekintse át a Felkészülés a Címtár-szinkronizálásra a [Microsoft 365-bencímtár-szinkronizálásracímet.](../enterprise/prepare-for-directory-synchronization.md) Különösen:

   - Győződjön meg arról, hogy a címtárban nem léteznek ismétlődő attribútumok a **következő** attribútumok esetén: mail , **proxyAddresses** és **userPrincipalName.** Ezeknek az értékeknek egyedinek kell lennie, és az ismétlődéseket el kell távolítani.
   
   - Azt javasoljuk, hogy minden helyi felhasználói fiók **userPrincipalName** (UPN) attribútumát úgy konfigurálja, hogy megegyezzon a licencelt Microsoft 365-felhasználónak megfelelő elsődleges e-mail-címmel. Például: *mary.shelley@contoso.com.local* mary@contoso *helyett*
   
   - Ha az Active Directory-tartomány egy nem átirányítható utótaggal végződik , például *.local* vagy *.lan*, internetes átirányítható utótag (például *.com* vagy *.org)* helyett, módosítsa a helyi felhasználói fiókok UPN-utótagját a Nem átirányítható tartomány előkészítése a [címtár-szinkronizáláshoz](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md)leírt módon. 

Az **idFix futtatása** az alábbi negyedik lépésben (4) azt is meg kell győződni arról, hogy a helyszíni Active Directory készen áll-e a címtár-szinkronizálásra.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Az Azure AD Connect telepítése és konfigurálása

Ha szinkronizálni szeretné a felhasználókat, csoportokat és névjegyeket a helyi Active Directoryból az Azure Active Directoryba, telepítse az Azure Active Directory Connect alkalmazást, és állítsa be a címtár-szinkronizálást. 

 1. A Felügyeleti [központban válassza](https://go.microsoft.com/fwlink/p/?linkid=2024339)a bal oldali navigációs **sávon** a Beállítás lehetőséget.

 2. A **Bejelentkezés és biztonság csoportban** válassza a Megtekintés lehetőséget a Felhasználók szinkronizálása a szervezet **címtárában csoportban.** 

 3. A Felhasználók **szinkronizálása a szervezeti** címtárból lapon válassza az Első **lépések lehetőséget.**

 4. Az első lépésben futtassa az IdFix eszközt a címtár-szinkronizálásra való felkészüléshez.

 5. A varázsló lépéseit követve töltse le az Azure AD Connectet, és szinkronizálja vele a tartomány által szabályozott felhasználókat a Microsoft 365-be.


További [információ: Címtár-szinkronizálás beállítása a Microsoft 365-ben.](../enterprise/set-up-directory-synchronization.md)

Az Azure AD Connect beállításainak konfigurálásakor azt javasoljuk, hogy engedélyezze a  jelszó-szinkronizálást, a zökkenőmentes egyszeri bejelentkezést és a jelszóvisszaírási funkciót, amelyet a Microsoft 365 Vállalati verzió is támogat. 

> [!NOTE]
> Az Azure AD Connect jelölőnégyzete után további lépésekkel is visszaírhatja a jelszavakat. További információért lásd: [Hogyan: jelszóvisszaírás konfigurálása](/azure/active-directory/authentication/howto-sspr-writeback). 

Ha a tartományhoz csatlakozott Windows 10-es eszközöket is kezelni szeretné, tekintse át A tartományhoz csatlakozott [Windows 10-es](manage-windows-devices.md) eszközök microsoft 365 Vállalati prémium verzió által történő kezelése hibrid Azure AD-csatlakozás beállítását engedélyező cikkeket.
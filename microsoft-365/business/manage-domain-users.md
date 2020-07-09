---
title: Tartományi felhasználók szinkronizálása a Microsoft 365-tel
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
description: Szinkronizálja a tartományvezérelt felhasználókat a Microsoft 365 vállalati verzióval.
ms.openlocfilehash: af9cb7c9b2b639edc2375679a73ab41c4cf6de71
ms.sourcegitcommit: 5b769f74bcc76ac8d38aad815d1728824783cd9f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081910"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a>Tartományi felhasználók szinkronizálása a Microsoft 365-tel

## <a name="1-prepare-for-directory-synchronization"></a>1. Felkészülés a címtár-szinkronizálásra 

Mielőtt szinkronizálja a felhasználókat és a számítógépeket a helyi Active Directory tartományból, tekintse át [a Felkészülés a Microsoft 365-tel a címtár-szinkronizálásra](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization)című részt. Különösen:

   - Győződjön meg arról, hogy a következő attribútumokhoz nem találhatók ismétlődések a könyvtárban: **mail**, **proxyAddresses**és **userPrincipalName**. Ezeknek az értékeknek egyedieknek kell lenniük, és minden ismétlődést el kell távolítani.
   
   - Azt javasoljuk, hogy minden helyi felhasználói fiókhoz konfigurálja a **userPrincipalName** (UPN) attribútumot úgy, hogy az megfeleljen a licencelt Microsoft 365-felhasználónak megfelelő elsődleges e-mail címnek. Például: *mary.shelley@contoso.com* helyett *mary@contoso.local*
   
   - Ha az Active Directory tartomány nem irányítható utótaggal végződik, például *.local* vagy *.lan*, az internetes irányítható utótag (például *.com* vagy *.org)* helyett, állítsa be először a helyi felhasználói fiókok UPN-utónevét a [Címtár-szinkronizálásra](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization)nem irányítható tartomány előkészítése című részben leírtak szerint. 

A **Run IdFix** az alábbi negyedik (4) lépésben azt is győződjön meg arról, hogy a helyszíni Active Directory készen áll a dir sync.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Az Azure AD Connect telepítése és konfigurálása

Ha szinkronizálni szeretné a felhasználókat, csoportokat és névjegyeket a helyi Active Directoryból az Azure Active Directoryba, telepítse az Azure Active Directory Connectet, és állítsa be a címtár-szinkronizálást. 

 1. A felügyeleti központban válassza a <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **telepítő lehetőséget** a bal oldali navigációs eszközben.

 2. A **Bejelentkezés és biztonság csoportban**válassza a **Nézet** lehetőséget a **szervezeti címtár felhasználók szinkronizálása csoportban.**

 3. A **felhasználók szinkronizálása a szervezet címtárlapján** válassza az **Első lépések**lehetőséget.

 4. Az első lépésben futtassa az IdFix eszközt a címtár-szinkronizáláselőkészítéséhez.

 5. Kövesse a varázsló lépéseit az Azure AD Connect letöltéséhez, és használja azt a tartományáltal vezérelt felhasználók microsoft 365-tel való szinkronizálásához.


További információ A [Microsoft 365 címtár-szinkronizálásának beállítása.](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization)

Az Azure AD Connect beállításainak konfigurálásakor azt javasoljuk, hogy engedélyezze **a jelszó-szinkronizálást**, a zökkenőmentes egyszeri bejelentkezést és a **jelszó-visszaírási** funkciót, amelyet a Microsoft 365 vállalati verzió is támogat. **Seamless Single Sign-On**

> [!NOTE]
> Az Azure AD Connect jelölőnégyzetén túl további lépések is bevannak téve a jelszó-visszaíráshoz. További információ: [Útmutató: jelszó-visszaírás konfigurálása.](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback) 

Ha tartományhoz csatlakozó Windows 10-eszközöket is kezelni szeretne, olvassa el [a Microsoft 365 Business Premium által felügyelt, tartományhoz csatlakozó Windows 10-eszközök engedélyezése](manage-windows-devices.md) hibrid Azure AD-csatlakozás beállításához című témakört. 
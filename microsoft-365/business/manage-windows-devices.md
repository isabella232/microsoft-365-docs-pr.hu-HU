---
title: Tartományhoz csatlakozott Windows 10-es eszközök microsoft 365 vállalati verziós kezelésének engedélyezése
f1.keywords:
- NOCSH
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
- OKR_SMB_M365
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Megtudhatja, hogy miként engedélyezheti a Microsoft 365 számára a helyi Active Directoryhoz csatlakozott Windows 10-eszközök védelmét néhány lépésben.
ms.openlocfilehash: adc125c32fe5aa56be8c17c07f28316602a36594
ms.sourcegitcommit: 46644f9778bc70ab6d62783e0a1e60ba2eccc27f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/08/2020
ms.locfileid: "44165809"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-for-business"></a>Tartományhoz csatlakozott Windows 10-es eszközök microsoft 365 vállalati verziós kezelésének engedélyezése

Ha a szervezet a helyszíni Windows Server Active Directoryt használja, beállíthatja a Microsoft 365 vállalati verziót a Windows 10-es eszközök védelmére, miközben továbbra is hozzáférhet a helyi hitelesítést igénylő helyszíni erőforrásokhoz.
A védelem beállításához hibrid **Azure AD-hez csatlakozott eszközöket**valósíthat meg. Ezek az eszközök a helyszíni Active Directoryhoz és az Azure Active Directoryhoz is csatlakoznak.

Ez a videó bemutatja, hogyan állíthatja be ezt a leggyakoribb forgatókönyvhöz, amelyet a következő lépések is részleteznek.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a>1. Felkészülés a címtár-szinkronizálásra 

Mielőtt szinkronizálja a felhasználókat és a számítógépeket a helyi Active Directory tartományból, tekintse át [a Felkészülés az Office 365-tel való címtár-szinkronizálásra](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization)című részt. Különösen:

   - Győződjön meg arról, hogy a következő attribútumokhoz nem találhatók ismétlődések a könyvtárban: **mail**, **proxyAddresses**és **userPrincipalName**. Ezeknek az értékeknek egyedieknek kell lenniük, és minden ismétlődést el kell távolítani.
   
   - Azt javasoljuk, hogy minden helyi felhasználói fiókhoz konfigurálja a **userPrincipalName** (UPN) attribútumot úgy, hogy az megfeleljen a licencelt Microsoft 365-felhasználónak megfelelő elsődleges e-mail címnek. Például: *mary.shelley@contoso.com* helyett *mary@contoso.local*
   
   - Ha az Active Directory tartomány nem irányítható utótaggal végződik, például *.local* vagy *.lan*, az internetes irányítható utótag (például *.com* vagy *.org)* helyett, állítsa be először a helyi felhasználói fiókok UPN-utónevét a [Címtár-szinkronizálásra](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization)nem irányítható tartomány előkészítése című részben leírtak szerint. 

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Az Azure AD Connect telepítése és konfigurálása

Ha szinkronizálni szeretné a felhasználókat, csoportokat és névjegyeket a helyi Active Directoryból az Azure Active Directoryba, telepítse az Azure Active Directory Connectet, és állítsa be a címtár-szinkronizálást. További információ: [Címtár-szinkronizálás beállítása az Office 365-höz.](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization)

> [!NOTE]
> A lépések pontosan ugyanazok a Microsoft 365 vállalati verziók esetében. 

Az Azure AD Connect beállításainak konfigurálásakor azt javasoljuk, hogy engedélyezze **a jelszó-szinkronizálást**, a zökkenőmentes egyszeri bejelentkezést és a **jelszó-visszaírási** funkciót, amelyet a Microsoft 365 vállalati verzió is támogat. **Seamless Single Sign-On**

> [!NOTE]
> Az Azure AD Connect jelölőnégyzetén túl további lépések is bevannak téve a jelszó-visszaíráshoz. További információ: [Útmutató: jelszó-visszaírás konfigurálása.](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback) 

## <a name="3-configure-hybrid-azure-ad-join"></a>3. Hibrid Azure AD-illesztés konfigurálása

Mielőtt engedélyezne Windows 10-es eszközöket hibrid Azure AD-csatlakozásra, győződjön meg arról, hogy megfelel az alábbi előfeltételeknek:

   - Az Azure AD Connect legújabb verzióját futtatja.

   - Az Azure AD connect szinkronizálta a hibrid Azure AD-hez csatlakozni kívánt eszközök összes számítógép-objektumát. Ha a számítógép-objektumok adott szervezeti egységekhez (OU) tartoznak, győződjön meg arról, hogy ezek a szervezeti egységek szinkronizálásra vannak beállítva az Azure AD-csatlakozásban is.

Ha hibrid Azure AD-csatlakozásként szeretné regisztrálni a meglévő tartományhoz csatlakozó Windows 10-eszközöket, kövesse az [oktatóanyag lépéseit: Hibrid Azure Active Directory-csatlakozás konfigurálása felügyelt tartományokhoz.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) Ez a hibrid lehetővé teszi, hogy a meglévő helyszíni Active Directory csatlakozott a Windows 10 számítógépek, és azokat felhő kész.
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a>4. Automatikus regisztráció engedélyezése a Windows 10-hez

 Ha automatikusan szeretné regisztrálni a Windows 10-es eszközöket mobileszköz-kezeléshez az Intune-ban, olvassa el a [Windows 10-es eszközök automatikus regisztrálása a csoportházirenddel című témakört.](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy) A csoportházirendet helyi számítógép-szinten, illetve tömeges műveletek esetén a Csoportházirend kezelése konzol és az ADMX-sablonok segítségével hozhatja létre ezt a csoportházirend-beállítást a tartományvezérlőn.

## <a name="5-configure-seamless-single-sign-on"></a>5. Zökkenőmentes egyszeri bejelentkezés konfigurálása

  A zökkenőmentes egyszeri bejelentkezés automatikusan aláírja a felhasználókat a Microsoft 365 felhőalapú erőforrásaiba, amikor vállalati számítógépeket használnak. Egyszerűen telepítse az Azure Active Directory zökkenőmentes egyszeri bejelentkezési szolgáltatásában ismertetett két [csoportházirend-beállítás egyikét: gyorsindítás.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature) A **Csoportházirend** beállítás nem teszi lehetővé a felhasználók számára a beállítások módosítását, míg a **Csoportházirend-beállítás** beállítás beállítja az értékeket, de a felhasználó számára is konfigurálható marad.

## <a name="6-set-up-windows-hello-for-business"></a>6. A Windows Hello Vállalati verzió beállítása

 A Windows Hello for Business a helyi számítógépre való bejelentkezéshez a jelszavakat erős kétfaktoros hitelesítéssel (2FA) helyettesíti. Az egyik tényező egy aszimmetrikus kulcspár, a másik pedig egy PIN-kód vagy más helyi kézmozdulat, például ujjlenyomat vagy arcfelismerés, ha az eszköz támogatja azt. Azt javasoljuk, hogy ahol lehetséges, cserélje le a jelszavakat a 2FA-ra és a Windows Hello for Business-re.

A hibrid Windows Hello for Business konfigurálásához tekintse át a [hibridkulcs megbízhatósági kapcsolatát a Windows Hello üzleti előfeltételekhez](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs). Ezután kövesse a [Hibrid Windows Hello for Business kulcsmegbízhatósági beállítások konfigurálása című útmutató utasításait.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings) 

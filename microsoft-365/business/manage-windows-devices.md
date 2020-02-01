---
title: A tartományhoz csatlakoztatott Windows 10-es eszközök kezelésének engedélyezése a Microsoft 365 Vállalati verzió számára
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
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Megtudhatja, hogy miként engedélyezheti a Microsoft 365 számára a helyi Active Directoryhoz csatlakozott Windows 10-es eszközök védelmét.
ms.openlocfilehash: 170703c7367f9c0e9cb4c10edbd81cb214aa1d3e
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593801"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>A tartományhoz csatlakoztatott Windows 10-es eszközök kezelésének engedélyezése a Microsoft 365 Vállalati verzió számára

Ha szervezete a helyszínen használja a Windows Server Active Directoryt, beállíthatja a Microsoft 365 Business alkalmazást a Windows 10-es eszközök védelmére, miközben továbbra is hozzáférhet a helyi hitelesítést igénylő helyszíni erőforrásokhoz.
A védelem beállításához valósíthatja meg a **hibrid Azure AD-csatlakozású eszközöket.** Ezek az eszközök a helyszíni Active Directoryhoz és az Azure Active Directoryhoz is csatlakoznak.

Ez a videó ismerteti a lépéseket, hogyan kell beállítani ezt a leggyakoribb forgatókönyv, amely szintén részletesen a következő lépéseket.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a>1. Felkészülés a címtár-szinkronizálásra 

Mielőtt szinkronizálna felhasználóival és számítógépeivel a helyi Active Directory-tartományból, olvassa el a Felkészülés az [Office 365-tel való címtár-szinkronizálásra](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization)című dokumentumban. Különösen:

   - Győződjön meg arról, hogy nincsenek ismétlődések a könyvtárban a következő attribútumok: **mail**, **proxyAddresses**és **userPrincipalName**. Ezeknek az értékeknek egyedinek kell lenniük, és minden ismétlődést el kell távolítani.
   
   - Azt javasoljuk, hogy konfigurálja a **userPrincipalName** (UPN) attribútumot minden helyi felhasználói fiókhoz, hogy megfeleljen a licencelt Microsoft 365 felhasználónak megfelelő elsődleges e-mail címnek. Például: *mary.shelley@contoso.com,* nem *pedig mary@contoso.local*
   
   - Ha az Active Directory-tartomány nem irányítható utótaggal végződik, például *.local* vagy *.lan*, az internetes irányítható utótag ( például *.com* vagy *.org*) helyett állítsa be a helyi felhasználói fiókok UPN-utótagot először a Nem irányítható tartomány előkészítése a [címtár-szinkronizáláshoz](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization)című részben leírtak szerint. 

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Az Azure AD Connect telepítése és konfigurálása

A helyi Active Directoryból származó felhasználók, csoportok és névjegyek azure Active Directoryba való szinkronizálásához telepítse az Azure Active Directory-csatlakozást, és állítsa be a címtár-szinkronizálást. További információ [az Office 365 címtár-szinkronizálásának beállítása.](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)

> [!NOTE]
> A lépések pontosan ugyanazok a Microsoft 365 Business esetében. 

Az Azure AD Connect beállításainak konfigurálásakor azt javasoljuk, hogy engedélyezze a **jelszó-szinkronizálást,** a **zökkenőmentes egyszeri bejelentkezést**és a **jelszó-visszaírási** funkciót, amelyet a Microsoft 365 Business is támogat.

> [!NOTE]
> Az Azure AD Connect jelölőnégyzeten túl további lépéseket is ellehet- e lépni a jelszó-visszaírással kapcsolatban. További információt [az Útmutató: jelszó-visszaírás konfigurálása](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback)című témakörben talál. 

## <a name="3-configure-hybrid-azure-ad-join"></a>3. Hibrid Azure AD-csatlakozás konfigurálása

Mielőtt engedélyezne, hogy a Windows 10-es eszközök hibrid Azure AD-csatlakozással legyenek, győződjön meg arról, hogy megfelel az alábbi előfeltételeknek:

   - Az Azure AD Connect legújabb verzióját futtatja.

   - Az Azure AD connect szinkronizálta az összes olyan eszköz számítógép-objektumát, amelyhez hibrid Azure AD-csatlakozást szeretne. Ha a számítógép-objektumok bizonyos szervezeti egységekhez (OU) tartoznak, akkor győződjön meg arról, hogy ezek a szervezeti egységek szinkronizálásra vannak beállítva az Azure AD-csatlakozásban is.

Ha meglévő tartományhoz csatlakozó Windows 10-es eszközöket hibrid Azure AD-csatlakozással szeretne regisztrálni, kövesse az [Oktatóanyag: Hibrid Azure Active Directory-csatlakozás konfigurálása felügyelt tartományokhoz](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join)című útmutató lépéseit. Ez a hibrid lehetővé teszi a meglévő helyszíni Active Directory csatlakozott Windows 10 számítógépek és azokat felhő kész.
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a>4. Automatikus regisztráció engedélyezése a Windows 10-hez

 Ha a Windows 10-es eszközöket az Intune-ban szeretné automatikusan regisztrálni mobileszköz-felügyeletre, olvassa el [A Windows 10-es eszköz automatikus regisztrálása csoportházirenddel című témakört.](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy) A csoportházirendet helyi számítógép-szinten vagy tömeges műveletek esetén állíthatja be a Csoportházirend-kezelő konzol és az ADMX sablonok segítségével, hogy létrehozza ezt a csoportházirend-beállítást a tartományvezérlőn.

## <a name="5-configure-seamless-single-sign-on"></a>5. Zökkenőmentes egyszeri bejelentkezés konfigurálása

  A zökkenőmentes egyszeri bejelentkezés automatikusan bejelentkezik a felhasználókat a Microsoft 365 felhőbeli erőforrásaikba, amikor vállalati számítógépeket használnak. Egyszerűen telepítse az [Azure Active Directory zökkenőmentes egyszeri bejelentkezés: Rövid útmutató](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature)című szolgáltatásában ismertetett két csoportházirend-beállítás egyikét. A **Csoportházirend** beállítás nem teszi lehetővé a felhasználók számára a beállítások módosítását, míg a **Csoportházirend-beállítás** beállítás az értékeket állítja be, de a felhasználó által konfigurálható beállításokat is lehetővé teszi számukra.

## <a name="6-set-up-windows-hello-for-business"></a>6. A Windows Hello Vállalati verzió beállítása

 A Windows Hello for Business a jelszavakat erős kétfaktoros hitelesítéssel (2FA) helyettesíti a helyi számítógépre való bejelentkezéshez. Az egyik tényező egy aszimmetrikus kulcspár, a másik pedig egy PIN-kód vagy más helyi kézmozdulat, például ujjlenyomat vagy arcfelismerés, ha a készülék támogatja azt. Javasoljuk, hogy ahol lehetséges, cserélje le a jelszavakat a 2FA és a Windows Hello for Business rendszerre.

A Hibrid Windows Hello for Business konfigurálásához tekintse át a Hibrid kulcs megbízható Windows Hello for Business prerequisites című kezelési [kártyáját.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs) Ezután kövesse a [Hibrid Windows Hello for Business kulcsmegbízhatósági beállításainak konfigurálása](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings)című részt. 

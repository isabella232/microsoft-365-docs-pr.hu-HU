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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Útmutató a Microsoft 365 a helyi AD-hez csatlakozott Windows 10-eszközök védelmének engedélyezéséhez.
ms.openlocfilehash: 392c57a7350a901c1481be632e880cc9fcaa6140
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575978"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>A tartományhoz csatlakoztatott Windows 10-es eszközök kezelésének engedélyezése a Microsoft 365 Vállalati verzió számára

Ha a szervezet helyi Windows Server Active Directoryt használ, beállíthatja a Microsoft 365 Business rendszert, hogy védje a Windows 10 eszközeit, miközben továbbra is fenntartja az intézményi erőforrásokhoz való hozzáférést, amelyekhez szükség van lokális hitelesítésre.
Ennek beállításához használhat **hibrid Azure-ad egyesített eszközöket**. Ezek olyan eszközök, amelyek mind a helyi Active Directory címtárba, mind a Azure Active Directoryba csatlakoztak.

A következő videó részletesen ismerteti, hogyan kell beállítani ezt a leggyakoribb forgatókönyvre, amely az alábbi lépésekben is részletes.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a>1. Felkészülés a címtár-szinkronizálásra 

Mielőtt a felhasználókat és a számítógépeket a helyi Active Directory-tartományból szinkronizálja, tekintse át a [felkészülés a címtár-szinkronizáláshoz az Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). Különösen:

   - Győződjön meg arról, hogy a könyvtárban nem találhatók ismétlődések a következő attribútumok számára: **mail**, **ProxyAddresses**és **userPrincipalName**. Ezeknek az értékeknek egyedieknek kell lenniük, és az ismétlődéseket el kell távolítani.
   
   - Javasoljuk, hogy minden helyi felhasználói fiók **userPrincipalName** (UPN) attribútuma úgy legyen konfigurálva, hogy megfeleljen az elsődleges e-mail címnek, amely megfelel a licencelt Microsoft 365 felhasználónak. Például *Mary.Shelley@contoso.com* , nem pedig *Mary @ contoso. local*
   
   - Ha az Active Directory tartomány nem útválasztható (például *. local* vagy *. LAN*) végződést ér el egy Internet-irányítható utótag, pl *. com* vagy *. org*helyett, akkor a helyi felhasználói fiókok UPN-utótagját először az alábbiak szerint kell módosítani [Nem útválasztható tartomány előkészítése a címtár-szinkronizáláshoz](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization). 

## <a name="2-install-and-configure-azure-ad-connect"></a>2. telepítése és konfigurálása Azure AD Connect

A felhasználók, csoportok és kapcsolattartók helyi Active Directoryból a Azure Active Directoryba történő szinkronizálásához telepítse az Azure Active Directory csatlakoztatása szolgáltatást és állítsa be a címtár-szinkronizálást. További tudnivalókat az [Office 365 címtár-szinkronizálás beállítása](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) című témakörben talál.

> [!NOTE]
> A lép van pontosan ugyanaz részére Mikroszkóp 365 teendő. 

A Azure AD Connect szolgáltatás beállításainak konfigurálásakor javasoljuk a **Jelszó-szinkronizálás** és a **zökkenőmentes egyszeri bejelentkezés**engedélyezését, valamint a **jelszó** írásának funkcióját, amelyet a Microsoft 365 Business is támogat.

> [!NOTE]
> Van néhány további lépés a jelszóírésre az Azure AD Connect-ben lévő jelölőnégyzeten kívül. További információ [: Hogyan-hoz configure jelszó writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

## <a name="3-configure-hybrid-azure-ad-join"></a>3. configure hibrid Azure AD illesztés

Mielőtt bekapcsolódott a Windows 10 eszköz a Hybrid Azure Active Directory-hoz, győződjön meg arról, hogy megfelel az alábbi feltételeknek:

   - A legújabb verziójú Azure AD Connect-et futtatja.

   - Azúrkék AD összeköt birtokol szinkronizál minden a számítógép tárgy-ból berendezés ön akar-hoz lenni hibrid Azure AD összekapcsolt. Ha a számítógép-objektumok meghatározott szervezeti egységekhez tartoznak, akkor győződjön meg arról, hogy ezek a szervezeti egységek szinkronizálásra vannak beállítva a Azure AD Connect-ben is.

Ha már meglévő, tartományhoz csatlakoztatott Windows 10-eszközt szeretne regisztrálni a Hybrid Azure AD csatlakozásakor, kövesse az [oktatóprogram: a hibrid Azure Active Directory-illesztés konfigurálása felügyelt tartományokhoz](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join)című témakört. Ez hibrid-lehetővé teszi, hogy a meglévő helyszíni Active Directory-hoz csatlakozott a Windows 10 számítógépet, és tegyék felhő kész.
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a>4. engedélyezze az automatikus igénylést a Windows 10

 A Windows 10 eszköznek az Intune mobil eszközkezeléséhez történő automatikus igényléséhez olvassa el a [Windows 10 eszköz regisztrálása a csoportházirenddel automatikusan](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy)című témakört. A csoportházirendet helyi számítógép szinten, illetve tömeges műveletek esetén a csoportházirendet a Csoportházirend kezelése konzollal és az ADMX-sablonok használatával is létrehozhatja a tartományvezérlőn.

## <a name="5-configure-seamless-single-sign-on"></a>5. a zökkenőmentes egyszeri bejelentkezés beállítása

  A problémamentes egyszeri bejelentkezés a felhasználókat automatikusan aláírja a Microsoft 365 felhőalapú erőforrásaira, amikor vállalati számítógépeket használnak. Egyszerűen telepítse az [Azure Active Directory problémamentes egyszeri bejelentkezés: Gyors indítás](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature)című témakörben ismertetett két csoportházirend-beállítás egyikét. A **csoportházirend-beállítás nem** teszi lehetővé a felhasználók számára a beállításaik módosítását, **míg a csoportházirend** -beállítás az értékeket állítja be, de a felhasználó által konfigurálható értéket is hagy.

## <a name="6-set-up-windows-hello-for-business"></a>6. felállít Windows Szia részére teendő

 Windows Szia részére teendő helyettesít jelszó-val erős kettő-tényező hitelesítés (2FA) részére jel-ba egy helyi számítógép. Az egyik tényező egy aszimmetrikus kulcspár, a másik pedig egy PIN-kód vagy más helyi mozdulat, például ujjlenyomat vagy Arcfelismerés, ha az eszköz támogatja. Javasoljuk, hogy cserélje ki a jelszavakat a 2FA és a Windows Hello for Business, ahol lehetséges.

-Hoz configure hibrid Windows Szia részére teendő, áttekintés a [hibrid kulcs hisz Windows Szia részére teendő előfeltétel](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs). Akkor követ a oktatás-ban [configure hibrid Windows Szia részére teendő kulcs hisz elintézés](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings). 

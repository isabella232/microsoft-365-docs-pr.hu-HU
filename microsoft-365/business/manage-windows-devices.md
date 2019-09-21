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
ms.openlocfilehash: 9bfd540c0ff113762485f62707f1975ff53accc4
ms.sourcegitcommit: 1162d676b036449ea4220de8a6642165190e3398
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068105"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>A tartományhoz csatlakoztatott Windows 10-es eszközök kezelésének engedélyezése a Microsoft 365 Vállalati verzió számára

Ha a szervezet helyi Windows Server Active Directoryt használ, beállíthatja a Microsoft 365 Business rendszert, hogy védje a Windows 10 eszközeit, miközben továbbra is fenntartja az intézményi erőforrásokhoz való hozzáférést, amelyekhez szükség van lokális hitelesítésre. Ezt úgy állíthatja be, hogy először a Azure Active Directoryval szinkronizálja az Active Directory címtárat, majd regisztrálja a Windows 10 eszközöket az azúrkék HIRDETÉSRE, és a Microsoft 365 Business mobileszköz-kezelést végez.
A következő videó részletesen ismerteti, hogy hogyan lehet ezt beállítani a leggyakoribb forgatókönyvhöz.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a>A Microsoft 365 Business által kezelhető, tartományhoz csatlakoztatott eszközök beállítása

Ahhoz, hogy a szervezet tartományhoz csatlakoztatott eszközeit úgy állítsa be, hogy a helyszíni Active Directory címtáron kívül az Azure Active Directory által nyújtott szolgáltatások előnyeit is élvezheti, a **hibrid Azure beépített eszközöket**is implementálja. Ezek olyan eszközök, amelyek mind a helyi Active Directory címtárba, mind a Azure Active Directoryba csatlakoztak. A Hybrid Azure egyesített eszközök a Microsoft 365 Business által védhetők és kezelhetők. 
  
Hajtsa végre az alábbi lépéseket a Microsoft 365 Business által a Hybrid Azure AD által egyesített és kezelt Windows 10-eszközök elérhetővé tétele érdekében.
  
1. **Felkészülés a címtár-szinkronizálásra**: mielőtt a felhasználókat és a számítógépeket a helyi Active Directory-tartományból szinkronizálja, tekintse át a [felkészülés a címtár-szinkronizáláshoz az Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). Különösen:

   - Győződjön meg arról, hogy a könyvtárban nem találhatók ismétlődések a következő attribútumok számára: **mail**, **ProxyAddresses**és **userPrincipalName**. Ezeknek az értékeknek egyedieknek kell lenniük, és az ismétlődéseket el kell távolítani.
   
   - Azt javasoljuk, hogy minden helyi felhasználói fiók **userPrincipalName** (UPN) attribútuma úgy legyen beállítva, hogy megfeleljen az elsődleges e-mail címnek, amely megfelel a licencelt Microsoft 365 felhasználónak. Például **Mary.Shelley@contoso.com** , nem pedig **Mary @ contoso. local**
   
   - Ha az Active Directory tartomány nem útválasztható (például **. local** vagy **. LAN**) végződést ér el egy Internet-irányítható utótag, pl **. com** vagy **. org**helyett, akkor a helyi felhasználói fiókok UPN-utótagját először az alábbiak szerint kell módosítani [Nem útválasztható tartomány előkészítése a címtár-szinkronizáláshoz](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization). 

2. **Telepítsük és állítsuk be az Azure ad Connect**: a felhasználók, csoportok és névjegyek szinkronizálása a helyi Active Directory-címtárból a Azure Active Directory címtárszolgáltatásból, futtassa a címtár-szinkronizálás varázslót az Azure Active Directory Connect szolgáltatásból. További tudnivalókat az [Office 365 címtár-szinkronizálás beállítása](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) című témakörben talál.
    
    > [!NOTE]
    > A lép van pontosan ugyanaz részére Mikroszkóp 365 teendő. 
    
A Azure AD Connect szolgáltatás beállításainak konfigurálásakor javasoljuk a **Jelszó-szinkronizálás** és a **zökkenőmentes egyszeri bejelentkezés**engedélyezését, valamint a **jelszó** írásának funkcióját, amelyet a Microsoft 365 Business is támogat.

> [!NOTE]
> Van néhány további lépés a jelszóírésre az Azure AD Connect-ben lévő jelölőnégyzeten kívül. Folyamodik [Hogyan--hoz configure jelszó writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 
     
3. **Állítsa be a Hybrid Azure ad illesztést**: mielőtt csatlakoznia kellene a Windows 10 eszköznek a Hybrid Azure ad-hez, győződjön meg arról, hogy megfelel az alábbi feltételeknek:

   - A legújabb verziójú Azure AD Connect-et futtatja.

   - Azúrkék AD összeköt birtokol szinkronizál minden a számítógép tárgy-ból berendezés ön akar-hoz lenni hibrid Azure AD összekapcsolt. Ha a számítógép-objektumok meghatározott szervezeti egységekhez tartoznak, akkor győződjön meg arról, hogy ezek a szervezeti egységek szinkronizálásra vannak beállítva a Azure AD Connect-ben is.

Ha már meglévő, tartományhoz csatlakoztatott Windows 10-eszközt szeretne regisztrálni a Hybrid Azure AD csatlakozásakor, kövesse az [oktatóprogram: a hibrid Azure Active Directory-illesztés konfigurálása felügyelt tartományokhoz](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join)című témakört. Ez hibrid-lehetővé teszi, hogy a meglévő helyszíni Active Directory-hoz csatlakozott a Windows 10 számítógépet, és tegyék felhő kész.
    
4. **A Windows 10 automatikus tanúsítványigénylésének engedélyezése**: Ha az Intune szolgáltatással automatikusan szeretné igényelni a Windows 10 eszközt a mobil eszközkezeléshez, olvassa el [a Windows 10 eszköz regisztrálása](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy)a csoportházirend segítségével című témakört. A csoportházirendet helyi számítógép szinten, illetve tömeges műveletek esetén a csoportházirendet a Csoportházirend kezelése konzollal és az ADMX-sablonok segítségével is létrehozhatja a tartományvezérlőn.

5. **A zökkenőmentes egyszeri bejelentkezés beállítása**: a zökkenőmentes egyszeri bejelentkezés a felhasználókat automatikusan aláírja a Microsoft 365 felhőalapú erőforrásaira, amikor vállalati számítógépeket használnak. Egyszerűen telepítse az [Azure Active Directory problémamentes egyszeri bejelentkezés: Gyors indítás](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature)című témakörben ismertetett két csoportházirend-beállítás egyikét. A **csoportházirend-beállítás nem** teszi lehetővé a felhasználók számára a beállításaik módosítását, **míg a csoportházirend** -beállítás az értékeket állítja be, de a felhasználó által konfigurálható értéket is hagy.

6. **Felállít Windows Szia részére teendő**: Windows Szia részére teendő helyettesít jelszó-val erős kettő-tényező hitelesítés (2fa) részére jel-ba egy helyi számítógép. Az egyik tényező egy aszimmetrikus kulcspár, a másik pedig egy PIN-kód vagy más helyi mozdulat, például ujjlenyomat vagy Arcfelismerés, ha az eszköz támogatja. Azt javasoljuk, hogy cserélje ki a jelszavakat a 2FA és a Windows Hello for Business, ahol lehetséges.

-Hoz configure hibrid Windows Szia részére teendő, áttekintés a [hibrid kulcs hisz Windows Szia részére teendő előfeltétel](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs). Akkor követ a oktatás-hoz [configure hibrid Windows Szia részére teendő kulcs hisz elintézés](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings). 

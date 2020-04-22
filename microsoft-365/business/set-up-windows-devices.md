---
title: Windows-eszközök beállítása Microsoft 365 Business Premium-felhasználók számára
f1.keywords:
- CSH
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
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: Ismerje meg, hogyan állíthatja be a Windows 10 Pro rendszert futtató Windows-eszközöket a Microsoft 365 Business Premium felhasználók számára, lehetővé téve a központi felügyeleti és biztonsági vezérlőket.
ms.openlocfilehash: efe81a5547496f502232e1db2f3f092165475641
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/21/2020
ms.locfileid: "43635452"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a>Windows-eszközök beállítása Microsoft 365 Business Premium-felhasználók számára

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-premium-users"></a>A Windows-eszközök Microsoft 365 Business Premium-felhasználók számára való beállításának előfeltételei

Mielőtt beállíthatna Windows-eszközöket a Microsoft 365 Business Premium felhasználók számára, győződjön meg arról, hogy az összes Windows-eszközön Windows 10 Pro, 1703-as verzió (Alkotói frissítés) fut. A Windows 10 Pro a Windows 10 Business telepítésének előfeltétele, amely olyan felhőszolgáltatások és eszközkezelési képességek készlete, amelyek kiegészítik a Windows 10 Pro rendszert, és lehetővé teszik a Microsoft 365 Business Premium központosított felügyeletét és biztonsági ellenőrzését.
  
Ha Windows 7 Pro, Windows 8 Pro vagy Windows 8.1 Pro rendszert futtató Windows-eszközökkel rendelkezik, a Microsoft 365 Business Premium előfizetése feljogosítja Önt a Windows 10 frissítésére.
  
Ha többet szeretne megtudni arról, hogy hogyan frissítheti Windows-eszközeit a Windows 10 Pro alkotói frissítésére, kövesse a következő témakörben szereplő lépéseket: [Windows-eszközök frissítése a Windows Pro alkotói frissítésére](upgrade-to-windows-pro-creators-update.md).
  
Lásd: [Ellenőrizze, hogy az eszköz csatlakozik-e az Azure AD-hez,](#verify-the-device-is-connected-to-azure-ad) hogy ellenőrizze, hogy rendelkezik-e a frissítéssel, vagy győződjön meg arról, hogy a frissítés működött.

Tekintse n fel a Windows Microsoft 365-höz való csatlakoztatásáról szóló rövid videót.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

Ha hasznosnak találta ezt a videót, tekintse meg a [teljes tanfolyamok kisvállalatoknak és Microsoft 365-újoncoknak](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) című témakört.
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>Windows 10-es eszközök csatlakoztatása a szervezet Azure AD szolgáltatásához

Ha a szervezet összes Windows-eszköze frissítve lett a Windows 10 Pro Alkotók frissítésére, vagy már fut a Windows 10 Pro Creators Update, csatlakozhat ezekhez az eszközökhöz a szervezet Azure Active Directoryjához. Az eszközök csatlakoztatása után automatikusan frissülnek a Windows 10 Business szolgáltatásra, amely a Microsoft 365 Business Premium-előfizetés része.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>Vadonatúj vagy újonnan frissített Windows 10 Pro-eszköz esetén

A Windows 10 Pro alkotói frissítését futtató vadonatúj eszköz, illetve egy olyan eszköz esetén, amely frissítve lett ugyan a Windows 10 Pro alkotói frissítésére, de még nem lett elvégezve rajta a Windows 10-es eszköz beállítása, kövesse az alábbi lépéseket.
  
1. Kezdje meg a Windows 10-es eszköz beállítását, amíg a **Hogyan szeretné beállítani?** lapra nem jut. 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. Itt válassza **a Beállítás egy szervezethez** lehetőséget, majd adja meg a microsoft 365 Vállalati prémium verzióhoz megadott felhasználónevét és jelszavát. 
    
3. Fejezze be a Windows 10-es eszköz beállítását.
    
   Ha végzett, a felhasználó csatlakoztatva lesz a szervezet Azure AD szolgáltatásához. Ha meg szeretne győződni arról, hogy sikerült-e a csatlakoztatás, olvassa el az [Annak ellenőrzése, hogy az eszköz csatlakoztatva van-e az Azure AD szolgáltatáshoz](#verify-the-device-is-connected-to-azure-ad) című szakaszt. 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a>Már beállított és a Windows 10 Prót futtató eszköz esetén

 **Felhasználók csatlakoztatása az Azure AD-hez:**
  
1. A felhasználó Windows rendszerű PC-jén, amelyen a Windows 10 Pro 1703-as verziója (alkotói frissítés) fut (lásd [előfeltételek](pre-requisites-for-data-protection.md)), kattintson a Windows emblémára, majd a Beállítások ikonra.
  
   ![In the Start menu, click Windows Settings icon](../media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. A **Beállítások** lapon válassza a **Fiókok** lehetőséget.
  
   ![In Windows Settings, go to Accounts](../media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. **Az Ön adatai** lapon kattintson a **Hozzáférés munkahelyi vagy iskolai rendszerhez** \> **Csatlakozás** elemre.
  
   ![Choose Connect under Access work or school](../media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. A **Munkahelyi vagy iskolai fiók beállítása** párbeszédpanel **Más műveletek** csoportjában válassza **Az eszköz csatlakoztatása az Azure Active Directoryhoz** lehetőséget.
  
   ![Click Join this device to Azure Active Directory](../media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. On the **Let's get you signed in** page, enter your work or school account \> **Next**.
  
   On the **Enter password** page, enter your password \> **Sign in**.
  
   ![Enter your work or school email on the Let's get you signed in page](../media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. A **Győződjön meg arról, hogy ez a szervezet** lap, ellenőrizze, hogy az adatok helyesek- e, majd kattintson a Csatlakozás **gombra.**
  
   A **Minden készen áll** lapon kattintson a **Kész** elemre.
  
   ![On the Make sure this is your organization screen, click Join](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
Szinkronizálja újból a OneDrive Vállalati verzióba esetleg feltöltött fájlokat. Ha külső gyártótól származó eszközt használt a profilok és fájlok áttelepítéséhez, szinkronizálja azokat az új profillal is.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>Annak ellenőrzése, hogy az eszköz csatlakoztatva van-e az Azure AD szolgáltatáshoz

A szinkronizálási állapot ellenőrzéséhez a **Hozzáférés munkahelyi vagy iskolai rendszerhez** lap **Beállítások** csoportjában kattintson a **Csatlakoztatva** _ \<organization name\> _ területre az **Információ** és a **Leválasztás** gomb megjelenítéséhez. Kattintson az **Információ** gombra a szinkronizálás állapotának megjelenítéséhez. 
  
A Szinkronizálás állapota lapon a Szinkronizálás elemre kattintva beszerezheti a legújabb mobileszköz-kezelési házirendeket a PC-re.
  
A Microsoft 365 Business Premium-fiók használatának megkezdéséhez lépjen a Windows **Start** gombjára, kattintson a jobb gombbal az aktuális fiók képére, majd **a Fiók váltása parancsra.** Jelentkezzen be a szervezeti e-mail-címével és jelszavával.
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-device-is-upgraded-to-windows-10-business"></a>Annak ellenőrzése, hogy az eszköz frissítve lett-e a Windows 10 Business verzióra

Ellenőrizze, hogy az Azure AD-hez csatlakozott Windows 10-es eszközei a Microsoft 365 Business Premium-előfizetés részeként windows 10 Business rendszerre frissítették-e.
  
1. Válassza a **Beállítások** \> **Rendszer** \> **Névjegy** lehetőséget.
    
2. Győződjön meg arról, hogy a **Kiadás** feliratnál a **Windows 10 Business** terméknév szerepel.
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>Következő lépések

A mobileszközök beállításához olvassa el A [mobileszközök beállítása Microsoft 365 Business Premium-felhasználók számára](set-up-mobile-devices.md), Az eszközvédelmi vagy alkalmazásvédelmi szabályzatok beállításához a [Microsoft 365 vállalati verzió kezelése.](manage.md)
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a>A Microsoft 365 Business Premium beállításával és használatával kapcsolatos további információk

[Microsoft 365 üzleti oktatóvideók](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)

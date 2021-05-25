---
title: Az eszköz Windows beállítása a Microsoft 365 Vállalati prémium verzió számára
f1.keywords:
- CSH
ms.author: sharik
author: skjerland
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
- AdminSurgePortfolio
- okr_smb
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: Állítsa be Windows központi felügyelet és Windows 10 Pro felügyeleti Microsoft 365 Vállalati prémium verzió felügyeleti és biztonsági vezérlők engedélyezésével.
ms.openlocfilehash: 7a9c75f6ec14605225d40c103c18e62937e773bf
ms.sourcegitcommit: 17f0aada83627d9defa0acf4db03a2d58e46842f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/24/2021
ms.locfileid: "52635874"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a>Az eszköz Windows beállítása a Microsoft 365 Vállalati prémium verzió számára

## <a name="before-you-begin"></a>Az első lépések

Mielőtt Windows eszközét Microsoft 365 Vállalati prémium verzió, győződjön meg arról, hogy az összes Windows-eszközön az 1703-as verzió (alkotói frissítés) Windows 10 Pro fut. Windows 10 Pro a Windows 10 Business üzembe helyezésének előfeltétele, amely a Windows 10 Pro-et kiegészítő felhőalapú szolgáltatások és eszközkezelési képességek készlete, amely lehetővé teszi az Microsoft 365 Vállalati prémium verzió központi felügyeletét és Microsoft 365 Vállalati prémium verzió.
  
Ha 7 Pro, Windows 8 Pro vagy Windows 8.1 Pro-t futtató Windows Windows-es eszközével rendelkezik, az Microsoft 365 Vállalati prémium verzió-előfizetés feljogosítja a Windows 10 frissítésére.
  
Ha többet szeretne megtudni arról, hogy hogyan frissítheti Windows-eszközeit a Windows 10 Pro alkotói frissítésére, kövesse a következő témakörben szereplő lépéseket: [Windows-eszközök frissítése a Windows Pro alkotói frissítésére](upgrade-to-windows-pro-creators-update.md).
  
Az [Annak ellenőrzése, hogy az eszköz](#verify-the-device-is-connected-to-azure-ad) csatlakoztatva van-e az Azure AD szolgáltatáshoz? vagy a frissítés megfelelő voltának ellenőrzéséhez lásd: Az eszköz csatlakoztatva van az Azure AD szolgáltatáshoz.

## <a name="watch-connect-your-pc-to-microsoft-365-business"></a>Watch: Csatlakozás pc to Microsoft 365 Vállalati verzió

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

Ha hasznosnak találta ezt a videót, tekintse meg a [teljes tanfolyamok kisvállalatoknak és Microsoft 365-újoncoknak](../business-video/index.yml) című cikket.
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>Windows 10-es eszközök csatlakoztatása a szervezet Azure AD szolgáltatásához

Ha a Windows összes eszközét frissítette az Windows 10 Pro alkotói frissítésre, vagy már futtatja az Windows 10 Pro alkotói frissítést, csatlakozhat ezekhez az eszközökhez a szervezet Azure Active Directory. Miután csatlakozott az eszközökhez, a rendszer automatikusan frissíti őket a Windows 10 Business verzióra, amely az Ön Microsoft 365 Vállalati prémium verzió része.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>Vadonatúj vagy újonnan frissített Windows 10 Pro-eszköz esetén

A Windows 10 Pro alkotói frissítését futtató vadonatúj eszköz, illetve egy olyan eszköz esetén, amely frissítve lett ugyan a Windows 10 Pro alkotói frissítésére, de még nem lett elvégezve rajta a Windows 10-es eszköz beállítása, kövesse az alábbi lépéseket.
  
1. Kezdje meg a Windows 10-es eszköz beállítását, amíg a **Hogyan szeretné beállítani?** lapra nem jut. 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. Itt válassza a **Beállítás szervezet számára lehetőséget,** majd adja meg a szervezethez tartozó felhasználónevét és Microsoft 365 Vállalati prémium verzió. 
    
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
  
6. Az **Ez az Ön szervezete?** lapon ellenőrizze, hogy helyesek-e az adatok, és válassza a Csatlakozás **gombot.**
  
   A **Minden beállítás meg van állítva!** lap, **ékes** Kész .
  
   ![A Legyen ez az Ön szervezete képernyőn válassza a Csatlakozás gombot.](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
Szinkronizálja újból a OneDrive Vállalati verzióba esetleg feltöltött fájlokat. Ha egy külső eszközt használt a profil és a fájlok áttelepítéséhez, azokat is szinkronizálja az új profilba.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>Annak ellenőrzése, hogy az eszköz csatlakoztatva van-e az Azure AD szolgáltatáshoz

A szinkronizálási állapot ellenőrzéséhez az Access munkahelyi vagy iskolai Gépház **területén** válassza a Csatlakoztatva **_** _ terület lehetőséget az Információ és a Kapcsolat bontása gomb  \<organization name\> **eléréséhez.**  Az **Információ lehetőséget** választva lekérte a szinkronizálás állapotát. 
  
A Szinkronizálás **állapota** lapon  a Szinkronizálás lehetőséget választva szerezze be a legújabb mobileszköz-kezelési házirendeket a pc-re.
  
A fiók használatának Microsoft 365 Vállalati prémium verzió kattintson a Windows **Start** gombra, kattintson a jobb gombbal az aktuális fiókképre, és válassza a **Fiókváltás gombra.** Jelentkezzen be a szervezeti e-mail-címével és jelszavával.
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-pc-is-upgraded-to-windows-10-business"></a>Ellenőrizze, hogy a számítógép frissítve van-e Windows 10 Business

Ellenőrizze, hogy az Azure AD-hez Windows 10 eszközén a Windows 10 Business előfizetése részeként Microsoft 365 Vállalati prémium verzió-e.
  
1. Válassza a **Beállítások** \> **Rendszer** \> **Névjegy** lehetőséget.
    
2. Győződjön meg arról, hogy a **Kiadás** feliratnál a **Windows 10 Business** terméknév szerepel.
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>Következő lépések

A mobileszközök beállításához lásd: Mobileszközök beállítása Microsoft 365 Vállalati prémium verzió [felhasználóknak](set-up-mobile-devices.md), eszközvédelmi és alkalmazásvédelmi házirendek beállításához lásd: Vállalati Microsoft 365 [kezelése.](manage.md)
  
## <a name="related-content"></a>Kapcsolódó tartalom

[Microsoft 365 vállalati verziós oktatóvideók](../business-video/index.yml) (hivatkozáslap)

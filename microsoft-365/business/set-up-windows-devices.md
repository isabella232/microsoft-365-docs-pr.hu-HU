---
title: Windows rendszerű eszközök beállítása a Microsoft 365 Business felhasználóinak
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: 'Megtudhatja, hogyan állíthatja be a Windows-eszközök Windows 10 Pro futó Microsoft 365 üzleti felhasználók számára. '
ms.openlocfilehash: 482199b175c568bfae420619aa02024303894789
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982855"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-users"></a>Windows rendszerű eszközök beállítása a Microsoft 365 Business felhasználóinak

## <a name="prerequisites"></a>Előfeltételek

Mielőtt beállítaná a Windows-eszközöket a Microsoft 365 Business felhasználóinál, győződjön meg arról, hogy az összes Windows-eszközön a Windows 10 Pro 1703-as verziója (alkotói frissítés) fut. A Windows 10 Pro megléte előfeltétele a Windows 10 Business üzembe helyezésének, amely a Windows 10 Prót kiegészítő felhőszolgáltatásokat és eszközkezelési lehetőségeket tartalmaz, és lehetővé teszi a Microsoft 365 Business központi kezelését és biztonsági szabályozását.
  
Ha Ön Windows 7 Pro, Windows 8 Pro vagy Windows 8.1 Pro rendszerű Windows-eszközökkel rendelkezik, akkor Microsoft 365 Business-előfizetése feljogosítja a Windows 10-re való frissítésre.
  
Ha többet szeretne megtudni arról, hogy hogyan frissítheti Windows-eszközeit a Windows 10 Pro alkotói frissítésére, kövesse a következő témakörben szereplő lépéseket: [Windows-eszközök frissítése a Windows Pro alkotói frissítésére](upgrade-to-windows-pro-creators-update.md).
  
Az [Annak ellenőrzése, hogy az eszköz frissítve lett-e a Windows 10 Business verzióra](set-up-windows-devices.md#bkmk_verifywin10) című szakasz segítségével ellenőrizheti, hogy rendelkezik-e a frissítéssel, vagy meggyőződhet a frissítés sikerességéről. 
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>Windows 10-es eszközök csatlakoztatása a szervezet Azure AD szolgáltatásához

Ha már a szervezet összes Windows-eszköze frissítve lett a Windows 10 Pro alkotói frissítésére, vagy már eleve a Windows 10 Pro alkotói frissítését futtatja, csatlakoztathatja az eszközöket a szervezet Azure Active Directory szolgáltatásához. A csatlakoztatott eszközök automatikusan a Windows 10 Business verzióra frissülnek, amely része a Microsoft 365 Business-előfizetésnek.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>Vadonatúj vagy újonnan frissített Windows 10 Pro-eszköz esetén

A Windows 10 Pro alkotói frissítését futtató vadonatúj eszköz, illetve egy olyan eszköz esetén, amely frissítve lett ugyan a Windows 10 Pro alkotói frissítésére, de még nem lett elvégezve rajta a Windows 10-es eszköz beállítása, kövesse az alábbi lépéseket.
  
1. Kezdje meg a Windows 10-es eszköz beállítását, amíg a **Hogyan szeretné beállítani?** lapra nem jut. 
    
    ![On the How would you like to set up page, choose Set up for an organization](media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. Itt válassza a **Beállítás szervezeti használatra** lehetőséget, és adja meg a Microsoft 365 Businesshez használt felhasználónevét és jelszavát. 
    
3. Fejezze be a Windows 10-es eszköz beállítását.
    
   Ha végzett, a felhasználó csatlakoztatva lesz a szervezet Azure AD szolgáltatásához. Ha meg szeretne győződni arról, hogy sikerült-e a csatlakoztatás, olvassa el az [Annak ellenőrzése, hogy az eszköz csatlakoztatva van-e az Azure AD szolgáltatáshoz](set-up-windows-devices.md#bkmk_verifyaad) című szakaszt. 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a>Már beállított és a Windows 10 Prót futtató eszköz esetén

 **Felhasználók csatlakoztatása az Azure AD-hez:**
  
1. A felhasználó Windows rendszerű PC-jén, amelyen a Windows 10 Pro 1703-as verziója (alkotói frissítés) fut (lásd [előfeltételek](pre-requisites-for-data-protection.md)), kattintson a Windows emblémára, majd a Beállítások ikonra.
  
   ![In the Start menu, click Windows Settings icon](media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. A **Beállítások** lapon válassza a **Fiókok** lehetőséget.
  
   ![In Windows Settings, go to Accounts](media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. **Az Ön adatai** lapon kattintson a **Hozzáférés munkahelyi vagy iskolai rendszerhez** \> **Csatlakozás** elemre.
  
   ![Choose Connect under Access work or school](media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. A **Munkahelyi vagy iskolai fiók beállítása** párbeszédpanel **Más műveletek** csoportjában válassza **Az eszköz csatlakoztatása az Azure Active Directoryhoz** lehetőséget.
  
   ![Click Join this device to Azure Active Directory](media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. Az **indulás Ön bejelentkezett a** lapon adja meg a műhely vagy iskola fiók \> **Tovább**.
  
   A **jelszó megadni** lapon írja be a jelszót \> **Jelentkezzen be**.
  
   ![Enter your work or school email on the Let's get you signed in page](media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. A a ** győződjön meg arról, hogy ez a szervezet ** lap, győződjön meg arról, hogy az adatok helyesek, és kattintsunk a **Csatlakozás**gombra.
  
   A **Minden készen áll** lapon kattintson a **Kész** elemre.
  
   ![On the Make sure this is your organization screen, click Join](media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
Szinkronizálja újból a OneDrive Vállalati verzióba esetleg feltöltött fájlokat. Ha egy külső eszközt vett igénybe a profil és a fájlok áttelepítéséhez, ezeket is szinkronizálja az új profilba.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>Annak ellenőrzése, hogy az eszköz csatlakoztatva van-e az Azure AD szolgáltatáshoz

A szinkronizálási állapot ellenőrzéséhez a **Hozzáférés munkahelyi vagy iskolai rendszerhez** lap **Beállítások** csoportjában kattintson a **Csatlakoztatva** _ \<organization name\> _ területre az **Információ** és a **Leválasztás** gomb megjelenítéséhez. Kattintson az **Információ** gombra a szinkronizálás állapotának megjelenítéséhez. 
  
A Szinkronizálás állapota lapon a Szinkronizálás elemre kattintva beszerezheti a legújabb mobileszköz-kezelési házirendeket a PC-re.
  
A Microsoft 365 Business-fiók használatának megkezdéséhez kattintson a Windows **Start** gombjára, kattintson a jobb gombbal az aktuális fiókjának a képére, és válassza a **Fiókváltás** parancsot. Jelentkezzen be a szervezeti e-mail-címével és jelszavával.
  
![Click Info button to view synchronization status](media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-device-is-upgraded-to-windows-10-business"></a>Annak ellenőrzése, hogy az eszköz frissítve lett-e a Windows 10 Business verzióra

Ellenőrizheti, hogy megtörtént-e az Azure AD szolgáltatáshoz csatlakoztatott Windows 10-es eszközök frissítése Windows 10 Business verzióra, a Microsoft 365 Business-előfizetése részeként.
  
1. Válassza a **Beállítások** \> **Rendszer** \> **Névjegy** lehetőséget.
    
2. Győződjön meg arról, hogy a **Kiadás** feliratnál a **Windows 10 Business** terméknév szerepel.
    
    ![Verify that Windows edition is Windows 10 Business.](media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>Következő lépések

A mobileszközök beállításáról a [Mobileszközök beállítása a Microsoft 365 Business felhasználóinak](set-up-mobile-devices.md), az eszközvédelmi vagy appvédelmi beállítások megadásáról pedig [A Microsoft 365 Business kezelése](manage.md) című témakörben tájékozódhat.
  

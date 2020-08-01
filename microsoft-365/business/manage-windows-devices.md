---
title: Tartományhoz csatlakozott Windows 10-es eszközök microsoft 365 vállalati verziós kezelésének engedélyezése
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
description: Megtudhatja, hogy miként engedélyezheti a Microsoft 365 számára a helyi Active Directoryhoz csatlakozott Windows 10-eszközök védelmét néhány lépésben.
ms.openlocfilehash: 2eaf5aa76cae1680b93af008af615ae872e4fb20
ms.sourcegitcommit: fab425ea4580d1924fb421e6db233d135f5b7d19
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/31/2020
ms.locfileid: "46533785"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>A tartományhoz csatlakozó Windows 10-eszközök Microsoft 365 Business Premium általi kezelésének engedélyezése

Ha a szervezet a helyszíni Windows Server Active Directoryt használja, beállíthatja a Microsoft 365 Business Premium rendszert a Windows 10-es eszközök védelmére, miközben továbbra is hozzáférhet a helyi hitelesítést igénylő helyszíni erőforrásokhoz.
A védelem beállításához hibrid **Azure AD-hez csatlakozott eszközöket**valósíthat meg. Ezek az eszközök a helyszíni Active Directoryhoz és az Azure Active Directoryhoz is csatlakoznak.

Ez a videó bemutatja, hogyan állíthatja be ezt a leggyakoribb forgatókönyvhöz, amelyet a következő lépések is részleteznek.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a>Mielőtt elkezdene, végezze el az alábbi lépéseket:
- Szinkronizálja a felhasználókat az Azure AD-vel az Azure AD Connect segítségével.
- Teljes Azure AD Connect szervezeti egység (OU) szinkronizálás.
- Győződjön meg arról, hogy a szinkronizált tartomány összes felhasználója rendelkezik licenccel a Microsoft 365 Business Premium szolgáltatáshoz.

A lépésekről a [Tartományfelhasználók szinkronizálása a Microsofthoz](manage-domain-users.md) című témakörben található.

## <a name="1-verify-mdm-authority-in-intune"></a>1. Az MDM-szolgáltató ellenőrzése az Intune-ban

Lépjen a portal.azure.com, és a lap tetején keresse meg az Intune-t.
A Microsoft Intune lapon válassza az **Eszközregisztráció** lehetőséget, és az **Áttekintés** lapon győződjön meg arról, hogy az **MDM-szolgáltató** **intune-i.**

- Ha az **MDM-szolgáltató** **nincs,** kattintson az **MDM-szolgáltatóra** az **Intune**beállításához.
- Ha az **MDM-szolgáltató** **a Microsoft Office 365**, nyissa meg az **Eszközök**  >  **regisztrálása eszközök,** és használja a **Add MDM hatóság** párbeszéd a jobb oldalon, hogy adjunk **Intune MDM** hatóság (a **Add MDM-szolgáltató** párbeszédpanel csak akkor érhető el, ha az **MDM-szolgáltató** van beállítva a Microsoft Office 365).

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. Ellenőrizze, hogy az Azure AD engedélyezve van-e a számítógépek hez való csatlakozáshoz

- Nyissa meg a felügyeleti központot, <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> és válassza az Azure Active **Directory** (válassza az összes megjelenítése, ha az Azure Active Directory nem látható) a **Felügyeleti központok** listájában. 
- Az **Azure Active Directory felügyeleti központban**nyissa meg az Azure Active **Directoryt,** válassza **az Eszközök,** majd **az Eszközbeállítások lehetőséget.**
- Annak**ellenőrzése, hogy a felhasználók csatlakozhatnak-e az Azure AD-hez,** engedélyezve van-e 
    1. Az összes felhasználó engedélyezéséhez állítsa az **Összes**beállítását.
    2. Adott felhasználók engedélyezéséhez állítsa **a Kijelölt** beállítást egy adott felhasználói csoport engedélyezéséhez.
        - Adja hozzá az Azure AD-ben szinkronizált kívánt tartományi felhasználókat egy [biztonsági csoporthoz.](../admin/create-groups/create-groups.md)
        - Válassza **a Csoportok kijelölése** lehetőséget az MDM felhasználói hatókörének engedélyezéséhez az adott biztonsági csoporthoz.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. Ellenőrizze, hogy az Azure AD engedélyezve van-e az MDM-hez

- Lépjen a felügyeleti központba, <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> és válassza a **Végpontkezelők**t lehetőséget (válassza **az Összes megjelenítése** lehetőséget, ha az **Endpoint Manager** nem látható)
- A **Microsoft Endpoint Manager felügyeleti központban**nyissa meg **az Eszközök**  >  **windows**  >  **Windows-igénylés**  >  **automatikus igénylése**című lehetőséget.
- Ellenőrizze, hogy az MDM felhasználói hatóköre engedélyezve van-e.

    1. Az összes számítógép igényléséhez állítsa az **Összes** beállításra, hogy automatikusan regisztráljon minden olyan felhasználói számítógépet, amely az Azure AD-hez és az új számítógépekhez csatlakozik, amikor a felhasználók munkahelyi fiókot adnak hozzá a Windowshoz.
    2. A **Bizonyos** beállításra a felhasználók egy adott csoportjának számítógépeinek regisztrálására.
        -  Adja hozzá az Azure AD-ben szinkronizált kívánt tartományi felhasználókat egy [biztonsági csoporthoz.](../admin/create-groups/create-groups.md)
        -  Válassza **a Csoportok kijelölése** lehetőséget az MDM felhasználói hatókörének engedélyezéséhez az adott biztonsági csoporthoz.

## <a name="4-create-the-required-resources"></a>4. A szükséges erőforrások létrehozása 

A [hibrid Azure AD-illesztés konfigurálásához](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) szükséges feladatok végrehajtása leegyszerűsödött a [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell modulban található [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) parancsmag használatával. A parancsmag meghívásakor létrehozza és konfigurálja a szükséges szolgáltatáscsatlakozási pontot és csoportházirendet.

Ezt a modult a PowerShell egy példányából a következő meghívással telepítheti:

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> Javasoljuk, hogy telepítse ezt a modult a Windows Server azure AD Connect futó.

A szükséges szolgáltatáscsatlakozási pont és csoportházirend létrehozásához meg kell hívnia az [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) parancsmamot. A feladat végrehajtásakor szüksége lesz a Microsoft 365 Business Premium globális rendszergazdai hitelesítő adataira. Ha készen áll az erőforrások létrehozására, hívja meg a következőket:

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

Az első parancs kapcsolatot létesít a Microsoft felhőjével, és amikor a rendszer kéri, adja meg a Microsoft 365 Business Premium globális rendszergazdai hitelesítő adatait.

## <a name="5-link-the-group-policy"></a>5. A csoportházirend összekapcsolása

1. A Csoportházirend kezelése konzolon (GPMC) kattintson a jobb gombbal arra a helyre, ahol össze szeretné kapcsolni a házirendet, és válassza a Helyi menü *Meglévő csoportházirend-házirendjének csatolása parancsot.*
2. Jelölje ki a fenti lépésben létrehozott házirendet, majd kattintson az **OK**gombra.

## <a name="get-the-latest-administrative-templates"></a>A legújabb felügyeleti sablonok beszerezhetése

Ha nem látja az **Automatikus MDM-regisztráció engedélyezése az alapértelmezett Azure AD-hitelesítő adatokkal című házirendet,** annak az lehet az oka, hogy nincs telepítve az ADMX a Windows 10, 1803-as, 1803-as vagy 1903-as verzióhoz. A probléma megoldásához kövesse az alábbi lépéseket (Megjegyzés: a legújabb MDM.admx visszafelé kompatibilis):

1.  Letöltés: [Felügyeleti sablonok (.admx) a Windows 10 2019 májusi frissítéséhez (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).
2.  Telepítse a csomagot az elsődleges tartományvezérlőre (PDC).
3.  Navigálás a mappa verziójától függően: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.
4.  Nevezze át a **Házirenddefiníciók mappát** a **PolicyDefinitions**fenti elérési útján.
5.  A **PolicyDefinitions** mappa másolása a **C:\Windows\SYSVOL\domain\Policies mappába.** 
    -   Ha a teljes tartományközponti házirend-tárolót kíván használni, adja hozzá a PolicyDefinitions tartalmát.
6.  Indítsa újra az elsődleges tartományvezérlőt, hogy a házirend elérhető legyen. Ez eljárás akarat dolgozik részére akármi jövő változat jól.

Ezen a ponton látnia kell a házirend **automatikus MDM-regisztráció engedélyezése az alapértelmezett Azure AD hitelesítő adatok elérhető** használatával.

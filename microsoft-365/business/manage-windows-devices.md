---
title: A tartományhoz csatlakozott Windows 10-es eszközök kezelése a Microsoft 365 Vállalati verzióval
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
description: Megtudhatja, hogyan engedélyezheti a Microsoft 365-nek, hogy mindössze néhány lépésben védje a helyi Active Directoryhoz csatlakozott Windows 10-es eszközöket.
ms.openlocfilehash: 0b597110447272be128bfe1866234ac25a8e67e6
ms.sourcegitcommit: 070724118be25cd83418d2a56863da95582dae65
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/03/2021
ms.locfileid: "50407078"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>A tartományhoz csatlakozott Windows 10-es eszközök kezelése a Microsoft 365 Vállalati prémium verzióval

Ha szervezete helyszíni Windows Server Active Directoryt használ, beállíthatja a Microsoft 365 Vállalati prémium verzióban a Windows 10-es eszközök védelmét, miközben továbbra is hozzáférhet a helyi hitelesítést igénylő helyszíni erőforrásokhoz.
A védelem beállításához hibrid Azure AD-hez csatlakozott eszközöket **kell implementálja.** Ezek az eszközök a helyszíni Active Directoryhoz és az Azure Active Directoryhoz is csatlakoznak.

Ebből a videóból megtudhatja, hogy miként állíthatja be ezt a leggyakoribb forgatókönyvhöz, amely az alábbi lépésekben is részletesen le van írják.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a>Mielőtt neki kezd, győződjön meg arról, hogy a következő lépéseket kell végrehajtania:
- Szinkronizálja a felhasználókat az Azure AD-be az Azure AD Connect segítségével.
- Az Azure AD Connect szervezeti egység (OU) szinkronizálásának befejezése.
- Győződjön meg arról, hogy a szinkronizált összes tartományi felhasználó rendelkezik Licenccel a Microsoft 365 Vállalati prémium verzióhoz.

See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.

## <a name="1-verify-mdm-authority-in-intune"></a>1. A MDM Authority ellenőrzése az Intune-ban

A [Végpontkezelőben](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) a Microsoft Intune lapon válassza az Eszköz regisztrálása **lehetőséget,** majd az **Áttekintés** lapon győződjön meg arról, hogy az **MDM-felügyelet** **Intune.**

- Ha **a MDM authority (MDM authority** is None) (Nincs) **beállításhoz** kattintson az **MDM-hez,** és állítsa **be Intune-ra.**
- Ha a Microsoft **Office 365-ös**  **MDM-hitelesítést** használja, az Eszközök regisztrálása eszközre ugrás után vegye fel az Intune MDM-hatót a jobb oldalon található MDM authority (Az MDM-felügyelet hozzáadása párbeszédpanel csak akkor érhető el, ha a  >   **MDM Authority** beállítása Microsoft Office 365).   

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. Annak ellenőrzése, hogy az Azure AD engedélyezve van-e a számítógépekhez való csatlakozáshoz

- A Felügyeleti központok listában válassza az Azure Active Directory felügyeleti központját (válassza az Összes megjelenítése, ha az Azure Active Directory nem <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> látható) lehetőséget.   
- Az **Azure Active Directory Felügyeleti központban** válassza az **Azure Active Directory** lehetőséget, válassza az **Eszközök,** majd az **Eszközbeállítások lehetőséget.**
- Annak ellenőrzése, hogy a **Felhasználók csatlakozhatnak-e** az Azure AD-hez, engedélyezve van-e 
    1. Ha az összes felhasználót engedélyezni szeretné, állítsa a **Mind beállításra.**
    2. Ha csak bizonyos felhasználókat szeretné engedélyezni, állítsa **a Bejelölve** beállítást a felhasználók egy adott csoportjának engedélyezéséhez.
        - Adja hozzá az Azure AD-ban szinkronizált kívánt tartományfelhasználót egy [biztonsági csoporthoz.](../admin/create-groups/create-groups.md)
        - Válassza **a Csoportok kiválasztása lehetőséget,** ha engedélyezni szeretné az MDM-felhasználó hatókörét az adott biztonsági csoportban.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. Annak ellenőrzése, hogy az Azure AD engedélyezve van-e az MDM-hez

- Menjen a felügyeleti központba, és válassza a Végpontkezelő t lehetőséget (válassza az Összes megjelenítése, ha nem látható a <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  **Végpontkezelő)** lehetőséget. 
- A **Microsoft Endpoint Manager Felügyeleti központban** a Windows-regisztráció automatikus beléptetése eszközcsoportot kell  >    >    >  **látnia.**
- Ellenőrizze, hogy engedélyezve van-e az MDM felhasználói hatóköre.

    1. Ha az összes számítógépet  regisztrálnia kell, állítsa Az összes beállításra úgy, hogy automatikusan regisztrálja az Azure AD-hez és az új számítógépekhez csatlakozott összes felhasználói számítógépet, amikor a felhasználók munkahelyi fiókot adnak hozzá a Windowshoz.
    2. A **"Néhány" beállításra** beállítva regisztrálja egy adott felhasználócsoport számítógépeit.
        -  Adja hozzá az Azure AD-ban szinkronizált kívánt tartományfelhasználót egy [biztonsági csoporthoz.](../admin/create-groups/create-groups.md)
        -  Válassza **a Csoportok kiválasztása lehetőséget,** ha engedélyezni szeretné az MDM-felhasználó hatókörét az adott biztonsági csoportban.

## <a name="4-create-the-required-resources"></a>4. A szükséges erőforrások létrehozása 

A hibrid Azure [AD-illesztés](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) konfigurálására vonatkozó szükséges feladatok végrehajtása egyszerűbbé lett a [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell modulban található [Inicializálás-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) parancsmag használatával. Amikor meghívja ezt a parancsmagot, a parancsmag létrehozza és konfigurálja a szükséges szolgáltatási csatlakozási pontot és csoportházirendet.

A modult a PowerShell egy példányából az alábbi meg invoking segítségével telepítheti:

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> Javasoljuk, hogy telepítse ezt a modult az Azure AD Connectet futtató Windows Serveren.

A szükséges szolgáltatási csatlakozási pont és csoportházirend létrehozásához meg kell hívnia az  [Inicializálás-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) parancsmagot. A feladat végrehajtásához szüksége lesz a Microsoft 365 Vállalati prémium verzió globális rendszergazdai hitelesítő adataira. Ha készen áll az erőforrások létrehozására, hívja meg az alábbiakat:

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

Az első parancs kapcsolatot létesít a Microsoft felhővel, és amikor a rendszer kéri, adja meg a Microsoft 365 Vállalati prémium verzió globális rendszergazdai hitelesítő adatait.

## <a name="5-link-the-group-policy"></a>5. A csoportházirend összekapcsolása

1. A Csoportházirend kezelése konzolon (GPMC) kattintson a jobb gombbal arra a helyre, ahol a házirendet össze szeretné csatolni, és válassza a Helyi menü Meglévő *csoportházirend-objektum* csatolása parancsát.
2. Jelölje ki a fenti lépésben létrehozott házirendet, majd kattintson az **OK gombra.**

## <a name="get-the-latest-administrative-templates"></a>A legújabb felügyeleti sablonok letöltése

Ha nem látja az Automatikus **MDM-regisztráció** engedélyezése alapértelmezett Azure AD hitelesítő adatokkal házirendet, annak az lehet az oka, hogy nem telepítette az ADMX-et a Windows 10-es, 1803-as vagy újabb verziójához. A probléma megoldásához kövesse az alábbi lépéseket (megjegyzés: az MDM.admx legújabb kompatibilis az előző verzióval):

1.  Letöltés: [Felügyeleti sablonok (.admx) a Windows 10 2020. októberi frissítéséhez (20H2).](https://www.microsoft.com/download/102157)
2.  Telepítse a csomagot egy tartományvezérlőre.
3.  A felügyeleti sablonok verziójától függően navigáljon a mappához: **C:\Program Files (x86)\Microsoft Csoportházirend\Windows 10 2020. októberi frissítés (20H2)**.
4.  Nevezze át **a Fenti elérési út Házirenddefiníciók** **mappáját a PolicyDefinitions névre.**
5.  Másolja a **PolicyDefinitions** mappát a SYSVOL-megosztásba, amely alapértelmezés szerint a **C:\Windows\SYSVOL\domain\Policies** mappában található. 
    -   Ha egy központi házirend-tárolót szeretne használni a teljes tartományhoz, ott vegye fel a PolicyDefinitions tartalmát.
6.  Ha több tartományvezérlője van, várja meg, amíg a SYSVOL replikálja a házirendeket. Ez az eljárás a felügyeleti sablonok jövőbeli verzióival is működik.

Ezen a ponton láthatja az Automatikus MDM-regisztráció engedélyezése alapértelmezett **Azure AD-hitelesítő adatokkal elérhető** házirendet.

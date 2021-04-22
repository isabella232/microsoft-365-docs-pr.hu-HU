---
title: A tartományhoz csatlakozott Windows 10-es eszközök microsoft 365 vállalati verziós kezelése
f1.keywords:
- CSH
ms.author: efrene
author: efrene
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
ms.openlocfilehash: c9f5a21d993200abcf9ecf1fa236879245e1c153
ms.sourcegitcommit: 4076b43a4b661de029f6307ddc1a989ab3108edb
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2021
ms.locfileid: "51939502"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>A tartományhoz csatlakozott Windows 10-es eszközök kezelése a Microsoft 365 Business Premiumval

Ha szervezete helyszíni Windows Server Active Directoryt használ, beállíthatja a Microsoft 365 Business Premiumt a Windows 10-es eszközök védelme érdekében úgy, hogy közben továbbra is hozzáférjen a helyi hitelesítést igénylő helyszíni erőforrásokhoz.
A védelem beállításához hibrid Azure AD-hez csatlakozású eszközöket **kell implementálja.** Ezek az eszközök a helyszíni Active Directoryhoz és az Azure Active Directoryhoz egyaránt csatlakoznak.

Ez a videó bemutatja, hogy miként állíthatja be ezt a leggyakoribb forgatókönyvhöz, amely az alábbi lépésekben is részletesen le van írják.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a>Mielőtt neki kezd, győződjön meg arról, hogy végre kell ezeket a lépéseket:
- Felhasználók szinkronizálása az Azure AD-be az Azure AD Connect használatával.
- Az Azure AD Connect szervezeti egység (OU) szinkronizálásának befejezése.
- Győződjön meg arról, hogy a szinkronizált összes tartományfelhasználó rendelkezik Licenccel a Microsoft 365 Vállalati prémium verzióhoz.

A [lépéseket a Tartományfelhasználók szinkronizálása a Microsofttal](manage-domain-users.md) lásd.

## <a name="1-verify-mdm-authority-in-intune"></a>1. A MDM Authority ellenőrzése az Intune-ban

Válassza a [Végpontkezelő lehetőséget,](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) majd a Microsoft Intune lapon válassza az Eszköz regisztrálása **lehetőséget,** majd az **Áttekintés** lapon győződjön meg arról, hogy az **MDM authority** **az Intune.**

- Ha **az MDM authority** (Nincs) **beállításnál** az MDM authority (Nincs) beállításhoz kattintson az **MDM authority (MDM-hitelesítés)** elemre az **Intune beállításhoz.**
- Ha az **MDM** authority a **Microsoft Office 365,** válassza az Eszközök regisztrálása eszközt, és az Intune MDM authority hozzáadásához használja a jobb oldalon az   >   **MDM** authority (MDM Authority hozzáadása) párbeszédpanelt (az **MDM Authority** hozzáadása párbeszédpanel csak akkor érhető el, ha a Microsoft Office 365-ösre van beállítva az **MDM** **Authority).**

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. Annak ellenőrzése, hogy az Azure AD engedélyezve van-e a számítógépekhez való csatlakozáshoz

- A Felügyeleti központban válassza az Azure Active Directory lehetőséget (válassza Az összes megjelenítése, ha az Azure Active Directory nem látható) lehetőséget a Felügyeleti <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **központok listában.**  
- Az **Azure Active Directory Felügyeleti központban** válassza az **Azure Active Directory** lehetőséget, válassza az **Eszközök,** majd az **Eszközbeállítások lehetőséget.**
- Annak ellenőrzése, hogy a **Felhasználók csatlakozhatnak-e az Azure AD-hez** engedélyezve van-e 
    1. Az összes felhasználó engedélyezéséhez állítsa a Mind **beállításra.**
    2. Ha csak bizonyos felhasználókat szeretné engedélyezni, állítsa **a Bejelölve** beállítást egy adott felhasználócsoport engedélyezéséhez.
        - Adja hozzá az Azure AD-ban szinkronizált tartományfelhasználót egy [biztonsági csoporthoz.](../admin/create-groups/create-groups.md)
        - Válassza **a Csoportok kiválasztása lehetőséget,** ha engedélyezni szeretné az MDM-felhasználók hatókörét az adott biztonsági csoportban.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. Annak ellenőrzése, hogy az Azure AD engedélyezve van-e az MDM-hez

- A felügyeleti központ megnyitásához válassza <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> a Endpoint  **Managemen**  t (Az összes megjelenítése, ha a Végpontkezelő nem látható) lehetőséget.
- A **Microsoft Endpoint Manager Felügyeleti központban** menjen az **Eszközök**  >    >  **Windows Enrollment** Automatikus  >  **regisztrálása lapra.**
- Ellenőrizze, hogy engedélyezve van-e az MDM felhasználói hatóköre.

    1. Az összes számítógép regisztrálásának beállítását a Mind beállításra állítva automatikusan regisztrálja az Azure AD szolgáltatáshoz és az új számítógépekhez regisztrált összes számítógépet, amikor a felhasználók munkahelyi fiókot hozzáadnak a Windowshoz. 
    2. A Néhány **beállításra** beállítva regisztrálja egy adott felhasználócsoport számítógépeit.
        -  Adja hozzá az Azure AD-ban szinkronizált tartományfelhasználót egy [biztonsági csoporthoz.](../admin/create-groups/create-groups.md)
        -  Válassza **a Csoportok kiválasztása lehetőséget,** ha engedélyezni szeretné az MDM-felhasználók hatókörét az adott biztonsági csoportban.

## <a name="4-create-the-required-resources"></a>4. A szükséges erőforrások létrehozása 

A hibrid Azure [AD-illesztés](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) konfigurálására vonatkozó szükséges feladatok végrehajtása egyszerűbbé lett a [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell modulban található [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) parancsmag használatával. Amikor meghívja ezt a parancsmagot, az létrehozza és konfigurálja a szükséges szolgáltatási csatlakozási pontot és csoportházirendet.

A modult az alábbi PowerShell-példányból való megtelepítésével telepítheti:

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> Javasoljuk, hogy telepítse ezt a modult az Azure AD Connectet futtató Windows Serverre.

A szükséges szolgáltatási csatlakozási pont és csoportházirend létrehozásához meg kell hívnia az  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) parancsmagot. A feladat végrehajtásához szüksége lesz a Microsoft 365 Vállalati prémium verziós globális rendszergazdai hitelesítő adataira. Ha készen áll az erőforrások létrehozására, hívja meg az alábbiakat:

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

Az első parancs kapcsolatot létesít a Microsoft felhővel, és amikor a rendszer kéri, adja meg a Microsoft 365 Vállalati prémium verziós globális rendszergazdai hitelesítő adatait.

## <a name="5-link-the-group-policy"></a>5. A csoportházirend csatolása

1. A Csoportházirend kezelése konzolon (GPMC) kattintson a jobb gombbal arra a helyre, ahová a házirendet össze szeretnécsatni, és válassza a helyi menü Meglévő *csoportházirend-objektum* csatolása parancsát.
2. Jelölje ki a fenti lépésben létrehozott házirendet, majd kattintson az **OK gombra.**

## <a name="get-the-latest-administrative-templates"></a>Szerezze be a legújabb felügyeleti sablonokat

Ha nem látható az Automatikus **MDM-regisztráció** engedélyezése az Azure AD alapértelmezett hitelesítő adataival házirend, annak az lehet az oka, hogy nincs telepítve az ADMX a Windows 10 10-es vagy újabb verziójához. A probléma megoldásához kövesse az alábbi lépéseket (megjegyzés: A legújabb MDM.admx visszamenőlegesen kompatibilis:

1.  Letöltés: [Rendszergazdai sablonok (.admx) a Windows 10 2020. októberi frissítéséhez (20H2)](https://www.microsoft.com/download/102157).
2.  Telepítse a csomagot egy tartományvezérlőn.
3.  A felügyeleti sablonok verziójától függően a következő mappába navigálhat: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 October 2020 Update (20H2)**.
4.  Nevezze át **a Policy Definitions mappát** a fenti útvonalon a **PolicyDefinitions névre.**
5.  Másolja **a PolicyDefinitions** mappát a SYSVOL megosztásba, amely alapértelmezés szerint a **C:\Windows\SYSVOL\tartomány\Policies** helyen található. 
    -   Ha a teljes tartományhoz egy központi házirendtárat szeretne használni, adja hozzá a HázirendDefinitions mező tartalmát.
6.  Ha több tartományvezérlője van, várja meg, amíg a SYSVOL replikálja a házirendeket. Ez az eljárás a felügyeleti sablonok későbbi verzióival is működni fog.

Ezen a ponton látnia kell az Automatikus **MDM-regisztráció** engedélyezése az alapértelmezett Azure AD-beli hitelesítő adatokkal elérhető házirendet.

## <a name="related-content"></a>Kapcsolódó tartalom

[A tartományfelhasználók szinkronizálása a Microsoft 365-be](manage-domain-users.md) (cikk) Csoport létrehozása a Felügyeleti [központban](../admin/create-groups/create-groups.md) (cikk) Oktatóprogram: A hibrid [Azure Active Directory-alapú](/azure/active-directory/devices/hybrid-azuread-join-managed-domains.md) csatlakozás konfigurálása felügyelt tartományokhoz (cikk)
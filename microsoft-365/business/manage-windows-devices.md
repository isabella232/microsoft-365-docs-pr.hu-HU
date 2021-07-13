---
title: Tartományhoz Windows 10 eszközök vállalati verziós Microsoft 365 kezelése
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
- AdminTemplateSet
search.appverid:
- BCS160
- MET150
description: Ebből a cikkből megtudhatja, Microsoft 365 pár lépésben hogyan védheti a helyi Active Directoryhoz Windows 10 a helyi Active Directoryhoz Windows 10 eszközét.
ms.openlocfilehash: 9cc7ca01cec667465e9114083fecdc56ef4e7ce7
ms.sourcegitcommit: 00f001019c653269d85718d410f970887d904304
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/12/2021
ms.locfileid: "53393379"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>A tartományhoz Windows 10 eszközöknek a felhasználók által Microsoft 365 Vállalati prémium verzió

Ha szervezete helyszíni Windows Server Active Directory használ, beállíthatja a Microsoft 365 Vállalati prémium verzió-t az Windows 10-eszközök védelmére, miközben továbbra is hozzáfér a helyi hitelesítést igénylő helyszíni erőforrásokhoz.
A védelem beállításához hibrid Azure AD-hez csatlakozású eszközöket **kell implementálja.** Ezek az eszközök a helyszíni Active Directoryhoz és a számítógépéhez Azure Active Directory.

## <a name="watch-configure-hybrid-azure-active-directory-join"></a>Watch: Configure Hybrid Azure Active Directory join

Ez a videó bemutatja, hogy miként állíthatja be ezt a leggyakoribb forgatókönyvhöz, amely az alábbi lépésekben is részletesen le van írják.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="before-you-begin"></a>Az első lépések

- Szinkronizálja a felhasználókat az Azure AD szolgáltatásba az Azure AD Csatlakozás.
- Az Azure AD Csatlakozás szervezeti egység (OU) szinkronizálásának befejezése.
- Győződjön meg arról, hogy az összes szinkronizált tartományfelhasználó rendelkezik licenccel a Microsoft 365 Vállalati prémium verzió.

A [lépéseket a Tartományfelhasználók szinkronizálása a Microsofttal](manage-domain-users.md) lásd.

## <a name="1-verify-mdm-authority-in-intune"></a>1. A MDM Authority ellenőrzése az Intune-ban

Válassza [a Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) lap Microsoft Intune eszközregisztrálás **lehetőséget,** majd az Áttekintés  lapon ellenőrizze, hogy az **MDM authority** az **Intune.**

- Ha **az MDM authority** (Nincs) **beállításnál** az MDM authority (Nincs) beállításhoz kattintson az **MDM authority (MDM-hitelesítés)** elemre az **Intune beállításhoz.**
- Ha **mDM** authority is **Microsoft Office 365**, menjen az Eszközök regisztrálása eszközre, és az Intune MDM authority hozzáadásához használja a jobb oldalon az MDM authority (MDM Authority hozzáadása) párbeszédpanelt (az MDM Authority hozzáadása párbeszédpanel csak akkor érhető el, ha  >   az **MDM Authority (MDM** Authority) beállítás Microsoft Office 365).   

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. Annak ellenőrzése, hogy az Azure AD engedélyezve van-e a számítógépekhez való csatlakozáshoz

- A Felügyeleti központ megnyitásához a Felügyeleti központok <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **listában válassza** Azure Active Directory (válassza Az  összes megjelenítése, Azure Active Directory látható) lehetőséget. 
- A Azure Active Directory **Felügyeleti központban válassza** a Azure Active Directory **,** majd az Eszközök, majd az  **Eszközbeállítások lehetőséget.**
- Annak ellenőrzése, hogy a **Felhasználók csatlakozhatnak-e az Azure AD-hez** engedélyezve van-e 
    1. Az összes felhasználó engedélyezéséhez állítsa a Mind **beállításra.**
    2. Ha csak bizonyos felhasználókat szeretné engedélyezni, állítsa **a Bejelölve** beállítást egy adott felhasználócsoport engedélyezéséhez.
        - Adja hozzá az Azure AD-ban szinkronizált tartományfelhasználót egy [biztonsági csoporthoz.](../admin/create-groups/create-groups.md)
        - Válassza **a Csoportok kiválasztása lehetőséget,** ha engedélyezni szeretné az MDM-felhasználók hatókörét az adott biztonsági csoportban.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. Annak ellenőrzése, hogy az Azure AD engedélyezve van-e az MDM-hez

- A felügyeleti központ megnyitásához válassza a Végpont kezelése 1 lehetőséget (ha nem látható az összes Endpoint Manager <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> lehetőséget)   
- A Microsoft Endpoint Manager **Felügyeleti központban az** Eszközök Windows  >    >  **Windows**  >  **központban.**
- Ellenőrizze, hogy engedélyezve van-e az MDM felhasználói hatóköre.

    1. Az összes számítógép regisztrálásának beállítását a Mind beállításra állítva automatikusan regisztrálja az Azure AD szolgáltatáshoz és az új számítógépekhez regisztrált összes felhasználói számítógépet, amikor a felhasználók munkahelyi fiókot Windows. 
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
> Javasoljuk, hogy telepítse ezt a modult az Azure AD-Windows futtató Csatlakozás.

A szükséges szolgáltatási csatlakozási pont és csoportházirend létrehozásához meg kell hívnia az  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) parancsmagot. A feladat végrehajtásához Microsoft 365 Vállalati prémium verzió globális rendszergazdai hitelesítő adatokra lesz szüksége. Ha készen áll az erőforrások létrehozására, hívja meg az alábbiakat:

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

Az első parancs kapcsolatot létesít a Microsoft-felhővel, és amikor a rendszer kéri, adja meg Microsoft 365 Vállalati prémium verzió globális rendszergazdai hitelesítő adatait.

## <a name="5-link-the-group-policy"></a>5. A csoportházirend csatolása

1. A Csoportházirend kezelése konzolon (GPMC) kattintson a jobb gombbal arra a helyre, ahová a házirendet össze szeretnécsatni, és válassza a helyi menü Meglévő *csoportházirend-objektum* csatolása parancsát.
2. Jelölje ki a fenti lépésben létrehozott házirendet, majd kattintson az **OK gombra.**

## <a name="get-the-latest-administrative-templates"></a>Szerezze be a legújabb felügyeleti sablonokat

Ha nem látja az Automatikus **MDM-regisztráció** engedélyezése alapértelmezett Azure AD-beli hitelesítő adatokkal házirendet, annak az lehet az oka, hogy nincs telepítve az ADMX az Windows 10 1803-as vagy újabb verziójához. A probléma megoldásához kövesse az alábbi lépéseket (megjegyzés: A legújabb MDM.admx visszamenőlegesen kompatibilis:

1. Letöltés: [Rendszergazdai sablonok (.admx) Windows 10 2020. októberi frissítéshez (20H2).](https://www.microsoft.com/download/102157)
2. Telepítse a csomagot egy tartományvezérlőn.
3. A felügyeleti sablonok verziójától függően a következő mappába navigálhat: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 2020. októberi frissítés (20H2)**.
4. Nevezze át **a Policy Definitions mappát** a fenti útvonalon a **PolicyDefinitions névre.**
5. Másolja **a PolicyDefinitions** mappát a SYSVOL megosztásba, amely alapértelmezés szerint a **C:\Windows\SYSVOL\tartomány\Policies** helyen található.
   - Ha a teljes tartományhoz egy központi házirendtárat szeretne használni, adja hozzá a HázirendDefinitions mező tartalmát.
6. Ha több tartományvezérlője van, várja meg, amíg a SYSVOL replikálja a házirendeket. Ez az eljárás a felügyeleti sablonok későbbi verzióival is működni fog.

Ezen a ponton látnia kell az Automatikus **MDM-regisztráció** engedélyezése az alapértelmezett Azure AD-beli hitelesítő adatokkal elérhető házirendet.

## <a name="related-content"></a>Kapcsolódó tartalom

[Tartományfelhasználók szinkronizálása a Microsoft 365](manage-domain-users.md) (cikk)\
[Csoport létrehozása a Felügyeleti központban](../admin/create-groups/create-groups.md) (cikk)\
[Oktatóprogram: A hibrid Azure Active Directory konfigurálása felügyelt tartományokhoz](/azure/active-directory/devices/hybrid-azuread-join-managed-domains.md) (cikk)
---
title: Helyszíni erőforrások elérése Azure AD-hez csatlakozott eszközről a Microsoft 365 Vállalati verzióban
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: M365-subscription-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
- AdminTemplateSet
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Megtudhatja, hogy miként férhet hozzá helyszíni erőforrásokhoz, például üzletági alkalmazásokhoz, fájlmegosztáshoz és nyomtatókhoz egy Azure Active Directory-Windows 10 eszközről.
ms.openlocfilehash: 71d60e0187c917dffb7390afcedf22dc73f44008
ms.sourcegitcommit: 00f001019c653269d85718d410f970887d904304
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/12/2021
ms.locfileid: "53393459"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Helyszíni erőforrások elérése Azure AD-hez Microsoft 365 Vállalati prémium verzió

Ez a cikk a Microsoft 365 Vállalati prémium verzió.

Minden Windows 10 eszközhöz, amely Azure Active Directory csatlakozik, hozzáféréssel rendelkezik az összes felhőalapú erőforráshoz, például a Microsoft 365-alkalmazásokhoz, és a felhasználó Microsoft 365 Vállalati prémium verzió. A helyszíni erőforrásokhoz, például üzletági alkalmazásokhoz, fájlmegosztáshoz és nyomtatókhoz való hozzáférést is engedélyezheti. A hozzáférés engedélyezése érdekében az [Azure AD Csatlakozás](/azure/active-directory/connect/active-directory-aadconnect) segítségével szinkronizálja a helyszíni Active Directory-címtárát a Azure Active Directory.

További információért olvassa el a Bevezetés az [eszközkezelésbe a Azure Active Directory.](/azure/active-directory/device-management-introduction)
A lépéseket az alábbi szakaszokban is összegzi.

## <a name="run-azure-ad-connect"></a>Az Azure AD-Csatlakozás

Az alábbi lépésekkel engedélyezheti szervezete Azure AD-hez csatlakozott eszközeinek a helyszíni erőforrásokhoz való hozzáférést.

1. Ha a felhasználókat, csoportokat és névjegyeket a helyi Active Directoryból a Azure Active Directory-ba szeretné szinkronizálni, futtassa a Címtár-szinkronizálási varázslót és az Azure AD Csatlakozás-t a Címtár-szinkronizálás beállítása [Office 365.](../enterprise/set-up-directory-synchronization.md)

2. Miután befejeződött a címtár-szinkronizálás, győződjön meg arról, hogy a Windows 10 az Azure AD-hez csatlakozva. Ez a lépés minden egyes eszközön Windows 10 történik. További [információt A Windows beállítása a Microsoft 365 Vállalati prémium verzió számára.](set-up-windows-devices.md)

3. Miután az Windows 10 eszköz csatlakozott az Azure AD-hez, minden felhasználónak újra kell indítania az eszközét, és be kell jelentkeznie a Microsoft 365 Vállalati prémium verzió hitelesítő adataival. Mostantól minden eszköz rendelkezik hozzáféréssel a helyszíni erőforrásokhoz is.

Az Azure AD-hez csatlakozott eszközök helyszíni erőforrásaihoz való hozzáféréshez nincs szükség további lépésekre. Ez a funkció a beépített Windows 10.

Ha nem jelszó módszert szeretne használni az AADJ-eszközre, például PIN-kódot/metrikust a WHFB hitelesítő adataival, majd helyi erőforrásokat (megosztásokat, nyomtatókat stb.) szeretne használni, kérjük, kövesse ezt a [cikket.](/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

Ha szervezete nem áll készen a fent ismertetett Azure AD-hez csatlakozású eszközkonfigurációban való telepítésre, fontolja meg a hibrid [Azure AD-csatlakozású eszközkonfiguráció beállítását.](manage-windows-devices.md)

### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Megfontolandó szempontok az Windows Azure AD-hez való csatlakozáskor

Ha az Windows eszköz, amelyhez az Azure-AD-hez csatlakozott, korábban tartományhoz csatlakozott vagy munkacsoportban volt, vegye figyelembe az alábbi korlátozásokat:

- Amikor egy eszköz csatlakozik az Azure AD-hez, egy új felhasználót hoz létre anélkül, hogy létező profilra hivatkozna. A profilokat manuálisan kell áttelepíteni. A felhasználói profilok olyan információkat tartalmaznak, mint például a kedvencek, helyi fájlok, böngészőbeállítások Start menü beállítások. A legjobb megoldás, ha megkeres egy külső eszközt, amely leképezi a meglévő fájlokat és beállításokat az új profilra.

- Ha az eszköz csoportházirend-objektumokat használ, előfordulhat, hogy egyes CSOPORTHÁZIREND-objektumok nem tartalmaznak hasonló konfigurációszolgáltatót [az](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) Intune-ban. Az [MMAT eszközzel megkereshetők](https://www.microsoft.com/download/details.aspx?id=45520) a meglévő GPOS-hez használható hasonló CSP-k.

- Előfordulhat, hogy a felhasználók nem tudják hitelesíteni az Active Directory-hitelesítéstől függő alkalmazásokat. Kiértékelheti a régi appot, és lehetőség szerint frissítheti a modern Auth hitelesítést használó appra.

- Az Active Directory-nyomtatók felderítése nem működik. Minden felhasználónak meg lehet adni közvetlen nyomtatóútját, vagy használhatja az [Univerzális nyomtatást.](/universal-print/)

### <a name="related-articles"></a>Kapcsolódó cikkek

[Az Azure AD-szolgáltatások Csatlakozás](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

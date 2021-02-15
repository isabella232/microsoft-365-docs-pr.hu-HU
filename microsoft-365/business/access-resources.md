---
title: Helyszíni erőforrások elérése Azure AD-hez csatlakozott eszközről a Microsoft 365 Vállalati verzióban
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Megtudhatja, hogy miként férhet hozzá helyszíni erőforrásokhoz, például üzleti alkalmazásokhoz, fájlmegosztáshoz és nyomtatókhoz egy Windows 10-es eszközhöz csatlakozott Azure Active Directory-eszközről.
ms.openlocfilehash: fc02fd30f41f25f52e653e750a6bdfd1bd7f800e
ms.sourcegitcommit: a62ac3c01ba700a51b78a647e2301f27ac437c5a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2021
ms.locfileid: "50233840"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Helyszíni erőforrások elérése Azure AD-hez csatlakozott eszközről a Microsoft 365 Vállalati prémium verzióban

Ez a cikk a Microsoft 365 Vállalati prémium verzióra vonatkozik.

Minden olyan Windows 10-es eszköz, amelyhez az Azure Active Directory csatlakozik, hozzáférhet az összes felhőalapú erőforráshoz, például a Microsoft 365-apphoz, és a Microsoft 365 Vállalati prémium verzió védheti. Engedélyezheti a hozzáférést a helyszíni erőforrásokhoz is, például üzletági alkalmazásokhoz, fájlmegosztáshoz és nyomtatókhoz. A hozzáférés engedélyezése érdekében az [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) segítségével szinkronizálja a helyszíni Active Directoryt az Azure Active Directoryval. 

További információért olvassa el az Eszközkezelés az [Azure Active Directoryban – Bevezetés.](https://docs.microsoft.com/azure/active-directory/device-management-introduction)
A lépéseket az alábbi szakaszokban is összegzi.
 
## <a name="run-azure-ad-connect"></a>Az Azure AD Connect futtatása

Az alábbi lépéseket követve engedélyezheti a szervezet Azure AD-hez csatlakozott eszközeinek a helyszíni erőforrásokhoz való hozzáférést.
  
1. Ha szinkronizálni szeretné a felhasználókat, csoportokat és névjegyeket a helyi Active Directoryból az Azure Active Directoryba, futtassa a Címtár-szinkronizálási varázslót és az Azure AD Connectet az [Office 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization)címtár-szinkronizálásának beállításával.
    
2. A címtár-szinkronizálás befejezése után győződjön meg arról, hogy szervezete Windows 10-es eszközeihez az Azure AD csatlakozik. Ez a lépés minden Windows 10-es eszközön külön-külön történik. További [információt a Windows-eszközök beállítása a Microsoft 365 Vállalati prémium](set-up-windows-devices.md) verzió felhasználóinak. 
    
3. Miután a Windows 10-es eszközök csatlakoztak az Azure AD-hez, minden felhasználónak újra kell indítania az eszközét, és be kell jelentkeznie a Microsoft 365 Vállalati prémium verziós hitelesítő adataival. Mostantól minden eszköz hozzáférhet a helyszíni erőforrásokhoz is.
    
Az Azure AD-hez csatlakozott eszközök helyszíni erőforrásaihoz való hozzáféréshez nincs szükség további lépésekre. Ez a funkció a Windows 10 beépített szolgáltatása. 

Ha a jelszótól (PÉLDÁUL PIN-kód/Metrikus stb.) kívül más AADJ-eszközre szeretne bejelentkezni a WHFB hitelesítő adatain keresztül, majd a helyi erőforrásokhoz (megosztások, nyomtatók) szeretne hozzáférni. stb.), kérjük, kövesse az https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Ha szervezete nem áll készen a fent ismertetett Azure AD-hez való csatlakozású eszközkonfiguráció telepítésére, fontolja meg a hibrid Azure AD-hez való csatlakozású [eszközkonfiguráció beállítását.](manage-windows-devices.md)
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Megfontolandó szempontok, amikor Windows-eszközökhöz csatlakozik az Azure AD szolgáltatáshoz

Ha az Azure-AD szolgáltatáshoz csatlakozott Windows-eszköz korábban tartományhoz csatlakozott vagy munkacsoport tagja volt, vegye figyelembe az alábbi korlátozásokat:
  
- Amikor egy eszközhez az Azure AD csatlakozik, egy új felhasználót hoz létre anélkül, hogy egy meglévő profilra hivatkozna. A profilokat manuálisan kell áttelepíteni. A felhasználói profilok olyan információkat tartalmaznak, mint a kedvencek, a helyi fájlok, a böngésző beállításai és a Start menü beállításai. A legjobb megoldás, ha egy külső gyártótól származó eszközt keres a meglévő fájlok és beállítások új profilhoz való leképezéséhez.

- Ha az eszköz csoportházirend-objektumokat használ, előfordulhat, hogy egyes csoportházirend-objektumok nem tartalmaznak hasonló konfigurációs [szolgáltatót](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) az Intune-ban. Az [MMAT eszközzel megkereshetők](https://www.microsoft.com/download/details.aspx?id=45520) a meglévő csoportházirend-objektumok hasonló CSP-ii.

- Előfordulhat, hogy a felhasználók nem tudják hitelesíteni az Active Directory-hitelesítéstől függő alkalmazásokat. Kiértékelheti a régi appot, és lehetőség szerint frissítheti a modern Auth hitelesítést használó appra.

- Az Active Directory-nyomtatók felderítése nem működik. Minden felhasználónak meg kell adnia a nyomtató közvetlen elérési útját, vagy használhatja az [Univerzális nyomtatást.](https://aka.ms/UPDocs)

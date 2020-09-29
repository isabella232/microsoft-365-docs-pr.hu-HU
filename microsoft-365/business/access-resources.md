---
title: Hozzáférés helyszíni erőforrásokhoz a Microsoft 365 Business Azure AD-csatlakoztatott eszközéről
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
description: Ebből a témakörből megtudhatja, hogy miként érheti el a helyszíni erőforrásokat, például a üzletági alkalmazások, a fájlmegosztás és a nyomtatókat egy Azure Active Directory-kapcsolattal rendelkező Windows 10-es eszközön.
ms.openlocfilehash: 2144268f5cbab67c39d5902622c61c0c35e6481c
ms.sourcegitcommit: 15be7822220041c25fc52565f1c64d252e442d89
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/28/2020
ms.locfileid: "48295310"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Hozzáférés helyszíni erőforrásokhoz a Microsoft 365 vállalati prémium verzióban elérhető Azure AD-eszközről

Ez a cikk a Microsoft 365 vállalati prémium verzióra vonatkozik.

Bármely olyan Windows 10-es eszköz, amely az Azure Active Directoryval van csatlakoztatva, hozzáféréssel rendelkezik az összes felhőalapú erőforráshoz, például a Microsoft 365-alkalmazásaihoz, és a Microsoft 365 Business Premium által is védett. A helyszíni erőforrások, például a üzletági (LOB) alkalmazások, a fájlmegosztás és a nyomtatók elérését is engedélyezheti. Az Access engedélyezéséhez az [Azure ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) segítségével szinkronizálja a helyszíni Active Directoryt az Azure Active Directoryval. 

További információért olvassa el az [eszközkezelés az Azure Active Directoryban – bevezetés](https://docs.microsoft.com/azure/active-directory/device-management-introduction)című témakört.
A lépéseket az alábbi szakaszokban is összegezjük.
 
## <a name="run-azure-ad-connect"></a>Az Azure AD Connect futtatása

A helyszíni erőforrások eléréséhez kövesse az alábbi lépéseket, amelyek lehetővé teszik a szervezet Azure AD egyesített eszközeinek elérését.
  
1. Ha a helyi Active Directoryból szeretné szinkronizálni a felhasználókat, a csoportokat és a névjegyeket az Azure Active Directoryhoz, futtassa a címtár-szinkronizálás varázslót és az Azure AD Connect parancsot a [címtár-szinkronizálás beállítása az Office 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization)-ban című témakörben leírtak szerint.
    
2. A címtár-szinkronizálás befejeződése után győződjön meg arról, hogy szervezete Windows 10-es eszközei az Azure AD-hoz csatlakoznak. Ezt a lépést egyenként elvégezheti minden Windows 10-es eszközön. Részletekért olvassa el a [Windows-eszközök beállítása a Microsoft 365 Business Premium felhasználói](set-up-windows-devices.md) számára című témakört. 
    
3. Miután a Windows 10-es eszközök az Azure AD-ra csatlakoznak, minden felhasználónak újra kell indítania az eszközeit, és be kell írnia a Microsoft 365 vállalati prémium verziós hitelesítő adataival. Minden eszközön elérhetők a helyszíni erőforrások is.
    
További lépésekre nincs szükség az Azure AD-hoz csatlakoztatott eszközök helyszíni erőforrásaihoz való hozzáférés megkezdéséhez. Ez a funkció a Windows 10 rendszerbe épül. 

Ha azt tervezi, hogy a AADJ-eszközre szeretne bejelentkezni, például a PIN-kód/bio-metrikus WHFB-beli hitelesítő adatokkal, jelentkezzen be, majd nyissa meg a helyszíni erőforrásokat (megosztásokat, nyomtatókat stb.). stb.), kérjük, kövesse az alábbi lépéseket https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Ha szervezete nem hajlandó telepíteni az Azure AD csatlakoztatott eszköz konfigurációjában leírt konfigurációt, fontolja meg a [hibrid Azure ad csatlakoztatott eszköz konfigurációjának](manage-windows-devices.md)beállítását.
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>A Windows-eszközök Azure AD-hoz való csatlakozásának szempontjai

Ha az Azure-AD-hoz csatlakoztatott Windows-eszköz korábban tartományhoz csatlakozik vagy egy munkacsoportban van, vegye figyelembe az alábbi korlátozásokat:
  
- Ha egy eszköz az Azure AD-hoz csatlakozik, egy új felhasználót hoz létre a meglévő profil hivatkozása nélkül. A profilokat manuálisan kell áttelepíteni. A felhasználói profilok olyan információkat tartalmaznak, mint például a Kedvencek, a helyi fájlok, a böngésző beállításai és a Start menü beállításai. A legjobb megoldás egy külső féltől származó eszköz megkeresése a meglévő fájlok és beállítások új profilba való megfeleltetéséhez.

- Ha az eszköz csoportházirend-objektumokat (GPO) használ, előfordulhat, hogy egyes csoportházirend-objektumok nem rendelkeznek összehasonlító [konfigurációs szolgáltatóval](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) az Intune szolgáltatásban. A [MMAT eszköz](https://www.microsoft.com/download/details.aspx?id=45520) futtatása a meglévő csoportházirend-objektumokhoz hasonló kriptográfiai szolgáltatók megkereséséhez.

- A felhasználók nem tudnak hitelesíteni olyan alkalmazásokat, amelyek az Active Directory-hitelesítéstől függenek. Értékelje ki a régi alkalmazást, és fontolja meg, hogy egy olyan alkalmazásra frissít, amely a modern hitelesítést használja, ha lehetséges.

- Az Active Directory-nyomtató felderítése nem működik. Közvetlen nyomtatási elérési utakat is biztosíthat az összes felhasználónak, vagy használhatja a [hibrid Felhőbeli nyomtatást](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).

---
title: Helyszíni erőforrások elérése Azure AD-csatlakozású eszközről a Microsoft 365 Vállalati verzióban
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
description: Megtudhatja, hogy miként férhet hozzá a helyszíni erőforrásokhoz, például üzletági alkalmazásokhoz, fájlmegosztáshoz és nyomtatókhoz egy Azure Active Directoryhoz csatlakozott Windows 10-es eszközről.
ms.openlocfilehash: 1bca0beb3ccc78e670ad33ce446b9b3f7c372ba7
ms.sourcegitcommit: 39609c4d8c432c8e7d7a31cb35c8020e5207385b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/30/2021
ms.locfileid: "51445348"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Helyszíni erőforrások elérése Azure AD-csatlakozású eszközről a Microsoft 365 Vállalati prémium verzióban

Ez a cikk a Microsoft 365 Vállalati prémium verzióra vonatkozik.

Minden olyan Windows 10-es eszköz, amelyhez az Azure Active Directory csatlakozik, hozzáféréssel rendelkezik az összes felhőalapú erőforráshoz, például a Microsoft 365-alkalmazásokhoz, és a Microsoft 365 Business Premiumval védheti őket. A helyszíni erőforrásokhoz, például üzletági alkalmazásokhoz, fájlmegosztáshoz és nyomtatókhoz való hozzáférést is engedélyezheti. A hozzáférés engedélyezése érdekében az [Azure AD Connect](/azure/active-directory/connect/active-directory-aadconnect) segítségével szinkronizálja a helyszíni Active Directoryt az Azure Active Directoryval. 

További információ: Eszközkezelés az [Azure Active Directoryban –](/azure/active-directory/device-management-introduction)Bevezetés.
A lépéseket az alábbi szakaszokban is összegzi.
 
## <a name="run-azure-ad-connect"></a>Az Azure AD Connect futtatása

Az alábbi lépésekkel engedélyezheti szervezete Azure AD-hez csatlakozott eszközeinek a helyszíni erőforrásokhoz való hozzáférést.
  
1. Ha a felhasználókat, csoportokat és névjegyeket a helyi Active Directoryból az Azure Active Directoryba szeretné szinkronizálni, futtassa a Címtár-szinkronizálási varázslót és az Azure AD Connectet az Office 365 címtár-szinkronizálásának beállítása [leírásának lépéseit használva.](../enterprise/set-up-directory-synchronization.md)
    
2. A címtár-szinkronizálás befejezése után győződjön meg arról, hogy a szervezet Windows 10-es eszközeihez az Azure AD csatlakozik. Ez a lépés minden Windows 10-es eszközön külön-külön történik. További [információt a Windows-eszközök beállítása a Microsoft 365 Vállalati prémium verzió felhasználóinak.](set-up-windows-devices.md) 
    
3. Miután a Windows 10-es eszközök csatlakoztak az Azure AD-hez, minden felhasználónak újra kell indítania az eszközét, és be kell jelentkeznie a Microsoft 365 Business Premiums hitelesítő adataival. Mostantól minden eszköz rendelkezik hozzáféréssel a helyszíni erőforrásokhoz is.
    
Az Azure AD-hez csatlakozott eszközök helyszíni erőforrásaihoz való hozzáféréshez nincs szükség további lépésekre. Ez a funkció a Windows 10 beépített szolgáltatása. 

Ha az AADJ-eszközre nem jelszó módszert szeretne használni (például PIN-kód/metrikus adatokat a WHFB hitelesítő adataival), majd helyi erőforrásokat (megosztásokat, nyomtatókat) szeretne használni. stb.), kövesse az https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Ha szervezete nem áll készen a fent ismertetett Azure AD-hez csatlakozású eszközkonfigurációban való telepítésre, fontolja meg a hibrid [Azure AD-csatlakozású eszközkonfiguráció beállítását.](manage-windows-devices.md)
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Megfontolandó szempontok a Windows-eszközök Azure AD-hez való csatlakozásakor

Ha az Azure-AD-hoz csatlakozott Windows-eszköz korábban tartományhoz csatlakozott vagy munkacsoportban volt, vegye figyelembe az alábbi korlátozásokat:
  
- Amikor egy eszköz csatlakozik az Azure AD-hez, egy új felhasználót hoz létre anélkül, hogy létező profilra hivatkozna. A profilokat manuálisan kell áttelepíteni. A felhasználói profilok olyan információkat tartalmaznak, mint például a kedvencek, a helyi fájlok, a böngésző beállításai és a Start menü beállításai. A legjobb megoldás, ha megkeres egy külső eszközt, amely leképezi a meglévő fájlokat és beállításokat az új profilra.

- Ha az eszköz csoportházirend-objektumokat használ, előfordulhat, hogy egyes CSOPORTHÁZIREND-objektumok nem tartalmaznak hasonló konfigurációszolgáltatót [az](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) Intune-ban. Az [MMAT eszközzel megkereshetők](https://www.microsoft.com/download/details.aspx?id=45520) a meglévő GPOS-hez használható hasonló CSP-k.

- Előfordulhat, hogy a felhasználók nem tudják hitelesíteni az Active Directory-hitelesítéstől függő alkalmazásokat. Kiértékelheti a régi appot, és lehetőség szerint frissítheti a modern Auth hitelesítést használó appra.

- Az Active Directory-nyomtatók felderítése nem működik. Minden felhasználónak meg lehet adni közvetlen nyomtatóútját, vagy használhatja az [Univerzális nyomtatást.](/universal-print/)

### <a name="related-articles"></a>Kapcsolódó cikkek

[Az Azure AD Connect előfeltételei](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

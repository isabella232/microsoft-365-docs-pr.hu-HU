---
title: Helyszíni erőforrások elérése Azure AD-hez csatlakozó eszközről a Microsoft 365 Vállalati verzióban
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
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Megtudhatja, hogy miként férhet hozzá a helyszíni erőforrásokhoz, például az üzleti alkalmazások sorához, a fájlmegosztásokhoz és a nyomtatókhoz egy Azure Active Directoryhoz csatlakozott Windows 10-es eszközről.
ms.openlocfilehash: 653b53d29e84bbdc91273cb78b9b8407c0f6a209
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593233"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>Helyszíni erőforrások elérése Azure AD-hez csatlakozó eszközről a Microsoft 365 Vállalati verzióban

Minden Olyan Windows 10-es eszköz, amely hez csatlakozott az Azure Active Directory, minden felhőalapú erőforráshoz, például az Office 365-alkalmazásokhoz hozzáfér, és a Microsoft 365 Vállalati verzió is védheti őket. Engedélyezheti a helyszíni erőforrások, például üzletági alkalmazások, fájlmegosztások és nyomtatók elérését is. A hozzáférés engedélyezéséhez az [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) segítségével szinkronizálhatja a helyszíni Active Directoryt az Azure Active Directoryval. 

További információ: [Bevezetés az Eszközkezelés bemutatkozása az Azure Active Directoryban című témakörben.](https://docs.microsoft.com/azure/active-directory/device-management-introduction)
A lépések a következő szakaszokban is összefoglalva.

> [!IMPORTANT]
> Ez az eljárás csak az OAuth-ra és az NTLM-re vonatkozik. A Kerberos nem támogatott.
 
## <a name="run-azure-ad-connect"></a>Az Azure AD Connect futtatása

Hajtsa végre az alábbi lépéseket, hogy a szervezet Azure AD-csatlakozású eszközök a helyszíni erőforrások eléréséhez.
  
1. A helyi Active Directoryból származó felhasználók, csoportok és névjegyek szinkronizálásához futtassa a Címtár-szinkronizálás varázslót és az Azure AD Connectet az [Office 365 címtár-szinkronizálásának beállítása](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)című részben leírtak szerint.
    
2. A címtár-szinkronizálás befejezése után győződjön meg arról, hogy a szervezet Windows 10-es eszközei azure-ad-csatlakozással vannak elválasztva. Ez a lépés minden Windows 10-es eszközön külön-külön történik. A részletekért olvassa el [a Windows-eszközök beállítása a Microsoft 365 Vállalati verzió felhasználóiszámára.](set-up-windows-devices.md) 
    
3. Miután a Windows 10-es eszközök Azure AD-csatlakozása, minden felhasználónak újra kell indítania az eszközeit, és be kell jelentkeznie a Microsoft 365 Vállalati verzió hitelesítő adataival. Mostantól minden eszköz hozzáférhet a helyszíni erőforrásokhoz is.
    
Nincs szükség további lépésekre az Azure AD-hez csatlakozott eszközök helyszíni erőforrásaihoz való hozzáféréshez. Ez a funkció be van építve a Windows 10-be. 

Ha azt tervezi, hogy jelentkezzen be az AADJ eszköz más jelszó módszer, mint a PIN /Bio-metrikus WHFB hitelesítő bejelentkezés, majd a hozzáférést a helyszíni erőforrások (részvények, nyomtatók.. stb), kérjük, kövessehttps://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Ha a szervezet nem áll készen a fent leírt Azure AD-csatlakozású eszközkonfigurációban való üzembe helyezésre, fontolja meg [a hibrid Azure AD-csatlakozású eszköz konfigurációjának](manage-windows-devices.md)beállítását.
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>A Windows-eszközök Azure AD-höz való csatlakozásának szempontjai

Ha az Azure-AD-hez csatlakozott Windows-eszköz korábban tartományhoz csatlakozott vagy munkacsoportban volt, vegye figyelembe az alábbi korlátozásokat:
  
- Amikor egy eszköz Az Azure AD csatlakozik, létrehoz egy új felhasználót anélkül, hogy egy meglévő profilra hivatkozna. A profilokat manuálisan kell áttelepíteni. A felhasználói profil olyan információkat tartalmaz, mint a kedvencek, a helyi fájlok, a böngésző beállításai és a Start menü beállításai. A legjobb megközelítés az, hogy talál egy harmadik féltől származó eszköz, hogy feltérképezze a meglévő fájlokat és beállításokat az új profilt.

- Ha az eszköz csoportházirend-objektumokat (GPO) használ, előfordulhat, hogy egyes csoportházirend-objektumok nem rendelkeznek hasonló [konfigurációs szolgáltatóval](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) az Intune-ban. Futtassa az [MMAT eszközt,](https://www.microsoft.com/download/details.aspx?id=45520) hogy összehasonlítható csoportházirend-szolgáltatókat keressen a meglévő csoportházirend-szolgáltatókhoz.

- A felhasználók nem tudnak hitelesíteni az Active Directory hitelesítésétől függő alkalmazásokat. Értékelje ki az örökölt alkalmazást, és lehetőség szerint frissítsen egy modern hitelesítést használó alkalmazásra.

- Az Active Directory nyomtatófelderítése nem fog működni. Közvetlen nyomtatóútvonalakat biztosíthat az összes felhasználó számára, vagy használhatja a [Hibrid felhőnyomtatást.](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy)

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
description: Megtudhatja, hogy miként férhet hozzá a helyszíni erőforrásokhoz, például az üzleti alkalmazásokhoz, a fájlmegosztásokhoz és a nyomtatókhoz egy Azure Active Directoryhoz csatlakozó Windows 10-eszközről.
ms.openlocfilehash: 9615ecc9469992d3e5a7479f4799c610db11fb41
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471251"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Helyszíni erőforrások elérése Azure AD-hez csatlakozott eszközről a Microsoft 365 Business Premium szolgáltatásban

Ez a cikk a Microsoft 365 Business Premium szolgáltatásra vonatkozik.

Minden Olyan Windows 10-eszköz, amelyhez az Azure Active Directory csatlakozott, hozzáfér az összes felhőalapú erőforráshoz, például a Microsoft 365-alkalmazásokhoz, és a Microsoft 365 Business Premium által védett. A helyszíni erőforrásokhoz, például üzletági (LOB)-alkalmazásokhoz, fájlmegosztásokhoz és nyomtatókhoz való hozzáférést is engedélyezheti. A hozzáférés engedélyezéséhez az [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) segítségével szinkronizálja a helyszíni Active Directoryt az Azure Active Directoryval. 

További információ: [Bevezetés az eszközkezelésbe az Azure Active Directoryban című témakörben.](https://docs.microsoft.com/azure/active-directory/device-management-introduction)
A lépéseket a következő szakaszok is összefoglalják.

> [!IMPORTANT]
> Ez az eljárás csak az OAuth és az NTLM vonatkozik. A Kerberos nem támogatott.
 
## <a name="run-azure-ad-connect"></a>Az Azure AD Connect futtatása

Hajtsa végre az alábbi lépéseket, hogy a szervezet Azure AD-hez csatlakozott eszközök a helyszíni erőforrások eléréséhez.
  
1. Ha a felhasználókat, csoportokat és névjegyeket a helyi Active Directoryból az Azure Active Directoryba szeretné szinkronizálni, futtassa a Címtár-szinkronizálás varázslót és az Azure AD Connectet az [Office 365 címtár-szinkronizálásának beállítása](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization)című részében leírtak szerint.
    
2. A címtár-szinkronizálás befejezése után győződjön meg arról, hogy a szervezet Windows 10-es eszközei azure AD-hez csatlakoznak. Ez a lépés minden Windows 10-es eszközön külön-külön történik. A részleteket a [Windows-eszközök beállítása Microsoft 365 Business Premium-felhasználók számára.](set-up-windows-devices.md) 
    
3. Miután a Windows 10-es eszközök csatlakozott az Azure AD-hez, minden felhasználónak újra kell indítania az eszközeit, és be kell jelentkeznie a Microsoft 365 Business Premium hitelesítő adataival. Mostantól minden eszköz hozzáférhet a helyszíni erőforrásokhoz is.
    
Nincs szükség további lépésekre az Azure AD-hez csatlakozó eszközök helyszíni erőforrásaihoz való hozzáféréshez. Ez a funkció be van építve a Windows 10-be. 

Ha azt tervezi, hogy jelentkezzen be az AADJ eszköz más, mint a jelszó módszer, mint a PIN/Bio-metric keresztül WHFB hitelesítő adatok bejelentkezés, majd a hozzáférést a helyszíni erőforrások (részvények, nyomtatók.. stb), kérjük, kövessehttps://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Ha a szervezet nem áll készen a fent leírt Azure AD-hez csatlakozott eszközkonfigurációban való üzembe helyezésre, fontolja meg [a hibrid Azure AD-hez csatlakozott eszköz konfigurációjának beállítását.](manage-windows-devices.md)
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>A Windows-eszközök Azure AD-hez való csatlakozásával kapcsolatos szempontok

Ha az Azure-AD által csatlakozott Windows-eszköz korábban tartományhoz volt csatlakoztatva vagy munkacsoportban volt, vegye figyelembe a következő korlátozásokat:
  
- Amikor egy eszköz höz csatlakozik az Azure AD, új felhasználót hoz létre anélkül, hogy egy meglévő profilra hivatkozna. A profilokat manuálisan kell áttelepíteni. A felhasználói profilok olyan információkat tartalmaznak, mint a kedvencek, a helyi fájlok, a böngésző beállításai és a Start menü beállításai. A legjobb megközelítés az, hogy talál egy harmadik féltől származó eszköz leképezése a meglévő fájlokat és beállításokat az új profilt.

- Ha az eszköz csoportházirend-objektumokat (GPO) használ, előfordulhat, hogy egyes csoportházirend-objektumok nem rendelkeznek hasonló [konfigurációs szolgáltatóval](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) az Intune-ban. Futtassa az [MMAT eszközt](https://www.microsoft.com/download/details.aspx?id=45520) a meglévő csoportházirend-szolgáltatók hoz hasonló kriptámok megkereséséhez.

- A felhasználók nem tudják hitelesíteni az Active Directory hitelesítésétől függő alkalmazásokat. Értékelje ki az örökölt alkalmazást, és ha lehetséges, fontolja meg a modern hitelesítést használó alkalmazásra való frissítést.

- Az Active Directory nyomtatófelderítésnem fog működni. Közvetlen nyomtatóelérési utakat adhat meg minden felhasználónak, vagy használhatja a [Hybrid Cloud Print szolgáltatást.](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy)

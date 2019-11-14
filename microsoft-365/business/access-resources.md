---
title: Az intézményi erőforrásokhoz való hozzáférés egy Azure alapú AD-illesztett eszközről a Microsoft 365 Business
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
description: Tájékoztatás arról, hogyan lehet hozzáférni az intézményi erőforrásokhoz, például az üzleti alkalmazások, a fájlmegosztások és a nyomtatók eléréséhez egy Azure Active Directory-hoz csatlakozott a Windows 10 eszközhöz.
ms.openlocfilehash: fdc1eca6913ba6af4f6b65691fdee2165e7c827e
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/14/2019
ms.locfileid: "38323395"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>Az intézményi erőforrásokhoz való hozzáférés egy Azure alapú AD-illesztett eszközről a Microsoft 365 Business

Minden olyan Windows 10 eszköz, amely Azure Active Directory-hoz csatlakozott, hozzáfér minden felhőalapú erőforráshoz, például az Office 365 alkalmazásokhoz, és a Microsoft 365 Business védhető. Az intézményi erőforrásokhoz, például az ÜZLETÁGI alkalmazásokhoz, a fájlmegosztásokhoz és a nyomtatókhoz is hozzáférést engedélyezhet. A hozzáférés engedélyezéséhez az [Azure ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) használatával szinkronizálhatja a helyi Active Directoryt az Azure Active Directoryval. 

További információ: [Bevezetés az eszközkezelésben az Azure Active Directory szolgáltatásban](https://docs.microsoft.com/azure/active-directory/device-management-introduction).
A lépéseket a következő szakaszokban is összefoglaltuk.

## <a name="run-azure-ad-connect"></a>Fuss Azure AD Connect

Hajtsa végre az alábbi lépéseket annak engedélyezéséhez, hogy a szervezet Azure AD csatlakozott eszközei hozzáférhessenek az intézményi erőforrásokhoz.
  
1. A felhasználók, csoportok és kapcsolattartók helyi Active Directoryból a Azure Active Directoryba való szinkronizálásához futtassa a címtár-szinkronizálás varázslót és a Azure AD Connect szolgáltatást az [Office 365 címtár-szinkronizálás beállítása](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)című témakörben leírtak szerint.
    
2. A címtár-szinkronizálás befejeződését követően győződjön meg arról, hogy a szervezet Windows 10-eszközei csatlakoztak az Azure Active Directoryhoz. Ez a lépés egyenként történik minden Windows 10 eszközön. További részleteket a [Windows-eszközök beállítása a Microsoft 365 üzleti felhasználóknak](set-up-windows-devices.md) című témakörben találhat. 
    
3. Miután a Windows 10 eszközöket a Azure AD csatlakozott, mindegyik felhasználónak újra kell indítania az eszközöket, és be kell jelentkeznie a Microsoft 365 Business hitelesítő adataival. Mostantól minden eszköz hozzáfér az intézményi erőforrásokhoz is.
    
A Azure Active Directory-eszközök intézményi erőforrásainak eléréséhez nincs szükség további lépésekre. Ez a funkció a Windows 10-be van beépítve. 
  
Ha a szervezet nem áll készen a fent leírt Azure Active Directory egyesített eszközkonfigurációban történő telepítésére, érdemes a [hibrid Azure ad egyesített eszközkonfigurációt](manage-windows-devices.md)beállítani.
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Megfontolások a Windows-eszközök Azure AD-hez való csatlakozásakor

Ha az Azure-AD csatlakozott Windows-eszköz korábban tartományhoz vagy munkacsoporthoz csatlakozott, vegye figyelembe az alábbi korlátozásokat:
  
- Amikor egy eszköz Azure AD csatlakozik, új felhasználót hoz létre anélkül, hogy hivatkoznia kellene egy meglévő profilra. A profilokat kézzel kell áttelepíteni. A felhasználói profil olyan információkat tartalmaz, mint a Kedvencek, a helyi fájlok, a böngésző beállításai és a Start menü beállításai. A legjobb megoldás az, ha egy külső gyártótól származó eszközt talál a meglévő fájloknak és beállításoknak az új profilba való leképezéshez.

- Ha az eszköz csoportházirend-objektumokat (GPO) használ, előfordulhat, hogy egyes csoportházirend-objektumok nem rendelkeznek hasonló konfigurációs szolgáltatóval (CSP) az Intune [szolgáltatásban](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) . Futtassa a [Mmat eszközt](https://www.microsoft.com/download/details.aspx?id=45520) a meglévő csoportházirend-objektumok összehasonlítható kriptográfiai szolgáltatók kereséséhez.

- A felhasználók nem lesznek képesek hitelesíteni az Active Directory-hitelesítésnek függő alkalmazásokat. Értékelje az örökölt alkalmazást, és ha lehetséges, fontolja meg a modern Auth-ot használó alkalmazások frissítését.

- Az Active Directory nyomtatófelderítése nem működik. Az összes felhasználó számára közvetlen nyomtatóútvonalat adhat meg, vagy a [hibrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy)programot használhatja.

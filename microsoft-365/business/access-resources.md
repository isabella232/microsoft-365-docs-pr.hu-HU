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
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Tájékoztatás arról, hogyan juthat hozzá a helyi erőforrásokhoz, például az üzleti alkalmazásokhoz, a fájlmegosztásokhoz és a nyomtatókhoz egy Azure Active Directory-hoz csatlakozott a Windows 10 eszközhöz.
ms.openlocfilehash: ab9049e78617372463b8446dc8f8bc0089d8c117
ms.sourcegitcommit: 91ff1d4339f0f043c2b43997d87d84677c79e279
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2019
ms.locfileid: "36981661"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>Az intézményi erőforrásokhoz való hozzáférés egy Azure alapú AD-illesztett eszközről a Microsoft 365 Business

Akármi Windows 10 berendezés ez minden Azure Aktivál Címtár összekapcsolt akarat volna belépés-hoz minden felhő-kiindulópontul szolgáló anyagi javak mint-a Hivatal 365 apps és lehet megvéd mellett Mikroszkóp 365 teendő. Ahhoz, hogy az intézményi erőforrásokhoz, például a Business line (LOB) alkalmazásokhoz, a fájlmegosztásokhoz és a nyomtatókhoz is hozzáférést lehessen biztosítani, az [Azure ad Connect](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect)használatával szinkronizálni kell az intézményi Active Directoryt az Azure Active Directoryval. A következő videó részletesen ismerteti, hogy hogyan lehet ezt beállítani a leggyakoribb forgatókönyvhöz.
 
> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]

További információ: [Bevezetés az eszközkezelésben az Azure Active Directory címtárban](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) .
A lépéseket a következő szakaszokban is összefoglaltuk.

## <a name="run-azure-ad-connect"></a>Fuss Azure AD Connect

Hajtsa végre az alábbi lépéseket annak engedélyezéséhez, hogy a szervezet Azure AD csatlakozott eszközei hozzáférhessenek az intézményi erőforrásokhoz.
  
1. A felhasználók, csoportok és kapcsolattartók helyi Active Directoryból Azure Active Directoryba történő szinkronizálásához futtassa a címtár-szinkronizáló varázslót és az Azure AD Connect szolgáltatást az [Office 365 címtár-szinkronizálás beállítása](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)című témakörben leírtak szerint.
    
2. A címtár-szinkronizálás befejezését követően ellenőrizze, hogy a szervezet Windows 10 eszközeivel van-e csatlakoztatva Azure AD. Ez a lépés egyenként történik minden Windows 10 eszközön. További részleteket a [Windows-eszközök beállítása a Microsoft 365 üzleti felhasználóknak](set-up-windows-devices.md) című témakörben találhat. 
    
3. Miután a Windows 10 készülékek Azure csatlakozott, minden felhasználónak kell újraindítani a készülékek és logika-val a Microsoft 365 üzleti mandátumát. Az eszközök mostantól az intézményi erőforrásokhoz is hozzáférnek.
    
A Azure Active Directory-eszközök intézményi erőforrásainak eléréséhez nincs szükség további lépésekre. Ez a Windows 10 beépített funkcionalitása. 
  
Ha a szervezet nem áll készen a fent leírt Azure Active Directory egyesített Eszközkonfigurációban történő telepítésére, fontolja meg a [hibrid Azure Adategyesített eszközkonfiguráció](manage-windows-devices.md)beállítását.
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a>Megfontolások a Windows-eszközök Azure AD-hez való csatlakozásakor

Ha egy előzőleg tartományhoz vagy munkacsoporthoz tartozó Windows-eszközhöz csatlakozna Azure alapú hirdetés, akkor az alábbi korlátozásokat kell figyelembe vennie:
  
- Amikor egy eszköz Azure AD csatlakozik, új felhasználót hoz létre anélkül, hogy hivatkoznia kellene egy meglévő profilra. A kijavításához a profilokat kézzel kell áttelepíteni. A felhasználói profil olyan információkat tartalmaz, mint a Kedvencek, a helyi fájlok, a böngésző beállításai, a Start menü beállításai, stb. A legjobb megoldás egy harmadik féltől származó eszköz megkeresése a meglévő fájloknak és beállításoknak az új profilba való leképezéshez

- Ha az eszköz csoportházirend-objektumokat (GPO) használ, előfordulhat, hogy egyes csoportházirend-objektumok nem rendelkeznek hasonló konfigurációs szolgáltatóval (CSP) az Intune [szolgáltatásban](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) . Futtassa a [Mmat eszközt](https://www.microsoft.com/download/details.aspx?id=45520) a meglévő csoportházirend-objektumok összehasonlítható kriptográfiai szolgáltatók kereséséhez.

- A felhasználók nem lesznek képesek hitelesíteni az Active Directory-hitelesítésnek függő alkalmazásokat. Foglalkozni ezzel az értékelést használ egy örökölt app, és fontolja meg frissítését egy app, amely használja a modern Auth, ha lehetséges.

- Az Active Directory nyomtatófelderítése nem fog működni. A javításához közvetlen nyomtatóelérési útvonalat adjon meg minden felhasználó számára, vagy használja a [hibrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy)programot.

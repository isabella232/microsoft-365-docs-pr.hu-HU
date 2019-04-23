---
title: Hozzáférés a helyi erőforrások egy Azure AD csatlakozott eszközről a Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
description: Útmutató helyi erőforrásokhoz való hozzáférés, mint a sorban az üzleti alkalmazások, fájlmegosztásokat és Azure Active Directoryból nyomtatókat csatlakozott Windows 10 eszköz.
ms.openlocfilehash: 212685bc229f519152e69b09d0a745bfac7a38cd
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32276881"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>Hozzáférés a helyi erőforrások egy Azure AD csatlakozott eszközről a Microsoft 365 Business

Bármely Windows 10 eszköz Azure Active Directory tartományhoz hozzáférhet az összes felhő alapú erőforrásokhoz, például az Office 365 apps és a Microsoft 365 üzleti lehet védeni. Üzleti sor (LOB) alkalmazások, fájlmegosztásokat és nyomtatók helyi erőforrások elérésének engedélyezése is, szinkronizálnia kell a helyszíni Active Directory az Azure Active Directory [Azure AD csatlakozás](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect)segítségével. Lásd [Bevezetés eszköz kezelése az Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) további. 
  
## <a name="run-azure-ad-connect"></a>Csatlakozás végrehajtása Azure AD

Kövesse az alábbi lépéseket ahhoz, hogy a szervezet csatlakozott Azure AD eszközök helyi erőforrásokhoz való hozzáférést.
  
1. A felhasználók, csoportok és a helyi Active Directory ügyfelek Active Directory Azure szinkronizálásához futtassa a címtár-szinkronizálás varázsló és Azure AD csatlakozás, a [Office 365 címtár-szinkronizálás beállítása](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
2. A címtár-szinkronizálás befejezése után ellenőrizze, hogy a szervezet Windows 10 eszközök Azure AD a tartományhoz. Ebben a lépésben a Windows 10 eszközök külön-külön történik. Részletekért lásd a [Microsoft 365 üzleti felhasználók számára a Windows-eszközök beállítása](set-up-windows-devices.md) . 
    
3. Miután a Windows 10 eszközök csatlakoztatva Azure AD, minden felhasználó eszköz és a bejelentkezés hitelesítő adataikat a Microsoft 365 üzleti kell indítsa újra. Minden eszköz már rendelkezik, valamint a helyi erőforrásokhoz való hozzáférést.
    
További lépések nem szükségesek a helyi erőforrások az Azure Active Directory tartományhoz eszközök elérésére. Ez a rendelkezésre álló Windows 10 beépített szolgáltatása. 
  
Ha a szervezet nem telepíthető az Azure AD csatlakozott a következő eszközkonfiguráció a fent leírt, fontolja meg a [hibrid Azure AD Joined eszköz konfigurációs](manage-windows-devices.md)beállítását.
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a>Eszközök a Windows Azure AD összekapcsolásakor szempontok

Ha egy Windows-eszköz, amely előzőleg a tartományhoz való csatlakozás Azure AD vagy munkacsoportban kell vegye figyelembe a következő korlátozásokat:
  
- Ha Azure AD az eszköz csatlakozik, nem hivatkozik egy létező profilt hoz új felhasználó. A javításhoz profilokat kell manuálisan kell áttelepíteni. A felhasználói profil tartalmaz információkat, például a Kedvencek, helyi fájlok, a böngésző beállításait, Start menü Beállítások, stb. A legjobb megközelítés, hogy megtalálja a meglévő fájlokat és beállításokat az új profil hozzárendelése egy külső fejlesztésű eszköz
    
- Ha az eszköz csoport csoportházirend-objektumok (GPO) használ, egyes csoportházirend-objektumok nem lehet az összehasonlítható [Konfigurációs szolgáltató](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) Intune. Futtassa a [MMAT eszközt](https://www.microsoft.com/download/details.aspx?id=45520) összehasonlítható CSP meglévő csoportházirend-objektumok kereséséhez. 
    
- A felhasználók nem tudják hitelesíteni az Active Directory hitelesítési függő alkalmazások. Ez egy régebbi alkalmazás segítségével értékeli és fontolja meg egy modern Auth lehetőleg használó alkalmazás frissítése.
    
- Az Active Directory nyomtató felderítése nem fog működni. A javításhoz közvetlen nyomtatók elérési útját adja meg az összes felhasználó számára, vagy [Hibrid felhő nyomtatási](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy)emelés.
    


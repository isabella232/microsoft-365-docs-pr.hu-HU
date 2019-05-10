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
ms.openlocfilehash: 2be8eb16b9d17547d3bc4c3e4fe499b4c14117a4
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660269"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a><span data-ttu-id="6f12a-103">Hozzáférés a helyi erőforrások egy Azure AD csatlakozott eszközről a Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="6f12a-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>

<span data-ttu-id="6f12a-104">Bármely Windows 10 eszköz Azure Active Directory tartományhoz hozzáférhet az összes felhő alapú erőforrásokhoz, például az Office 365 apps és a Microsoft 365 üzleti lehet védeni.</span><span class="sxs-lookup"><span data-stu-id="6f12a-104">Any Windows 10 device that is Azure Active Directory joined will have access to all cloud-based resources such as your Office 365 apps and can be protected by Microsoft 365 Business.</span></span> <span data-ttu-id="6f12a-105">Üzleti sor (LOB) alkalmazások, fájlmegosztásokat és nyomtatók helyi erőforrások elérésének engedélyezése is, szinkronizálnia kell a helyszíni Active Directory az Azure Active Directory [Azure AD csatlakozás](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect)segítségével.</span><span class="sxs-lookup"><span data-stu-id="6f12a-105">To also allow access to on-premises resources like Line Of Business (LOB) apps, file shares, and printers, you must synchronize your on-premises Active Directory with Azure Active Directory by using [Azure AD Connect](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect).</span></span> <span data-ttu-id="6f12a-106">Lásd [Bevezetés eszköz kezelése az Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) további.</span><span class="sxs-lookup"><span data-stu-id="6f12a-106">See [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) to learn more.</span></span> 
  
## <a name="run-azure-ad-connect"></a><span data-ttu-id="6f12a-107">Csatlakozás végrehajtása Azure AD</span><span class="sxs-lookup"><span data-stu-id="6f12a-107">Run Azure AD Connect</span></span>

<span data-ttu-id="6f12a-108">Kövesse az alábbi lépéseket ahhoz, hogy a szervezet csatlakozott Azure AD eszközök helyi erőforrásokhoz való hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="6f12a-108">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="6f12a-109">A felhasználók, csoportok és a helyi Active Directory ügyfelek Active Directory Azure szinkronizálásához futtassa a címtár-szinkronizálás varázsló és Azure AD csatlakozás, a [Office 365 címtár-szinkronizálás beállítása](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="6f12a-109">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
2. <span data-ttu-id="6f12a-110">A címtár-szinkronizálás befejezése után ellenőrizze, hogy a szervezet Windows 10 eszközök Azure AD a tartományhoz.</span><span class="sxs-lookup"><span data-stu-id="6f12a-110">After the directory synchronization has completed, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="6f12a-111">Ebben a lépésben a Windows 10 eszközök külön-külön történik.</span><span class="sxs-lookup"><span data-stu-id="6f12a-111">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="6f12a-112">Részletekért lásd a [Microsoft 365 üzleti felhasználók számára a Windows-eszközök beállítása](set-up-windows-devices.md) .</span><span class="sxs-lookup"><span data-stu-id="6f12a-112">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="6f12a-113">Miután a Windows 10 eszközök csatlakoztatva Azure AD, minden felhasználó eszköz és a bejelentkezés hitelesítő adataikat a Microsoft 365 üzleti kell indítsa újra.</span><span class="sxs-lookup"><span data-stu-id="6f12a-113">Once the Windows 10 devices are Azure AD joined, each user should reboot their devices and login with their Microsoft 365 Business credentials.</span></span> <span data-ttu-id="6f12a-114">Minden eszköz már rendelkezik, valamint a helyi erőforrásokhoz való hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="6f12a-114">All devices will now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="6f12a-115">További lépések nem szükségesek a helyi erőforrások az Azure Active Directory tartományhoz eszközök elérésére.</span><span class="sxs-lookup"><span data-stu-id="6f12a-115">No additional steps are required to get access to on-premise resources for Azure AD joined devices.</span></span> <span data-ttu-id="6f12a-116">Ez a rendelkezésre álló Windows 10 beépített szolgáltatása.</span><span class="sxs-lookup"><span data-stu-id="6f12a-116">This is built-in functionality available in Windows 10.</span></span> 
  
<span data-ttu-id="6f12a-117">Ha a szervezet nem telepíthető az Azure AD csatlakozott a következő eszközkonfiguráció a fent leírt, fontolja meg a [hibrid Azure AD Joined eszköz konfigurációs](manage-windows-devices.md)beállítását.</span><span class="sxs-lookup"><span data-stu-id="6f12a-117">If your organization is not ready to deploy in the Azure AD Joined Device Configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a><span data-ttu-id="6f12a-118">Eszközök a Windows Azure AD összekapcsolásakor szempontok</span><span class="sxs-lookup"><span data-stu-id="6f12a-118">Considerations when joining your Windows devices to Azure AD</span></span>

<span data-ttu-id="6f12a-119">Ha egy Windows-eszköz, amely előzőleg a tartományhoz való csatlakozás Azure AD vagy munkacsoportban kell vegye figyelembe a következő korlátozásokat:</span><span class="sxs-lookup"><span data-stu-id="6f12a-119">If you are Azure AD joining a Windows device that has previously been domain-joined or in a workgroup, you need to consider the following limitations:</span></span>
  
- <span data-ttu-id="6f12a-120">Ha Azure AD az eszköz csatlakozik, nem hivatkozik egy létező profilt hoz új felhasználó.</span><span class="sxs-lookup"><span data-stu-id="6f12a-120">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="6f12a-121">A javításhoz profilokat kell manuálisan kell áttelepíteni.</span><span class="sxs-lookup"><span data-stu-id="6f12a-121">To fix this, profiles need to be manually migrated.</span></span> <span data-ttu-id="6f12a-122">A felhasználói profil tartalmaz információkat, például a Kedvencek, helyi fájlok, a böngésző beállításait, Start menü Beállítások, stb. A legjobb megközelítés, hogy megtalálja a meglévő fájlokat és beállításokat az új profil hozzárendelése egy külső fejlesztésű eszköz</span><span class="sxs-lookup"><span data-stu-id="6f12a-122">A user profile contains information like favorites, local files, browser settings, Start menu settings, etc. A best approach is to find a third-party tool to map existing files and settings to the new profile</span></span>

- <span data-ttu-id="6f12a-123">Ha az eszköz csoport csoportházirend-objektumok (GPO) használ, egyes csoportházirend-objektumok nem lehet az összehasonlítható [Konfigurációs szolgáltató](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) Intune.</span><span class="sxs-lookup"><span data-stu-id="6f12a-123">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="6f12a-124">Futtassa a [MMAT eszközt](https://www.microsoft.com/download/details.aspx?id=45520) összehasonlítható CSP meglévő csoportházirend-objektumok kereséséhez.</span><span class="sxs-lookup"><span data-stu-id="6f12a-124">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="6f12a-125">A felhasználók nem tudják hitelesíteni az Active Directory hitelesítési függő alkalmazások.</span><span class="sxs-lookup"><span data-stu-id="6f12a-125">Users will not be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="6f12a-126">Ez egy régebbi alkalmazás segítségével értékeli és fontolja meg egy modern Auth lehetőleg használó alkalmazás frissítése.</span><span class="sxs-lookup"><span data-stu-id="6f12a-126">To deal with this evaluate using a legacy app and consider updating to an app that uses modern Auth if possible.</span></span>

- <span data-ttu-id="6f12a-127">Az Active Directory nyomtató felderítése nem fog működni.</span><span class="sxs-lookup"><span data-stu-id="6f12a-127">Active Directory printer discovery will not work.</span></span> <span data-ttu-id="6f12a-128">A javításhoz közvetlen nyomtatók elérési útját adja meg az összes felhasználó számára, vagy [Hibrid felhő nyomtatási](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy)emelés.</span><span class="sxs-lookup"><span data-stu-id="6f12a-128">To fix this, provide direct printer paths for all users or leverage [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>

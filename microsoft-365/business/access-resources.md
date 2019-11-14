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
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a><span data-ttu-id="a7f1e-103">Az intézményi erőforrásokhoz való hozzáférés egy Azure alapú AD-illesztett eszközről a Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="a7f1e-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>

<span data-ttu-id="a7f1e-104">Minden olyan Windows 10 eszköz, amely Azure Active Directory-hoz csatlakozott, hozzáfér minden felhőalapú erőforráshoz, például az Office 365 alkalmazásokhoz, és a Microsoft 365 Business védhető.</span><span class="sxs-lookup"><span data-stu-id="a7f1e-104">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Office 365 apps, and can be protected by Microsoft 365 Business.</span></span> <span data-ttu-id="a7f1e-105">Az intézményi erőforrásokhoz, például az ÜZLETÁGI alkalmazásokhoz, a fájlmegosztásokhoz és a nyomtatókhoz is hozzáférést engedélyezhet.</span><span class="sxs-lookup"><span data-stu-id="a7f1e-105">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="a7f1e-106">A hozzáférés engedélyezéséhez az [Azure ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) használatával szinkronizálhatja a helyi Active Directoryt az Azure Active Directoryval.</span><span class="sxs-lookup"><span data-stu-id="a7f1e-106">To allow access, use [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span> 

<span data-ttu-id="a7f1e-107">További információ: [Bevezetés az eszközkezelésben az Azure Active Directory szolgáltatásban](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span><span class="sxs-lookup"><span data-stu-id="a7f1e-107">To learn more, see [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="a7f1e-108">A lépéseket a következő szakaszokban is összefoglaltuk.</span><span class="sxs-lookup"><span data-stu-id="a7f1e-108">The steps are also summarized in the following sections.</span></span>

## <a name="run-azure-ad-connect"></a><span data-ttu-id="a7f1e-109">Fuss Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="a7f1e-109">Run Azure AD Connect</span></span>

<span data-ttu-id="a7f1e-110">Hajtsa végre az alábbi lépéseket annak engedélyezéséhez, hogy a szervezet Azure AD csatlakozott eszközei hozzáférhessenek az intézményi erőforrásokhoz.</span><span class="sxs-lookup"><span data-stu-id="a7f1e-110">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="a7f1e-111">A felhasználók, csoportok és kapcsolattartók helyi Active Directoryból a Azure Active Directoryba való szinkronizálásához futtassa a címtár-szinkronizálás varázslót és a Azure AD Connect szolgáltatást az [Office 365 címtár-szinkronizálás beállítása](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)című témakörben leírtak szerint.</span><span class="sxs-lookup"><span data-stu-id="a7f1e-111">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
2. <span data-ttu-id="a7f1e-112">A címtár-szinkronizálás befejeződését követően győződjön meg arról, hogy a szervezet Windows 10-eszközei csatlakoztak az Azure Active Directoryhoz.</span><span class="sxs-lookup"><span data-stu-id="a7f1e-112">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="a7f1e-113">Ez a lépés egyenként történik minden Windows 10 eszközön.</span><span class="sxs-lookup"><span data-stu-id="a7f1e-113">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="a7f1e-114">További részleteket a [Windows-eszközök beállítása a Microsoft 365 üzleti felhasználóknak](set-up-windows-devices.md) című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="a7f1e-114">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="a7f1e-115">Miután a Windows 10 eszközöket a Azure AD csatlakozott, mindegyik felhasználónak újra kell indítania az eszközöket, és be kell jelentkeznie a Microsoft 365 Business hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="a7f1e-115">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business credentials.</span></span> <span data-ttu-id="a7f1e-116">Mostantól minden eszköz hozzáfér az intézményi erőforrásokhoz is.</span><span class="sxs-lookup"><span data-stu-id="a7f1e-116">All devices now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="a7f1e-117">A Azure Active Directory-eszközök intézményi erőforrásainak eléréséhez nincs szükség további lépésekre.</span><span class="sxs-lookup"><span data-stu-id="a7f1e-117">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="a7f1e-118">Ez a funkció a Windows 10-be van beépítve.</span><span class="sxs-lookup"><span data-stu-id="a7f1e-118">This functionality is built into Windows 10.</span></span> 
  
<span data-ttu-id="a7f1e-119">Ha a szervezet nem áll készen a fent leírt Azure Active Directory egyesített eszközkonfigurációban történő telepítésére, érdemes a [hibrid Azure ad egyesített eszközkonfigurációt](manage-windows-devices.md)beállítani.</span><span class="sxs-lookup"><span data-stu-id="a7f1e-119">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="a7f1e-120">Megfontolások a Windows-eszközök Azure AD-hez való csatlakozásakor</span><span class="sxs-lookup"><span data-stu-id="a7f1e-120">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="a7f1e-121">Ha az Azure-AD csatlakozott Windows-eszköz korábban tartományhoz vagy munkacsoporthoz csatlakozott, vegye figyelembe az alábbi korlátozásokat:</span><span class="sxs-lookup"><span data-stu-id="a7f1e-121">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>
  
- <span data-ttu-id="a7f1e-122">Amikor egy eszköz Azure AD csatlakozik, új felhasználót hoz létre anélkül, hogy hivatkoznia kellene egy meglévő profilra.</span><span class="sxs-lookup"><span data-stu-id="a7f1e-122">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="a7f1e-123">A profilokat kézzel kell áttelepíteni.</span><span class="sxs-lookup"><span data-stu-id="a7f1e-123">Profiles must be manually migrated.</span></span> <span data-ttu-id="a7f1e-124">A felhasználói profil olyan információkat tartalmaz, mint a Kedvencek, a helyi fájlok, a böngésző beállításai és a Start menü beállításai.</span><span class="sxs-lookup"><span data-stu-id="a7f1e-124">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="a7f1e-125">A legjobb megoldás az, ha egy külső gyártótól származó eszközt talál a meglévő fájloknak és beállításoknak az új profilba való leképezéshez.</span><span class="sxs-lookup"><span data-stu-id="a7f1e-125">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="a7f1e-126">Ha az eszköz csoportházirend-objektumokat (GPO) használ, előfordulhat, hogy egyes csoportházirend-objektumok nem rendelkeznek hasonló konfigurációs szolgáltatóval (CSP) az Intune [szolgáltatásban](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) .</span><span class="sxs-lookup"><span data-stu-id="a7f1e-126">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="a7f1e-127">Futtassa a [Mmat eszközt](https://www.microsoft.com/download/details.aspx?id=45520) a meglévő csoportházirend-objektumok összehasonlítható kriptográfiai szolgáltatók kereséséhez.</span><span class="sxs-lookup"><span data-stu-id="a7f1e-127">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="a7f1e-128">A felhasználók nem lesznek képesek hitelesíteni az Active Directory-hitelesítésnek függő alkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="a7f1e-128">Users won't be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="a7f1e-129">Értékelje az örökölt alkalmazást, és ha lehetséges, fontolja meg a modern Auth-ot használó alkalmazások frissítését.</span><span class="sxs-lookup"><span data-stu-id="a7f1e-129">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="a7f1e-130">Az Active Directory nyomtatófelderítése nem működik.</span><span class="sxs-lookup"><span data-stu-id="a7f1e-130">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="a7f1e-131">Az összes felhasználó számára közvetlen nyomtatóútvonalat adhat meg, vagy a [hibrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy)programot használhatja.</span><span class="sxs-lookup"><span data-stu-id="a7f1e-131">You can provide direct printer paths for all users or use [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>

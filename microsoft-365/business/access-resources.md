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
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a><span data-ttu-id="854fa-103">Helyszíni erőforrások elérése Azure AD-hez csatlakozó eszközről a Microsoft 365 Vállalati verzióban</span><span class="sxs-lookup"><span data-stu-id="854fa-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>

<span data-ttu-id="854fa-104">Minden Olyan Windows 10-es eszköz, amely hez csatlakozott az Azure Active Directory, minden felhőalapú erőforráshoz, például az Office 365-alkalmazásokhoz hozzáfér, és a Microsoft 365 Vállalati verzió is védheti őket.</span><span class="sxs-lookup"><span data-stu-id="854fa-104">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Office 365 apps, and can be protected by Microsoft 365 Business.</span></span> <span data-ttu-id="854fa-105">Engedélyezheti a helyszíni erőforrások, például üzletági alkalmazások, fájlmegosztások és nyomtatók elérését is.</span><span class="sxs-lookup"><span data-stu-id="854fa-105">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="854fa-106">A hozzáférés engedélyezéséhez az [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) segítségével szinkronizálhatja a helyszíni Active Directoryt az Azure Active Directoryval.</span><span class="sxs-lookup"><span data-stu-id="854fa-106">To allow access, use [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span> 

<span data-ttu-id="854fa-107">További információ: [Bevezetés az Eszközkezelés bemutatkozása az Azure Active Directoryban című témakörben.](https://docs.microsoft.com/azure/active-directory/device-management-introduction)</span><span class="sxs-lookup"><span data-stu-id="854fa-107">To learn more, see [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="854fa-108">A lépések a következő szakaszokban is összefoglalva.</span><span class="sxs-lookup"><span data-stu-id="854fa-108">The steps are also summarized in the following sections.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="854fa-109">Ez az eljárás csak az OAuth-ra és az NTLM-re vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="854fa-109">This procedure is only applicable to OAuth and NTLM.</span></span> <span data-ttu-id="854fa-110">A Kerberos nem támogatott.</span><span class="sxs-lookup"><span data-stu-id="854fa-110">Kerberos is not supported.</span></span>
 
## <a name="run-azure-ad-connect"></a><span data-ttu-id="854fa-111">Az Azure AD Connect futtatása</span><span class="sxs-lookup"><span data-stu-id="854fa-111">Run Azure AD Connect</span></span>

<span data-ttu-id="854fa-112">Hajtsa végre az alábbi lépéseket, hogy a szervezet Azure AD-csatlakozású eszközök a helyszíni erőforrások eléréséhez.</span><span class="sxs-lookup"><span data-stu-id="854fa-112">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="854fa-113">A helyi Active Directoryból származó felhasználók, csoportok és névjegyek szinkronizálásához futtassa a Címtár-szinkronizálás varázslót és az Azure AD Connectet az [Office 365 címtár-szinkronizálásának beállítása](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)című részben leírtak szerint.</span><span class="sxs-lookup"><span data-stu-id="854fa-113">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
2. <span data-ttu-id="854fa-114">A címtár-szinkronizálás befejezése után győződjön meg arról, hogy a szervezet Windows 10-es eszközei azure-ad-csatlakozással vannak elválasztva.</span><span class="sxs-lookup"><span data-stu-id="854fa-114">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="854fa-115">Ez a lépés minden Windows 10-es eszközön külön-külön történik.</span><span class="sxs-lookup"><span data-stu-id="854fa-115">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="854fa-116">A részletekért olvassa el [a Windows-eszközök beállítása a Microsoft 365 Vállalati verzió felhasználóiszámára.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="854fa-116">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="854fa-117">Miután a Windows 10-es eszközök Azure AD-csatlakozása, minden felhasználónak újra kell indítania az eszközeit, és be kell jelentkeznie a Microsoft 365 Vállalati verzió hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="854fa-117">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business credentials.</span></span> <span data-ttu-id="854fa-118">Mostantól minden eszköz hozzáférhet a helyszíni erőforrásokhoz is.</span><span class="sxs-lookup"><span data-stu-id="854fa-118">All devices now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="854fa-119">Nincs szükség további lépésekre az Azure AD-hez csatlakozott eszközök helyszíni erőforrásaihoz való hozzáféréshez.</span><span class="sxs-lookup"><span data-stu-id="854fa-119">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="854fa-120">Ez a funkció be van építve a Windows 10-be.</span><span class="sxs-lookup"><span data-stu-id="854fa-120">This functionality is built into Windows 10.</span></span> 

<span data-ttu-id="854fa-121">Ha azt tervezi, hogy jelentkezzen be az AADJ eszköz más jelszó módszer, mint a PIN /Bio-metrikus WHFB hitelesítő bejelentkezés, majd a hozzáférést a helyszíni erőforrások (részvények, nyomtatók.. stb), kérjük, kövessehttps://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span><span class="sxs-lookup"><span data-stu-id="854fa-121">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares,printers..etc), please follow https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span></span>
  
<span data-ttu-id="854fa-122">Ha a szervezet nem áll készen a fent leírt Azure AD-csatlakozású eszközkonfigurációban való üzembe helyezésre, fontolja meg [a hibrid Azure AD-csatlakozású eszköz konfigurációjának](manage-windows-devices.md)beállítását.</span><span class="sxs-lookup"><span data-stu-id="854fa-122">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="854fa-123">A Windows-eszközök Azure AD-höz való csatlakozásának szempontjai</span><span class="sxs-lookup"><span data-stu-id="854fa-123">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="854fa-124">Ha az Azure-AD-hez csatlakozott Windows-eszköz korábban tartományhoz csatlakozott vagy munkacsoportban volt, vegye figyelembe az alábbi korlátozásokat:</span><span class="sxs-lookup"><span data-stu-id="854fa-124">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>
  
- <span data-ttu-id="854fa-125">Amikor egy eszköz Az Azure AD csatlakozik, létrehoz egy új felhasználót anélkül, hogy egy meglévő profilra hivatkozna.</span><span class="sxs-lookup"><span data-stu-id="854fa-125">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="854fa-126">A profilokat manuálisan kell áttelepíteni.</span><span class="sxs-lookup"><span data-stu-id="854fa-126">Profiles must be manually migrated.</span></span> <span data-ttu-id="854fa-127">A felhasználói profil olyan információkat tartalmaz, mint a kedvencek, a helyi fájlok, a böngésző beállításai és a Start menü beállításai.</span><span class="sxs-lookup"><span data-stu-id="854fa-127">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="854fa-128">A legjobb megközelítés az, hogy talál egy harmadik féltől származó eszköz, hogy feltérképezze a meglévő fájlokat és beállításokat az új profilt.</span><span class="sxs-lookup"><span data-stu-id="854fa-128">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="854fa-129">Ha az eszköz csoportházirend-objektumokat (GPO) használ, előfordulhat, hogy egyes csoportházirend-objektumok nem rendelkeznek hasonló [konfigurációs szolgáltatóval](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) az Intune-ban.</span><span class="sxs-lookup"><span data-stu-id="854fa-129">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="854fa-130">Futtassa az [MMAT eszközt,](https://www.microsoft.com/download/details.aspx?id=45520) hogy összehasonlítható csoportházirend-szolgáltatókat keressen a meglévő csoportházirend-szolgáltatókhoz.</span><span class="sxs-lookup"><span data-stu-id="854fa-130">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="854fa-131">A felhasználók nem tudnak hitelesíteni az Active Directory hitelesítésétől függő alkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="854fa-131">Users won't be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="854fa-132">Értékelje ki az örökölt alkalmazást, és lehetőség szerint frissítsen egy modern hitelesítést használó alkalmazásra.</span><span class="sxs-lookup"><span data-stu-id="854fa-132">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="854fa-133">Az Active Directory nyomtatófelderítése nem fog működni.</span><span class="sxs-lookup"><span data-stu-id="854fa-133">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="854fa-134">Közvetlen nyomtatóútvonalakat biztosíthat az összes felhasználó számára, vagy használhatja a [Hibrid felhőnyomtatást.](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy)</span><span class="sxs-lookup"><span data-stu-id="854fa-134">You can provide direct printer paths for all users or use [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>

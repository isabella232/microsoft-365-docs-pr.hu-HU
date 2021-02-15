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
description: Megtudhatja, hogy miként férhet hozzá helyszíni erőforrásokhoz, például üzleti alkalmazásokhoz, fájlmegosztáshoz és nyomtatókhoz egy Windows 10-es eszközhöz csatlakozott Azure Active Directory-eszközről.
ms.openlocfilehash: fc02fd30f41f25f52e653e750a6bdfd1bd7f800e
ms.sourcegitcommit: a62ac3c01ba700a51b78a647e2301f27ac437c5a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2021
ms.locfileid: "50233840"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a><span data-ttu-id="ad917-103">Helyszíni erőforrások elérése Azure AD-hez csatlakozott eszközről a Microsoft 365 Vállalati prémium verzióban</span><span class="sxs-lookup"><span data-stu-id="ad917-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium</span></span>

<span data-ttu-id="ad917-104">Ez a cikk a Microsoft 365 Vállalati prémium verzióra vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="ad917-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="ad917-105">Minden olyan Windows 10-es eszköz, amelyhez az Azure Active Directory csatlakozik, hozzáférhet az összes felhőalapú erőforráshoz, például a Microsoft 365-apphoz, és a Microsoft 365 Vállalati prémium verzió védheti.</span><span class="sxs-lookup"><span data-stu-id="ad917-105">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Microsoft 365 apps, and can be protected by Microsoft 365 Business Premium.</span></span> <span data-ttu-id="ad917-106">Engedélyezheti a hozzáférést a helyszíni erőforrásokhoz is, például üzletági alkalmazásokhoz, fájlmegosztáshoz és nyomtatókhoz.</span><span class="sxs-lookup"><span data-stu-id="ad917-106">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="ad917-107">A hozzáférés engedélyezése érdekében az [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) segítségével szinkronizálja a helyszíni Active Directoryt az Azure Active Directoryval.</span><span class="sxs-lookup"><span data-stu-id="ad917-107">To allow access, use [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span> 

<span data-ttu-id="ad917-108">További információért olvassa el az Eszközkezelés az [Azure Active Directoryban – Bevezetés.](https://docs.microsoft.com/azure/active-directory/device-management-introduction)</span><span class="sxs-lookup"><span data-stu-id="ad917-108">To learn more, see [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="ad917-109">A lépéseket az alábbi szakaszokban is összegzi.</span><span class="sxs-lookup"><span data-stu-id="ad917-109">The steps are also summarized in the following sections.</span></span>
 
## <a name="run-azure-ad-connect"></a><span data-ttu-id="ad917-110">Az Azure AD Connect futtatása</span><span class="sxs-lookup"><span data-stu-id="ad917-110">Run Azure AD Connect</span></span>

<span data-ttu-id="ad917-111">Az alábbi lépéseket követve engedélyezheti a szervezet Azure AD-hez csatlakozott eszközeinek a helyszíni erőforrásokhoz való hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="ad917-111">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="ad917-112">Ha szinkronizálni szeretné a felhasználókat, csoportokat és névjegyeket a helyi Active Directoryból az Azure Active Directoryba, futtassa a Címtár-szinkronizálási varázslót és az Azure AD Connectet az [Office 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization)címtár-szinkronizálásának beállításával.</span><span class="sxs-lookup"><span data-stu-id="ad917-112">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization).</span></span>
    
2. <span data-ttu-id="ad917-113">A címtár-szinkronizálás befejezése után győződjön meg arról, hogy szervezete Windows 10-es eszközeihez az Azure AD csatlakozik.</span><span class="sxs-lookup"><span data-stu-id="ad917-113">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="ad917-114">Ez a lépés minden Windows 10-es eszközön külön-külön történik.</span><span class="sxs-lookup"><span data-stu-id="ad917-114">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="ad917-115">További [információt a Windows-eszközök beállítása a Microsoft 365 Vállalati prémium](set-up-windows-devices.md) verzió felhasználóinak.</span><span class="sxs-lookup"><span data-stu-id="ad917-115">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="ad917-116">Miután a Windows 10-es eszközök csatlakoztak az Azure AD-hez, minden felhasználónak újra kell indítania az eszközét, és be kell jelentkeznie a Microsoft 365 Vállalati prémium verziós hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="ad917-116">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business Premium credentials.</span></span> <span data-ttu-id="ad917-117">Mostantól minden eszköz hozzáférhet a helyszíni erőforrásokhoz is.</span><span class="sxs-lookup"><span data-stu-id="ad917-117">All devices now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="ad917-118">Az Azure AD-hez csatlakozott eszközök helyszíni erőforrásaihoz való hozzáféréshez nincs szükség további lépésekre.</span><span class="sxs-lookup"><span data-stu-id="ad917-118">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="ad917-119">Ez a funkció a Windows 10 beépített szolgáltatása.</span><span class="sxs-lookup"><span data-stu-id="ad917-119">This functionality is built into Windows 10.</span></span> 

<span data-ttu-id="ad917-120">Ha a jelszótól (PÉLDÁUL PIN-kód/Metrikus stb.) kívül más AADJ-eszközre szeretne bejelentkezni a WHFB hitelesítő adatain keresztül, majd a helyi erőforrásokhoz (megosztások, nyomtatók) szeretne hozzáférni. stb.), kérjük, kövesse az https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span><span class="sxs-lookup"><span data-stu-id="ad917-120">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares,printers..etc), please follow https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span></span>
  
<span data-ttu-id="ad917-121">Ha szervezete nem áll készen a fent ismertetett Azure AD-hez való csatlakozású eszközkonfiguráció telepítésére, fontolja meg a hibrid Azure AD-hez való csatlakozású [eszközkonfiguráció beállítását.](manage-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="ad917-121">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="ad917-122">Megfontolandó szempontok, amikor Windows-eszközökhöz csatlakozik az Azure AD szolgáltatáshoz</span><span class="sxs-lookup"><span data-stu-id="ad917-122">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="ad917-123">Ha az Azure-AD szolgáltatáshoz csatlakozott Windows-eszköz korábban tartományhoz csatlakozott vagy munkacsoport tagja volt, vegye figyelembe az alábbi korlátozásokat:</span><span class="sxs-lookup"><span data-stu-id="ad917-123">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>
  
- <span data-ttu-id="ad917-124">Amikor egy eszközhez az Azure AD csatlakozik, egy új felhasználót hoz létre anélkül, hogy egy meglévő profilra hivatkozna.</span><span class="sxs-lookup"><span data-stu-id="ad917-124">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="ad917-125">A profilokat manuálisan kell áttelepíteni.</span><span class="sxs-lookup"><span data-stu-id="ad917-125">Profiles must be manually migrated.</span></span> <span data-ttu-id="ad917-126">A felhasználói profilok olyan információkat tartalmaznak, mint a kedvencek, a helyi fájlok, a böngésző beállításai és a Start menü beállításai.</span><span class="sxs-lookup"><span data-stu-id="ad917-126">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="ad917-127">A legjobb megoldás, ha egy külső gyártótól származó eszközt keres a meglévő fájlok és beállítások új profilhoz való leképezéséhez.</span><span class="sxs-lookup"><span data-stu-id="ad917-127">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="ad917-128">Ha az eszköz csoportházirend-objektumokat használ, előfordulhat, hogy egyes csoportházirend-objektumok nem tartalmaznak hasonló konfigurációs [szolgáltatót](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) az Intune-ban.</span><span class="sxs-lookup"><span data-stu-id="ad917-128">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="ad917-129">Az [MMAT eszközzel megkereshetők](https://www.microsoft.com/download/details.aspx?id=45520) a meglévő csoportházirend-objektumok hasonló CSP-ii.</span><span class="sxs-lookup"><span data-stu-id="ad917-129">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="ad917-130">Előfordulhat, hogy a felhasználók nem tudják hitelesíteni az Active Directory-hitelesítéstől függő alkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="ad917-130">Users might not be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="ad917-131">Kiértékelheti a régi appot, és lehetőség szerint frissítheti a modern Auth hitelesítést használó appra.</span><span class="sxs-lookup"><span data-stu-id="ad917-131">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="ad917-132">Az Active Directory-nyomtatók felderítése nem működik.</span><span class="sxs-lookup"><span data-stu-id="ad917-132">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="ad917-133">Minden felhasználónak meg kell adnia a nyomtató közvetlen elérési útját, vagy használhatja az [Univerzális nyomtatást.](https://aka.ms/UPDocs)</span><span class="sxs-lookup"><span data-stu-id="ad917-133">You can provide direct printer paths for all users or use [Universal Print](https://aka.ms/UPDocs).</span></span>

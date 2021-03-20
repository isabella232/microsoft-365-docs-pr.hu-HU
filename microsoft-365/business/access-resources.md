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
ms.openlocfilehash: b78509d72cbd9b3c121039c4965625bf5c21c7e0
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913522"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a><span data-ttu-id="a6abe-103">Helyszíni erőforrások elérése Azure AD-csatlakozású eszközről a Microsoft 365 Vállalati prémium verzióban</span><span class="sxs-lookup"><span data-stu-id="a6abe-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium</span></span>

<span data-ttu-id="a6abe-104">Ez a cikk a Microsoft 365 Vállalati prémium verzióra vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="a6abe-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="a6abe-105">Minden olyan Windows 10-es eszköz, amelyhez az Azure Active Directory csatlakozik, hozzáféréssel rendelkezik az összes felhőalapú erőforráshoz, például a Microsoft 365-alkalmazásokhoz, és a Microsoft 365 Business Premiumval védheti őket.</span><span class="sxs-lookup"><span data-stu-id="a6abe-105">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Microsoft 365 apps, and can be protected by Microsoft 365 Business Premium.</span></span> <span data-ttu-id="a6abe-106">A helyszíni erőforrásokhoz, például üzletági alkalmazásokhoz, fájlmegosztáshoz és nyomtatókhoz való hozzáférést is engedélyezheti.</span><span class="sxs-lookup"><span data-stu-id="a6abe-106">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="a6abe-107">A hozzáférés engedélyezése érdekében az [Azure AD Connect](/azure/active-directory/connect/active-directory-aadconnect) segítségével szinkronizálja a helyszíni Active Directoryt az Azure Active Directoryval.</span><span class="sxs-lookup"><span data-stu-id="a6abe-107">To allow access, use [Azure AD Connect](/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span> 

<span data-ttu-id="a6abe-108">További információ: Eszközkezelés az [Azure Active Directoryban –](/azure/active-directory/device-management-introduction)Bevezetés.</span><span class="sxs-lookup"><span data-stu-id="a6abe-108">To learn more, see [Introduction to device management in Azure Active Directory](/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="a6abe-109">A lépéseket az alábbi szakaszokban is összegzi.</span><span class="sxs-lookup"><span data-stu-id="a6abe-109">The steps are also summarized in the following sections.</span></span>
 
## <a name="run-azure-ad-connect"></a><span data-ttu-id="a6abe-110">Az Azure AD Connect futtatása</span><span class="sxs-lookup"><span data-stu-id="a6abe-110">Run Azure AD Connect</span></span>

<span data-ttu-id="a6abe-111">Az alábbi lépésekkel engedélyezheti szervezete Azure AD-hez csatlakozott eszközeinek a helyszíni erőforrásokhoz való hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="a6abe-111">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="a6abe-112">Ha a felhasználókat, csoportokat és névjegyeket a helyi Active Directoryból az Azure Active Directoryba szeretné szinkronizálni, futtassa a Címtár-szinkronizálási varázslót és az Azure AD Connectet az Office 365 címtár-szinkronizálásának beállítása [leírásának lépéseit használva.](../enterprise/set-up-directory-synchronization.md)</span><span class="sxs-lookup"><span data-stu-id="a6abe-112">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](../enterprise/set-up-directory-synchronization.md).</span></span>
    
2. <span data-ttu-id="a6abe-113">A címtár-szinkronizálás befejezése után győződjön meg arról, hogy a szervezet Windows 10-es eszközeihez az Azure AD csatlakozik.</span><span class="sxs-lookup"><span data-stu-id="a6abe-113">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="a6abe-114">Ez a lépés minden Windows 10-es eszközön külön-külön történik.</span><span class="sxs-lookup"><span data-stu-id="a6abe-114">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="a6abe-115">További [információt a Windows-eszközök beállítása a Microsoft 365 Vállalati prémium verzió felhasználóinak.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="a6abe-115">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="a6abe-116">Miután a Windows 10-es eszközök csatlakoztak az Azure AD-hez, minden felhasználónak újra kell indítania az eszközét, és be kell jelentkeznie a Microsoft 365 Business Premiums hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="a6abe-116">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business Premium credentials.</span></span> <span data-ttu-id="a6abe-117">Mostantól minden eszköz rendelkezik hozzáféréssel a helyszíni erőforrásokhoz is.</span><span class="sxs-lookup"><span data-stu-id="a6abe-117">All devices now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="a6abe-118">Az Azure AD-hez csatlakozott eszközök helyszíni erőforrásaihoz való hozzáféréshez nincs szükség további lépésekre.</span><span class="sxs-lookup"><span data-stu-id="a6abe-118">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="a6abe-119">Ez a funkció a Windows 10 beépített szolgáltatása.</span><span class="sxs-lookup"><span data-stu-id="a6abe-119">This functionality is built into Windows 10.</span></span> 

<span data-ttu-id="a6abe-120">Ha az AADJ-eszközre nem jelszó módszert szeretne használni (például PIN-kód/metrikus adatokat a WHFB hitelesítő adataival), majd helyi erőforrásokat (megosztásokat, nyomtatókat) szeretne használni. stb.), kövesse az https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span><span class="sxs-lookup"><span data-stu-id="a6abe-120">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares,printers..etc), please follow https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span></span>
  
<span data-ttu-id="a6abe-121">Ha szervezete nem áll készen a fent ismertetett Azure AD-hez csatlakozású eszközkonfigurációban való telepítésre, fontolja meg a hibrid [Azure AD-csatlakozású eszközkonfiguráció beállítását.](manage-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="a6abe-121">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="a6abe-122">Megfontolandó szempontok a Windows-eszközök Azure AD-hez való csatlakozásakor</span><span class="sxs-lookup"><span data-stu-id="a6abe-122">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="a6abe-123">Ha az Azure-AD-hoz csatlakozott Windows-eszköz korábban tartományhoz csatlakozott vagy munkacsoportban volt, vegye figyelembe az alábbi korlátozásokat:</span><span class="sxs-lookup"><span data-stu-id="a6abe-123">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>
  
- <span data-ttu-id="a6abe-124">Amikor egy eszköz csatlakozik az Azure AD-hez, egy új felhasználót hoz létre anélkül, hogy létező profilra hivatkozna.</span><span class="sxs-lookup"><span data-stu-id="a6abe-124">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="a6abe-125">A profilokat manuálisan kell áttelepíteni.</span><span class="sxs-lookup"><span data-stu-id="a6abe-125">Profiles must be manually migrated.</span></span> <span data-ttu-id="a6abe-126">A felhasználói profilok olyan információkat tartalmaznak, mint például a kedvencek, a helyi fájlok, a böngésző beállításai és a Start menü beállításai.</span><span class="sxs-lookup"><span data-stu-id="a6abe-126">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="a6abe-127">A legjobb megoldás, ha megkeres egy külső eszközt, amely leképezi a meglévő fájlokat és beállításokat az új profilra.</span><span class="sxs-lookup"><span data-stu-id="a6abe-127">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="a6abe-128">Ha az eszköz csoportházirend-objektumokat használ, előfordulhat, hogy egyes CSOPORTHÁZIREND-objektumok nem tartalmaznak hasonló konfigurációszolgáltatót [az](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) Intune-ban.</span><span class="sxs-lookup"><span data-stu-id="a6abe-128">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="a6abe-129">Az [MMAT eszközzel megkereshetők](https://www.microsoft.com/download/details.aspx?id=45520) a meglévő GPOS-hez használható hasonló CSP-k.</span><span class="sxs-lookup"><span data-stu-id="a6abe-129">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="a6abe-130">Előfordulhat, hogy a felhasználók nem tudják hitelesíteni az Active Directory-hitelesítéstől függő alkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="a6abe-130">Users might not be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="a6abe-131">Kiértékelheti a régi appot, és lehetőség szerint frissítheti a modern Auth hitelesítést használó appra.</span><span class="sxs-lookup"><span data-stu-id="a6abe-131">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="a6abe-132">Az Active Directory-nyomtatók felderítése nem működik.</span><span class="sxs-lookup"><span data-stu-id="a6abe-132">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="a6abe-133">Minden felhasználónak meg lehet adni közvetlen nyomtatóútját, vagy használhatja az [Univerzális nyomtatást.](/universal-print/)</span><span class="sxs-lookup"><span data-stu-id="a6abe-133">You can provide direct printer paths for all users or use [Universal Print](/universal-print/).</span></span>
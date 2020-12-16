---
title: Hozzáférés helyszíni erőforrásokhoz a Microsoft 365 Business Azure AD-csatlakoztatott eszközéről
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
description: Ebből a témakörből megtudhatja, hogy miként érheti el a helyszíni erőforrásokat, például a üzletági alkalmazások, a fájlmegosztás és a nyomtatókat egy Azure Active Directory-kapcsolattal rendelkező Windows 10-es eszközön.
ms.openlocfilehash: 22edf0c23d6318e1f70bcb21b2cd697ea0a75da4
ms.sourcegitcommit: 849b365bd3eaa9f3c3a9ef9f5973ef81af9156fa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/16/2020
ms.locfileid: "49688233"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a><span data-ttu-id="a354e-103">Hozzáférés helyszíni erőforrásokhoz a Microsoft 365 vállalati prémium verzióban elérhető Azure AD-eszközről</span><span class="sxs-lookup"><span data-stu-id="a354e-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium</span></span>

<span data-ttu-id="a354e-104">Ez a cikk a Microsoft 365 vállalati prémium verzióra vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="a354e-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="a354e-105">Bármely olyan Windows 10-es eszköz, amely az Azure Active Directoryval van csatlakoztatva, hozzáféréssel rendelkezik az összes felhőalapú erőforráshoz, például a Microsoft 365-alkalmazásaihoz, és a Microsoft 365 Business Premium által is védett.</span><span class="sxs-lookup"><span data-stu-id="a354e-105">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Microsoft 365 apps, and can be protected by Microsoft 365 Business Premium.</span></span> <span data-ttu-id="a354e-106">A helyszíni erőforrások, például a üzletági (LOB) alkalmazások, a fájlmegosztás és a nyomtatók elérését is engedélyezheti.</span><span class="sxs-lookup"><span data-stu-id="a354e-106">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="a354e-107">Az Access engedélyezéséhez az [Azure ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) segítségével szinkronizálja a helyszíni Active Directoryt az Azure Active Directoryval.</span><span class="sxs-lookup"><span data-stu-id="a354e-107">To allow access, use [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span> 

<span data-ttu-id="a354e-108">További információért olvassa el az [eszközkezelés az Azure Active Directoryban – bevezetés](https://docs.microsoft.com/azure/active-directory/device-management-introduction)című témakört.</span><span class="sxs-lookup"><span data-stu-id="a354e-108">To learn more, see [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="a354e-109">A lépéseket az alábbi szakaszokban is összegezjük.</span><span class="sxs-lookup"><span data-stu-id="a354e-109">The steps are also summarized in the following sections.</span></span>
 
## <a name="run-azure-ad-connect"></a><span data-ttu-id="a354e-110">Az Azure AD Connect futtatása</span><span class="sxs-lookup"><span data-stu-id="a354e-110">Run Azure AD Connect</span></span>

<span data-ttu-id="a354e-111">A helyszíni erőforrások eléréséhez kövesse az alábbi lépéseket, amelyek lehetővé teszik a szervezet Azure AD egyesített eszközeinek elérését.</span><span class="sxs-lookup"><span data-stu-id="a354e-111">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="a354e-112">Ha a helyi Active Directoryból szeretné szinkronizálni a felhasználókat, a csoportokat és a névjegyeket az Azure Active Directoryhoz, futtassa a címtár-szinkronizálás varázslót és az Azure AD Connect parancsot a [címtár-szinkronizálás beállítása az Office 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization)-ban című témakörben leírtak szerint.</span><span class="sxs-lookup"><span data-stu-id="a354e-112">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization).</span></span>
    
2. <span data-ttu-id="a354e-113">A címtár-szinkronizálás befejeződése után győződjön meg arról, hogy szervezete Windows 10-es eszközei az Azure AD-hoz csatlakoznak.</span><span class="sxs-lookup"><span data-stu-id="a354e-113">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="a354e-114">Ezt a lépést egyenként elvégezheti minden Windows 10-es eszközön.</span><span class="sxs-lookup"><span data-stu-id="a354e-114">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="a354e-115">Részletekért olvassa el a [Windows-eszközök beállítása a Microsoft 365 Business Premium felhasználói](set-up-windows-devices.md) számára című témakört.</span><span class="sxs-lookup"><span data-stu-id="a354e-115">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="a354e-116">Miután a Windows 10-es eszközök az Azure AD-ra csatlakoznak, minden felhasználónak újra kell indítania az eszközeit, és be kell írnia a Microsoft 365 vállalati prémium verziós hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="a354e-116">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business Premium credentials.</span></span> <span data-ttu-id="a354e-117">Minden eszközön elérhetők a helyszíni erőforrások is.</span><span class="sxs-lookup"><span data-stu-id="a354e-117">All devices now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="a354e-118">További lépésekre nincs szükség az Azure AD-hoz csatlakoztatott eszközök helyszíni erőforrásaihoz való hozzáférés megkezdéséhez.</span><span class="sxs-lookup"><span data-stu-id="a354e-118">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="a354e-119">Ez a funkció a Windows 10 rendszerbe épül.</span><span class="sxs-lookup"><span data-stu-id="a354e-119">This functionality is built into Windows 10.</span></span> 

<span data-ttu-id="a354e-120">Ha azt tervezi, hogy a AADJ-eszközre szeretne bejelentkezni, például a PIN-kód/bio-metrikus WHFB-beli hitelesítő adatokkal, jelentkezzen be, majd nyissa meg a helyszíni erőforrásokat (megosztásokat, nyomtatókat stb.). stb.), kérjük, kövesse az alábbi lépéseket https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span><span class="sxs-lookup"><span data-stu-id="a354e-120">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares,printers..etc), please follow https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span></span>
  
<span data-ttu-id="a354e-121">Ha szervezete nem hajlandó telepíteni az Azure AD csatlakoztatott eszköz konfigurációjában leírt konfigurációt, fontolja meg a [hibrid Azure ad csatlakoztatott eszköz konfigurációjának](manage-windows-devices.md)beállítását.</span><span class="sxs-lookup"><span data-stu-id="a354e-121">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="a354e-122">A Windows-eszközök Azure AD-hoz való csatlakozásának szempontjai</span><span class="sxs-lookup"><span data-stu-id="a354e-122">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="a354e-123">Ha az Azure-AD-hoz csatlakoztatott Windows-eszköz korábban tartományhoz csatlakozik vagy egy munkacsoportban van, vegye figyelembe az alábbi korlátozásokat:</span><span class="sxs-lookup"><span data-stu-id="a354e-123">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>
  
- <span data-ttu-id="a354e-124">Ha egy eszköz az Azure AD-hoz csatlakozik, egy új felhasználót hoz létre a meglévő profil hivatkozása nélkül.</span><span class="sxs-lookup"><span data-stu-id="a354e-124">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="a354e-125">A profilokat manuálisan kell áttelepíteni.</span><span class="sxs-lookup"><span data-stu-id="a354e-125">Profiles must be manually migrated.</span></span> <span data-ttu-id="a354e-126">A felhasználói profilok olyan információkat tartalmaznak, mint például a Kedvencek, a helyi fájlok, a böngésző beállításai és a Start menü beállításai.</span><span class="sxs-lookup"><span data-stu-id="a354e-126">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="a354e-127">A legjobb megoldás egy külső féltől származó eszköz megkeresése a meglévő fájlok és beállítások új profilba való megfeleltetéséhez.</span><span class="sxs-lookup"><span data-stu-id="a354e-127">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="a354e-128">Ha az eszköz csoportházirend-objektumokat (GPO) használ, előfordulhat, hogy egyes csoportházirend-objektumok nem rendelkeznek összehasonlító [konfigurációs szolgáltatóval](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) az Intune szolgáltatásban.</span><span class="sxs-lookup"><span data-stu-id="a354e-128">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="a354e-129">A [MMAT eszköz](https://www.microsoft.com/download/details.aspx?id=45520) futtatása a meglévő csoportházirend-objektumokhoz hasonló kriptográfiai szolgáltatók megkereséséhez.</span><span class="sxs-lookup"><span data-stu-id="a354e-129">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="a354e-130">A felhasználók nem tudnak hitelesíteni olyan alkalmazásokat, amelyek az Active Directory-hitelesítéstől függenek.</span><span class="sxs-lookup"><span data-stu-id="a354e-130">Users won't be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="a354e-131">Értékelje ki a régi alkalmazást, és fontolja meg, hogy egy olyan alkalmazásra frissít, amely a modern hitelesítést használja, ha lehetséges.</span><span class="sxs-lookup"><span data-stu-id="a354e-131">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="a354e-132">Az Active Directory-nyomtató felderítése nem működik.</span><span class="sxs-lookup"><span data-stu-id="a354e-132">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="a354e-133">Közvetlen nyomtatási elérési utakat is biztosíthat minden felhasználó számára, vagy [univerzális nyomtatást](https://aka.ms/UPDocs)használhat.</span><span class="sxs-lookup"><span data-stu-id="a354e-133">You can provide direct printer paths for all users or use [Universal Print](https://aka.ms/UPDocs).</span></span>

---
title: Helyszíni erőforrások elérése Azure AD-hez Microsoft 365 Vállalati verzió
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: Megtudhatja, hogy miként férhet hozzá helyszíni erőforrásokhoz, például üzletági alkalmazásokhoz, fájlmegosztáshoz és nyomtatókhoz egy Azure Active Directory-Windows 10 eszközről.
ms.openlocfilehash: 72b3c5ae538cad24fc12e25717dedccb2fdc9017
ms.sourcegitcommit: 4fb1226d5875bf5b9b29252596855a6562cea9ae
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/08/2021
ms.locfileid: "52843322"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a><span data-ttu-id="e55c2-103">Helyszíni erőforrások elérése Azure AD-hez Microsoft 365 Vállalati prémium verzió</span><span class="sxs-lookup"><span data-stu-id="e55c2-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium</span></span>

<span data-ttu-id="e55c2-104">Ez a cikk a Microsoft 365 Vállalati prémium verzió.</span><span class="sxs-lookup"><span data-stu-id="e55c2-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="e55c2-105">Minden Windows 10 eszközhöz, amely Azure Active Directory csatlakozik, hozzáféréssel rendelkezik az összes felhőalapú erőforráshoz, például a Microsoft 365-alkalmazásokhoz, és a felhasználó Microsoft 365 Vállalati prémium verzió.</span><span class="sxs-lookup"><span data-stu-id="e55c2-105">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Microsoft 365 apps, and can be protected by Microsoft 365 Business Premium.</span></span> <span data-ttu-id="e55c2-106">A helyszíni erőforrásokhoz, például üzletági alkalmazásokhoz, fájlmegosztáshoz és nyomtatókhoz való hozzáférést is engedélyezheti.</span><span class="sxs-lookup"><span data-stu-id="e55c2-106">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="e55c2-107">A hozzáférés engedélyezése érdekében az [Azure AD Csatlakozás](/azure/active-directory/connect/active-directory-aadconnect) segítségével szinkronizálja a helyszíni Active Directory-címtárát a Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e55c2-107">To allow access, use [Azure AD Connect](/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span>

<span data-ttu-id="e55c2-108">További információért olvassa el a Bevezetés az [eszközkezelésbe a Azure Active Directory.](/azure/active-directory/device-management-introduction)</span><span class="sxs-lookup"><span data-stu-id="e55c2-108">To learn more, see [Introduction to device management in Azure Active Directory](/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="e55c2-109">A lépéseket az alábbi szakaszokban is összegzi.</span><span class="sxs-lookup"><span data-stu-id="e55c2-109">The steps are also summarized in the following sections.</span></span>

## <a name="run-azure-ad-connect"></a><span data-ttu-id="e55c2-110">Az Azure AD-Csatlakozás</span><span class="sxs-lookup"><span data-stu-id="e55c2-110">Run Azure AD Connect</span></span>

<span data-ttu-id="e55c2-111">Az alábbi lépésekkel engedélyezheti szervezete Azure AD-hez csatlakozott eszközeinek a helyszíni erőforrásokhoz való hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="e55c2-111">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>

1. <span data-ttu-id="e55c2-112">Ha a felhasználókat, csoportokat és névjegyeket a helyi Active Directoryból a Azure Active Directory-ba szeretné szinkronizálni, futtassa a Címtár-szinkronizálási varázslót és az Azure AD Csatlakozás-t a Címtár-szinkronizálás beállítása [Office 365.](../enterprise/set-up-directory-synchronization.md)</span><span class="sxs-lookup"><span data-stu-id="e55c2-112">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](../enterprise/set-up-directory-synchronization.md).</span></span>

2. <span data-ttu-id="e55c2-113">Miután befejeződött a címtár-szinkronizálás, győződjön meg arról, hogy a Windows 10 az Azure AD-hez csatlakozva.</span><span class="sxs-lookup"><span data-stu-id="e55c2-113">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="e55c2-114">Ez a lépés minden egyes eszközön Windows 10 történik.</span><span class="sxs-lookup"><span data-stu-id="e55c2-114">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="e55c2-115">További [információt A Windows beállítása a Microsoft 365 Vállalati prémium verzió számára.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="e55c2-115">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for details.</span></span>

3. <span data-ttu-id="e55c2-116">Miután az Windows 10 eszköz csatlakozott az Azure AD-hez, minden felhasználónak újra kell indítania az eszközét, és be kell jelentkeznie a Microsoft 365 Vállalati prémium verzió hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="e55c2-116">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business Premium credentials.</span></span> <span data-ttu-id="e55c2-117">Mostantól minden eszköz rendelkezik hozzáféréssel a helyszíni erőforrásokhoz is.</span><span class="sxs-lookup"><span data-stu-id="e55c2-117">All devices now have access to on-premises resources as well.</span></span>

<span data-ttu-id="e55c2-118">Az Azure AD-hez csatlakozott eszközök helyszíni erőforrásaihoz való hozzáféréshez nincs szükség további lépésekre.</span><span class="sxs-lookup"><span data-stu-id="e55c2-118">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="e55c2-119">Ez a funkció a beépített Windows 10.</span><span class="sxs-lookup"><span data-stu-id="e55c2-119">This functionality is built into Windows 10.</span></span>

<span data-ttu-id="e55c2-120">Ha nem jelszó módszert szeretne használni az AADJ-eszközre, például PIN-kódot/metrikust a WHFB hitelesítő adataival, majd helyi erőforrásokat (megosztásokat, nyomtatókat stb.) szeretne használni, kérjük, kövesse ezt a [cikket.](/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)</span><span class="sxs-lookup"><span data-stu-id="e55c2-120">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares, printers, etc.), please follow [this article](/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="e55c2-121">Ha szervezete nem áll készen a fent ismertetett Azure AD-hez csatlakozású eszközkonfigurációban való telepítésre, fontolja meg a hibrid [Azure AD-csatlakozású eszközkonfiguráció beállítását.](manage-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="e55c2-121">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>

### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="e55c2-122">Megfontolandó szempontok az Windows Azure AD-hez való csatlakozáskor</span><span class="sxs-lookup"><span data-stu-id="e55c2-122">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="e55c2-123">Ha az Windows eszköz, amelyhez az Azure-AD-hez csatlakozott, korábban tartományhoz csatlakozott vagy munkacsoportban volt, vegye figyelembe az alábbi korlátozásokat:</span><span class="sxs-lookup"><span data-stu-id="e55c2-123">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>

- <span data-ttu-id="e55c2-124">Amikor egy eszköz csatlakozik az Azure AD-hez, egy új felhasználót hoz létre anélkül, hogy létező profilra hivatkozna.</span><span class="sxs-lookup"><span data-stu-id="e55c2-124">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="e55c2-125">A profilokat manuálisan kell áttelepíteni.</span><span class="sxs-lookup"><span data-stu-id="e55c2-125">Profiles must be manually migrated.</span></span> <span data-ttu-id="e55c2-126">A felhasználói profilok olyan információkat tartalmaznak, mint például a kedvencek, a helyi fájlok, a böngésző beállításai és a Start menü beállításai.</span><span class="sxs-lookup"><span data-stu-id="e55c2-126">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="e55c2-127">A legjobb megoldás, ha megkeres egy külső eszközt, amely leképezi a meglévő fájlokat és beállításokat az új profilra.</span><span class="sxs-lookup"><span data-stu-id="e55c2-127">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="e55c2-128">Ha az eszköz csoportházirend-objektumokat használ, előfordulhat, hogy egyes CSOPORTHÁZIREND-objektumok nem tartalmaznak hasonló konfigurációszolgáltatót [az](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) Intune-ban.</span><span class="sxs-lookup"><span data-stu-id="e55c2-128">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="e55c2-129">Az [MMAT eszközzel megkereshetők](https://www.microsoft.com/download/details.aspx?id=45520) a meglévő GPOS-hez használható hasonló CSP-k.</span><span class="sxs-lookup"><span data-stu-id="e55c2-129">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="e55c2-130">Előfordulhat, hogy a felhasználók nem tudják hitelesíteni az Active Directory-hitelesítéstől függő alkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="e55c2-130">Users might not be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="e55c2-131">Kiértékelheti a régi appot, és lehetőség szerint frissítheti a modern Auth hitelesítést használó appra.</span><span class="sxs-lookup"><span data-stu-id="e55c2-131">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="e55c2-132">Az Active Directory-nyomtatók felderítése nem működik.</span><span class="sxs-lookup"><span data-stu-id="e55c2-132">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="e55c2-133">Minden felhasználónak meg lehet adni közvetlen nyomtatóútját, vagy használhatja az [Univerzális nyomtatást.](/universal-print/)</span><span class="sxs-lookup"><span data-stu-id="e55c2-133">You can provide direct printer paths for all users or use [Universal Print](/universal-print/).</span></span>

### <a name="related-articles"></a><span data-ttu-id="e55c2-134">Kapcsolódó cikkek</span><span class="sxs-lookup"><span data-stu-id="e55c2-134">Related Articles</span></span>

[<span data-ttu-id="e55c2-135">Az Azure AD-szolgáltatások Csatlakozás</span><span class="sxs-lookup"><span data-stu-id="e55c2-135">Prerequisites for Azure AD Connect</span></span>](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

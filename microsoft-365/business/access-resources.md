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
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Megtudhatja, hogy miként férhet hozzá a helyszíni erőforrásokhoz, például az üzleti alkalmazásokhoz, a fájlmegosztásokhoz és a nyomtatókhoz egy Azure Active Directoryhoz csatlakozó Windows 10-eszközről.
ms.openlocfilehash: 980efbf09349cc0203ac50ae5e028c008d5694ca
ms.sourcegitcommit: 46644f9778bc70ab6d62783e0a1e60ba2eccc27f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/08/2020
ms.locfileid: "44165901"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a><span data-ttu-id="a6181-103">Helyszíni erőforrások elérése Azure AD-hez csatlakozott eszközről a Microsoft 365 Business Premium szolgáltatásban</span><span class="sxs-lookup"><span data-stu-id="a6181-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium</span></span>

<span data-ttu-id="a6181-104">Minden Olyan Windows 10-eszköz, amelyhez az Azure Active Directory csatlakozott, hozzáfér az összes felhőalapú erőforráshoz, például a Microsoft 365-alkalmazásokhoz, és a Microsoft 365 Business Premium által védett.</span><span class="sxs-lookup"><span data-stu-id="a6181-104">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Microsoft 365 apps, and can be protected by Microsoft 365 Business Premium.</span></span> <span data-ttu-id="a6181-105">A helyszíni erőforrásokhoz, például üzletági (LOB)-alkalmazásokhoz, fájlmegosztásokhoz és nyomtatókhoz való hozzáférést is engedélyezheti.</span><span class="sxs-lookup"><span data-stu-id="a6181-105">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="a6181-106">A hozzáférés engedélyezéséhez az [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) segítségével szinkronizálja a helyszíni Active Directoryt az Azure Active Directoryval.</span><span class="sxs-lookup"><span data-stu-id="a6181-106">To allow access, use [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span> 

<span data-ttu-id="a6181-107">További információ: [Bevezetés az eszközkezelésbe az Azure Active Directoryban című témakörben.](https://docs.microsoft.com/azure/active-directory/device-management-introduction)</span><span class="sxs-lookup"><span data-stu-id="a6181-107">To learn more, see [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="a6181-108">A lépéseket a következő szakaszok is összefoglalják.</span><span class="sxs-lookup"><span data-stu-id="a6181-108">The steps are also summarized in the following sections.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a6181-109">Ez az eljárás csak az OAuth és az NTLM vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="a6181-109">This procedure is only applicable to OAuth and NTLM.</span></span> <span data-ttu-id="a6181-110">A Kerberos nem támogatott.</span><span class="sxs-lookup"><span data-stu-id="a6181-110">Kerberos is not supported.</span></span>
 
## <a name="run-azure-ad-connect"></a><span data-ttu-id="a6181-111">Az Azure AD Connect futtatása</span><span class="sxs-lookup"><span data-stu-id="a6181-111">Run Azure AD Connect</span></span>

<span data-ttu-id="a6181-112">Hajtsa végre az alábbi lépéseket, hogy a szervezet Azure AD-hez csatlakozott eszközök a helyszíni erőforrások eléréséhez.</span><span class="sxs-lookup"><span data-stu-id="a6181-112">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="a6181-113">Ha a felhasználókat, csoportokat és névjegyeket a helyi Active Directoryból az Azure Active Directoryba szeretné szinkronizálni, futtassa a Címtár-szinkronizálás varázslót és az Azure AD Connectet az [Office 365 címtár-szinkronizálásának beállítása](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization)című részében leírtak szerint.</span><span class="sxs-lookup"><span data-stu-id="a6181-113">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization).</span></span>
    
2. <span data-ttu-id="a6181-114">A címtár-szinkronizálás befejezése után győződjön meg arról, hogy a szervezet Windows 10-es eszközei azure AD-hez csatlakoznak.</span><span class="sxs-lookup"><span data-stu-id="a6181-114">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="a6181-115">Ez a lépés minden Windows 10-es eszközön külön-külön történik.</span><span class="sxs-lookup"><span data-stu-id="a6181-115">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="a6181-116">A részleteket a [Windows-eszközök beállítása Microsoft 365 Business Premium-felhasználók számára.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="a6181-116">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="a6181-117">Miután a Windows 10-es eszközök csatlakozott az Azure AD-hez, minden felhasználónak újra kell indítania az eszközeit, és be kell jelentkeznie a Microsoft 365 Business Premium hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="a6181-117">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business Premium credentials.</span></span> <span data-ttu-id="a6181-118">Mostantól minden eszköz hozzáférhet a helyszíni erőforrásokhoz is.</span><span class="sxs-lookup"><span data-stu-id="a6181-118">All devices now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="a6181-119">Nincs szükség további lépésekre az Azure AD-hez csatlakozó eszközök helyszíni erőforrásaihoz való hozzáféréshez.</span><span class="sxs-lookup"><span data-stu-id="a6181-119">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="a6181-120">Ez a funkció be van építve a Windows 10-be.</span><span class="sxs-lookup"><span data-stu-id="a6181-120">This functionality is built into Windows 10.</span></span> 

<span data-ttu-id="a6181-121">Ha azt tervezi, hogy jelentkezzen be az AADJ eszköz más, mint a jelszó módszer, mint a PIN/Bio-metric keresztül WHFB hitelesítő adatok bejelentkezés, majd a hozzáférést a helyszíni erőforrások (részvények, nyomtatók.. stb), kérjük, kövessehttps://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span><span class="sxs-lookup"><span data-stu-id="a6181-121">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares,printers..etc), please follow https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base</span></span>
  
<span data-ttu-id="a6181-122">Ha a szervezet nem áll készen a fent leírt Azure AD-hez csatlakozott eszközkonfigurációban való üzembe helyezésre, fontolja meg [a hibrid Azure AD-hez csatlakozott eszköz konfigurációjának beállítását.](manage-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="a6181-122">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="a6181-123">A Windows-eszközök Azure AD-hez való csatlakozásával kapcsolatos szempontok</span><span class="sxs-lookup"><span data-stu-id="a6181-123">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="a6181-124">Ha az Azure-AD által csatlakozott Windows-eszköz korábban tartományhoz volt csatlakoztatva vagy munkacsoportban volt, vegye figyelembe a következő korlátozásokat:</span><span class="sxs-lookup"><span data-stu-id="a6181-124">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>
  
- <span data-ttu-id="a6181-125">Amikor egy eszköz höz csatlakozik az Azure AD, új felhasználót hoz létre anélkül, hogy egy meglévő profilra hivatkozna.</span><span class="sxs-lookup"><span data-stu-id="a6181-125">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="a6181-126">A profilokat manuálisan kell áttelepíteni.</span><span class="sxs-lookup"><span data-stu-id="a6181-126">Profiles must be manually migrated.</span></span> <span data-ttu-id="a6181-127">A felhasználói profilok olyan információkat tartalmaznak, mint a kedvencek, a helyi fájlok, a böngésző beállításai és a Start menü beállításai.</span><span class="sxs-lookup"><span data-stu-id="a6181-127">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="a6181-128">A legjobb megközelítés az, hogy talál egy harmadik féltől származó eszköz leképezése a meglévő fájlokat és beállításokat az új profilt.</span><span class="sxs-lookup"><span data-stu-id="a6181-128">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="a6181-129">Ha az eszköz csoportházirend-objektumokat (GPO) használ, előfordulhat, hogy egyes csoportházirend-objektumok nem rendelkeznek hasonló [konfigurációs szolgáltatóval](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) az Intune-ban.</span><span class="sxs-lookup"><span data-stu-id="a6181-129">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="a6181-130">Futtassa az [MMAT eszközt](https://www.microsoft.com/download/details.aspx?id=45520) a meglévő csoportházirend-szolgáltatók hoz hasonló kriptámok megkereséséhez.</span><span class="sxs-lookup"><span data-stu-id="a6181-130">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="a6181-131">A felhasználók nem tudják hitelesíteni az Active Directory hitelesítésétől függő alkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="a6181-131">Users won't be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="a6181-132">Értékelje ki az örökölt alkalmazást, és ha lehetséges, fontolja meg a modern hitelesítést használó alkalmazásra való frissítést.</span><span class="sxs-lookup"><span data-stu-id="a6181-132">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="a6181-133">Az Active Directory nyomtatófelderítésnem fog működni.</span><span class="sxs-lookup"><span data-stu-id="a6181-133">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="a6181-134">Közvetlen nyomtatóelérési utakat adhat meg minden felhasználónak, vagy használhatja a [Hybrid Cloud Print szolgáltatást.](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy)</span><span class="sxs-lookup"><span data-stu-id="a6181-134">You can provide direct printer paths for all users or use [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>

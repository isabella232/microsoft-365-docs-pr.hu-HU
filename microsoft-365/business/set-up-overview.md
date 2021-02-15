---
title: A beállítás áttekintése
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Ismerje meg a Microsoft 365 Vállalati prémium verzió beállítási lépéseit, az előfizetéstől, a tartományok és felhasználók hozzáadásától a biztonsági házirendek beállításán át stb.
ms.openlocfilehash: 46370166a9d5e8c9308b8947513e631c159f0b86
ms.sourcegitcommit: 815229e39a0f905d9f06717f00dc82e2a028fa7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48842130"
---
# <a name="overview-of-setup"></a><span data-ttu-id="02af5-103">A beállítás áttekintése</span><span class="sxs-lookup"><span data-stu-id="02af5-103">Overview of setup</span></span>

<span data-ttu-id="02af5-104">Nézze meg a Microsoft 365 Vállalati prémium verzió beállítását bemutató rövid videót.</span><span class="sxs-lookup"><span data-stu-id="02af5-104">Watch a short video about Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

<span data-ttu-id="02af5-105">Ha hasznosnak találta ezt a videót, tekintse meg a [teljes tanfolyamok kisvállalatoknak és Microsoft 365-újoncoknak](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) című cikket.</span><span class="sxs-lookup"><span data-stu-id="02af5-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

<span data-ttu-id="02af5-106">A beállítási lépések nagy része az irányított beállításban is el lehet végezve, de a többi beállítás is szerepel a listában.</span><span class="sxs-lookup"><span data-stu-id="02af5-106">Most of the setup steps can be done in the guided setup, but the other options are also listed.</span></span>

## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="02af5-107">1. lépés: A tartomány és a felhasználók hozzáadása</span><span class="sxs-lookup"><span data-stu-id="02af5-107">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="02af5-108">**[Tartomány hozzáadása](set-up.md#add-your-domain-to-personalize-sign-in)** (ha a regisztráció során vásárolta meg a tartományt, [](sign-up.md)ez a lépés már megtörtént.)</span><span class="sxs-lookup"><span data-stu-id="02af5-108">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

   - <span data-ttu-id="02af5-109">**Felhasználók hozzáadása**</span><span class="sxs-lookup"><span data-stu-id="02af5-109">**Add users**.</span></span> <span data-ttu-id="02af5-110">A felhasználókat a következő három módon adhat hozzá:</span><span class="sxs-lookup"><span data-stu-id="02af5-110">You can add users in any of the three ways:</span></span>
        - <span data-ttu-id="02af5-111">Az interaktív [beállításban.](set-up.md#add-users-in-the-wizard)</span><span class="sxs-lookup"><span data-stu-id="02af5-111">In the [guided setup](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="02af5-112">Ha helyszíni Active Directoryval rendelkezik, akkor címtár-szinkronizálással adhat hozzá felhasználókat az [Azure AD Connect](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) használatával.</span><span class="sxs-lookup"><span data-stu-id="02af5-112">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="02af5-113">A felügyeleti [központban később is](add-users-m365b.md) felvehet felhasználókat.</span><span class="sxs-lookup"><span data-stu-id="02af5-113">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="02af5-114">2. lépés: Biztonsági házirendek és eszközök beállítása</span><span class="sxs-lookup"><span data-stu-id="02af5-114">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="02af5-115">Az interaktív [beállítással konfigurálhatja](set-up.md#protect-your-organization) az eszköz-házirendeket.</span><span class="sxs-lookup"><span data-stu-id="02af5-115">Use the [guided setup](set-up.md#protect-your-organization) to configure device policies.</span></span> 
  - <span data-ttu-id="02af5-116">A felügyeleti központban és az [](view-policies-and-devices.md) Intune portálon is felvehet további funkciókat, illetve szerkesztheti [őket.](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)</span><span class="sxs-lookup"><span data-stu-id="02af5-116">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="02af5-117">A beállítási varázsló a veszélyforrások elleni védelem és az adatveszteség-megelőzés alapvető beállításait is be fogja állítani.</span><span class="sxs-lookup"><span data-stu-id="02af5-117">The setup wizard will also set up basic threat protection and data loss prevention settings.</span></span>
  
  <span data-ttu-id="02af5-118">A beállítási varázsló biztonsági beállításain kívül az alábbi beállítások felvételével növelheti a biztonságot:</span><span class="sxs-lookup"><span data-stu-id="02af5-118">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

- <span data-ttu-id="02af5-119">**E-mail kártevők elleni védelem**</span><span class="sxs-lookup"><span data-stu-id="02af5-119">**Email malware protection**</span></span>
- <span data-ttu-id="02af5-120">**Adathalászat elleni védelem az Office 365- ös Defenderben**</span><span class="sxs-lookup"><span data-stu-id="02af5-120">**Anti-phishing in Defender for Office 365**</span></span>
- <span data-ttu-id="02af5-121">**Exchange Online Archiválás**</span><span class="sxs-lookup"><span data-stu-id="02af5-121">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="02af5-122">**Azure Information Protection (1. csomag)**</span><span class="sxs-lookup"><span data-stu-id="02af5-122">**Azure Information Protection (Plan1**)</span></span>

<span data-ttu-id="02af5-123">Első lépések a veszélyforrások [elleni védelem](increase-threat-protection.md) növelése és a megfelelőségi [funkciók beállítása.](set-up-compliance.md)</span><span class="sxs-lookup"><span data-stu-id="02af5-123">To get started, see [increase threat protection](increase-threat-protection.md) and [set up compliance features](set-up-compliance.md).</span></span>

<span data-ttu-id="02af5-124">A [microsoftos 365 Vállalati prémium](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) verzió biztonságossá 10 legjobb módjait is bevetve útitérképet láthat az ajánlott biztonsági eljárásokról.</span><span class="sxs-lookup"><span data-stu-id="02af5-124">See also [top 10 ways to secure your Microsoft 365 Business Premium](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a road-map of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="02af5-125">3. lépés: Windows 10-es eszközök beállítása és kezelése</span><span class="sxs-lookup"><span data-stu-id="02af5-125">Step 3: Set up and manage Windows 10 devices</span></span>

<span data-ttu-id="02af5-126">Az irányított beállítás befejezése után meg kell védenie a szervezet összes Windows 10-es számítógépét.</span><span class="sxs-lookup"><span data-stu-id="02af5-126">After you complete the guided setup, you will want to protect all the Windows 10 computers in your organization.</span></span>
  
- <span data-ttu-id="02af5-127">A Windows 10 [](pre-requisites-for-data-protection.md) Pro a Microsoft 365 Vállalati prémium verzió előfeltétele, ha azonban Windows 7 Pro, Windows 8 Pro vagy Windows 8.1 Pro rendszert rendelkezik, előfizetése feljogosítja a [Windows 10 Pro frissítésre.](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update)</span><span class="sxs-lookup"><span data-stu-id="02af5-127">Windows 10 Pro is a [prerequisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business Premium, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
- <span data-ttu-id="02af5-128">A Windows [10-es](secure-win-10-pcs.md) eszközökre vonatkozó házirendek beállításához kövesse a Biztonságos Windows 10-es PC-k lépéseit.</span><span class="sxs-lookup"><span data-stu-id="02af5-128">Follow the steps in [secure Windows 10 PCs](secure-win-10-pcs.md) to set up policies for Windows 10 devices.</span></span>

<span data-ttu-id="02af5-129">Amikor egy Windows 10-es eszközhöz csatlakozik az Azure AD-hez, a Windows 10-es számítógépekhez beállított házirendek vonatkoznak rá.</span><span class="sxs-lookup"><span data-stu-id="02af5-129">When you join a Windows 10 device to Azure AD, the policies you set for Windows 10 computers get applied to it.</span></span> <span data-ttu-id="02af5-130">További információt a [Windows-eszközök beállítása a Microsoft 365 felhasználóinak.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="02af5-130">For more information, see [Set up Windows devices for Microsoft 365 users](set-up-windows-devices.md).</span></span>

## <a name="step-4-install-microsoft-365-apps-for-business"></a><span data-ttu-id="02af5-131">4. lépés: A Microsoft 365 Vállalati verziós alkalmazások telepítése</span><span class="sxs-lookup"><span data-stu-id="02af5-131">Step 4: Install Microsoft 365 Apps for business</span></span>
- <span data-ttu-id="02af5-132">A beállítási varázslóval automatikusan telepítheti az Office-t a [Windows-eszközökre.](set-up.md#deploy-office-365-client-apps)</span><span class="sxs-lookup"><span data-stu-id="02af5-132">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="02af5-133">A felhasználók [telepíthetik a Windowsra](https://docs.microsoft.com/office365/admin/setup/install-applications) és az eszközökre telepített Office-alkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="02af5-133">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="02af5-134">Speciális</span><span class="sxs-lookup"><span data-stu-id="02af5-134">Advanced</span></span>
- <span data-ttu-id="02af5-135">**Új eszközök beállítása az Autopilottal**</span><span class="sxs-lookup"><span data-stu-id="02af5-135">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="02af5-136">A [Windows Autopilottal](add-autopilot-devices-and-profile.md) automatikusan előre konfigurálhatja az új **Windows** 10-es eszközöket [](https://www.microsoft.com/solution-providers/search) a felhasználóknak, de egyszerűbb lehet egy olyan partnert szerezni, aki ezt meg tudja tenni Önért.</span><span class="sxs-lookup"><span data-stu-id="02af5-136">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="02af5-137">A Microsoft [Store-ban](https://go.microsoft.com/fwlink/?linkid=874598)is megkérhet egy felhőalapú technológiai szakértőt, hogy állítsa be a megvásárolt új eszközöket.</span><span class="sxs-lookup"><span data-stu-id="02af5-137">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), and ask a cloud technology expert to set up new devices that you purchase.</span></span>

- <span data-ttu-id="02af5-138">**Helyszíni erőforrások elérése**</span><span class="sxs-lookup"><span data-stu-id="02af5-138">**Access on-premises resources**</span></span>

     - <span data-ttu-id="02af5-139">Ha szervezete helyszíni Windows Server Active Directoryt használ, beállíthatja a Microsoft 365 Vállalati prémium verzióban a Windows 10-es eszközök védelmét, miközben továbbra is hozzáférhet a helyi hitelesítést igénylő helyszíni erőforrásokhoz.</span><span class="sxs-lookup"><span data-stu-id="02af5-139">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="02af5-140">A beállítás beállításához kövesse az [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) (Tartományhoz csatlakozott Windows 10-es eszközök engedélyezése) beállítás lépéseit.</span><span class="sxs-lookup"><span data-stu-id="02af5-140">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="02af5-141">Ez az előnyben részesített módszer, és az ebben az állapotban használt eszközöket hibrid Azure AD-hez csatlakozott eszközöknek nevezzük.</span><span class="sxs-lookup"><span data-stu-id="02af5-141">This is the preferred method, and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="02af5-142">Ha vállalata rendelkezik helyi Active Directory-címtárral, amely helyszíni erőforrásokat (például fájlmegosztásokat és nyomtatókat) tartalmaz, az alábbi lépéseket követve hozzáférést adhat az Azure AD-hez csatlakozott eszközöknek: A [Microsoft 365](access-resources.md)Vállalati prémium verzió Azure AD-hez csatlakozott eszközén helyszíni erőforrásokhoz férhet hozzá.</span><span class="sxs-lookup"><span data-stu-id="02af5-142">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers), you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium](access-resources.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="02af5-143">Lásd még</span><span class="sxs-lookup"><span data-stu-id="02af5-143">See also</span></span>

[<span data-ttu-id="02af5-144">Microsoft 365 Vállalati verziós oktatóvideók</span><span class="sxs-lookup"><span data-stu-id="02af5-144">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)

---
title: A beállítás áttekintése
f1.keywords:
- NOCSH
ms.author: kwekua
author: kwekua
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
description: Ismerje meg a Microsoft 365 Vállalati prémium verzió beállítási lépéseit, az előfizetéstől az előfizetésen át a tartományok és felhasználók hozzáadásán át a biztonsági házirendek beállításán át a biztonsági házirendek beállításához stb.
ms.openlocfilehash: 749acbfdbde92ad97b09dc720c85dd850b76c9cf
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579934"
---
# <a name="overview-of-setup"></a><span data-ttu-id="39b88-103">A beállítás áttekintése</span><span class="sxs-lookup"><span data-stu-id="39b88-103">Overview of setup</span></span>

<span data-ttu-id="39b88-104">Tekintsen meg egy rövid videót a Microsoft 365 Vállalati prémium verzió beállításról.</span><span class="sxs-lookup"><span data-stu-id="39b88-104">Watch a short video about Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

<span data-ttu-id="39b88-105">Ha hasznosnak találta ezt a videót, tekintse meg a [teljes tanfolyamok kisvállalatoknak és Microsoft 365-újoncoknak](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) című cikket.</span><span class="sxs-lookup"><span data-stu-id="39b88-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

<span data-ttu-id="39b88-106">A beállítási lépések nagy része az irányított telepítés során megjelenik, de a többi lehetőség is szerepel a listában.</span><span class="sxs-lookup"><span data-stu-id="39b88-106">Most of the setup steps can be done in the guided setup, but the other options are also listed.</span></span>

## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="39b88-107">1. lépés: A tartomány és a felhasználók hozzáadása</span><span class="sxs-lookup"><span data-stu-id="39b88-107">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="39b88-108">**[Tartomány hozzáadása](set-up.md#add-your-domain-to-personalize-sign-in)** (ha a regisztráció során megvásárolta a tartományt, [](sign-up.md)ez a lépés már megtörtént.)</span><span class="sxs-lookup"><span data-stu-id="39b88-108">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

   - <span data-ttu-id="39b88-109">**Felhasználók hozzáadása gombra.**</span><span class="sxs-lookup"><span data-stu-id="39b88-109">**Add users**.</span></span> <span data-ttu-id="39b88-110">A felhasználókat a következő három módszer bármelyikében felveheti:</span><span class="sxs-lookup"><span data-stu-id="39b88-110">You can add users in any of the three ways:</span></span>
        - <span data-ttu-id="39b88-111">Az irányított [beállításban](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="39b88-111">In the [guided setup](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="39b88-112">Ha helyszíni Active Directoryval rendelkezik, a címtár-szinkronizálással felhasználókat adhat hozzá az [Azure AD Connect](../enterprise/set-up-directory-synchronization.md) használatával.</span><span class="sxs-lookup"><span data-stu-id="39b88-112">Use directory synchronization to [add users by using Azure AD Connect](../enterprise/set-up-directory-synchronization.md) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="39b88-113">A felhasználókat [később is hozzáadhatja a](../admin/add-users/add-users.md) Felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="39b88-113">You can also [add users later](../admin/add-users/add-users.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="39b88-114">2. lépés: Biztonsági házirendek beállítása és eszközök beállítása</span><span class="sxs-lookup"><span data-stu-id="39b88-114">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="39b88-115">Az eszköz [házirendek konfigurálása az](set-up.md#protect-your-organization) interaktív beállítással.</span><span class="sxs-lookup"><span data-stu-id="39b88-115">Use the [guided setup](set-up.md#protect-your-organization) to configure device policies.</span></span> 
  - <span data-ttu-id="39b88-116">További funkciókat is felvehet vagy szerkeszthet később a felügyeleti [központban](view-policies-and-devices.md) és az [Intune portálon.](/intune/tutorial-walkthrough-intune-portal)</span><span class="sxs-lookup"><span data-stu-id="39b88-116">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="39b88-117">A beállítási varázsló alapszintű veszélyforrás-védelmi és adatveszteség-megelőzési beállításokat is beállít.</span><span class="sxs-lookup"><span data-stu-id="39b88-117">The setup wizard will also set up basic threat protection and data loss prevention settings.</span></span>
  
  <span data-ttu-id="39b88-118">A beállítási varázsló biztonsági beállításain kívül az alábbi beállítások megadásával növelheti a biztonságot:</span><span class="sxs-lookup"><span data-stu-id="39b88-118">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

- <span data-ttu-id="39b88-119">**Kártevők elleni védelem az e-mailekben**</span><span class="sxs-lookup"><span data-stu-id="39b88-119">**Email malware protection**</span></span>
- <span data-ttu-id="39b88-120">**Adathalászat elleni védelem az Office 365 Defenderben**</span><span class="sxs-lookup"><span data-stu-id="39b88-120">**Anti-phishing in Defender for Office 365**</span></span>
- <span data-ttu-id="39b88-121">**Exchange Online Archiválás**</span><span class="sxs-lookup"><span data-stu-id="39b88-121">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="39b88-122">**Azure Information Protection (1. csomag)**</span><span class="sxs-lookup"><span data-stu-id="39b88-122">**Azure Information Protection (Plan1**)</span></span>

<span data-ttu-id="39b88-123">Első lépések: A veszélyforrások [elleni védelem](increase-threat-protection.md) növelése és megfelelőségi [funkciók beállítása.](set-up-compliance.md)</span><span class="sxs-lookup"><span data-stu-id="39b88-123">To get started, see [increase threat protection](increase-threat-protection.md) and [set up compliance features](set-up-compliance.md).</span></span>

<span data-ttu-id="39b88-124">A 10 legjobb módszer a [Microsoft 365 Vállalati prémium](/office365/admin/security-and-compliance/secure-your-business-data) verzió biztonságának biztonságára vonatkozó gyakorlati tanácsokért tekintse meg az utcatérképet.</span><span class="sxs-lookup"><span data-stu-id="39b88-124">See also [top 10 ways to secure your Microsoft 365 Business Premium](/office365/admin/security-and-compliance/secure-your-business-data) for a road-map of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="39b88-125">3. lépés: Windows 10-es eszközök beállítása és kezelése</span><span class="sxs-lookup"><span data-stu-id="39b88-125">Step 3: Set up and manage Windows 10 devices</span></span>

<span data-ttu-id="39b88-126">Az irányított beállítás befejezése után meg kell védenie a szervezet összes Windows 10-es számítógépét.</span><span class="sxs-lookup"><span data-stu-id="39b88-126">After you complete the guided setup, you will want to protect all the Windows 10 computers in your organization.</span></span>
  
- <span data-ttu-id="39b88-127">A Windows 10 Pro előfeltétele [a](pre-requisites-for-data-protection.md) Microsoft 365 Business Premium terméknek, ha azonban Windows 7 Pro, Windows 8 Pro vagy Windows 8.1 Pro rendszerrel rendelkezik, előfizetése feljogosítja a Windows 10 Pro verzióra [való frissítésre.](./upgrade-to-windows-pro-creators-update.md)</span><span class="sxs-lookup"><span data-stu-id="39b88-127">Windows 10 Pro is a [prerequisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business Premium, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](./upgrade-to-windows-pro-creators-update.md).</span></span>
- <span data-ttu-id="39b88-128">Kövesse a [biztonságos Windows 10-es PC-k](secure-win-10-pcs.md) lépéseit a Windows 10-es eszközökhöz beállított házirendek beállításához.</span><span class="sxs-lookup"><span data-stu-id="39b88-128">Follow the steps in [secure Windows 10 PCs](secure-win-10-pcs.md) to set up policies for Windows 10 devices.</span></span>

<span data-ttu-id="39b88-129">Amikor egy Windows 10-es eszközhöz csatlakozik az Azure AD-hez, a Windows 10-es számítógépeken beállított házirendek érvényesek rá.</span><span class="sxs-lookup"><span data-stu-id="39b88-129">When you join a Windows 10 device to Azure AD, the policies you set for Windows 10 computers get applied to it.</span></span> <span data-ttu-id="39b88-130">További információt a Windows-eszközök beállítása [a Microsoft 365 felhasználóinak.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="39b88-130">For more information, see [Set up Windows devices for Microsoft 365 users](set-up-windows-devices.md).</span></span>

## <a name="step-4-install-microsoft-365-apps-for-business"></a><span data-ttu-id="39b88-131">4. lépés: A Microsoft 365 Vállalati verziós alkalmazások telepítése</span><span class="sxs-lookup"><span data-stu-id="39b88-131">Step 4: Install Microsoft 365 Apps for business</span></span>
- <span data-ttu-id="39b88-132">Az Office-t automatikusan telepítheti a Windows-eszközökre a [beállítási varázslóval.](set-up.md#deploy-office-365-client-apps)</span><span class="sxs-lookup"><span data-stu-id="39b88-132">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="39b88-133">A felhasználók [telepíthetinek Office-appokat](/office365/admin/setup/install-applications) Windowsra és eszközökre.</span><span class="sxs-lookup"><span data-stu-id="39b88-133">Let users [install Office apps](/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="39b88-134">Speciális</span><span class="sxs-lookup"><span data-stu-id="39b88-134">Advanced</span></span>
- <span data-ttu-id="39b88-135">**Új eszközök beállítása az Autopilottal**</span><span class="sxs-lookup"><span data-stu-id="39b88-135">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="39b88-136">A [Windows Autopilottal](add-autopilot-devices-and-profile.md) automatikusan előre konfigurálhatja az új **Windows** 10-es eszközöket [](https://www.microsoft.com/solution-providers/search) a felhasználóknak, de egyszerűbb lehet egy partnert kihozni, aki ezt meg tudja tenni Önért.</span><span class="sxs-lookup"><span data-stu-id="39b88-136">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="39b88-137">A Microsoft [Store](https://go.microsoft.com/fwlink/?linkid=874598)áruházban meg is kérhet egy felhőtechnológia-szakértőt, hogy állítsa be a megvásárolt új eszközöket.</span><span class="sxs-lookup"><span data-stu-id="39b88-137">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), and ask a cloud technology expert to set up new devices that you purchase.</span></span>

- <span data-ttu-id="39b88-138">**Helyszíni erőforrások elérése**</span><span class="sxs-lookup"><span data-stu-id="39b88-138">**Access on-premises resources**</span></span>

     - <span data-ttu-id="39b88-139">Ha szervezete helyszíni Windows Server Active Directoryt használ, beállíthatja a Microsoft 365 Business Premiumt a Windows 10-es eszközök védelme érdekében úgy, hogy közben továbbra is hozzáférjen a helyi hitelesítést igénylő helyszíni erőforrásokhoz.</span><span class="sxs-lookup"><span data-stu-id="39b88-139">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="39b88-140">A beállítás beállításához kövesse A tartományhoz csatlakozott [Windows 10-es eszközök microsoft 365 Vállalati prémium](manage-windows-devices.md) verzió által történő kezelése.</span><span class="sxs-lookup"><span data-stu-id="39b88-140">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="39b88-141">Ez az előnyben részesített módszer, az ebben az állapotban használt eszközök pedig hibrid Azure AD-hez csatlakozott eszközök.</span><span class="sxs-lookup"><span data-stu-id="39b88-141">This is the preferred method, and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="39b88-142">Ha vállalata helyi Active Directory-címtárral rendelkezik, amely helyszíni erőforrásokat (például fájlmegosztásokat és nyomtatókat) tartalmaz, az alábbi lépéseket követve hozzáférést adhat Azure AD-hez eszközének ezekhez az erőforrásokhoz: Hozzáférés helyszíni erőforrásokhoz egy Azure AD-hez csatlakozott eszközről a [Microsoft 365 Vállalati prémium verzióban.](access-resources.md)</span><span class="sxs-lookup"><span data-stu-id="39b88-142">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers), you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium](access-resources.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="39b88-143">Lásd még</span><span class="sxs-lookup"><span data-stu-id="39b88-143">See also</span></span>

[<span data-ttu-id="39b88-144">Microsoft 365 Vállalati verzió – oktatóvideók</span><span class="sxs-lookup"><span data-stu-id="39b88-144">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
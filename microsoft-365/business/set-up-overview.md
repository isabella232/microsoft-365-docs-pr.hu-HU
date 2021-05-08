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
description: Megtudhatja, hogy hogyan Microsoft 365 Vállalati prémium verzió, az előfizetéstől a tartományok és felhasználók felvételén át a biztonsági házirendek beállításán át a biztonsági házirendek beállításához.
ms.openlocfilehash: 008a5c51698589667acc0d01649f67dab33b4c58
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52245064"
---
# <a name="overview-of-setup"></a><span data-ttu-id="bd614-103">A beállítás áttekintése</span><span class="sxs-lookup"><span data-stu-id="bd614-103">Overview of setup</span></span>

<span data-ttu-id="bd614-104">Tekintsen meg egy rövid videót a Microsoft 365 Vállalati prémium verzió beállításról.</span><span class="sxs-lookup"><span data-stu-id="bd614-104">Watch a short video about Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

<span data-ttu-id="bd614-105">Ha hasznosnak találta ezt a videót, tekintse meg a [teljes tanfolyamok kisvállalatoknak és Microsoft 365-újoncoknak](../business-video/index.yml) című cikket.</span><span class="sxs-lookup"><span data-stu-id="bd614-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](../business-video/index.yml).</span></span>

<span data-ttu-id="bd614-106">A beállítási lépések nagy része az irányított telepítés során megjelenik, de a többi lehetőség is szerepel a listában.</span><span class="sxs-lookup"><span data-stu-id="bd614-106">Most of the setup steps can be done in the guided setup, but the other options are also listed.</span></span>

## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="bd614-107">1. lépés: A tartomány és a felhasználók hozzáadása</span><span class="sxs-lookup"><span data-stu-id="bd614-107">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="bd614-108">**[Tartomány hozzáadása](set-up.md#add-your-domain-to-personalize-sign-in)** (ha a regisztráció során megvásárolta a tartományt, [](sign-up.md)ez a lépés már megtörtént.)</span><span class="sxs-lookup"><span data-stu-id="bd614-108">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

   - <span data-ttu-id="bd614-109">**Felhasználók hozzáadása gombra.**</span><span class="sxs-lookup"><span data-stu-id="bd614-109">**Add users**.</span></span> <span data-ttu-id="bd614-110">A felhasználókat a következő három módszer bármelyikében felveheti:</span><span class="sxs-lookup"><span data-stu-id="bd614-110">You can add users in any of the three ways:</span></span>
        - <span data-ttu-id="bd614-111">Az irányított [beállításban](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="bd614-111">In the [guided setup](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="bd614-112">A címtár-szinkronizálással felhasználókat adhat hozzá az [Azure AD](../enterprise/set-up-directory-synchronization.md) Csatlakozás használatával, ha helyszíni Active Directoryval rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="bd614-112">Use directory synchronization to [add users by using Azure AD Connect](../enterprise/set-up-directory-synchronization.md) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="bd614-113">A felhasználókat [később is hozzáadhatja a](../admin/add-users/add-users.md) Felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="bd614-113">You can also [add users later](../admin/add-users/add-users.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="bd614-114">2. lépés: Biztonsági házirendek beállítása és eszközök beállítása</span><span class="sxs-lookup"><span data-stu-id="bd614-114">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="bd614-115">Az eszköz [házirendek konfigurálása az](set-up.md#protect-your-organization) interaktív beállítással.</span><span class="sxs-lookup"><span data-stu-id="bd614-115">Use the [guided setup](set-up.md#protect-your-organization) to configure device policies.</span></span> 
  - <span data-ttu-id="bd614-116">További funkciókat is felvehet vagy szerkeszthet később a felügyeleti [központban](view-policies-and-devices.md) és az [Intune portálon.](/intune/tutorial-walkthrough-intune-portal)</span><span class="sxs-lookup"><span data-stu-id="bd614-116">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="bd614-117">A beállítási varázsló alapszintű veszélyforrás-védelmi és adatveszteség-megelőzési beállításokat is beállít.</span><span class="sxs-lookup"><span data-stu-id="bd614-117">The setup wizard will also set up basic threat protection and data loss prevention settings.</span></span>
  
  <span data-ttu-id="bd614-118">A beállítási varázsló biztonsági beállításain kívül az alábbi beállítások megadásával növelheti a biztonságot:</span><span class="sxs-lookup"><span data-stu-id="bd614-118">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

- <span data-ttu-id="bd614-119">**Kártevők elleni védelem az e-mailekben**</span><span class="sxs-lookup"><span data-stu-id="bd614-119">**Email malware protection**</span></span>
- <span data-ttu-id="bd614-120">**Adathalászat elleni védelem a Defender Office 365**</span><span class="sxs-lookup"><span data-stu-id="bd614-120">**Anti-phishing in Defender for Office 365**</span></span>
- <span data-ttu-id="bd614-121">**Exchange Online Archiválás**</span><span class="sxs-lookup"><span data-stu-id="bd614-121">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="bd614-122">**Azure Information Protection (1. csomag)**</span><span class="sxs-lookup"><span data-stu-id="bd614-122">**Azure Information Protection (Plan1**)</span></span>

<span data-ttu-id="bd614-123">Első lépések: A veszélyforrások [elleni védelem](increase-threat-protection.md) növelése és megfelelőségi [funkciók beállítása.](set-up-compliance.md)</span><span class="sxs-lookup"><span data-stu-id="bd614-123">To get started, see [increase threat protection](increase-threat-protection.md) and [set up compliance features](set-up-compliance.md).</span></span>

<span data-ttu-id="bd614-124">Az ajánlott biztonsági eljárásokról a [10](/office365/admin/security-and-compliance/secure-your-business-data) legjobb Microsoft 365 Vállalati prémium verzió kínálunk.</span><span class="sxs-lookup"><span data-stu-id="bd614-124">See also [top 10 ways to secure your Microsoft 365 Business Premium](/office365/admin/security-and-compliance/secure-your-business-data) for a road-map of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="bd614-125">3. lépés: A mobileszközök Windows 10 kezelése</span><span class="sxs-lookup"><span data-stu-id="bd614-125">Step 3: Set up and manage Windows 10 devices</span></span>

<span data-ttu-id="bd614-126">Az irányított beállítás befejezése után meg kell védenie a Windows 10 összes számítógépét.</span><span class="sxs-lookup"><span data-stu-id="bd614-126">After you complete the guided setup, you will want to protect all the Windows 10 computers in your organization.</span></span>
  
- <span data-ttu-id="bd614-127">Windows 10 Pro a Microsoft 365 Vállalati prémium verzió [](pre-requisites-for-data-protection.md) előfeltétele, de ha Windows 7 Pro, Windows 8 Pro vagy Windows 8.1 Pro verzióval rendelkezik, előfizetése feljogosítja a Windows 10 Pro. [](./upgrade-to-windows-pro-creators-update.md)</span><span class="sxs-lookup"><span data-stu-id="bd614-127">Windows 10 Pro is a [prerequisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business Premium, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](./upgrade-to-windows-pro-creators-update.md).</span></span>
- <span data-ttu-id="bd614-128">A pc-k biztonságos Windows 10 [a](secure-win-10-pcs.md) házirendek beállításához Windows 10 eszközökre.</span><span class="sxs-lookup"><span data-stu-id="bd614-128">Follow the steps in [secure Windows 10 PCs](secure-win-10-pcs.md) to set up policies for Windows 10 devices.</span></span>

<span data-ttu-id="bd614-129">Amikor egy Windows 10 eszközhöz csatlakozik az Azure AD-hez, a számítógéphez Windows 10 házirendeket alkalmazza a rendszer.</span><span class="sxs-lookup"><span data-stu-id="bd614-129">When you join a Windows 10 device to Azure AD, the policies you set for Windows 10 computers get applied to it.</span></span> <span data-ttu-id="bd614-130">További információt A mobileszközök beállítása [Windows felhasználóknak Microsoft 365.](set-up-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="bd614-130">For more information, see [Set up Windows devices for Microsoft 365 users](set-up-windows-devices.md).</span></span>

## <a name="step-4-install-microsoft-365-apps-for-business"></a><span data-ttu-id="bd614-131">4. lépés: A Üzleti Microsoft 365-alkalmazások</span><span class="sxs-lookup"><span data-stu-id="bd614-131">Step 4: Install Microsoft 365 Apps for business</span></span>
- <span data-ttu-id="bd614-132">A telepítővarázsló Office automatikusan telepítheti Windows eszközén. [](set-up.md#deploy-office-365-client-apps)</span><span class="sxs-lookup"><span data-stu-id="bd614-132">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="bd614-133">A felhasználók [telepíthet Office appokat](/office365/admin/setup/install-applications) a Windows eszközökhöz.</span><span class="sxs-lookup"><span data-stu-id="bd614-133">Let users [install Office apps](/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="bd614-134">Speciális</span><span class="sxs-lookup"><span data-stu-id="bd614-134">Advanced</span></span>
- <span data-ttu-id="bd614-135">**Új eszközök beállítása az Autopilottal**</span><span class="sxs-lookup"><span data-stu-id="bd614-135">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="bd614-136">A Windows [Autopilottal](add-autopilot-devices-and-profile.md) automatikusan előre konfigurálhatja  az új Windows 10-eszközöket a felhasználók számára, de [](https://www.microsoft.com/solution-providers/search) egyszerűbb, ha egy olyan partnert szerez be, aki ezt meg tudja tenni Önért.</span><span class="sxs-lookup"><span data-stu-id="bd614-136">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="bd614-137">Azt is beállíthatja, hogy [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), és kérje meg egy felhőtechnológiát szakértőt, hogy állítsa be a megvásárolt új eszközöket.</span><span class="sxs-lookup"><span data-stu-id="bd614-137">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), and ask a cloud technology expert to set up new devices that you purchase.</span></span>

- <span data-ttu-id="bd614-138">**Helyszíni erőforrások elérése**</span><span class="sxs-lookup"><span data-stu-id="bd614-138">**Access on-premises resources**</span></span>

     - <span data-ttu-id="bd614-139">Ha szervezete helyszíni Windows Server Active Directoryt használ, beállíthatja a Microsoft 365 Vállalati prémium verzió-t az Windows 10-eszközök védelmére, miközben továbbra is hozzáfér a helyi hitelesítést igénylő helyszíni erőforrásokhoz.</span><span class="sxs-lookup"><span data-stu-id="bd614-139">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="bd614-140">A beállításhoz kövesse A tartományhoz Windows 10 eszközök felhasználói [Microsoft 365 Vállalati prémium verzió](manage-windows-devices.md) beállításának lépéseit.</span><span class="sxs-lookup"><span data-stu-id="bd614-140">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="bd614-141">Ez az előnyben részesített módszer, az ebben az állapotban használt eszközök pedig hibrid Azure AD-hez csatlakozott eszközök.</span><span class="sxs-lookup"><span data-stu-id="bd614-141">This is the preferred method, and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="bd614-142">Ha vállalata rendelkezik olyan helyi Active Directory-címtárral, amely helyszíni erőforrásokat (például fájlmegosztásokat és nyomtatókat) tartalmaz, az alábbi lépéseket követve hozzáférést adhat Azure AD-hez eszközének az erőforrásokhoz: Hozzáférés helyszíni erőforrásokhoz [egy Azure AD-hez](access-resources.md)csatlakozott eszközről a Microsoft 365 Vállalati prémium verzió-ban.</span><span class="sxs-lookup"><span data-stu-id="bd614-142">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers), you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium](access-resources.md).</span></span>

## <a name="related-content"></a><span data-ttu-id="bd614-143">Kapcsolódó tartalom</span><span class="sxs-lookup"><span data-stu-id="bd614-143">Related content</span></span>

<span data-ttu-id="bd614-144">[Microsoft 365 vállalati verziós oktatóvideók](../business-video/index.yml) (hivatkozáslap)</span><span class="sxs-lookup"><span data-stu-id="bd614-144">[Microsoft 365 for business training videos](../business-video/index.yml) (link page)</span></span>
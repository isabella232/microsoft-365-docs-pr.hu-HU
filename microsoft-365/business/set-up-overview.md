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
description: Ismerje meg a Microsoft 365 vállalati prémium verzió telepítési lépéseit, a feliratkozást, a tartomány és a felhasználók hozzáadását, illetve a biztonsági házirendek beállítását.
ms.openlocfilehash: 46370166a9d5e8c9308b8947513e631c159f0b86
ms.sourcegitcommit: 815229e39a0f905d9f06717f00dc82e2a028fa7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48842130"
---
# <a name="overview-of-setup"></a><span data-ttu-id="22429-103">A beállítás áttekintése</span><span class="sxs-lookup"><span data-stu-id="22429-103">Overview of setup</span></span>

<span data-ttu-id="22429-104">Tekintsen meg egy rövid videót a Microsoft 365 vállalati prémium verzió telepítéséről.</span><span class="sxs-lookup"><span data-stu-id="22429-104">Watch a short video about Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

<span data-ttu-id="22429-105">Ha hasznosnak találta ezt a videót, tekintse meg a [teljes tanfolyamok kisvállalatoknak és Microsoft 365-újoncoknak](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) című cikket.</span><span class="sxs-lookup"><span data-stu-id="22429-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

<span data-ttu-id="22429-106">A beállítási lépések többsége az irányított beállításban végezhető el, de a további lehetőségek is szerepelnek a listában.</span><span class="sxs-lookup"><span data-stu-id="22429-106">Most of the setup steps can be done in the guided setup, but the other options are also listed.</span></span>

## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="22429-107">Első lépés: a tartomány és a felhasználók felvétele</span><span class="sxs-lookup"><span data-stu-id="22429-107">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="22429-108">**[Tartomány felvétele](set-up.md#add-your-domain-to-personalize-sign-in)** (ha a [regisztráció](sign-up.md)során vásárolta meg a tartományt, ez a lépés már elkészült.)</span><span class="sxs-lookup"><span data-stu-id="22429-108">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

   - <span data-ttu-id="22429-109">**Felhasználók hozzáadása**</span><span class="sxs-lookup"><span data-stu-id="22429-109">**Add users**.</span></span> <span data-ttu-id="22429-110">A felhasználók a következő három módon adhatók hozzá:</span><span class="sxs-lookup"><span data-stu-id="22429-110">You can add users in any of the three ways:</span></span>
        - <span data-ttu-id="22429-111">Az [irányított beállításban](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="22429-111">In the [guided setup](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="22429-112">A címtár-szinkronizálás segítségével [felhasználókat vehet fel az Azure ad Connect segítségével](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) , ha helyszíni Active Directoryval rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="22429-112">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="22429-113">A felügyeleti központban [később is hozzáadhat felhasználókat](add-users-m365b.md) .</span><span class="sxs-lookup"><span data-stu-id="22429-113">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="22429-114">2. lépés: biztonsági házirendek beállítása és eszközök beállítása</span><span class="sxs-lookup"><span data-stu-id="22429-114">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="22429-115">Az [irányított beállítás](set-up.md#protect-your-organization) segítségével konfigurálhatja az eszközök házirendjeit.</span><span class="sxs-lookup"><span data-stu-id="22429-115">Use the [guided setup](set-up.md#protect-your-organization) to configure device policies.</span></span> 
  - <span data-ttu-id="22429-116">Később a [felügyeleti központban](view-policies-and-devices.md) és az [Intune portálon](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)is hozzáadhat további vagy szerkesztheti őket.</span><span class="sxs-lookup"><span data-stu-id="22429-116">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="22429-117">A beállítási varázsló a fenyegetések elleni védelem és az adatvesztés megelőzésére szolgáló beállításokat is megadhatja.</span><span class="sxs-lookup"><span data-stu-id="22429-117">The setup wizard will also set up basic threat protection and data loss prevention settings.</span></span>
  
  <span data-ttu-id="22429-118">A beállítási varázsló biztonsági beállításain kívül az alábbi beállítások megadásával növelheti a biztonságot:</span><span class="sxs-lookup"><span data-stu-id="22429-118">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

- <span data-ttu-id="22429-119">**E-mailes kártevők elleni védelem**</span><span class="sxs-lookup"><span data-stu-id="22429-119">**Email malware protection**</span></span>
- <span data-ttu-id="22429-120">**Az adathalászat elleni védekezés az Office 365 Defender-ban**</span><span class="sxs-lookup"><span data-stu-id="22429-120">**Anti-phishing in Defender for Office 365**</span></span>
- <span data-ttu-id="22429-121">**Exchange Online Archiválás**</span><span class="sxs-lookup"><span data-stu-id="22429-121">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="22429-122">**Azure Information Protection (Plan1** )</span><span class="sxs-lookup"><span data-stu-id="22429-122">**Azure Information Protection (Plan1** )</span></span>

<span data-ttu-id="22429-123">A kezdéshez lásd: a [fenyegetések elleni védelem növelése](increase-threat-protection.md) és a [megfelelőségi funkciók beállítása](set-up-compliance.md).</span><span class="sxs-lookup"><span data-stu-id="22429-123">To get started, see [increase threat protection](increase-threat-protection.md) and [set up compliance features](set-up-compliance.md).</span></span>

<span data-ttu-id="22429-124">Lásd még az [első 10 módszer a Microsoft 365 vállalati prémium verzió biztonságossá](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) tételére a legjobb biztonsági gyakorlatok térképéhez.</span><span class="sxs-lookup"><span data-stu-id="22429-124">See also [top 10 ways to secure your Microsoft 365 Business Premium](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a road-map of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="22429-125">3. lépés: a Windows 10-es eszközök beállítása és kezelése</span><span class="sxs-lookup"><span data-stu-id="22429-125">Step 3: Set up and manage Windows 10 devices</span></span>

<span data-ttu-id="22429-126">Az irányított beállítás befejezése után védenie kell a szervezete összes Windows 10-es számítógépét.</span><span class="sxs-lookup"><span data-stu-id="22429-126">After you complete the guided setup, you will want to protect all the Windows 10 computers in your organization.</span></span>
  
- <span data-ttu-id="22429-127">A Windows 10 Pro a Microsoft 365 vállalati prémium verzió [előfeltétele](pre-requisites-for-data-protection.md) , de ha Windows 7 Pro, Windows 8 Pro vagy Windows 8,1 Pro verziót futtat, az előfizetése feljogosítja a [Windows 10 Pro rendszerre való frissítésre](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span><span class="sxs-lookup"><span data-stu-id="22429-127">Windows 10 Pro is a [prerequisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business Premium, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
- <span data-ttu-id="22429-128">Kövesse a [Windows 10 rendszerű PC-k biztonsága](secure-win-10-pcs.md) című témakör lépéseit a Windows 10-es eszközök házirendjeinek beállításához.</span><span class="sxs-lookup"><span data-stu-id="22429-128">Follow the steps in [secure Windows 10 PCs](secure-win-10-pcs.md) to set up policies for Windows 10 devices.</span></span>

<span data-ttu-id="22429-129">Amikor Windows 10-es eszközre csatlakozik az Azure AD-hoz, a rendszer a Windows 10 rendszerű számítógépekre beállított házirendeket alkalmazza.</span><span class="sxs-lookup"><span data-stu-id="22429-129">When you join a Windows 10 device to Azure AD, the policies you set for Windows 10 computers get applied to it.</span></span> <span data-ttu-id="22429-130">További információt a Windows- [eszközök beállítása a Microsoft 365-felhasználók](set-up-windows-devices.md)számára című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="22429-130">For more information, see [Set up Windows devices for Microsoft 365 users](set-up-windows-devices.md).</span></span>

## <a name="step-4-install-microsoft-365-apps-for-business"></a><span data-ttu-id="22429-131">4. lépés: a Microsoft 365-alkalmazások vállalati verzió telepítése</span><span class="sxs-lookup"><span data-stu-id="22429-131">Step 4: Install Microsoft 365 Apps for business</span></span>
- <span data-ttu-id="22429-132">A [beállítási varázsló](set-up.md#deploy-office-365-client-apps)segítségével automatikusan telepítheti az Office-t a Windows-eszközökön.</span><span class="sxs-lookup"><span data-stu-id="22429-132">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="22429-133">Az [Office-alkalmazások telepítése](https://docs.microsoft.com/office365/admin/setup/install-applications) Windows rendszerre és eszközökre</span><span class="sxs-lookup"><span data-stu-id="22429-133">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="22429-134">Speciális</span><span class="sxs-lookup"><span data-stu-id="22429-134">Advanced</span></span>
- <span data-ttu-id="22429-135">**Új eszközök beállítása az Autopilot használatával**</span><span class="sxs-lookup"><span data-stu-id="22429-135">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="22429-136">A [Windows Autopilot](add-autopilot-devices-and-profile.md) segítségével automatikusan megadhatja az **új** Windows 10-es eszközöket a felhasználóknak, de egyszerűbb lehet egy olyan [partner](https://www.microsoft.com/solution-providers/search) beszerzése, aki ezt elvégezheti.</span><span class="sxs-lookup"><span data-stu-id="22429-136">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="22429-137">A [Microsoft áruházat](https://go.microsoft.com/fwlink/?linkid=874598)is elérheti, és megkérheti a felhőalapú technológiai szakértőt, hogy állítsa be a megvásárolt új eszközöket.</span><span class="sxs-lookup"><span data-stu-id="22429-137">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), and ask a cloud technology expert to set up new devices that you purchase.</span></span>

- <span data-ttu-id="22429-138">**Hozzáférés helyszíni erőforrásokhoz**</span><span class="sxs-lookup"><span data-stu-id="22429-138">**Access on-premises resources**</span></span>

     - <span data-ttu-id="22429-139">Ha a szervezete a Windows Server Active Directoryt használja helyszíniként, beállíthatja a Microsoft 365 vállalati prémium verziót a Windows 10-es eszközök védelmére, miközben továbbra is megőrizheti a helyi hitelesítéshez szükséges helyszíni erőforrásokhoz való hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="22429-139">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="22429-140">Kövesse a [tartományhoz csatlakoztatott Windows 10-es eszközök kezelésének engedélyezése a Microsoft 365 vállalati prémium](manage-windows-devices.md) verzióban című témakör lépéseit.</span><span class="sxs-lookup"><span data-stu-id="22429-140">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="22429-141">Ez a preferált módszer, és az ebben az állapotban lévő eszközök neve hibrid Azure AD összekapcsolt eszközök.</span><span class="sxs-lookup"><span data-stu-id="22429-141">This is the preferred method, and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="22429-142">Ha a vállalkozása rendelkezik helyi Active Directory-címtárral, amely egy helyszíni erőforrásokat (például fájlmegosztás és nyomtató) tartalmaz, az alábbi lépésekkel érheti el az Azure AD-csatlakozású eszközök elérését az alábbi lépésekkel: a [helyszíni erőforrások elérése a Microsoft 365 Business Premium rendszer Azure ad-eszközéről](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="22429-142">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers), you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium](access-resources.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="22429-143">Lásd még</span><span class="sxs-lookup"><span data-stu-id="22429-143">See also</span></span>

[<span data-ttu-id="22429-144">Microsoft 365 vállalati verziós képzési videók</span><span class="sxs-lookup"><span data-stu-id="22429-144">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)

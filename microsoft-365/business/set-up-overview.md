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
description: Ismerje meg a Microsoft 365 Business Premium beállítási lépéseit, az előfizetéstől a tartomány és felhasználók hozzáadásáig, a biztonsági házirendek beállításáig és egyebekig.
ms.openlocfilehash: a808ae5761c1bc5706966a3f7de95f96f8f7c8c8
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44785812"
---
# <a name="overview-of-setup"></a><span data-ttu-id="75881-103">A beállítás áttekintése</span><span class="sxs-lookup"><span data-stu-id="75881-103">Overview of setup</span></span>

<span data-ttu-id="75881-104">Tekintse meg a Microsoft 365 Business Premium beállításáról szóló rövid videót.</span><span class="sxs-lookup"><span data-stu-id="75881-104">Watch a short video about Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

<span data-ttu-id="75881-105">Ha hasznosnak találta ezt a videót, tekintse meg a [teljes tanfolyamok kisvállalatoknak és Microsoft 365-újoncoknak](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) című cikket.</span><span class="sxs-lookup"><span data-stu-id="75881-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

<span data-ttu-id="75881-106">A beállítási lépések többsége elvégezhető a telepítővarázslóban, de a többi lehetőség is szerepel a listában.</span><span class="sxs-lookup"><span data-stu-id="75881-106">Most of the setup steps can be done in the setup wizard, but the other options are also listed.</span></span>

## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="75881-107">1. lépés: Tartomány és felhasználók hozzáadása</span><span class="sxs-lookup"><span data-stu-id="75881-107">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="75881-108">**[Adja hozzá a tartományt](set-up.md#add-your-domain-to-personalize-sign-in)** (ha a regisztráció során vásárolta meg a [tartományt,](sign-up.md)ez a lépés már megtörtént.)</span><span class="sxs-lookup"><span data-stu-id="75881-108">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

   - <span data-ttu-id="75881-109">**Felhasználók hozzáadása**.</span><span class="sxs-lookup"><span data-stu-id="75881-109">**Add users**.</span></span> <span data-ttu-id="75881-110">A felhasználókat a következő három módon veheti fel:</span><span class="sxs-lookup"><span data-stu-id="75881-110">You can add users in any of the three ways:</span></span>
        - <span data-ttu-id="75881-111">A [varázslóban.](set-up.md#add-users-in-the-wizard)</span><span class="sxs-lookup"><span data-stu-id="75881-111">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="75881-112">A címtár-szinkronizálás használatával [felhasználókat adhat hozzá az Azure AD Connect használatával,](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) ha rendelkezik egy helyszíni Active directory használatával.</span><span class="sxs-lookup"><span data-stu-id="75881-112">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="75881-113">Később a felügyeleti központban is [hozzáadhat felhasználókat.](add-users-m365b.md)</span><span class="sxs-lookup"><span data-stu-id="75881-113">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="75881-114">2. lépés: Biztonsági házirendek beállítása és eszközök konfigurálása</span><span class="sxs-lookup"><span data-stu-id="75881-114">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="75881-115">Az eszközházirendek konfigurálásához használja a [Telepítő varázslót.](set-up.md#protect-your-organization)</span><span class="sxs-lookup"><span data-stu-id="75881-115">Use the [Setup wizard](set-up.md#protect-your-organization) to configure device policies.</span></span> 
  - <span data-ttu-id="75881-116">A [felügyeleti központban](view-policies-and-devices.md) és az [Intune-portálon](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)később is hozzáadhat vagy szerkesztheti őket.</span><span class="sxs-lookup"><span data-stu-id="75881-116">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="75881-117">A telepítővarázsló alapszintű veszélyforrások elleni védelmet és adatveszteség-megelőzési beállításokat is beállít.</span><span class="sxs-lookup"><span data-stu-id="75881-117">The setup wizard will also set up basic threat protection and data loss prevention settings.</span></span>
  
  <span data-ttu-id="75881-118">A beállítási varázsló biztonsági beállításai mellett a következő beállítások hozzáadásával növelheti a biztonságot:</span><span class="sxs-lookup"><span data-stu-id="75881-118">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

- <span data-ttu-id="75881-119">**E-mail malware védelem**</span><span class="sxs-lookup"><span data-stu-id="75881-119">**Email malware protection**</span></span>
- <span data-ttu-id="75881-120">**ATP adathalászat elleni**</span><span class="sxs-lookup"><span data-stu-id="75881-120">**ATP anti-phishing**</span></span>
- <span data-ttu-id="75881-121">**Exchange Online Archiválás**</span><span class="sxs-lookup"><span data-stu-id="75881-121">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="75881-122">**Azure Information Protection (1. terv)**</span><span class="sxs-lookup"><span data-stu-id="75881-122">**Azure Information Protection (Plan1**)</span></span>

<span data-ttu-id="75881-123">Első lépésekhez olvassa el a [veszélyforrások elleni védelem növelése](increase-threat-protection.md) és a megfelelőségi funkciók beállítása című [témakört.](set-up-compliance.md)</span><span class="sxs-lookup"><span data-stu-id="75881-123">To get started, see [increase threat protection](increase-threat-protection.md) and [set up compliance features](set-up-compliance.md).</span></span>

<span data-ttu-id="75881-124">A legjobb biztonsági gyakorlatok megvalósítását a [Microsoft 365 Business Premium szolgáltatás védelmének első 10 témakörében](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) is megtekintheti.</span><span class="sxs-lookup"><span data-stu-id="75881-124">See also [top 10 ways to secure your Microsoft 365 Business Premium](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="75881-125">3. lépés: Windows 10-es eszközök beállítása és kezelése</span><span class="sxs-lookup"><span data-stu-id="75881-125">Step 3: Set up and manage Windows 10 devices</span></span>

<span data-ttu-id="75881-126">A beállítási varázsló futtatása után a szervezet összes Windwos 10 számítógépét meg kell vásárolnia.</span><span class="sxs-lookup"><span data-stu-id="75881-126">After you run the set up wizard, you will want to proctect all the Windwos 10 computers in your organization.</span></span>
  
- <span data-ttu-id="75881-127">A Windows 10 Pro a Microsoft 365 Business Premium [előfeltétele,](pre-requisites-for-data-protection.md) de ha Windows 7 Pro, Windows 8 Pro vagy Windows 8.1 Pro rendszerrel rendelkezik, előfizetése feljogosítja Önt a [Windows 10 Pro frissítésére.](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update)</span><span class="sxs-lookup"><span data-stu-id="75881-127">Windows 10 Pro is a [prerequisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business Premium, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
- <span data-ttu-id="75881-128">Kövesse a [windows 10-es számítógépek biztonságos](secure-win-10-pcs.md) beállításának lépéseit a Windows 10-es eszközökházirendjeinek beállításához.</span><span class="sxs-lookup"><span data-stu-id="75881-128">Follow the steps in [secure Windows 10 PCs](secure-win-10-pcs.md) to set up policies for Windows 10 devices.</span></span>

<span data-ttu-id="75881-129">Amikor csatlakozik egy Windows 10-es eszközhöz az Azure AD-hez, a Windows 10-es számítógépekhez beállított házirendek lesznek alkalmazva.</span><span class="sxs-lookup"><span data-stu-id="75881-129">When you join a Windows 10 device to Azure AD, the policies you set for Windows 10 computers get applied to it.</span></span> <span data-ttu-id="75881-130">További információt a [Windows-eszközök beállítása Microsoft 365-felhasználók számára](set-up-windows-devices.md)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="75881-130">For more information, see [Set up Windows devices for Microsoft 365 users](set-up-windows-devices.md).</span></span>

## <a name="step-4-install-microsoft-365-apps-for-business"></a><span data-ttu-id="75881-131">4. lépés: Microsoft 365 vállalati alkalmazások telepítése</span><span class="sxs-lookup"><span data-stu-id="75881-131">Step 4: Install Microsoft 365 Apps for business</span></span>
- <span data-ttu-id="75881-132">A [telepítővarázslóval](set-up.md#deploy-office-365-client-apps)automatikusan telepítheti az Office-t a Windows-eszközökre.</span><span class="sxs-lookup"><span data-stu-id="75881-132">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="75881-133">A felhasználók telepíthetik a Windows és az eszközök [Office-alkalmazásait.](https://docs.microsoft.com/office365/admin/setup/install-applications)</span><span class="sxs-lookup"><span data-stu-id="75881-133">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="75881-134">Speciális</span><span class="sxs-lookup"><span data-stu-id="75881-134">Advanced</span></span>
- <span data-ttu-id="75881-135">**Új eszközök beállítása az Autopilot segítségével**</span><span class="sxs-lookup"><span data-stu-id="75881-135">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="75881-136">A [Windows Autopilot](add-autopilot-devices-and-profile.md) segítségével automatikusan előre konfigurálhatja az **új** Windows 10-es eszközöket egy felhasználó számára, de egyszerűbb lehet olyan [partnert](https://www.microsoft.com/solution-providers/search) szerezni, aki ezt megteheti Ön számára.</span><span class="sxs-lookup"><span data-stu-id="75881-136">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="75881-137">A [Microsoft Store-ban](https://go.microsoft.com/fwlink/?linkid=874598)is megnyithatja a Microsoft Store-t, és megkérhet egy felhőtechnológiai szakértőt, hogy állítson be új eszközöket.</span><span class="sxs-lookup"><span data-stu-id="75881-137">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), and ask a cloud technology expert to set up new devices that you purchase.</span></span>

- <span data-ttu-id="75881-138">**Helyszíni erőforrások elérése**</span><span class="sxs-lookup"><span data-stu-id="75881-138">**Access on-premises resources**</span></span>

     - <span data-ttu-id="75881-139">Ha a szervezet a helyszíni Windows Server Active Directoryt használja, beállíthatja a Microsoft 365 Business Premium rendszert a Windows 10-es eszközök védelmére, miközben továbbra is hozzáférhet a helyi hitelesítést igénylő helyszíni erőforrásokhoz.</span><span class="sxs-lookup"><span data-stu-id="75881-139">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="75881-140">A beállításhoz kövesse a [Tartományhoz csatlakozó Windows 10-eszközök Microsoft 365 Business Premium által idomainak engedélyezéséhez](manage-windows-devices.md) szükséges lépéseket.</span><span class="sxs-lookup"><span data-stu-id="75881-140">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="75881-141">Ez az előnyben részesített módszer, és az ilyen állapotban lévő eszközöket hibrid Azure AD-hez csatlakozó eszközöknek nevezzük.</span><span class="sxs-lookup"><span data-stu-id="75881-141">This is the preferred method, and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="75881-142">Ha a vállalkozás rendelkezik egy helyi Active Directoryval, amely néhány helyszíni erőforrást (például fájlmegosztásokat és nyomtatókat) tartalmaz, az Azure AD-hez csatlakoztatt eszközöknek hozzáférést adhat ezekhez az erőforrásokhoz az alábbi lépések végrehajtásával: [Helyszíni erőforrások elérése a Microsoft 365 Business Premium szolgáltatásban egy Azure AD-hez csatlakozott eszközről.](access-resources.md)</span><span class="sxs-lookup"><span data-stu-id="75881-142">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers), you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium](access-resources.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="75881-143">Lásd még</span><span class="sxs-lookup"><span data-stu-id="75881-143">See also</span></span>

[<span data-ttu-id="75881-144">Microsoft 365 üzleti oktatóvideók</span><span class="sxs-lookup"><span data-stu-id="75881-144">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)

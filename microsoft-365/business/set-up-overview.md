---
title: A beállítás áttekintése
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: A Microsoft 365 Business telepítési lépéseinek áttekintése.
ms.openlocfilehash: f531830bffbe1cb6ce4e39ee2ba12da5738a2684
ms.sourcegitcommit: 8c244b38c43dd00c4ef0102f8bed02ab36639a6b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39967623"
---
# <a name="overview-of-setup"></a><span data-ttu-id="5debb-103">A beállítás áttekintése</span><span class="sxs-lookup"><span data-stu-id="5debb-103">Overview of setup</span></span>

<span data-ttu-id="5debb-104">A telepítési lépések többsége elvégezhető a telepítővarázslóban, de a többi beállítás is listázható.</span><span class="sxs-lookup"><span data-stu-id="5debb-104">Most of the setup steps can be done in the setup wizard, but the other options are also listed.</span></span>

## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="5debb-105">1. lépés: a tartomány és a felhasználók hozzáadása</span><span class="sxs-lookup"><span data-stu-id="5debb-105">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="5debb-106">**[Add hozzá a domain](set-up.md#add-your-domain-to-personalize-sign-in)** (ha vásárolta a domain [regisztráció](sign-up.md)során, ez a lépés már megtörtént.)</span><span class="sxs-lookup"><span data-stu-id="5debb-106">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="5debb-107">**Hozzáadhatnak felhasználókat**.</span><span class="sxs-lookup"><span data-stu-id="5debb-107">**Add users**.</span></span> <span data-ttu-id="5debb-108">A felhasználókat háromféle módon adhatja hozzá a felhasználókhoz:</span><span class="sxs-lookup"><span data-stu-id="5debb-108">You can add users in any of the three ways:</span></span>
        - <span data-ttu-id="5debb-109">A [varázslóban](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="5debb-109">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="5debb-110">Ha intézményi Active Directory címtárral rendelkezik, a címtár-szinkronizálás segítségével [felhasználókat adhat hozzá az azúrkék ad Connect alkalmazással](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) .</span><span class="sxs-lookup"><span data-stu-id="5debb-110">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="5debb-111">Később az admin központban is [hozzáadhat felhasználókat](add-users-m365b.md) .</span><span class="sxs-lookup"><span data-stu-id="5debb-111">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="5debb-112">2. lépés: biztonsági házirendek beállítása és eszközök konfigurálása</span><span class="sxs-lookup"><span data-stu-id="5debb-112">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="5debb-113">Az eszközházirendek konfigurálásához használja a [telepítővarázslót](set-up.md#protect-your-organization) .</span><span class="sxs-lookup"><span data-stu-id="5debb-113">Use the [Setup wizard](set-up.md#protect-your-organization) to configure device policies.</span></span> 
  - <span data-ttu-id="5debb-114">Később az [Admin központban](view-policies-and-devices.md) és az [Intune portálon](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)is hozzáadhat további, vagy szerkesztheti azokat.</span><span class="sxs-lookup"><span data-stu-id="5debb-114">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="5debb-115">A telepítő varázsló emellett alapvető fenyegetettséget és adatvesztés-megelőzési beállításokat is beállít.</span><span class="sxs-lookup"><span data-stu-id="5debb-115">The setup wizard will also set up basic threat protection and data loss prevention settings.</span></span>
  
  <span data-ttu-id="5debb-116">A Beállításvarázsló biztonsági beállításai mellett a következő beállítások hozzáadásával növelheti biztonságát:</span><span class="sxs-lookup"><span data-stu-id="5debb-116">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>


- <span data-ttu-id="5debb-117">**E-mail malware-védelem**</span><span class="sxs-lookup"><span data-stu-id="5debb-117">**Email malware protection**</span></span>
- <span data-ttu-id="5debb-118">**ATP anti-phishing**</span><span class="sxs-lookup"><span data-stu-id="5debb-118">**ATP anti-phishing**</span></span>
- <span data-ttu-id="5debb-119">**Exchange Online Archiválás**</span><span class="sxs-lookup"><span data-stu-id="5debb-119">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="5debb-120">**Azure információvédelem (Plan1**)</span><span class="sxs-lookup"><span data-stu-id="5debb-120">**Azure Information Protection (Plan1**)</span></span>


<span data-ttu-id="5debb-121">A kezdéshez tekintse [meg a speciális biztonsági házirendeket](set-up-advanced-security.md).</span><span class="sxs-lookup"><span data-stu-id="5debb-121">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

<span data-ttu-id="5debb-122">Lásd még a [10 legjobb módja a Microsoft 365 Business biztonságának](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) a legjobb biztonsági gyakorlatok útitervében való biztonságossá tétele érdekében.</span><span class="sxs-lookup"><span data-stu-id="5debb-122">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="5debb-123">3. lépés: a Windows 10-eszközök beállítása és kezelése</span><span class="sxs-lookup"><span data-stu-id="5debb-123">Step 3: Set up and manage Windows 10 devices</span></span>

<span data-ttu-id="5debb-124">A varázsló futtatása után a szervezet összes Windwos 10 számítógépét be szeretné szerezni.</span><span class="sxs-lookup"><span data-stu-id="5debb-124">After you run the set up wizard, you will want to proctect all the Windwos 10 computers in your organization.</span></span>
  
- <span data-ttu-id="5debb-125">Windows 10 Profi van egy [előfeltétel](pre-requisites-for-data-protection.md) részére Mikroszkóp 365 teendő, de ha önnek van Windows 7 profi, Windows 8 profi, vagy Windows 8,1 Profi,-a aláírás feljogosítja ön-hoz egy [feljavít-hoz Windows 10 profi](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span><span class="sxs-lookup"><span data-stu-id="5debb-125">Windows 10 Pro is a [prerequisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
- <span data-ttu-id="5debb-126">Kövesse a [Windows 10 PC](secure-win-10-pcs.md) -k biztonságának lépéseit a Windows 10 eszközök házirendjeinek beállításához.</span><span class="sxs-lookup"><span data-stu-id="5debb-126">Follow the steps in [secure Windows 10 PCs](secure-win-10-pcs.md) to set up policies for Windows 10 devices.</span></span>

<span data-ttu-id="5debb-127">Amikor csatlakozunk egy Windows 10 készüléket Azure AD-hez, a Windows 10 számítógépeire beállított házirendek kerülnek alkalmazásra.</span><span class="sxs-lookup"><span data-stu-id="5debb-127">When you join a Windows 10 device to Azure AD, the policies you set for Windows 10 computers get applied to it.</span></span> <span data-ttu-id="5debb-128">További információ: a [Windows-eszközök beállítása a Microsoft 365 üzleti felhasználók](set-up-windows-devices.md)számára.</span><span class="sxs-lookup"><span data-stu-id="5debb-128">For more information, see [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md).</span></span>

## <a name="step-4-install-office-365-business"></a><span data-ttu-id="5debb-129">4. lépés: telepítse az Office 365 Business</span><span class="sxs-lookup"><span data-stu-id="5debb-129">Step 4: Install Office 365 Business</span></span>
- <span data-ttu-id="5debb-130">Az Office-eszközöket a [telepítővarázslóval](set-up.md#deploy-office-365-client-apps)automatikusan is telepítheti a Windows-eszközökön.</span><span class="sxs-lookup"><span data-stu-id="5debb-130">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="5debb-131">A felhasználók [telepíthetik az Office-alkalmazásokat](https://docs.microsoft.com/office365/admin/setup/install-applications) a Windows és az eszközök számára.</span><span class="sxs-lookup"><span data-stu-id="5debb-131">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="5debb-132">Speciális</span><span class="sxs-lookup"><span data-stu-id="5debb-132">Advanced</span></span>
- <span data-ttu-id="5debb-133">**A robotpilóta használata új eszközök beállításához**</span><span class="sxs-lookup"><span data-stu-id="5debb-133">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="5debb-134">A [Windows automatikus vezérlőt](add-autopilot-devices-and-profile.md) használhatja a felhasználó számára az **új** Windows 10 eszköz automatikus konfigurálására, de egyszerűbb lehet olyan [partnert](https://www.microsoft.com/solution-providers/search) kérni, aki ezt megteheti.</span><span class="sxs-lookup"><span data-stu-id="5debb-134">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="5debb-135">Tudod is megy [Mikroszkóp készlet](https://go.microsoft.com/fwlink/?linkid=874598), és kérdez egy felhő technológia szakértő-hoz felállít új berendezés amit ön megvásárol.</span><span class="sxs-lookup"><span data-stu-id="5debb-135">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), and ask a cloud technology expert to set up new devices that you purchase.</span></span>

- <span data-ttu-id="5debb-136">**Az intézményi erőforrások elérése**</span><span class="sxs-lookup"><span data-stu-id="5debb-136">**Access on-premises resources**</span></span>

     - <span data-ttu-id="5debb-137">Ha a szervezet helyi Windows Server Active Directoryt használ, beállíthatja a Microsoft 365 Business rendszert, hogy védje a Windows 10 eszközeit, miközben továbbra is fenntartja az intézményi erőforrásokhoz való hozzáférést, amelyekhez szükség van lokális hitelesítésre.</span><span class="sxs-lookup"><span data-stu-id="5debb-137">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="5debb-138">Hajtsa végre a [Microsoft 365 Business által felügyelt, tartományhoz csatlakoztatott Windows 10 eszközök engedélyezésére](manage-windows-devices.md) vonatkozó lépéseket.</span><span class="sxs-lookup"><span data-stu-id="5debb-138">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="5debb-139">Ez az előnyben részesített módszer, és az ebben az állapotban lévő eszközök elnevezése Hybrid Azure hirdetési egyesített eszközök.</span><span class="sxs-lookup"><span data-stu-id="5debb-139">This is the preferred method, and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="5debb-140">Ha vállalkozása olyan helyi Active Directoryval rendelkezik, amely intézményi erőforrásokat (például fájlmegosztásokat és nyomtatókat) is tartalmaz, akkor az Azure-alapú AD-összekapcsolt eszközök számára hozzáférést biztosít ezekhez az erőforrásokhoz az alábbi lépések végrehajtásával: [a Microsoft 365 Business egy Azure rendszerű ad-illesztett eszközből származó intézményi erőforrások elérése](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="5debb-140">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers), you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="5debb-141">See also</span><span class="sxs-lookup"><span data-stu-id="5debb-141">See also</span></span>

[<span data-ttu-id="5debb-142">Microsoft 365 üzleti képzési videók</span><span class="sxs-lookup"><span data-stu-id="5debb-142">Microsoft 365 Business training videos</span></span>](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)

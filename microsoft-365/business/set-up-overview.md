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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: A Microsoft 365 Business beállítási lépéseinek áttekintése.
ms.openlocfilehash: 07cbd4fd187f78474783db848ac9b69068d2b44a
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/29/2020
ms.locfileid: "41595065"
---
# <a name="overview-of-setup"></a><span data-ttu-id="4bd1f-103">A beállítás áttekintése</span><span class="sxs-lookup"><span data-stu-id="4bd1f-103">Overview of setup</span></span>

<span data-ttu-id="4bd1f-104">Nézzen meg egy rövid videót a Microsoft 365 Vállalati verzió beállításáról.</span><span class="sxs-lookup"><span data-stu-id="4bd1f-104">Watch a short video about Microsoft 365 Business setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

<span data-ttu-id="4bd1f-105">Ha hasznosnak találta ezt a videót, tekintse meg a [teljes tanfolyamok kisvállalatoknak és Microsoft 365-újoncoknak](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) című témakört.</span><span class="sxs-lookup"><span data-stu-id="4bd1f-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

<span data-ttu-id="4bd1f-106">A beállítási lépések többsége elvégezhető a telepítővarázslóban, de a többi beállítás is megjelenik a listában.</span><span class="sxs-lookup"><span data-stu-id="4bd1f-106">Most of the setup steps can be done in the setup wizard, but the other options are also listed.</span></span>

## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="4bd1f-107">1. lépés: Tartomány és felhasználók hozzáadása</span><span class="sxs-lookup"><span data-stu-id="4bd1f-107">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="4bd1f-108">**[Adja hozzá a tartományt](set-up.md#add-your-domain-to-personalize-sign-in)** (ha [a regisztráció](sign-up.md)során vásárolta meg a tartományt, ez a lépés már megtörtént.)</span><span class="sxs-lookup"><span data-stu-id="4bd1f-108">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="4bd1f-109">**Felhasználók hozzáadása**.</span><span class="sxs-lookup"><span data-stu-id="4bd1f-109">**Add users**.</span></span> <span data-ttu-id="4bd1f-110">A felhasználókat a következő három módszer közül választhatja ki:</span><span class="sxs-lookup"><span data-stu-id="4bd1f-110">You can add users in any of the three ways:</span></span>
        - <span data-ttu-id="4bd1f-111">A [varázslóban.](set-up.md#add-users-in-the-wizard)</span><span class="sxs-lookup"><span data-stu-id="4bd1f-111">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="4bd1f-112">A címtár-szinkronizálás használatával [felhasználókat vehet fel az Azure AD Connect használatával,](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) ha helyszíni Active directoryval rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="4bd1f-112">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="4bd1f-113">[Később is hozzáadhat felhasználókat](add-users-m365b.md) a felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="4bd1f-113">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="4bd1f-114">2. lépés: Biztonsági házirendek beállítása és eszközök konfigurálása</span><span class="sxs-lookup"><span data-stu-id="4bd1f-114">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="4bd1f-115">Az eszközházirendek konfigurálása a [Telepítő varázslóval.](set-up.md#protect-your-organization)</span><span class="sxs-lookup"><span data-stu-id="4bd1f-115">Use the [Setup wizard](set-up.md#protect-your-organization) to configure device policies.</span></span> 
  - <span data-ttu-id="4bd1f-116">Később további vagy szerkesztheti őket a [felügyeleti központban](view-policies-and-devices.md) és az [Intune-portálon.](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)</span><span class="sxs-lookup"><span data-stu-id="4bd1f-116">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="4bd1f-117">A telepítővarázsló beállítja az alapvető veszélyforrások elleni védelem és az adatvesztés-megelőzési beállításokat is.</span><span class="sxs-lookup"><span data-stu-id="4bd1f-117">The setup wizard will also set up basic threat protection and data loss prevention settings.</span></span>
  
  <span data-ttu-id="4bd1f-118">A telepítővarázsló biztonsági beállításai mellett a következő beállítások hozzáadásával növelheti a biztonságot:</span><span class="sxs-lookup"><span data-stu-id="4bd1f-118">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

- <span data-ttu-id="4bd1f-119">**Rosszindulatú programok elleni védelem e-mailben**</span><span class="sxs-lookup"><span data-stu-id="4bd1f-119">**Email malware protection**</span></span>
- <span data-ttu-id="4bd1f-120">**ATP adathalászat elleni**</span><span class="sxs-lookup"><span data-stu-id="4bd1f-120">**ATP anti-phishing**</span></span>
- <span data-ttu-id="4bd1f-121">**Exchange Online Archiválás**</span><span class="sxs-lookup"><span data-stu-id="4bd1f-121">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="4bd1f-122">**Azure Information Protection (1. terv**)</span><span class="sxs-lookup"><span data-stu-id="4bd1f-122">**Azure Information Protection (Plan1**)</span></span>

<span data-ttu-id="4bd1f-123">Első lépésekhez olvassa el a [fenyegetésvédelem növelése](increase-threat-protection.md) és [a megfelelőségi funkciók beállítása](set-up-compliance.md)című témakört.</span><span class="sxs-lookup"><span data-stu-id="4bd1f-123">To get started, see [increase threat protection](increase-threat-protection.md) and [set up compliance features](set-up-compliance.md).</span></span>

<span data-ttu-id="4bd1f-124">Tekintse meg a [Microsoft 365 Business 10 legfontosabb módját](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) a legjobb biztonsági eljárások ütemtervéhez.</span><span class="sxs-lookup"><span data-stu-id="4bd1f-124">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="4bd1f-125">3. lépés: Windows 10-es eszközök beállítása és kezelése</span><span class="sxs-lookup"><span data-stu-id="4bd1f-125">Step 3: Set up and manage Windows 10 devices</span></span>

<span data-ttu-id="4bd1f-126">A beállítási varázsló futtatása után érdemes ellátni a szervezet összes Windwos 10 számítógépét.</span><span class="sxs-lookup"><span data-stu-id="4bd1f-126">After you run the set up wizard, you will want to proctect all the Windwos 10 computers in your organization.</span></span>
  
- <span data-ttu-id="4bd1f-127">A Windows 10 Pro a Microsoft 365 Business [előfeltétele,](pre-requisites-for-data-protection.md) de ha Windows 7 Pro, Windows 8 Pro vagy Windows 8.1 Pro rendszert használ, az előfizetés feljogosítja Önt a [Windows 10 Pro rendszerre való frissítésre.](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update)</span><span class="sxs-lookup"><span data-stu-id="4bd1f-127">Windows 10 Pro is a [prerequisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
- <span data-ttu-id="4bd1f-128">A Windows [10 rendszerű számítógépek biztonságos](secure-win-10-pcs.md) védelmében a Windows 10-es eszközökre vonatkozó házirendek beállításához kövesse a lépéseket.</span><span class="sxs-lookup"><span data-stu-id="4bd1f-128">Follow the steps in [secure Windows 10 PCs](secure-win-10-pcs.md) to set up policies for Windows 10 devices.</span></span>

<span data-ttu-id="4bd1f-129">Amikor windows 10-es eszközt csatlakoztat az Azure AD-hez, a Windows 10-es számítógépekre beállított szabályzatok vonatkoznak rá.</span><span class="sxs-lookup"><span data-stu-id="4bd1f-129">When you join a Windows 10 device to Azure AD, the policies you set for Windows 10 computers get applied to it.</span></span> <span data-ttu-id="4bd1f-130">További információt [a Windows-eszközök beállítása a Microsoft 365 Vállalati verzió felhasználói számára](set-up-windows-devices.md)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="4bd1f-130">For more information, see [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md).</span></span>

## <a name="step-4-install-office-365-business"></a><span data-ttu-id="4bd1f-131">4. lépés: Az Office 365 Vállalati verzió telepítése</span><span class="sxs-lookup"><span data-stu-id="4bd1f-131">Step 4: Install Office 365 Business</span></span>
- <span data-ttu-id="4bd1f-132">Az Office automatikusan telepíthető a Windows-eszközökre a [telepítővarázsló segítségével.](set-up.md#deploy-office-365-client-apps)</span><span class="sxs-lookup"><span data-stu-id="4bd1f-132">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="4bd1f-133">Lehetővé teszi a felhasználók számára a Windows-alapú [Office-alkalmazások](https://docs.microsoft.com/office365/admin/setup/install-applications) és -eszközök telepítését.</span><span class="sxs-lookup"><span data-stu-id="4bd1f-133">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="4bd1f-134">Speciális</span><span class="sxs-lookup"><span data-stu-id="4bd1f-134">Advanced</span></span>
- <span data-ttu-id="4bd1f-135">**Új eszközök beállítása az Autopilot segítségével**</span><span class="sxs-lookup"><span data-stu-id="4bd1f-135">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="4bd1f-136">A [Windows Autopilot](add-autopilot-devices-and-profile.md) segítségével automatikusan előre konfigurálhatja az **új** Windows 10-es eszközöket a felhasználó számára, de egyszerűbb lehet olyan [partnert](https://www.microsoft.com/solution-providers/search) szerezni, aki ezt megteheti Ön számára.</span><span class="sxs-lookup"><span data-stu-id="4bd1f-136">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="4bd1f-137">A [Microsoft Store-ban](https://go.microsoft.com/fwlink/?linkid=874598)is megkérhet egy felhőtechnológiai szakértőt, hogy állítson be új, megvásárolt eszközöket.</span><span class="sxs-lookup"><span data-stu-id="4bd1f-137">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), and ask a cloud technology expert to set up new devices that you purchase.</span></span>

- <span data-ttu-id="4bd1f-138">**Helyszíni erőforrások elérése**</span><span class="sxs-lookup"><span data-stu-id="4bd1f-138">**Access on-premises resources**</span></span>

     - <span data-ttu-id="4bd1f-139">Ha szervezete a helyszínen használja a Windows Server Active Directoryt, beállíthatja a Microsoft 365 Business alkalmazást a Windows 10-es eszközök védelmére, miközben továbbra is hozzáférhet a helyi hitelesítést igénylő helyszíni erőforrásokhoz.</span><span class="sxs-lookup"><span data-stu-id="4bd1f-139">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="4bd1f-140">Kövesse a [Microsoft 365 Business által felügyelt tartományhoz csatlakozó Windows 10-eszközök engedélyezése](manage-windows-devices.md) című részt.</span><span class="sxs-lookup"><span data-stu-id="4bd1f-140">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="4bd1f-141">Ez az előnyben részesített módszer, és az ebben az állapotban lévő eszközöket hibrid Azure AD-csatlakozású eszközöknek nevezzük.</span><span class="sxs-lookup"><span data-stu-id="4bd1f-141">This is the preferred method, and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="4bd1f-142">Ha a vállalkozás a helyi Active Directory, amely tartalmaz néhány helyszíni erőforrások (például a fájlmegosztások és nyomtatók), adhat az Azure AD-csatlakozású eszközök hozzáférését ezekhez az erőforrásokhoz az alábbi lépéseket: Hozzáférés a helyszíni erőforrások egy [Azure AD-csatlakozású eszköz a Microsoft 365 Business.](access-resources.md)</span><span class="sxs-lookup"><span data-stu-id="4bd1f-142">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers), you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="4bd1f-143">Lásd még</span><span class="sxs-lookup"><span data-stu-id="4bd1f-143">See also</span></span>

[<span data-ttu-id="4bd1f-144">Microsoft 365 Vállalati verziós oktatóvideók</span><span class="sxs-lookup"><span data-stu-id="4bd1f-144">Microsoft 365 Business training videos</span></span>](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)

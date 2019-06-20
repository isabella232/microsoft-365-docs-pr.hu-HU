---
title: Beállítása – áttekintés
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: A Microsoft 365 üzleti lépések létrehozott áttekintése.
ms.openlocfilehash: ae7ed0aab36a6e759e0f0c1fbc3d3183273a284e
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/15/2019
ms.locfileid: "35086340"
---
# <a name="overview-of-setup"></a><span data-ttu-id="59b1d-103">A telepítő áttekintése</span><span class="sxs-lookup"><span data-stu-id="59b1d-103">Overview of setup</span></span>

<span data-ttu-id="59b1d-104">Lépéseket beállítása a legtöbb elvégezhető a telepítő varázsló, de az egyéb beállítások is szerepelnek.</span><span class="sxs-lookup"><span data-stu-id="59b1d-104">Most of the set up steps can be done in the setup wizard, but the other options are also listed.</span></span>


## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="59b1d-105">1. lépés: A tartomány és a felhasználó hozzáadása</span><span class="sxs-lookup"><span data-stu-id="59b1d-105">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="59b1d-106">**[A tartomány hozzáadása](set-up.md#add-your-domain-to-personalize-sign-in)** (a domain [regisztráció](sign-up.md)során vásárolt, ha ez a lépés már megtörtént.)</span><span class="sxs-lookup"><span data-stu-id="59b1d-106">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="59b1d-107">**Felhasználók hozzáadása**.</span><span class="sxs-lookup"><span data-stu-id="59b1d-107">**Add users**.</span></span> <span data-ttu-id="59b1d-108">Ez a három módokon teheti meg:</span><span class="sxs-lookup"><span data-stu-id="59b1d-108">You can do this in any of the three ways:</span></span>
        - <span data-ttu-id="59b1d-109">A [varázsló](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="59b1d-109">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="59b1d-110">Ha a helyszíni Active directory [Azure AD csatlakozás segítségével a felhasználók](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) hozzáadása a címtárszinkronizálás használata</span><span class="sxs-lookup"><span data-stu-id="59b1d-110">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="59b1d-111">Is [újabb felhasználók hozzáadása](add-users-m365b.md) a felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="59b1d-111">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="59b1d-112">2. lépés: Állítsa be a biztonsági házirendek és eszközök konfigurálása</span><span class="sxs-lookup"><span data-stu-id="59b1d-112">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="59b1d-113">A [telepítő varázsló](set-up.md#set-up-security-policies-and-device-configurations) segítségével konfigurálhatja az eszköz és a biztonsági házirendek.</span><span class="sxs-lookup"><span data-stu-id="59b1d-113">Use the [Setup wizard](set-up.md#set-up-security-policies-and-device-configurations) to configure device and security policies.</span></span> 
  - <span data-ttu-id="59b1d-114">Több hozzáadása vagy később a [felügyeleti központ](view-policies-and-devices.md) és az [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)szerkeszthetők is.</span><span class="sxs-lookup"><span data-stu-id="59b1d-114">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="59b1d-115">A telepítő varázsló a biztonsági beállítások mellett az alábbi beállítások hozzáadásával növelheti a biztonsági:</span><span class="sxs-lookup"><span data-stu-id="59b1d-115">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

      - <span data-ttu-id="59b1d-116">**E-mail rosszindulatú programok elleni védekezés**</span><span class="sxs-lookup"><span data-stu-id="59b1d-116">**Email malware protection**</span></span>
      - <span data-ttu-id="59b1d-117">**Speciális veszély védelmi (ATP) biztonságos kapcsolatok**</span><span class="sxs-lookup"><span data-stu-id="59b1d-117">**Advanced Threat Protection (ATP) Safe links**</span></span>
      - <span data-ttu-id="59b1d-118">**ATP biztonságos mellékletek**</span><span class="sxs-lookup"><span data-stu-id="59b1d-118">**ATP Safe Attachments**</span></span>
      - <span data-ttu-id="59b1d-119">**ATP-adathalászat**</span><span class="sxs-lookup"><span data-stu-id="59b1d-119">**ATP anti-phishing**</span></span>
      - <span data-ttu-id="59b1d-120">**Exchange Online Archiválás**</span><span class="sxs-lookup"><span data-stu-id="59b1d-120">**Exchange Online Archiving**</span></span>
      - <span data-ttu-id="59b1d-121">**Adatvesztés megelőzése (DLP)**</span><span class="sxs-lookup"><span data-stu-id="59b1d-121">**Data Loss Prevention (DLP)**</span></span>
      - <span data-ttu-id="59b1d-122">**Borzas információk védelméről (Plan1**)</span><span class="sxs-lookup"><span data-stu-id="59b1d-122">**Azure Information Protection (Plan1**)</span></span>

          <span data-ttu-id="59b1d-123">Get elindítani a [Speciális biztonsági házirendek beállítása](set-up-advanced-security.md)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="59b1d-123">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

        <span data-ttu-id="59b1d-124">Lásd még: [365 a Microsoft üzleti biztonságos felső 10 mód](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) a legjobb biztonsági gyakorlatok ütemterv.</span><span class="sxs-lookup"><span data-stu-id="59b1d-124">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="59b1d-125">3. lépés: Állítsa be, és a Windows 10 eszközök kezelése</span><span class="sxs-lookup"><span data-stu-id="59b1d-125">Step 3: Set up and manage Windows 10 devices</span></span>

   <span data-ttu-id="59b1d-126">Ha eszköz Windows 10 Azure ad, a házirendek beállítása a [2](#step-2-set-up-security-policies-and-configure-devices) a rendszer alkalmazza azt.</span><span class="sxs-lookup"><span data-stu-id="59b1d-126">When you join a Windows 10 device to Azure AD, the policies you set up in [Step 2](#step-2-set-up-security-policies-and-configure-devices) get applied to it.</span></span>

   - <span data-ttu-id="59b1d-127">Windows 10 Pro egy [előfeltételként](pre-requisites-for-data-protection.md) Microsoft 365 üzleti, de ha Windows 7 Pro, Windows 8 Pro vagy Pro Windows 8.1-, az előfizetés feljogosítja a, hogy [frissítsen a Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span><span class="sxs-lookup"><span data-stu-id="59b1d-127">Windows 10 Pro is a [pre-requisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
    - <span data-ttu-id="59b1d-128">A [telepítő varázsló](set-up.md#set-up-security-policies-and-device-configurations) segítségével konfigurálja a Windows 10 eszközök.</span><span class="sxs-lookup"><span data-stu-id="59b1d-128">Use the [setup wizard](set-up.md#set-up-security-policies-and-device-configurations) to configure policies for Windows 10 devices.</span></span>

## <a name="stes-4-install-office-365-business"></a><span data-ttu-id="59b1d-129">Stes 4: Telepítse az Office 365 üzleti</span><span class="sxs-lookup"><span data-stu-id="59b1d-129">Stes 4: Install Office 365 Business</span></span>
- <span data-ttu-id="59b1d-130">A [telepítő varázsló](set-up.md#deploy-office-365-client-apps)segítségével a Windows-eszközök automatikusan telepíthető Office.</span><span class="sxs-lookup"><span data-stu-id="59b1d-130">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="59b1d-131">Automatikusan [az Office telepítése](auto-install-or-uninstall-office.md) az admin center.</span><span class="sxs-lookup"><span data-stu-id="59b1d-131">Automatically [install Office](auto-install-or-uninstall-office.md) from the admin center.</span></span>
- <span data-ttu-id="59b1d-132">Lehetővé teszik a felhasználók [Office alkalmazások telepítése](https://docs.microsoft.com/office365/admin/setup/install-applications) a Windows és az eszközök.</span><span class="sxs-lookup"><span data-stu-id="59b1d-132">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="59b1d-133">Speciális</span><span class="sxs-lookup"><span data-stu-id="59b1d-133">Advanced</span></span>
- <span data-ttu-id="59b1d-134">**Automata segítségével állítsa be az új eszközök**</span><span class="sxs-lookup"><span data-stu-id="59b1d-134">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="59b1d-135">[Windows automata](add-autopilot-devices-and-profile.md) segítségével automatikusan előre konfigurálja egy felhasználó **Új** Windows 10 eszközök, de lehet egyszerűbben, egy [partner](https://www.microsoft.com/solution-providers/search) , aki teheti meg.</span><span class="sxs-lookup"><span data-stu-id="59b1d-135">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="59b1d-136">Ugrás a [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) is, és kérje meg a felhő technológia szakértői vásárol meg az új eszközök beállítása.</span><span class="sxs-lookup"><span data-stu-id="59b1d-136">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) and ask a cloud technology expert set up new devices you purchase for you.</span></span>

- <span data-ttu-id="59b1d-137">**Helyi erőforrások eléréséhez.**</span><span class="sxs-lookup"><span data-stu-id="59b1d-137">**Access on-premises resources**</span></span>

     - <span data-ttu-id="59b1d-138">Ha a szervezet használja a Windows Server Active Directory helyszíni, állíthat be Microsoft 365 üzleti védelme érdekében a Windows 10 eszközök továbbra is fenntartva helyi hitelesítést igénylő helyszíni erőforrásokhoz való hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="59b1d-138">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="59b1d-139">Kövesse a [Microsoft 365 üzleti által kezelt tartományhoz tartozó Windows 10 eszközök engedélyezése](manage-windows-devices.md) meg.</span><span class="sxs-lookup"><span data-stu-id="59b1d-139">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="59b1d-140">Ez a javasolt módszer és eszközök ebben az állapotban úgynevezett hibrid Azure AD eszközöket csatlakozott.</span><span class="sxs-lookup"><span data-stu-id="59b1d-140">This is the preferred method and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="59b1d-141">Ha a vállalatnál a helyi Active Directory, amely tartalmazza az egyes helyi erőforrásokat (például fájlmegosztásokat és nyomtatókat), a Borzas AD csatlakoztatott eszközök hozzáférést biztosíthat a forrásokhoz való lépések itt: [Access helyszíni erőforrásokat egy 365 üzleti Microsoft Azure AD csatlakozott eszköz](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="59b1d-141">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers) , you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

  
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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: A Microsoft 365 Business által létrehozott lépések áttekintése.
ms.openlocfilehash: f156d236a783942ec06d457c9b7ca087d12d6f58
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288575"
---
# <a name="overview-of-setup"></a><span data-ttu-id="e07e9-103">A beállítás áttekintése</span><span class="sxs-lookup"><span data-stu-id="e07e9-103">Overview of setup</span></span>

<span data-ttu-id="e07e9-104">A legtöbb beállítási lépés elvégezhető a telepítővarázslóban, de a többi beállítás is listázható.</span><span class="sxs-lookup"><span data-stu-id="e07e9-104">Most of the set up steps can be done in the setup wizard, but the other options are also listed.</span></span>


## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="e07e9-105">1. lépés: a tartomány és a felhasználók hozzáadása</span><span class="sxs-lookup"><span data-stu-id="e07e9-105">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="e07e9-106">**[Add hozzá a domain](set-up.md#add-your-domain-to-personalize-sign-in)** (ha vásárolta a domain [regisztráció](sign-up.md)során, ez a lépés már megtörtént.)</span><span class="sxs-lookup"><span data-stu-id="e07e9-106">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="e07e9-107">**Hozzáadhatnak felhasználókat**.</span><span class="sxs-lookup"><span data-stu-id="e07e9-107">**Add users**.</span></span> <span data-ttu-id="e07e9-108">Ezt megteheti a következő három módon:</span><span class="sxs-lookup"><span data-stu-id="e07e9-108">You can do this in any of the three ways:</span></span>
        - <span data-ttu-id="e07e9-109">A [varázslóban](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="e07e9-109">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="e07e9-110">Ha intézményi Active Directory címtárral rendelkezik, a címtár-szinkronizálás segítségével [felhasználókat adhat hozzá az azúrkék ad Connect alkalmazással](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) .</span><span class="sxs-lookup"><span data-stu-id="e07e9-110">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="e07e9-111">Később az admin központban is [hozzáadhat felhasználókat](add-users-m365b.md) .</span><span class="sxs-lookup"><span data-stu-id="e07e9-111">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="e07e9-112">2. lépés: biztonsági házirendek beállítása és eszközök konfigurálása</span><span class="sxs-lookup"><span data-stu-id="e07e9-112">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="e07e9-113">Az eszköz-és biztonsági házirendek konfigurálásához használja a [telepítővarázslót](set-up.md#set-up-security-policies-and-device-configurations) .</span><span class="sxs-lookup"><span data-stu-id="e07e9-113">Use the [Setup wizard](set-up.md#set-up-security-policies-and-device-configurations) to configure device and security policies.</span></span> 
  - <span data-ttu-id="e07e9-114">Később az [Admin központban](view-policies-and-devices.md) és az [Intune portálon](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal)is hozzáadhat további, vagy szerkesztheti azokat.</span><span class="sxs-lookup"><span data-stu-id="e07e9-114">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="e07e9-115">A Beállításvarázsló biztonsági beállításai mellett a következő beállítások hozzáadásával növelheti biztonságát:</span><span class="sxs-lookup"><span data-stu-id="e07e9-115">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

      - <span data-ttu-id="e07e9-116">**E-mail malware-védelem**</span><span class="sxs-lookup"><span data-stu-id="e07e9-116">**Email malware protection**</span></span>
      - <span data-ttu-id="e07e9-117">**Speciális Veszélyvédelmi (ATP) hivatkozások**</span><span class="sxs-lookup"><span data-stu-id="e07e9-117">**Advanced Threat Protection (ATP) Safe links**</span></span>
      - <span data-ttu-id="e07e9-118">**ATP-biztos mellékletek**</span><span class="sxs-lookup"><span data-stu-id="e07e9-118">**ATP Safe Attachments**</span></span>
      - <span data-ttu-id="e07e9-119">**ATP anti-phishing**</span><span class="sxs-lookup"><span data-stu-id="e07e9-119">**ATP anti-phishing**</span></span>
      - <span data-ttu-id="e07e9-120">**Exchange Online Archiválás**</span><span class="sxs-lookup"><span data-stu-id="e07e9-120">**Exchange Online Archiving**</span></span>
      - <span data-ttu-id="e07e9-121">**Adatvesztés megelőzése (DLP)**</span><span class="sxs-lookup"><span data-stu-id="e07e9-121">**Data Loss Prevention (DLP)**</span></span>
      - <span data-ttu-id="e07e9-122">**Azure információvédelem (Plan1**)</span><span class="sxs-lookup"><span data-stu-id="e07e9-122">**Azure Information Protection (Plan1**)</span></span>

          <span data-ttu-id="e07e9-123">A kezdéshez tekintse [meg a speciális biztonsági házirendeket](set-up-advanced-security.md).</span><span class="sxs-lookup"><span data-stu-id="e07e9-123">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

        <span data-ttu-id="e07e9-124">Lásd még a [10 legjobb módja a Microsoft 365 Business biztonságának](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) a legjobb biztonsági gyakorlatok útitervében való biztonságossá tétele érdekében.</span><span class="sxs-lookup"><span data-stu-id="e07e9-124">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="e07e9-125">3. lépés: a Windows 10-eszközök beállítása és kezelése</span><span class="sxs-lookup"><span data-stu-id="e07e9-125">Step 3: Set up and manage Windows 10 devices</span></span>

   <span data-ttu-id="e07e9-126">Amikor csatlakozunk egy Windows 10 készüléket Azure AD-hez, a [2](#step-2-set-up-security-policies-and-configure-devices) .</span><span class="sxs-lookup"><span data-stu-id="e07e9-126">When you join a Windows 10 device to Azure AD, the policies you set up in [Step 2](#step-2-set-up-security-policies-and-configure-devices) get applied to it.</span></span>

   - <span data-ttu-id="e07e9-127">Windows 10 Profi van egy [előtti-követelmény](pre-requisites-for-data-protection.md) részére Mikroszkóp 365 teendő, de ha önnek van Windows 7 profi, Windows 8 profi, vagy Windows 8,1 Profi,-a aláírás feljogosítja ön-hoz egy [feljavít-hoz Windows 10 profi](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span><span class="sxs-lookup"><span data-stu-id="e07e9-127">Windows 10 Pro is a [pre-requisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
    - <span data-ttu-id="e07e9-128">A Windows 10 eszközök házirendjeinek konfigurálásához használja a [telepítővarázslót](set-up.md#set-up-security-policies-and-device-configurations) .</span><span class="sxs-lookup"><span data-stu-id="e07e9-128">Use the [setup wizard](set-up.md#set-up-security-policies-and-device-configurations) to configure policies for Windows 10 devices.</span></span>

## <a name="stes-4-install-office-365-business"></a><span data-ttu-id="e07e9-129">Stes 4: telepítse az Office 365 Business</span><span class="sxs-lookup"><span data-stu-id="e07e9-129">Stes 4: Install Office 365 Business</span></span>
- <span data-ttu-id="e07e9-130">Az Office-eszközöket a [telepítővarázslóval](set-up.md#deploy-office-365-client-apps)automatikusan is telepítheti a Windows-eszközökön.</span><span class="sxs-lookup"><span data-stu-id="e07e9-130">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="e07e9-131">Gépiesen [felszerel hivatal](auto-install-or-uninstall-office.md) -ból admin központ.</span><span class="sxs-lookup"><span data-stu-id="e07e9-131">Automatically [install Office](auto-install-or-uninstall-office.md) from the admin center.</span></span>
- <span data-ttu-id="e07e9-132">A felhasználók [telepíthetik az Office-alkalmazásokat](https://docs.microsoft.com/office365/admin/setup/install-applications) a Windows és az eszközök számára.</span><span class="sxs-lookup"><span data-stu-id="e07e9-132">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="e07e9-133">Speciális</span><span class="sxs-lookup"><span data-stu-id="e07e9-133">Advanced</span></span>
- <span data-ttu-id="e07e9-134">**A robotpilóta használata új eszközök beállításához**</span><span class="sxs-lookup"><span data-stu-id="e07e9-134">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="e07e9-135">A [Windows automatikus vezérlőt](add-autopilot-devices-and-profile.md) használhatja a felhasználó számára az **új** Windows 10 eszköz automatikus konfigurálására, de egyszerűbb lehet olyan [partnert](https://www.microsoft.com/solution-providers/search) kérni, aki ezt megteheti.</span><span class="sxs-lookup"><span data-stu-id="e07e9-135">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="e07e9-136">Ön is látogasson el a [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) , és kérje a felhő-technológiai szakértő létrehozott új eszközöket vásárol az Ön számára.</span><span class="sxs-lookup"><span data-stu-id="e07e9-136">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) and ask a cloud technology expert set up new devices you purchase for you.</span></span>

- <span data-ttu-id="e07e9-137">**Az intézményi erőforrások elérése**</span><span class="sxs-lookup"><span data-stu-id="e07e9-137">**Access on-premises resources**</span></span>

     - <span data-ttu-id="e07e9-138">Ha a szervezet helyi Windows Server Active Directoryt használ, beállíthatja a Microsoft 365 Business rendszert, hogy védje a Windows 10 eszközeit, miközben továbbra is fenntartja az intézményi erőforrásokhoz való hozzáférést, amelyekhez szükség van lokális hitelesítésre.</span><span class="sxs-lookup"><span data-stu-id="e07e9-138">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="e07e9-139">Hajtsa végre a [Microsoft 365 Business által felügyelt, tartományhoz csatlakoztatott Windows 10 eszközök engedélyezésére](manage-windows-devices.md) vonatkozó lépéseket.</span><span class="sxs-lookup"><span data-stu-id="e07e9-139">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="e07e9-140">Ez az adott állapotú módszer és eszközök a hibrid Azure rendszerű hirdetési eszközök.</span><span class="sxs-lookup"><span data-stu-id="e07e9-140">This is the preferred method and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="e07e9-141">Ha vállalkozása olyan helyi Active Directoryval rendelkezik, amely intézményi erőforrásokat (például fájlmegosztásokat vagy nyomtatókat) tartalmaz, akkor az azúrkék AD-illesztett eszközök ezekhez az erőforrásokhoz való hozzáférését az alábbi lépések végrehajtásával adhatja meg: az [intézményi erőforrások elérése egy Azúrkék hirdetés-összekapcsolt berendezés-ban Mikroszkóp 365 teendő](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="e07e9-141">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers) , you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

  
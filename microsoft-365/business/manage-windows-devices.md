---
title: Tartományhoz csatlakozott Windows 10-es eszközök microsoft 365 vállalati verziós kezelésének engedélyezése
f1.keywords:
- CSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Megtudhatja, hogy miként engedélyezheti a Microsoft 365 számára a helyi Active Directoryhoz csatlakozott Windows 10-eszközök védelmét néhány lépésben.
ms.openlocfilehash: 6275c6c4be9cd9631ab095f8b0e1b39683022bb2
ms.sourcegitcommit: d988faa292c2661ffea43c7161aef92b2b4b99bc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/04/2020
ms.locfileid: "46560843"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="d58cb-103">A tartományhoz csatlakozó Windows 10-eszközök Microsoft 365 Business Premium általi kezelésének engedélyezése</span><span class="sxs-lookup"><span data-stu-id="d58cb-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="d58cb-104">Ha a szervezet a helyszíni Windows Server Active Directoryt használja, beállíthatja a Microsoft 365 Business Premium rendszert a Windows 10-es eszközök védelmére, miközben továbbra is hozzáférhet a helyi hitelesítést igénylő helyszíni erőforrásokhoz.</span><span class="sxs-lookup"><span data-stu-id="d58cb-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="d58cb-105">A védelem beállításához hibrid **Azure AD-hez csatlakozott eszközöket**valósíthat meg.</span><span class="sxs-lookup"><span data-stu-id="d58cb-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="d58cb-106">Ezek az eszközök a helyszíni Active Directoryhoz és az Azure Active Directoryhoz is csatlakoznak.</span><span class="sxs-lookup"><span data-stu-id="d58cb-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="d58cb-107">Ez a videó bemutatja, hogyan állíthatja be ezt a leggyakoribb forgatókönyvhöz, amelyet a következő lépések is részleteznek.</span><span class="sxs-lookup"><span data-stu-id="d58cb-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="d58cb-108">Mielőtt elkezdene, végezze el az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="d58cb-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="d58cb-109">Szinkronizálja a felhasználókat az Azure AD-vel az Azure AD Connect segítségével.</span><span class="sxs-lookup"><span data-stu-id="d58cb-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="d58cb-110">Teljes Azure AD Connect szervezeti egység (OU) szinkronizálás.</span><span class="sxs-lookup"><span data-stu-id="d58cb-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="d58cb-111">Győződjön meg arról, hogy a szinkronizált tartomány összes felhasználója rendelkezik licenccel a Microsoft 365 Business Premium szolgáltatáshoz.</span><span class="sxs-lookup"><span data-stu-id="d58cb-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="d58cb-112">A lépésekről a [Tartományfelhasználók szinkronizálása a Microsofthoz](manage-domain-users.md) című témakörben található.</span><span class="sxs-lookup"><span data-stu-id="d58cb-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="d58cb-113">1. Az MDM-szolgáltató ellenőrzése az Intune-ban</span><span class="sxs-lookup"><span data-stu-id="d58cb-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="d58cb-114">Nyissa meg az [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) lapot, és a Microsoft Intune lapon válassza az **Eszközregisztráció**lehetőséget, majd az **Áttekintés** lapon győződjön meg arról, hogy az **MDM-szolgáltató** **intune-i.**</span><span class="sxs-lookup"><span data-stu-id="d58cb-114">Go to [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) and on the Microsoft Intune page, select **Device enrollment**, then on the **Overview** page, make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="d58cb-115">Ha az **MDM-szolgáltató** **nincs,** kattintson az **MDM-szolgáltatóra** az **Intune**beállításához.</span><span class="sxs-lookup"><span data-stu-id="d58cb-115">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="d58cb-116">Ha az **MDM-szolgáltató** **a Microsoft Office 365**, nyissa meg az **Eszközök**  >  **regisztrálása eszközök,** és használja a **Add MDM hatóság** párbeszéd a jobb oldalon, hogy adjunk **Intune MDM** hatóság (a **Add MDM-szolgáltató** párbeszédpanel csak akkor érhető el, ha az **MDM-szolgáltató** van beállítva a Microsoft Office 365).</span><span class="sxs-lookup"><span data-stu-id="d58cb-116">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="d58cb-117">2. Ellenőrizze, hogy az Azure AD engedélyezve van-e a számítógépek hez való csatlakozáshoz</span><span class="sxs-lookup"><span data-stu-id="d58cb-117">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="d58cb-118">Nyissa meg a felügyeleti központot, <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> és válassza az Azure Active **Directory** (válassza az összes megjelenítése, ha az Azure Active Directory nem látható) a **Felügyeleti központok** listájában.</span><span class="sxs-lookup"><span data-stu-id="d58cb-118">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="d58cb-119">Az **Azure Active Directory felügyeleti központban**nyissa meg az Azure Active **Directoryt,** válassza **az Eszközök,** majd **az Eszközbeállítások lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="d58cb-119">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="d58cb-120">Annak**ellenőrzése, hogy a felhasználók csatlakozhatnak-e az Azure AD-hez,** engedélyezve van-e</span><span class="sxs-lookup"><span data-stu-id="d58cb-120">Verify**Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="d58cb-121">Az összes felhasználó engedélyezéséhez állítsa az **Összes**beállítását.</span><span class="sxs-lookup"><span data-stu-id="d58cb-121">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="d58cb-122">Adott felhasználók engedélyezéséhez állítsa **a Kijelölt** beállítást egy adott felhasználói csoport engedélyezéséhez.</span><span class="sxs-lookup"><span data-stu-id="d58cb-122">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="d58cb-123">Adja hozzá az Azure AD-ben szinkronizált kívánt tartományi felhasználókat egy [biztonsági csoporthoz.](../admin/create-groups/create-groups.md)</span><span class="sxs-lookup"><span data-stu-id="d58cb-123">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="d58cb-124">Válassza **a Csoportok kijelölése** lehetőséget az MDM felhasználói hatókörének engedélyezéséhez az adott biztonsági csoporthoz.</span><span class="sxs-lookup"><span data-stu-id="d58cb-124">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="d58cb-125">3. Ellenőrizze, hogy az Azure AD engedélyezve van-e az MDM-hez</span><span class="sxs-lookup"><span data-stu-id="d58cb-125">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="d58cb-126">Lépjen a felügyeleti központba, <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> és válassza a **Végpontkezelők**t lehetőséget (válassza **az Összes megjelenítése** lehetőséget, ha az **Endpoint Manager** nem látható)</span><span class="sxs-lookup"><span data-stu-id="d58cb-126">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen**t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="d58cb-127">A **Microsoft Endpoint Manager felügyeleti központban**nyissa meg **az Eszközök**  >  **windows**  >  **Windows-igénylés**  >  **automatikus igénylése**című lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="d58cb-127">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="d58cb-128">Ellenőrizze, hogy az MDM felhasználói hatóköre engedélyezve van-e.</span><span class="sxs-lookup"><span data-stu-id="d58cb-128">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="d58cb-129">Az összes számítógép igényléséhez állítsa az **Összes** beállításra, hogy automatikusan regisztráljon minden olyan felhasználói számítógépet, amely az Azure AD-hez és az új számítógépekhez csatlakozik, amikor a felhasználók munkahelyi fiókot adnak hozzá a Windowshoz.</span><span class="sxs-lookup"><span data-stu-id="d58cb-129">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="d58cb-130">A **Bizonyos** beállításra a felhasználók egy adott csoportjának számítógépeinek regisztrálására.</span><span class="sxs-lookup"><span data-stu-id="d58cb-130">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="d58cb-131">Adja hozzá az Azure AD-ben szinkronizált kívánt tartományi felhasználókat egy [biztonsági csoporthoz.](../admin/create-groups/create-groups.md)</span><span class="sxs-lookup"><span data-stu-id="d58cb-131">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="d58cb-132">Válassza **a Csoportok kijelölése** lehetőséget az MDM felhasználói hatókörének engedélyezéséhez az adott biztonsági csoporthoz.</span><span class="sxs-lookup"><span data-stu-id="d58cb-132">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-create-the-required-resources"></a><span data-ttu-id="d58cb-133">4. A szükséges erőforrások létrehozása</span><span class="sxs-lookup"><span data-stu-id="d58cb-133">4. Create the required resources</span></span> 

<span data-ttu-id="d58cb-134">A [hibrid Azure AD-illesztés konfigurálásához](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) szükséges feladatok végrehajtása leegyszerűsödött a [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell modulban található [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) parancsmag használatával.</span><span class="sxs-lookup"><span data-stu-id="d58cb-134">Performing the required tasks to [configure hybrid Azure AD join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) has been simplified through the use of the [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet found in the [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell module.</span></span> <span data-ttu-id="d58cb-135">A parancsmag meghívásakor létrehozza és konfigurálja a szükséges szolgáltatáscsatlakozási pontot és csoportházirendet.</span><span class="sxs-lookup"><span data-stu-id="d58cb-135">When you invoke this cmdlet it will create and configure the required service connection point and group policy.</span></span>

<span data-ttu-id="d58cb-136">Ezt a modult a PowerShell egy példányából a következő meghívással telepítheti:</span><span class="sxs-lookup"><span data-stu-id="d58cb-136">You can install this module by invoking the following from an instance of PowerShell:</span></span>

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> <span data-ttu-id="d58cb-137">Javasoljuk, hogy telepítse ezt a modult a Windows Server azure AD Connect futó.</span><span class="sxs-lookup"><span data-stu-id="d58cb-137">It is recommended that you install this module on the Windows Server running Azure AD Connect.</span></span>

<span data-ttu-id="d58cb-138">A szükséges szolgáltatáscsatlakozási pont és csoportházirend létrehozásához meg kell hívnia az [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) parancsmamot.</span><span class="sxs-lookup"><span data-stu-id="d58cb-138">To create the required service connection point and group policy, you will invoke the  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet.</span></span> <span data-ttu-id="d58cb-139">A feladat végrehajtásakor szüksége lesz a Microsoft 365 Business Premium globális rendszergazdai hitelesítő adataira.</span><span class="sxs-lookup"><span data-stu-id="d58cb-139">You will need your Microsoft 365 Business Premium global admin credentials when performing this task.</span></span> <span data-ttu-id="d58cb-140">Ha készen áll az erőforrások létrehozására, hívja meg a következőket:</span><span class="sxs-lookup"><span data-stu-id="d58cb-140">When you are ready to create the resources, invoke the following:</span></span>

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

<span data-ttu-id="d58cb-141">Az első parancs kapcsolatot létesít a Microsoft felhőjével, és amikor a rendszer kéri, adja meg a Microsoft 365 Business Premium globális rendszergazdai hitelesítő adatait.</span><span class="sxs-lookup"><span data-stu-id="d58cb-141">The first command will establish a connection with the Microsoft cloud, and when you are prompted, specify your Microsoft 365 Business Premium global admin credentials.</span></span>

## <a name="5-link-the-group-policy"></a><span data-ttu-id="d58cb-142">5. A csoportházirend összekapcsolása</span><span class="sxs-lookup"><span data-stu-id="d58cb-142">5. Link the Group Policy</span></span>

1. <span data-ttu-id="d58cb-143">A Csoportházirend kezelése konzolon (GPMC) kattintson a jobb gombbal arra a helyre, ahol össze szeretné kapcsolni a házirendet, és válassza a Helyi menü *Meglévő csoportházirend-házirendjének csatolása parancsot.*</span><span class="sxs-lookup"><span data-stu-id="d58cb-143">In the Group Policy Management Console (GPMC), right-click on the location where you want to link the policy and select *Link an existing GPO...* from the context menu.</span></span>
2. <span data-ttu-id="d58cb-144">Jelölje ki a fenti lépésben létrehozott házirendet, majd kattintson az **OK**gombra.</span><span class="sxs-lookup"><span data-stu-id="d58cb-144">Select the policy created in the above step, then click **OK**.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="d58cb-145">A legújabb felügyeleti sablonok beszerezhetése</span><span class="sxs-lookup"><span data-stu-id="d58cb-145">Get the latest Administrative Templates</span></span>

<span data-ttu-id="d58cb-146">Ha nem látja az **Automatikus MDM-regisztráció engedélyezése az alapértelmezett Azure AD-hitelesítő adatokkal című házirendet,** annak az lehet az oka, hogy nincs telepítve az ADMX a Windows 10, 1803-as, 1803-as vagy 1903-as verzióhoz.</span><span class="sxs-lookup"><span data-stu-id="d58cb-146">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, version 1809, or version 1903.</span></span> <span data-ttu-id="d58cb-147">A probléma megoldásához kövesse az alábbi lépéseket (Megjegyzés: a legújabb MDM.admx visszafelé kompatibilis):</span><span class="sxs-lookup"><span data-stu-id="d58cb-147">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="d58cb-148">Letöltés: [Felügyeleti sablonok (.admx) a Windows 10 2019 májusi frissítéséhez (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span><span class="sxs-lookup"><span data-stu-id="d58cb-148">Download: [Administrative Templates (.admx) for Windows 10 May 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span></span>
2.  <span data-ttu-id="d58cb-149">Telepítse a csomagot az elsődleges tartományvezérlőre (PDC).</span><span class="sxs-lookup"><span data-stu-id="d58cb-149">Install the package on the Primary Domain Controller (PDC).</span></span>
3.  <span data-ttu-id="d58cb-150">Navigálás a mappa verziójától függően: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span><span class="sxs-lookup"><span data-stu-id="d58cb-150">Navigate, depending on the version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span></span>
4.  <span data-ttu-id="d58cb-151">Nevezze át a **Házirenddefiníciók mappát** a **PolicyDefinitions**fenti elérési útján.</span><span class="sxs-lookup"><span data-stu-id="d58cb-151">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="d58cb-152">A **PolicyDefinitions** mappa másolása a **C:\Windows\SYSVOL\domain\Policies mappába.**</span><span class="sxs-lookup"><span data-stu-id="d58cb-152">Copy **PolicyDefinitions** folder to **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="d58cb-153">Ha a teljes tartományközponti házirend-tárolót kíván használni, adja hozzá a PolicyDefinitions tartalmát.</span><span class="sxs-lookup"><span data-stu-id="d58cb-153">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="d58cb-154">Indítsa újra az elsődleges tartományvezérlőt, hogy a házirend elérhető legyen.</span><span class="sxs-lookup"><span data-stu-id="d58cb-154">Restart the Primary Domain Controller for the policy to be available.</span></span> <span data-ttu-id="d58cb-155">Ez eljárás akarat dolgozik részére akármi jövő változat jól.</span><span class="sxs-lookup"><span data-stu-id="d58cb-155">This procedure will work for any future version as well.</span></span>

<span data-ttu-id="d58cb-156">Ezen a ponton látnia kell a házirend **automatikus MDM-regisztráció engedélyezése az alapértelmezett Azure AD hitelesítő adatok elérhető** használatával.</span><span class="sxs-lookup"><span data-stu-id="d58cb-156">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>

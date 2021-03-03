---
title: A tartományhoz csatlakozott Windows 10-es eszközök kezelése a Microsoft 365 Vállalati verzióval
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
description: Megtudhatja, hogyan engedélyezheti a Microsoft 365-nek, hogy mindössze néhány lépésben védje a helyi Active Directoryhoz csatlakozott Windows 10-es eszközöket.
ms.openlocfilehash: 0b597110447272be128bfe1866234ac25a8e67e6
ms.sourcegitcommit: 070724118be25cd83418d2a56863da95582dae65
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/03/2021
ms.locfileid: "50407078"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="edc71-103">A tartományhoz csatlakozott Windows 10-es eszközök kezelése a Microsoft 365 Vállalati prémium verzióval</span><span class="sxs-lookup"><span data-stu-id="edc71-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="edc71-104">Ha szervezete helyszíni Windows Server Active Directoryt használ, beállíthatja a Microsoft 365 Vállalati prémium verzióban a Windows 10-es eszközök védelmét, miközben továbbra is hozzáférhet a helyi hitelesítést igénylő helyszíni erőforrásokhoz.</span><span class="sxs-lookup"><span data-stu-id="edc71-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="edc71-105">A védelem beállításához hibrid Azure AD-hez csatlakozott eszközöket **kell implementálja.**</span><span class="sxs-lookup"><span data-stu-id="edc71-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="edc71-106">Ezek az eszközök a helyszíni Active Directoryhoz és az Azure Active Directoryhoz is csatlakoznak.</span><span class="sxs-lookup"><span data-stu-id="edc71-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="edc71-107">Ebből a videóból megtudhatja, hogy miként állíthatja be ezt a leggyakoribb forgatókönyvhöz, amely az alábbi lépésekben is részletesen le van írják.</span><span class="sxs-lookup"><span data-stu-id="edc71-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="edc71-108">Mielőtt neki kezd, győződjön meg arról, hogy a következő lépéseket kell végrehajtania:</span><span class="sxs-lookup"><span data-stu-id="edc71-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="edc71-109">Szinkronizálja a felhasználókat az Azure AD-be az Azure AD Connect segítségével.</span><span class="sxs-lookup"><span data-stu-id="edc71-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="edc71-110">Az Azure AD Connect szervezeti egység (OU) szinkronizálásának befejezése.</span><span class="sxs-lookup"><span data-stu-id="edc71-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="edc71-111">Győződjön meg arról, hogy a szinkronizált összes tartományi felhasználó rendelkezik Licenccel a Microsoft 365 Vállalati prémium verzióhoz.</span><span class="sxs-lookup"><span data-stu-id="edc71-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="edc71-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span><span class="sxs-lookup"><span data-stu-id="edc71-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="edc71-113">1. A MDM Authority ellenőrzése az Intune-ban</span><span class="sxs-lookup"><span data-stu-id="edc71-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="edc71-114">A [Végpontkezelőben](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) a Microsoft Intune lapon válassza az Eszköz regisztrálása **lehetőséget,** majd az **Áttekintés** lapon győződjön meg arról, hogy az **MDM-felügyelet** **Intune.**</span><span class="sxs-lookup"><span data-stu-id="edc71-114">Go to [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) and on the Microsoft Intune page, select **Device enrollment**, then on the **Overview** page, make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="edc71-115">Ha **a MDM authority (MDM authority** is None) (Nincs) **beállításhoz** kattintson az **MDM-hez,** és állítsa **be Intune-ra.**</span><span class="sxs-lookup"><span data-stu-id="edc71-115">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="edc71-116">Ha a Microsoft **Office 365-ös**  **MDM-hitelesítést** használja, az Eszközök regisztrálása eszközre ugrás után vegye fel az Intune MDM-hatót a jobb oldalon található MDM authority (Az MDM-felügyelet hozzáadása párbeszédpanel csak akkor érhető el, ha a  >   **MDM Authority** beállítása Microsoft Office 365).   </span><span class="sxs-lookup"><span data-stu-id="edc71-116">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="edc71-117">2. Annak ellenőrzése, hogy az Azure AD engedélyezve van-e a számítógépekhez való csatlakozáshoz</span><span class="sxs-lookup"><span data-stu-id="edc71-117">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="edc71-118">A Felügyeleti központok listában válassza az Azure Active Directory felügyeleti központját (válassza az Összes megjelenítése, ha az Azure Active Directory nem <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> látható) lehetőséget.  </span><span class="sxs-lookup"><span data-stu-id="edc71-118">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="edc71-119">Az **Azure Active Directory Felügyeleti központban** válassza az **Azure Active Directory** lehetőséget, válassza az **Eszközök,** majd az **Eszközbeállítások lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="edc71-119">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="edc71-120">Annak ellenőrzése, hogy a **Felhasználók csatlakozhatnak-e** az Azure AD-hez, engedélyezve van-e</span><span class="sxs-lookup"><span data-stu-id="edc71-120">Verify **Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="edc71-121">Ha az összes felhasználót engedélyezni szeretné, állítsa a **Mind beállításra.**</span><span class="sxs-lookup"><span data-stu-id="edc71-121">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="edc71-122">Ha csak bizonyos felhasználókat szeretné engedélyezni, állítsa **a Bejelölve** beállítást a felhasználók egy adott csoportjának engedélyezéséhez.</span><span class="sxs-lookup"><span data-stu-id="edc71-122">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="edc71-123">Adja hozzá az Azure AD-ban szinkronizált kívánt tartományfelhasználót egy [biztonsági csoporthoz.](../admin/create-groups/create-groups.md)</span><span class="sxs-lookup"><span data-stu-id="edc71-123">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="edc71-124">Válassza **a Csoportok kiválasztása lehetőséget,** ha engedélyezni szeretné az MDM-felhasználó hatókörét az adott biztonsági csoportban.</span><span class="sxs-lookup"><span data-stu-id="edc71-124">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="edc71-125">3. Annak ellenőrzése, hogy az Azure AD engedélyezve van-e az MDM-hez</span><span class="sxs-lookup"><span data-stu-id="edc71-125">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="edc71-126">Menjen a felügyeleti központba, és válassza a Végpontkezelő t lehetőséget (válassza az Összes megjelenítése, ha nem látható a <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  **Végpontkezelő)** lehetőséget. </span><span class="sxs-lookup"><span data-stu-id="edc71-126">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen** t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="edc71-127">A **Microsoft Endpoint Manager Felügyeleti központban** a Windows-regisztráció automatikus beléptetése eszközcsoportot kell  >    >    >  **látnia.**</span><span class="sxs-lookup"><span data-stu-id="edc71-127">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="edc71-128">Ellenőrizze, hogy engedélyezve van-e az MDM felhasználói hatóköre.</span><span class="sxs-lookup"><span data-stu-id="edc71-128">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="edc71-129">Ha az összes számítógépet  regisztrálnia kell, állítsa Az összes beállításra úgy, hogy automatikusan regisztrálja az Azure AD-hez és az új számítógépekhez csatlakozott összes felhasználói számítógépet, amikor a felhasználók munkahelyi fiókot adnak hozzá a Windowshoz.</span><span class="sxs-lookup"><span data-stu-id="edc71-129">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="edc71-130">A **"Néhány" beállításra** beállítva regisztrálja egy adott felhasználócsoport számítógépeit.</span><span class="sxs-lookup"><span data-stu-id="edc71-130">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="edc71-131">Adja hozzá az Azure AD-ban szinkronizált kívánt tartományfelhasználót egy [biztonsági csoporthoz.](../admin/create-groups/create-groups.md)</span><span class="sxs-lookup"><span data-stu-id="edc71-131">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="edc71-132">Válassza **a Csoportok kiválasztása lehetőséget,** ha engedélyezni szeretné az MDM-felhasználó hatókörét az adott biztonsági csoportban.</span><span class="sxs-lookup"><span data-stu-id="edc71-132">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-create-the-required-resources"></a><span data-ttu-id="edc71-133">4. A szükséges erőforrások létrehozása</span><span class="sxs-lookup"><span data-stu-id="edc71-133">4. Create the required resources</span></span> 

<span data-ttu-id="edc71-134">A hibrid Azure [AD-illesztés](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) konfigurálására vonatkozó szükséges feladatok végrehajtása egyszerűbbé lett a [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell modulban található [Inicializálás-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) parancsmag használatával.</span><span class="sxs-lookup"><span data-stu-id="edc71-134">Performing the required tasks to [configure hybrid Azure AD join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) has been simplified through the use of the [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet found in the [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell module.</span></span> <span data-ttu-id="edc71-135">Amikor meghívja ezt a parancsmagot, a parancsmag létrehozza és konfigurálja a szükséges szolgáltatási csatlakozási pontot és csoportházirendet.</span><span class="sxs-lookup"><span data-stu-id="edc71-135">When you invoke this cmdlet it will create and configure the required service connection point and group policy.</span></span>

<span data-ttu-id="edc71-136">A modult a PowerShell egy példányából az alábbi meg invoking segítségével telepítheti:</span><span class="sxs-lookup"><span data-stu-id="edc71-136">You can install this module by invoking the following from an instance of PowerShell:</span></span>

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> <span data-ttu-id="edc71-137">Javasoljuk, hogy telepítse ezt a modult az Azure AD Connectet futtató Windows Serveren.</span><span class="sxs-lookup"><span data-stu-id="edc71-137">It is recommended that you install this module on the Windows Server running Azure AD Connect.</span></span>

<span data-ttu-id="edc71-138">A szükséges szolgáltatási csatlakozási pont és csoportházirend létrehozásához meg kell hívnia az  [Inicializálás-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) parancsmagot.</span><span class="sxs-lookup"><span data-stu-id="edc71-138">To create the required service connection point and group policy, you will invoke the  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet.</span></span> <span data-ttu-id="edc71-139">A feladat végrehajtásához szüksége lesz a Microsoft 365 Vállalati prémium verzió globális rendszergazdai hitelesítő adataira.</span><span class="sxs-lookup"><span data-stu-id="edc71-139">You will need your Microsoft 365 Business Premium global admin credentials when performing this task.</span></span> <span data-ttu-id="edc71-140">Ha készen áll az erőforrások létrehozására, hívja meg az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="edc71-140">When you are ready to create the resources, invoke the following:</span></span>

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

<span data-ttu-id="edc71-141">Az első parancs kapcsolatot létesít a Microsoft felhővel, és amikor a rendszer kéri, adja meg a Microsoft 365 Vállalati prémium verzió globális rendszergazdai hitelesítő adatait.</span><span class="sxs-lookup"><span data-stu-id="edc71-141">The first command will establish a connection with the Microsoft cloud, and when you are prompted, specify your Microsoft 365 Business Premium global admin credentials.</span></span>

## <a name="5-link-the-group-policy"></a><span data-ttu-id="edc71-142">5. A csoportházirend összekapcsolása</span><span class="sxs-lookup"><span data-stu-id="edc71-142">5. Link the Group Policy</span></span>

1. <span data-ttu-id="edc71-143">A Csoportházirend kezelése konzolon (GPMC) kattintson a jobb gombbal arra a helyre, ahol a házirendet össze szeretné csatolni, és válassza a Helyi menü Meglévő *csoportházirend-objektum* csatolása parancsát.</span><span class="sxs-lookup"><span data-stu-id="edc71-143">In the Group Policy Management Console (GPMC), right-click on the location where you want to link the policy and select *Link an existing GPO...* from the context menu.</span></span>
2. <span data-ttu-id="edc71-144">Jelölje ki a fenti lépésben létrehozott házirendet, majd kattintson az **OK gombra.**</span><span class="sxs-lookup"><span data-stu-id="edc71-144">Select the policy created in the above step, then click **OK**.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="edc71-145">A legújabb felügyeleti sablonok letöltése</span><span class="sxs-lookup"><span data-stu-id="edc71-145">Get the latest Administrative Templates</span></span>

<span data-ttu-id="edc71-146">Ha nem látja az Automatikus **MDM-regisztráció** engedélyezése alapértelmezett Azure AD hitelesítő adatokkal házirendet, annak az lehet az oka, hogy nem telepítette az ADMX-et a Windows 10-es, 1803-as vagy újabb verziójához.</span><span class="sxs-lookup"><span data-stu-id="edc71-146">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, or later.</span></span> <span data-ttu-id="edc71-147">A probléma megoldásához kövesse az alábbi lépéseket (megjegyzés: az MDM.admx legújabb kompatibilis az előző verzióval):</span><span class="sxs-lookup"><span data-stu-id="edc71-147">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="edc71-148">Letöltés: [Felügyeleti sablonok (.admx) a Windows 10 2020. októberi frissítéséhez (20H2).](https://www.microsoft.com/download/102157)</span><span class="sxs-lookup"><span data-stu-id="edc71-148">Download: [Administrative Templates (.admx) for Windows 10 October 2020 Update (20H2)](https://www.microsoft.com/download/102157).</span></span>
2.  <span data-ttu-id="edc71-149">Telepítse a csomagot egy tartományvezérlőre.</span><span class="sxs-lookup"><span data-stu-id="edc71-149">Install the package on a Domain Controller.</span></span>
3.  <span data-ttu-id="edc71-150">A felügyeleti sablonok verziójától függően navigáljon a mappához: **C:\Program Files (x86)\Microsoft Csoportházirend\Windows 10 2020. októberi frissítés (20H2)**.</span><span class="sxs-lookup"><span data-stu-id="edc71-150">Navigate, depending on the Administrative Templates version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 October 2020 Update (20H2)**.</span></span>
4.  <span data-ttu-id="edc71-151">Nevezze át **a Fenti elérési út Házirenddefiníciók** **mappáját a PolicyDefinitions névre.**</span><span class="sxs-lookup"><span data-stu-id="edc71-151">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="edc71-152">Másolja a **PolicyDefinitions** mappát a SYSVOL-megosztásba, amely alapértelmezés szerint a **C:\Windows\SYSVOL\domain\Policies** mappában található.</span><span class="sxs-lookup"><span data-stu-id="edc71-152">Copy the **PolicyDefinitions** folder to your SYSVOL share, by default located at **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="edc71-153">Ha egy központi házirend-tárolót szeretne használni a teljes tartományhoz, ott vegye fel a PolicyDefinitions tartalmát.</span><span class="sxs-lookup"><span data-stu-id="edc71-153">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="edc71-154">Ha több tartományvezérlője van, várja meg, amíg a SYSVOL replikálja a házirendeket.</span><span class="sxs-lookup"><span data-stu-id="edc71-154">In case you have several Domain Controllers, wait for SYSVOL to replicate for the policies to be available.</span></span> <span data-ttu-id="edc71-155">Ez az eljárás a felügyeleti sablonok jövőbeli verzióival is működik.</span><span class="sxs-lookup"><span data-stu-id="edc71-155">This procedure will work for any future version of the Administrative Templates as well.</span></span>

<span data-ttu-id="edc71-156">Ezen a ponton láthatja az Automatikus MDM-regisztráció engedélyezése alapértelmezett **Azure AD-hitelesítő adatokkal elérhető** házirendet.</span><span class="sxs-lookup"><span data-stu-id="edc71-156">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>

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
ms.openlocfilehash: 857651081fb10856d28dd419333ebef655388407
ms.sourcegitcommit: e6e704cbd9a50fc7db1e6a0cf5d3f8c6cbb94363
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44564946"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="7d966-103">A tartományhoz csatlakozó Windows 10-eszközök Microsoft 365 Business Premium általi kezelésének engedélyezése</span><span class="sxs-lookup"><span data-stu-id="7d966-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="7d966-104">Ha a szervezet a helyszíni Windows Server Active Directoryt használja, beállíthatja a Microsoft 365 Business Premium rendszert a Windows 10-es eszközök védelmére, miközben továbbra is hozzáférhet a helyi hitelesítést igénylő helyszíni erőforrásokhoz.</span><span class="sxs-lookup"><span data-stu-id="7d966-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="7d966-105">A védelem beállításához hibrid **Azure AD-hez csatlakozott eszközöket**valósíthat meg.</span><span class="sxs-lookup"><span data-stu-id="7d966-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="7d966-106">Ezek az eszközök a helyszíni Active Directoryhoz és az Azure Active Directoryhoz is csatlakoznak.</span><span class="sxs-lookup"><span data-stu-id="7d966-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="7d966-107">Ez a videó bemutatja, hogyan állíthatja be ezt a leggyakoribb forgatókönyvhöz, amelyet a következő lépések is részleteznek.</span><span class="sxs-lookup"><span data-stu-id="7d966-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="7d966-108">Mielőtt elkezdene, végezze el az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="7d966-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="7d966-109">Szinkronizálja a felhasználókat az Azure AD-vel az Azure AD Connect segítségével.</span><span class="sxs-lookup"><span data-stu-id="7d966-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="7d966-110">Teljes Azure AD Connect szervezeti egység (OU) szinkronizálás.</span><span class="sxs-lookup"><span data-stu-id="7d966-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="7d966-111">Győződjön meg arról, hogy a szinkronizált tartomány összes felhasználója rendelkezik licenccel a Microsoft 365 Business Premium szolgáltatáshoz.</span><span class="sxs-lookup"><span data-stu-id="7d966-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="7d966-112">A lépésekről a [Tartományfelhasználók szinkronizálása a Microsofthoz](manage-domain-users.md) című témakörben található.</span><span class="sxs-lookup"><span data-stu-id="7d966-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="7d966-113">1. Az MDM-szolgáltató ellenőrzése az Intune-ban</span><span class="sxs-lookup"><span data-stu-id="7d966-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="7d966-114">Lépjen a portal.azure.com, és a lap tetején keresse meg az Intune-t.</span><span class="sxs-lookup"><span data-stu-id="7d966-114">Go to portal.azure.com and on the top of the page search for Intune.</span></span>
<span data-ttu-id="7d966-115">A Microsoft Intune lapon válassza az **Eszközregisztráció** lehetőséget, és az **Áttekintés** lapon győződjön meg arról, hogy az **MDM-szolgáltató** **intune-i.**</span><span class="sxs-lookup"><span data-stu-id="7d966-115">On the Microsoft Intune page, select **Device enrollment** and on the **Overview** page make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="7d966-116">Ha az **MDM-szolgáltató** **nincs,** kattintson az **MDM-szolgáltatóra** az **Intune**beállításához.</span><span class="sxs-lookup"><span data-stu-id="7d966-116">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="7d966-117">Ha az **MDM-szolgáltató** **a Microsoft Office 365**, nyissa meg az **Eszközök**  >  **regisztrálása eszközök,** és használja a **Add MDM hatóság** párbeszéd a jobb oldalon, hogy adjunk **Intune MDM** hatóság (a **Add MDM-szolgáltató** párbeszédpanel csak akkor érhető el, ha az **MDM-szolgáltató** van beállítva a Microsoft Office 365).</span><span class="sxs-lookup"><span data-stu-id="7d966-117">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="7d966-118">2. Ellenőrizze, hogy az Azure AD engedélyezve van-e a számítógépek hez való csatlakozáshoz</span><span class="sxs-lookup"><span data-stu-id="7d966-118">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="7d966-119">Nyissa meg a felügyeleti központot, <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> és válassza az Azure Active **Directory** (válassza az összes megjelenítése, ha az Azure Active Directory nem látható) a **Felügyeleti központok** listájában.</span><span class="sxs-lookup"><span data-stu-id="7d966-119">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="7d966-120">Az **Azure Active Directory felügyeleti központban**nyissa meg az Azure Active **Directoryt,** válassza **az Eszközök,** majd **az Eszközbeállítások lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="7d966-120">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="7d966-121">Annak**ellenőrzése, hogy a felhasználók csatlakozhatnak-e az Azure AD-hez,** engedélyezve van-e</span><span class="sxs-lookup"><span data-stu-id="7d966-121">Verify**Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="7d966-122">Az összes felhasználó engedélyezéséhez állítsa az **Összes**beállítását.</span><span class="sxs-lookup"><span data-stu-id="7d966-122">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="7d966-123">Adott felhasználók engedélyezéséhez állítsa **a Kijelölt** beállítást egy adott felhasználói csoport engedélyezéséhez.</span><span class="sxs-lookup"><span data-stu-id="7d966-123">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="7d966-124">Adja hozzá az Azure AD-ben szinkronizált kívánt tartományi felhasználókat egy [biztonsági csoporthoz.](../admin/create-groups/create-groups.md)</span><span class="sxs-lookup"><span data-stu-id="7d966-124">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="7d966-125">Válassza **a Csoportok kijelölése** lehetőséget az MDM felhasználói hatókörének engedélyezéséhez az adott biztonsági csoporthoz.</span><span class="sxs-lookup"><span data-stu-id="7d966-125">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="7d966-126">3. Ellenőrizze, hogy az Azure AD engedélyezve van-e az MDM-hez</span><span class="sxs-lookup"><span data-stu-id="7d966-126">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="7d966-127">Lépjen a felügyeleti központba, <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> és válassza a **Végpontkezelők**t lehetőséget (válassza **az Összes megjelenítése** lehetőséget, ha az **Endpoint Manager** nem látható)</span><span class="sxs-lookup"><span data-stu-id="7d966-127">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen**t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="7d966-128">A **Microsoft Endpoint Manager felügyeleti központban**nyissa meg **az Eszközök**  >  **windows**  >  **Windows-igénylés**  >  **automatikus igénylése**című lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7d966-128">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="7d966-129">Ellenőrizze, hogy az MDM felhasználói hatóköre engedélyezve van-e.</span><span class="sxs-lookup"><span data-stu-id="7d966-129">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="7d966-130">Az összes számítógép igényléséhez állítsa az **Összes** beállításra, hogy automatikusan regisztráljon minden olyan felhasználói számítógépet, amely az Azure AD-hez és az új számítógépekhez csatlakozik, amikor a felhasználók munkahelyi fiókot adnak hozzá a Windowshoz.</span><span class="sxs-lookup"><span data-stu-id="7d966-130">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="7d966-131">A **Bizonyos** beállításra a felhasználók egy adott csoportjának számítógépeinek regisztrálására.</span><span class="sxs-lookup"><span data-stu-id="7d966-131">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="7d966-132">Adja hozzá az Azure AD-ben szinkronizált kívánt tartományi felhasználókat egy [biztonsági csoporthoz.](../admin/create-groups/create-groups.md)</span><span class="sxs-lookup"><span data-stu-id="7d966-132">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="7d966-133">Válassza **a Csoportok kijelölése** lehetőséget az MDM felhasználói hatókörének engedélyezéséhez az adott biztonsági csoporthoz.</span><span class="sxs-lookup"><span data-stu-id="7d966-133">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-set-up-service-connection-point-scp"></a><span data-ttu-id="7d966-134">4. Szolgáltatás csatlakozási pontjának (SCP) beállítása</span><span class="sxs-lookup"><span data-stu-id="7d966-134">4. Set up Service connection point (SCP)</span></span>

<span data-ttu-id="7d966-135">Ezek a lépések egyszerűsödnek [a hibrid azure AD-illesztés](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join)konfigurálásából.</span><span class="sxs-lookup"><span data-stu-id="7d966-135">These steps are simplified from [configure hybrid azure AD join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span></span> <span data-ttu-id="7d966-136">Az Azure AD Connect és a Microsoft 365 Business Premium globális rendszergazdai és Active Directory-rendszergazdai jelszavak használatához szükséges lépések végrehajtásához.</span><span class="sxs-lookup"><span data-stu-id="7d966-136">To complete the steps you need to use Azure AD Connect and your Microsoft 365 Business Premium global admin and Active Directory admin passwords.</span></span>

1.  <span data-ttu-id="7d966-137">Indítsa el az Azure AD Connect et, és válassza **a Konfigurálás**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7d966-137">Start Azure AD Connect, and then select **Configure**.</span></span>
2.  <span data-ttu-id="7d966-138">A **További feladatok** lapon válassza az **Eszközbeállítások konfigurálása**lehetőséget, majd a **Tovább**gombot.</span><span class="sxs-lookup"><span data-stu-id="7d966-138">On the **Additional tasks**  page, select **Configure device options**, and then select **Next**.</span></span>
3.  <span data-ttu-id="7d966-139">Az **Áttekintés** lapon válassza a **Tovább lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="7d966-139">On the **Overview** page, select **Next**.</span></span>
4.  <span data-ttu-id="7d966-140">A Csatlakozás az **Azure AD-hez** lapon adja meg a Microsoft 365 Business Premium globális rendszergazdájának hitelesítő adatait.</span><span class="sxs-lookup"><span data-stu-id="7d966-140">On the **Connect to Azure AD** page, enter the credentials of a global administrator for Microsoft 365 Business Premium.</span></span>
5.  <span data-ttu-id="7d966-141">Az **Eszközbeállítások** lapon válassza a **Hibrid Azure AD-csatlakozás konfigurálása**lehetőséget, majd a **Tovább**gombot.</span><span class="sxs-lookup"><span data-stu-id="7d966-141">On the **Device options** page, select **Configure Hybrid Azure AD join**, and then select **Next**.</span></span>
6.  <span data-ttu-id="7d966-142">Az **SCP-lapon** minden olyan erdőesetében, ahol az Azure AD Connect konfigurálni szeretné az SCP-t, hajtsa végre a következő lépéseket, majd válassza a **Tovább**gombot:</span><span class="sxs-lookup"><span data-stu-id="7d966-142">On the **SCP** page, for each forest where you want Azure AD Connect to configure the SCP, complete the following steps, and then select **Next**:</span></span>
    - <span data-ttu-id="7d966-143">Jelölje be az erdő neve melletti négyzetet.</span><span class="sxs-lookup"><span data-stu-id="7d966-143">Check the box beside the forest name.</span></span> <span data-ttu-id="7d966-144">Az erdő nek az AD tartománynévnek kell lennie.</span><span class="sxs-lookup"><span data-stu-id="7d966-144">The forest should be your AD domain name.</span></span>
    - <span data-ttu-id="7d966-145">A **Hitelesítési szolgáltatás** oszlopban nyissa meg a legördülő menüt, és válassza ki az egyező tartománynevet (csak egy lehetőség lehet).</span><span class="sxs-lookup"><span data-stu-id="7d966-145">Under the **Authentication Service** column, open the dropdown and select matching domain name (there should only be one only option).</span></span>
    - <span data-ttu-id="7d966-146">A Tartományi rendszergazdahitelesítő adatok megadásához válassza a **Hozzáadás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7d966-146">Select **Add** to enter the domain administrator credentials.</span></span>  
7.  <span data-ttu-id="7d966-147">Az **Eszköz operációs rendszerek** lapon csak a Windows 10-es vagy újabb tartományhoz csatlakozó eszközök lehetőséget válassza.</span><span class="sxs-lookup"><span data-stu-id="7d966-147">On the **Device operating systems** page, select Windows 10 or later domain-joined devices only.</span></span>
8.  <span data-ttu-id="7d966-148">A **Konfigurálásra kész** lapon válassza a **Konfigurálás**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7d966-148">On the **Ready to configure** page, select **Configure**.</span></span>
9.  <span data-ttu-id="7d966-149">A **Konfiguráció befejeződése** lapon válassza a **Kilépés**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7d966-149">On the **Configuration complete** page, select **Exit**.</span></span>


## <a name="5-create-a-gpo-for-intune-enrollment--admx-method"></a><span data-ttu-id="7d966-150">5. Csoportházirend-azonosító létrehozása az Intune-regisztrációhoz – ADMX metódus</span><span class="sxs-lookup"><span data-stu-id="7d966-150">5. Create a GPO for Intune Enrollment – ADMX method</span></span>

<span data-ttu-id="7d966-151">Használja. ADMX sablonfájl.</span><span class="sxs-lookup"><span data-stu-id="7d966-151">Use .ADMX template file.</span></span>

1.  <span data-ttu-id="7d966-152">Jelentkezzen be az AD-kiszolgálóra, keressen és nyissa meg **a Kiszolgálókezelő**  >  **eszközei**  >  **csoportházirend-kezelést.**</span><span class="sxs-lookup"><span data-stu-id="7d966-152">Log on to AD server, search and open **Server Manager** > **Tools** > **Group Policy Management**.</span></span>
2.  <span data-ttu-id="7d966-153">Válassza ki a tartománynevét a **Tartományok területen,** és kattintson a jobb gombbal **a Csoportházirend-objektumok** elemre az **Új**lehetőség kiválasztásához.</span><span class="sxs-lookup"><span data-stu-id="7d966-153">Select your domain name under **Domains** and right-click **Group Policy Objects** to select **New**.</span></span>
3.  <span data-ttu-id="7d966-154">Adjon nevet az új csoportházirend-csatornának, például *"Cloud_Enrollment*", majd kattintson az **OK gombra.**</span><span class="sxs-lookup"><span data-stu-id="7d966-154">Give the new GPO an name, for example “*Cloud_Enrollment*” and then select **OK**.</span></span>
4.  <span data-ttu-id="7d966-155">Kattintson a jobb gombbal az új csoportházirend-objektumra a **Csoportházirendobjektumok csoportban,** és válassza **a Szerkesztés parancsot.**</span><span class="sxs-lookup"><span data-stu-id="7d966-155">Right-click the new GPO under **Group Policy Objects** and select **Edit**.</span></span>
5.  <span data-ttu-id="7d966-156">A **Csoportházirend kezelése szerkesztőben**nyissa meg a **Számítógép konfigurációs**  >  **házirendek**  >  **felügyeleti sablonok**  >  **Windows-összetevők**  >  **MDM**című részét.</span><span class="sxs-lookup"><span data-stu-id="7d966-156">In the **Group Policy Management Editor**, go to **Computer Configuration** > **Policies** > **Administrative Templates** > **Windows Components** > **MDM**.</span></span>
6. <span data-ttu-id="7d966-157">Kattintson a jobb gombbal **az Automatikus MDM-regisztráció engedélyezése az azure-beli AD-hitelesítő adatok használatával,** majd válassza az Engedélyezve az OK **parancsot.**  >  **OK**</span><span class="sxs-lookup"><span data-stu-id="7d966-157">Right-click **Enable automatic MDM enrollment using default Azure AD credentials** and then select **Enabled** > **OK**.</span></span> <span data-ttu-id="7d966-158">Zárja be a szerkesztőablakot.</span><span class="sxs-lookup"><span data-stu-id="7d966-158">Close the editor window.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="7d966-159">Ha nem látja az **Automatikus MDM-regisztráció engedélyezése az alapértelmezett Azure AD-hitelesítő adatokkal című házirendet,** [olvassa el a Legújabb felügyeleti sablonok beszerezhetése című témakört.](#get-the-latest-administrative-templates)</span><span class="sxs-lookup"><span data-stu-id="7d966-159">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, see [Get the latest Administrative Templates](#get-the-latest-administrative-templates).</span></span>

## <a name="6-deploy-the-group-policy"></a><span data-ttu-id="7d966-160">6. A csoportházirend telepítése</span><span class="sxs-lookup"><span data-stu-id="7d966-160">6. Deploy the Group Policy</span></span>

1.  <span data-ttu-id="7d966-161">A Kiszolgálókezelő **tartományok** > csoportházirend-objektumok csoportjában válassza ki a Cloud_Enrollment csoportházirend-objektumot a fenti 3.</span><span class="sxs-lookup"><span data-stu-id="7d966-161">In the Server Manager, under **Domains** > Group Policy objects, select the GPO from Step 3 above, for example “Cloud_Enrollment”.</span></span>
2.  <span data-ttu-id="7d966-162">Válassza **Scope** a csoportházirend-csoport házirend-eszközhatókör lapját.</span><span class="sxs-lookup"><span data-stu-id="7d966-162">Select the **Scope** tab for your GPO.</span></span>
3.  <span data-ttu-id="7d966-163">A csoportházirend-csoport hatóköre lapon kattintson a jobb gombbal a **Hivatkozások**csoporttartományra mutató hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="7d966-163">In the GPO’s Scope tab, right-click the link to the domain under **Links**.</span></span>
4.  <span data-ttu-id="7d966-164">Válassza **a Kényszerített lehetőséget** a csoportházirend-csoportházirend-csoport házirendjének üzembe helyezéséhez, majd az OK **gombot** a megerősítő képernyőn.</span><span class="sxs-lookup"><span data-stu-id="7d966-164">Select **Enforced** to deploy the GPO and then **OK** in the confirmation screen.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="7d966-165">A legújabb felügyeleti sablonok beszerezhetése</span><span class="sxs-lookup"><span data-stu-id="7d966-165">Get the latest Administrative Templates</span></span>

<span data-ttu-id="7d966-166">Ha nem látja az **Automatikus MDM-regisztráció engedélyezése az alapértelmezett Azure AD-hitelesítő adatokkal című házirendet,** annak az lehet az oka, hogy nincs telepítve az ADMX a Windows 10, 1803-as, 1803-as vagy 1903-as verzióhoz.</span><span class="sxs-lookup"><span data-stu-id="7d966-166">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, version 1809, or version 1903.</span></span> <span data-ttu-id="7d966-167">A probléma megoldásához kövesse az alábbi lépéseket (Megjegyzés: a legújabb MDM.admx visszafelé kompatibilis):</span><span class="sxs-lookup"><span data-stu-id="7d966-167">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="7d966-168">Letöltés: [Felügyeleti sablonok (.admx) a Windows 10 2019 májusi frissítéséhez (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span><span class="sxs-lookup"><span data-stu-id="7d966-168">Download: [Administrative Templates (.admx) for Windows 10 May 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span></span>
2.  <span data-ttu-id="7d966-169">Telepítse a csomagot az elsődleges tartományvezérlőre (PDC).</span><span class="sxs-lookup"><span data-stu-id="7d966-169">Install the package on the Primary Domain Controller (PDC).</span></span>
3.  <span data-ttu-id="7d966-170">Navigálás a mappa verziójától függően: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span><span class="sxs-lookup"><span data-stu-id="7d966-170">Navigate, depending on the version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span></span>
4.  <span data-ttu-id="7d966-171">Nevezze át a **Házirenddefiníciók mappát** a **PolicyDefinitions**fenti elérési útján.</span><span class="sxs-lookup"><span data-stu-id="7d966-171">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="7d966-172">A **PolicyDefinitions** mappa másolása a **C:\Windows\SYSVOL\domain\Policies mappába.**</span><span class="sxs-lookup"><span data-stu-id="7d966-172">Copy **PolicyDefinitions** folder to **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="7d966-173">Ha a teljes tartományközponti házirend-tárolót kíván használni, adja hozzá a PolicyDefinitions tartalmát.</span><span class="sxs-lookup"><span data-stu-id="7d966-173">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="7d966-174">Indítsa újra az elsődleges tartományvezérlőt, hogy a házirend elérhető legyen.</span><span class="sxs-lookup"><span data-stu-id="7d966-174">Restart the Primary Domain Controller for the policy to be available.</span></span> <span data-ttu-id="7d966-175">Ez eljárás akarat dolgozik részére akármi jövő változat jól.</span><span class="sxs-lookup"><span data-stu-id="7d966-175">This procedure will work for any future version as well.</span></span>

<span data-ttu-id="7d966-176">Ezen a ponton látnia kell a házirend **automatikus MDM-regisztráció engedélyezése az alapértelmezett Azure AD hitelesítő adatok elérhető** használatával.</span><span class="sxs-lookup"><span data-stu-id="7d966-176">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>


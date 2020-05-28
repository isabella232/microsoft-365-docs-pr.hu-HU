---
title: Tartományhoz csatlakozott Windows 10-es eszközök microsoft 365 vállalati verziós kezelésének engedélyezése
f1.keywords:
- NOCSH
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
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Megtudhatja, hogy miként engedélyezheti a Microsoft 365 számára a helyi Active Directoryhoz csatlakozott Windows 10-eszközök védelmét néhány lépésben.
ms.openlocfilehash: e7f83e620fbb43a478dba98f78d5f471a541aea7
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403058"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-for-business"></a><span data-ttu-id="17bb3-103">Tartományhoz csatlakozott Windows 10-es eszközök microsoft 365 vállalati verziós kezelésének engedélyezése</span><span class="sxs-lookup"><span data-stu-id="17bb3-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 for business</span></span>

<span data-ttu-id="17bb3-104">Ha a szervezet a helyszíni Windows Server Active Directoryt használja, beállíthatja a Microsoft 365 vállalati verziót a Windows 10-es eszközök védelmére, miközben továbbra is hozzáférhet a helyi hitelesítést igénylő helyszíni erőforrásokhoz.</span><span class="sxs-lookup"><span data-stu-id="17bb3-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 for business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="17bb3-105">A védelem beállításához hibrid **Azure AD-hez csatlakozott eszközöket**valósíthat meg.</span><span class="sxs-lookup"><span data-stu-id="17bb3-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="17bb3-106">Ezek az eszközök a helyszíni Active Directoryhoz és az Azure Active Directoryhoz is csatlakoznak.</span><span class="sxs-lookup"><span data-stu-id="17bb3-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="17bb3-107">Ez a videó bemutatja, hogyan állíthatja be ezt a leggyakoribb forgatókönyvhöz, amelyet a következő lépések is részleteznek.</span><span class="sxs-lookup"><span data-stu-id="17bb3-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="17bb3-108">1. Felkészülés a címtár-szinkronizálásra</span><span class="sxs-lookup"><span data-stu-id="17bb3-108">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="17bb3-109">Mielőtt szinkronizálja a felhasználókat és a számítógépeket a helyi Active Directory tartományból, tekintse át [a Felkészülés az Office 365-tel való címtár-szinkronizálásra](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization)című részt.</span><span class="sxs-lookup"><span data-stu-id="17bb3-109">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="17bb3-110">Különösen:</span><span class="sxs-lookup"><span data-stu-id="17bb3-110">In particular:</span></span>

   - <span data-ttu-id="17bb3-111">Győződjön meg arról, hogy a következő attribútumokhoz nem találhatók ismétlődések a könyvtárban: **mail**, **proxyAddresses**és **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="17bb3-111">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="17bb3-112">Ezeknek az értékeknek egyedieknek kell lenniük, és minden ismétlődést el kell távolítani.</span><span class="sxs-lookup"><span data-stu-id="17bb3-112">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="17bb3-113">Azt javasoljuk, hogy minden helyi felhasználói fiókhoz konfigurálja a **userPrincipalName** (UPN) attribútumot úgy, hogy az megfeleljen a licencelt Microsoft 365-felhasználónak megfelelő elsődleges e-mail címnek.</span><span class="sxs-lookup"><span data-stu-id="17bb3-113">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="17bb3-114">Például: *mary.shelley@contoso.com* helyett *mary@contoso.local*</span><span class="sxs-lookup"><span data-stu-id="17bb3-114">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="17bb3-115">Ha az Active Directory tartomány nem irányítható utótaggal végződik, például *.local* vagy *.lan*, az internetes irányítható utótag (például *.com* vagy *.org)* helyett, állítsa be először a helyi felhasználói fiókok UPN-utónevét a [Címtár-szinkronizálásra](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization)nem irányítható tartomány előkészítése című részben leírtak szerint.</span><span class="sxs-lookup"><span data-stu-id="17bb3-115">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="17bb3-116">2. Az Azure AD Connect telepítése és konfigurálása</span><span class="sxs-lookup"><span data-stu-id="17bb3-116">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="17bb3-117">Ha szinkronizálni szeretné a felhasználókat, csoportokat és névjegyeket a helyi Active Directoryból az Azure Active Directoryba, telepítse az Azure Active Directory Connectet, és állítsa be a címtár-szinkronizálást.</span><span class="sxs-lookup"><span data-stu-id="17bb3-117">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> <span data-ttu-id="17bb3-118">További információ: [Címtár-szinkronizálás beállítása az Office 365-höz.](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization)</span><span class="sxs-lookup"><span data-stu-id="17bb3-118">See [Set up directory synchronization for Office 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) to learn more.</span></span>

> [!NOTE]
> <span data-ttu-id="17bb3-119">A lépések pontosan ugyanazok a Microsoft 365 vállalati verziók esetében.</span><span class="sxs-lookup"><span data-stu-id="17bb3-119">The steps are exactly the same for Microsoft 365 for business.</span></span> 

<span data-ttu-id="17bb3-120">Az Azure AD Connect beállításainak konfigurálásakor azt javasoljuk, hogy engedélyezze **a jelszó-szinkronizálást**, a zökkenőmentes egyszeri bejelentkezést és a **jelszó-visszaírási** funkciót, amelyet a Microsoft 365 vállalati verzió is támogat. **Seamless Single Sign-On**</span><span class="sxs-lookup"><span data-stu-id="17bb3-120">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="17bb3-121">Az Azure AD Connect jelölőnégyzetén túl további lépések is bevannak téve a jelszó-visszaíráshoz.</span><span class="sxs-lookup"><span data-stu-id="17bb3-121">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="17bb3-122">További információ: [Útmutató: jelszó-visszaírás konfigurálása.](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="17bb3-122">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

## <a name="3-configure-hybrid-azure-ad-join"></a><span data-ttu-id="17bb3-123">3. Hibrid Azure AD-illesztés konfigurálása</span><span class="sxs-lookup"><span data-stu-id="17bb3-123">3. Configure Hybrid Azure AD Join</span></span>

<span data-ttu-id="17bb3-124">Mielőtt engedélyezne Windows 10-es eszközöket hibrid Azure AD-csatlakozásra, győződjön meg arról, hogy megfelel az alábbi előfeltételeknek:</span><span class="sxs-lookup"><span data-stu-id="17bb3-124">Before you enable Windows 10 devices to be Hybrid Azure AD joined, make sure that you meet the following prerequisites:</span></span>

   - <span data-ttu-id="17bb3-125">Az Azure AD Connect legújabb verzióját futtatja.</span><span class="sxs-lookup"><span data-stu-id="17bb3-125">You're running the latest version of Azure AD Connect.</span></span>

   - <span data-ttu-id="17bb3-126">Az Azure AD connect szinkronizálta a hibrid Azure AD-hez csatlakozni kívánt eszközök összes számítógép-objektumát.</span><span class="sxs-lookup"><span data-stu-id="17bb3-126">Azure AD connect has synchronized all the computer objects of the devices you want to be hybrid Azure AD joined.</span></span> <span data-ttu-id="17bb3-127">Ha a számítógép-objektumok adott szervezeti egységekhez (OU) tartoznak, győződjön meg arról, hogy ezek a szervezeti egységek szinkronizálásra vannak beállítva az Azure AD-csatlakozásban is.</span><span class="sxs-lookup"><span data-stu-id="17bb3-127">If the computer objects belong to specific organizational units (OU), then make sure these OUs are set for synchronization in Azure AD connect as well.</span></span>

<span data-ttu-id="17bb3-128">Ha hibrid Azure AD-csatlakozásként szeretné regisztrálni a meglévő tartományhoz csatlakozó Windows 10-eszközöket, kövesse az [oktatóanyag lépéseit: Hibrid Azure Active Directory-csatlakozás konfigurálása felügyelt tartományokhoz.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="17bb3-128">To register existing domain-joined Windows 10 devices as Hybrid Azure AD joined, follow the steps in the [Tutorial: Configure hybrid Azure Active Directory join for managed domains](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span></span> <span data-ttu-id="17bb3-129">Ez a hibrid lehetővé teszi, hogy a meglévő helyszíni Active Directory csatlakozott a Windows 10 számítógépek, és azokat felhő kész.</span><span class="sxs-lookup"><span data-stu-id="17bb3-129">This hybrid-enables your existing on-premises Active Directory joined Windows 10 computers and make them cloud ready.</span></span>
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a><span data-ttu-id="17bb3-130">4. Automatikus regisztráció engedélyezése a Windows 10-hez</span><span class="sxs-lookup"><span data-stu-id="17bb3-130">4. Enable automatic enrollment for Windows 10</span></span>

 <span data-ttu-id="17bb3-131">Ha automatikusan szeretné regisztrálni a Windows 10-es eszközöket mobileszköz-kezeléshez az Intune-ban, olvassa el a [Windows 10-es eszközök automatikus regisztrálása a csoportházirenddel című témakört.](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy)</span><span class="sxs-lookup"><span data-stu-id="17bb3-131">To automatically enroll Windows 10 devices for mobile device management in Intune, see [Enroll a Windows 10 device automatically using Group Policy](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy).</span></span> <span data-ttu-id="17bb3-132">A csoportházirendet helyi számítógép-szinten, illetve tömeges műveletek esetén a Csoportházirend kezelése konzol és az ADMX-sablonok segítségével hozhatja létre ezt a csoportházirend-beállítást a tartományvezérlőn.</span><span class="sxs-lookup"><span data-stu-id="17bb3-132">You can set the Group Policy at a local computer level, or for bulk operations, you can use the Group Policy Management Console and ADMX templates to create this Group Policy setting on your Domain Controller.</span></span>

## <a name="5-configure-seamless-single-sign-on"></a><span data-ttu-id="17bb3-133">5. Zökkenőmentes egyszeri bejelentkezés konfigurálása</span><span class="sxs-lookup"><span data-stu-id="17bb3-133">5. Configure Seamless Single Sign-On</span></span>

  <span data-ttu-id="17bb3-134">A zökkenőmentes egyszeri bejelentkezés automatikusan aláírja a felhasználókat a Microsoft 365 felhőalapú erőforrásaiba, amikor vállalati számítógépeket használnak.</span><span class="sxs-lookup"><span data-stu-id="17bb3-134">Seamless SSO automatically signs users into their Microsoft 365 cloud resources when they use corporate computers.</span></span> <span data-ttu-id="17bb3-135">Egyszerűen telepítse az Azure Active Directory zökkenőmentes egyszeri bejelentkezési szolgáltatásában ismertetett két [csoportházirend-beállítás egyikét: gyorsindítás.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature)</span><span class="sxs-lookup"><span data-stu-id="17bb3-135">Simply deploy one of the two Group Policy options described in [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature).</span></span> <span data-ttu-id="17bb3-136">A **Csoportházirend** beállítás nem teszi lehetővé a felhasználók számára a beállítások módosítását, míg a **Csoportházirend-beállítás** beállítás beállítja az értékeket, de a felhasználó számára is konfigurálható marad.</span><span class="sxs-lookup"><span data-stu-id="17bb3-136">The **Group Policy** option doesn't allow users to change their settings, while the **Group Policy Preference** option sets the values but also leaves them user-configurable.</span></span>

## <a name="6-set-up-windows-hello-for-business"></a><span data-ttu-id="17bb3-137">6. A Windows Hello Vállalati verzió beállítása</span><span class="sxs-lookup"><span data-stu-id="17bb3-137">6. Set up Windows Hello for Business</span></span>

 <span data-ttu-id="17bb3-138">A Windows Hello for Business a helyi számítógépre való bejelentkezéshez a jelszavakat erős kétfaktoros hitelesítéssel (2FA) helyettesíti.</span><span class="sxs-lookup"><span data-stu-id="17bb3-138">Windows Hello for Business replaces passwords with strong two-factor authentication (2FA) for signing into a local computer.</span></span> <span data-ttu-id="17bb3-139">Az egyik tényező egy aszimmetrikus kulcspár, a másik pedig egy PIN-kód vagy más helyi kézmozdulat, például ujjlenyomat vagy arcfelismerés, ha az eszköz támogatja azt.</span><span class="sxs-lookup"><span data-stu-id="17bb3-139">One factor is an asymmetric key pair, and the other is a PIN or other local gesture such as fingerprint or facial recognition if your device supports it.</span></span> <span data-ttu-id="17bb3-140">Azt javasoljuk, hogy ahol lehetséges, cserélje le a jelszavakat a 2FA-ra és a Windows Hello for Business-re.</span><span class="sxs-lookup"><span data-stu-id="17bb3-140">We recommend that you replace passwords with 2FA and Windows Hello for Business where possible.</span></span>

<span data-ttu-id="17bb3-141">A hibrid Windows Hello for Business konfigurálásához tekintse át a [hibridkulcs megbízhatósági kapcsolatát a Windows Hello üzleti előfeltételekhez](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs).</span><span class="sxs-lookup"><span data-stu-id="17bb3-141">To configure Hybrid Windows Hello for Business, review the [Hybrid Key trust Windows Hello for Business Prerequisites](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs).</span></span> <span data-ttu-id="17bb3-142">Ezután kövesse a [Hibrid Windows Hello for Business kulcsmegbízhatósági beállítások konfigurálása című útmutató utasításait.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings)</span><span class="sxs-lookup"><span data-stu-id="17bb3-142">Then follow the instructions in [Configure Hybrid Windows Hello for Business key trust settings](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings).</span></span> 

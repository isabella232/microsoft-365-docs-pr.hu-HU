---
title: A Microsoft 365 Vállalati prémium verzió beállítása
f1.keywords:
- NOCSH
ms.author: kwekua
author: kwekua
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
- TRN_SMB
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Megismerheti a fiókkal kapcsolatos Microsoft 365 Vállalati prémium verzió, például tartomány és felhasználók felvételét, biztonsági házirendek beállítását és sok minden más.
ms.openlocfilehash: 3e15f16db2a233d2e11d444600398102b075932d
ms.sourcegitcommit: 686f192e1a650ec805fe8e908b46ca51771ed41f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/24/2021
ms.locfileid: "52624389"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a><span data-ttu-id="7a268-103">A Microsoft 365 Vállalati prémium verzió beállítása a beállítási varázslóban</span><span class="sxs-lookup"><span data-stu-id="7a268-103">Set up Microsoft 365 Business Premium in the setup wizard</span></span>

## <a name="watch-overview-of-microsoft-365-setup"></a><span data-ttu-id="7a268-104">Watch: Overview of Microsoft 365 setup</span><span class="sxs-lookup"><span data-stu-id="7a268-104">Watch: Overview of Microsoft 365 setup</span></span>

<span data-ttu-id="7a268-105">Ez a videó áttekintést nyújt a Microsoft 365 Vállalati prémium verzió beállításról.</span><span class="sxs-lookup"><span data-stu-id="7a268-105">Watch this video for an overview of Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="7a268-106">Tartomány, felhasználók hozzáadása és házirendek beállítása</span><span class="sxs-lookup"><span data-stu-id="7a268-106">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="7a268-107">A (Microsoft 365 Vállalati prémium verzió vásárlásakor lehetősége van saját tartományt használni, illetve a regisztráció során vásárolni [egyet.](sign-up.md)</span><span class="sxs-lookup"><span data-stu-id="7a268-107">When you purchase Microsoft 365 Business Premium, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="7a268-108">Ha a feliratkozáskor új tartományt vásárolt, akkor a tartománya be van állítva, és a Felhasználók hozzáadása és licencek hozzárendelése gombra kell [lépnie.](#add-users-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="7a268-108">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="7a268-109">Tartomány hozzáadása a bejelentkezés személyre szabása</span><span class="sxs-lookup"><span data-stu-id="7a268-109">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="7a268-110">Jelentkezzen be [Microsoft 365 felügyeleti központba](https://admin.microsoft.com) globális rendszergazdai hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="7a268-110">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="7a268-111">A **varázslót az Ugrás** a beállításra gombra állítva indítsa el.</span><span class="sxs-lookup"><span data-stu-id="7a268-111">Choose **Go to setup** to start the wizard.</span></span>

    ![Válassza az Ugrás a beállításra lehetőséget.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="7a268-113">A **Saját appok Office lapján** tetszés szerint telepítheti az alkalmazásokat a saját számítógépén.</span><span class="sxs-lookup"><span data-stu-id="7a268-113">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="7a268-114">A **Tartomány hozzáadása lépésben** adja meg a használni kívánt tartománynevet (például contoso.com).</span><span class="sxs-lookup"><span data-stu-id="7a268-114">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="7a268-115">Ha a regisztráció során tartományt vásárolt, itt nem fogja látni **a** Tartomány hozzáadása lépést.</span><span class="sxs-lookup"><span data-stu-id="7a268-115">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="7a268-116">Ehelyett a [Felhasználók hozzáadása gombra](#add-users-and-assign-licenses) kell azt felvennie.</span><span class="sxs-lookup"><span data-stu-id="7a268-116">Go to [Add users](#add-users-and-assign-licenses) instead.</span></span>

    ![Képernyőkép a Bejelentkezési lap személyre szabása lapról.](../media/adddomain.png)

    
4. <span data-ttu-id="7a268-118">A varázsló lépéseit követve hozza létre a DNS-rekordokat bármely [DNS-szolgáltatónál](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) annak Microsoft 365, hogy Öné a tartomány.</span><span class="sxs-lookup"><span data-stu-id="7a268-118">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Microsoft 365](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="7a268-119">Ha ismeri a tartományát, olvassa el a [szolgáltatóra vonatkozó utasításokat is.](/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)</span><span class="sxs-lookup"><span data-stu-id="7a268-119">If you know your domain host, see also the [host specific instructions](/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="7a268-120">Ha az Ön tárhelyszolgáltatója a GoDaddy vagy más szolgáltató, amely támogatja a tartomány [csatlakoztatását,](/office365/admin/get-help-with-domains/domain-connect)a folyamat egyszerű, és a rendszer automatikusan kérni fogja, hogy jelentkezzen be, és a Microsoft hitelesítse magát az Ön nevében.</span><span class="sxs-lookup"><span data-stu-id="7a268-120">If your hosting provider is GoDaddy or another host enabled with [domain connect](/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![A GoDaddy Confirm Access (Hozzáférés megerősítése) lapon válassza a Authorize (Engedély) lehetőséget.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="7a268-122">Felhasználók felvétele és licencek hozzárendelése</span><span class="sxs-lookup"><span data-stu-id="7a268-122">Add users and assign licenses</span></span>

<span data-ttu-id="7a268-123">Felvehet felhasználókat a varázslóba, de [](../admin/add-users/add-users.md) később a Felügyeleti központban is.</span><span class="sxs-lookup"><span data-stu-id="7a268-123">You can add users in the wizard, but you can also [add users later](../admin/add-users/add-users.md) in the admin center.</span></span> <span data-ttu-id="7a268-124">Ha pedig helyi tartományvezérlője van, felhasználókat is felvehet az [Azure AD Csatlakozás.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="7a268-124">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="7a268-125">Felhasználók hozzáadása a varázslóban</span><span class="sxs-lookup"><span data-stu-id="7a268-125">Add users in the wizard</span></span>

<span data-ttu-id="7a268-126">A varázslóban hozzáadt minden felhasználóhoz automatikusan hozzárendel egy Microsoft 365 Vállalati prémium verzió licencet.</span><span class="sxs-lookup"><span data-stu-id="7a268-126">Any users you add in the wizard get automatically assigned a Microsoft 365 Business Premium license.</span></span>

![Képernyőkép a varázsló Új felhasználók hozzáadása lapról](../media/addnewuserspage.png)

1. <span data-ttu-id="7a268-128">Ha az Microsoft 365 Vállalati prémium verzió-előfizetéséhez vannak meglévő felhasználók (például ha az Azure AD Csatlakozás-t használta), akkor most lehetősége van licenceket rendelni hozzájuk.</span><span class="sxs-lookup"><span data-stu-id="7a268-128">If your Microsoft 365 Business Premium subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="7a268-129">Nyugodtan felvehet licenceket hozzájuk is.</span><span class="sxs-lookup"><span data-stu-id="7a268-129">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="7a268-130">A felhasználók hozzáadása után a hitelesítő adatokat is megoszthatja a felvett új felhasználókkal.</span><span class="sxs-lookup"><span data-stu-id="7a268-130">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="7a268-131">Ezeket kinyomtathatja, elküldheti e-mailben, vagy pedig letöltheti.</span><span class="sxs-lookup"><span data-stu-id="7a268-131">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="7a268-132">Tartomány csatlakoztatása</span><span class="sxs-lookup"><span data-stu-id="7a268-132">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="7a268-133">Ha az .onmicrosoft tartományt választotta, vagy az Azure AD Csatlakozás segítségével beállította a felhasználókat, ez a lépés nem látható.</span><span class="sxs-lookup"><span data-stu-id="7a268-133">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="7a268-134">A szolgáltatások beállításához frissítenie kell bizonyos rekordokat a DNS-szolgáltatónál vagy a tartományregisztrálónál.</span><span class="sxs-lookup"><span data-stu-id="7a268-134">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="7a268-135">A beállítási varázsló általában felismeri a regisztrálóját, és részletes útmutatást jelenít meg arról, hogy miként frissítheti a névkiszolgálói rekordokat a regisztráló webhelyén.</span><span class="sxs-lookup"><span data-stu-id="7a268-135">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="7a268-136">Ha nem így van, módosítsa a névkiszolgálói rekordokat úgy, hogy Microsoft 365 [tartományregisztrálónál beállítsa a rekordokat.](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md)</span><span class="sxs-lookup"><span data-stu-id="7a268-136">If it doesn't, [Change nameservers to set up Microsoft 365 with any domain registrar](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md).</span></span> 

    - <span data-ttu-id="7a268-137">Ha van meglévő DNS-rekordja, például egy meglévő webhelye, de a DNS-szolgáltató engedélyezve van a [tartományhoz](/office365/admin/get-help-with-domains/domain-connect)való csatlakozáshoz, válassza a Rekordok hozzáadása **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="7a268-137">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="7a268-138">A Choose **your online services (Online szolgáltatások kiválasztása)** lapon fogadja el az összes alapértelmezett beállítást, és válassza a **Tovább**, majd az **Authorize** (Engedély) lehetőséget a DNS-szolgáltatója lapján.</span><span class="sxs-lookup"><span data-stu-id="7a268-138">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="7a268-139">Ha más DNS-szolgáltatónál már van DNS-rekordja (a tartomány csatlakoztatása nem engedélyezett), akkor saját DNS-rekordjait kell kezelnie, hogy a meglévő szolgáltatások kapcsolatban maradjanak.</span><span class="sxs-lookup"><span data-stu-id="7a268-139">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="7a268-140">További [információt a tartományokkal kapcsolatos alapismeretek](/office365/admin/get-help-with-domains/dns-basics) között található.</span><span class="sxs-lookup"><span data-stu-id="7a268-140">See [domain basics](/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Rekordok aktiválása lap.](../media/activaterecords.png)

2. <span data-ttu-id="7a268-142">Kövesse a varázsló lépéseit, és állítsa be Önnek a levelezést és más szolgáltatásokat.</span><span class="sxs-lookup"><span data-stu-id="7a268-142">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="7a268-143">A szervezet védelme</span><span class="sxs-lookup"><span data-stu-id="7a268-143">Protect your organization</span></span> 

<span data-ttu-id="7a268-144">A varázslóban beállított házirendek automatikusan vonatkoznak a Minden [felhasználó](/office365/admin/create-groups/compare-groups#security-groups) nevű biztonsági *csoportra.*</span><span class="sxs-lookup"><span data-stu-id="7a268-144">The policies you set up in the wizard are applied automatically to a [Security group](/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="7a268-145">További csoportokat is létrehozhat, amelyekhez házirendeket rendelhet hozzá a Felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="7a268-145">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="7a268-146">A speciális **kiberfenyegetések** elleni védelem növelése érdekében javasoljuk, hogy fogadja el az alapértelmezett értékeket, hogy a Office 365 [Komplex](../security/office-365-security/defender-for-office-365.md) veszélyforrások elleni védelem megvizsgálja a fájlokat és hivatkozásokat az Office alkalmazásokban.</span><span class="sxs-lookup"><span data-stu-id="7a268-146">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](../security/office-365-security/defender-for-office-365.md) scan files and links in Office apps.</span></span>

    ![Képernyőkép a Védelem növelése lapról](../media/increasetreatprotection.png)


2. <span data-ttu-id="7a268-148">A  Bizalmas adatok kiszivárgásának megakadályozása lapon fogadja el az Office 365 Adatveszteség-megelőzés (DLP) alapértelmezett beállítását a bizalmas adatok nyomon követéséhez az Office-appokban, valamint annak érdekében, hogy megakadályozza ezeknek a szervezeten kívüli véletlen megosztását.</span><span class="sxs-lookup"><span data-stu-id="7a268-148">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="7a268-149">Az **Adatok védelme a mobileszközök Office** lapon hagyja be a mobilapp felügyeletét, bontsa ki a beállításokat, és tekintse át őket, majd válassza a Mobilappkezelési házirend **létrehozása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="7a268-149">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Képernyőkép a Mobileszközök Office adatokat lapról.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="7a268-151">Pc Windows 10 biztonságossá</span><span class="sxs-lookup"><span data-stu-id="7a268-151">Secure Windows 10 PCs</span></span>

<span data-ttu-id="7a268-152">A bal oldali  navigációs sávon válassza a Beállítás lehetőséget, majd a Bejelentkezés és biztonság alatt válassza A számítógép **Windows 10 lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="7a268-152">On the left nav, select **Setup** and then, under **Sign-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="7a268-153">Első **lépésekhez** válassza a Nézet lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7a268-153">Choose **View** to get started.</span></span> <span data-ttu-id="7a268-154">Részletes [útmutatást a számítógépei Windows 10 el.](secure-win-10-pcs.md)</span><span class="sxs-lookup"><span data-stu-id="7a268-154">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="7a268-155">Ügyfélalkalmazások Office 365 telepítése</span><span class="sxs-lookup"><span data-stu-id="7a268-155">Deploy Office 365 client apps</span></span>

<span data-ttu-id="7a268-156">Ha a telepítés során az Office-appok automatikus telepítését választotta, az alkalmazások az Windows 10-eszközökre fognak telepíteni, miután a felhasználók bejelentkeztek az Azure AD-be az Windows-eszközükről a munkahelyi hitelesítő adataik használatával.</span><span class="sxs-lookup"><span data-stu-id="7a268-156">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="7a268-157">Az iOS Office Android rendszerű mobileszközökön való telepítéséhez lásd: Mobileszközök beállítása az összes [Microsoft 365 Vállalati prémium verzió számára.](set-up-mobile-devices.md)</span><span class="sxs-lookup"><span data-stu-id="7a268-157">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="7a268-158">A frissítéseket egyenként Office is.</span><span class="sxs-lookup"><span data-stu-id="7a268-158">You can also install Office individually.</span></span> <span data-ttu-id="7a268-159">Útmutatásért [Office PC-re](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) vagy Mac gépre való telepítéséről.</span><span class="sxs-lookup"><span data-stu-id="7a268-159">See [install Office on a PC or Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="related-content"></a><span data-ttu-id="7a268-160">Kapcsolódó tartalom</span><span class="sxs-lookup"><span data-stu-id="7a268-160">Related content</span></span>

<span data-ttu-id="7a268-161">[Microsoft 365 vállalati verziós oktatóvideók](../business-video/index.yml) (hivatkozáslap)</span><span class="sxs-lookup"><span data-stu-id="7a268-161">[Microsoft 365 for business training videos](../business-video/index.yml) (link page)</span></span>

---
title: A Microsoft 365 Vállalati prémium verzió beállítása
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
description: Megismerheti a Microsoft 365 Vállalati prémium verzió beállítási lépéseit, például tartomány és felhasználók felvételét, biztonsági házirendek beállítását és sok más lépést.
ms.openlocfilehash: a06fb48ef5e1386a5c7b4df08500125f37943df6
ms.sourcegitcommit: dcb97fbfdae52960ae62b6faa707a05358193ed5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51198439"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a><span data-ttu-id="ca6b0-103">A Microsoft 365 Vállalati prémium verzió beállítása a beállítási varázslóban</span><span class="sxs-lookup"><span data-stu-id="ca6b0-103">Set up Microsoft 365 Business Premium in the setup wizard</span></span>

<span data-ttu-id="ca6b0-104">Ez a videó áttekintést nyújt a Microsoft 365 Vállalati prémium verzió beállításról.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-104">Watch this video for an overview of Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="ca6b0-105">Tartomány, felhasználók hozzáadása és házirendek beállítása</span><span class="sxs-lookup"><span data-stu-id="ca6b0-105">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="ca6b0-106">A Microsoft 365 Business Premium megvásárlásakor lehetősége van arra, hogy saját tartományát használja, vagy a regisztráció során [vásároljon egyet.](sign-up.md)</span><span class="sxs-lookup"><span data-stu-id="ca6b0-106">When you purchase Microsoft 365 Business Premium, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="ca6b0-107">Ha a feliratkozáskor új tartományt vásárolt, akkor a tartománya be van állítva, és a Felhasználók hozzáadása és licencek hozzárendelése gombra kell [lépnie.](#add-users-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="ca6b0-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="ca6b0-108">Tartomány hozzáadása a bejelentkezés személyre szabása</span><span class="sxs-lookup"><span data-stu-id="ca6b0-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="ca6b0-109">Jelentkezzen be a [Microsoft 365 Felügyeleti központba](https://admin.microsoft.com) a globális rendszergazdai hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="ca6b0-110">A **varázslót az Ugrás** a beállításra gombra állítva indítsa el.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-110">Choose **Go to setup** to start the wizard.</span></span>

    ![Válassza az Ugrás a beállításra lehetőséget.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="ca6b0-112">Az **Office-appok telepítése lapon** szükség esetén telepítheti az appokat a saját számítógépére.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-112">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="ca6b0-113">A **Tartomány hozzáadása lépésben** adja meg a használni kívánt tartománynevet (például contoso.com).</span><span class="sxs-lookup"><span data-stu-id="ca6b0-113">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="ca6b0-114">Ha a regisztráció során tartományt vásárolt, itt nem fogja látni **a** Tartomány hozzáadása lépést.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-114">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="ca6b0-115">Ehelyett a [Felhasználók hozzáadása gombra](#add-users-and-assign-licenses) kell azt felvennie.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-115">Go to [Add users](#add-users-and-assign-licenses) instead.</span></span>

    ![Képernyőkép a Bejelentkezési lap személyre szabása lapról.](../media/adddomain.png)

    
4. <span data-ttu-id="ca6b0-117">A varázsló lépéseit követve hozza létre a DNS-rekordokat bármely DNS-szolgáltatónál a [Microsoft 365](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) számára, amely igazolja, hogy Öné a tartomány.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-117">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Microsoft 365](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="ca6b0-118">Ha ismeri a tartományát, olvassa el a [szolgáltatóra vonatkozó utasításokat is.](/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)</span><span class="sxs-lookup"><span data-stu-id="ca6b0-118">If you know your domain host, see also the [host specific instructions](/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="ca6b0-119">Ha az Ön tárhelyszolgáltatója a GoDaddy vagy más szolgáltató, amely támogatja a tartomány [csatlakoztatását,](/office365/admin/get-help-with-domains/domain-connect)a folyamat egyszerű, és a rendszer automatikusan kérni fogja, hogy jelentkezzen be, és a Microsoft hitelesítse magát az Ön nevében.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-119">If your hosting provider is GoDaddy or another host enabled with [domain connect](/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![A GoDaddy Confirm Access (Hozzáférés megerősítése) lapon válassza a Authorize (Engedély) lehetőséget.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="ca6b0-121">Felhasználók felvétele és licencek hozzárendelése</span><span class="sxs-lookup"><span data-stu-id="ca6b0-121">Add users and assign licenses</span></span>

<span data-ttu-id="ca6b0-122">Felvehet felhasználókat a varázslóba, de [](../admin/add-users/add-users.md) később a Felügyeleti központban is.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-122">You can add users in the wizard, but you can also [add users later](../admin/add-users/add-users.md) in the admin center.</span></span> <span data-ttu-id="ca6b0-123">Ha pedig helyi tartományvezérlője van, felhasználókat is felvehet az [Azure AD Connect használatával.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="ca6b0-123">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="ca6b0-124">Felhasználók hozzáadása a varázslóban</span><span class="sxs-lookup"><span data-stu-id="ca6b0-124">Add users in the wizard</span></span>

<span data-ttu-id="ca6b0-125">A varázslóban automatikusan hozzárendel egy Microsoft 365 Vállalati prémium verziós licencet.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-125">Any users you add in the wizard get automatically assigned a Microsoft 365 Business Premium license.</span></span>

![Képernyőkép a varázsló Új felhasználók hozzáadása lapról](../media/addnewuserspage.png)

1. <span data-ttu-id="ca6b0-127">Ha Microsoft 365 Vállalati prémium verziós előfizetése már rendelkezik felhasználókkal (például ha az Azure AD Connectet használta), akkor most lehetősége van licenceket rendelni hozzájuk.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-127">If your Microsoft 365 Business Premium subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="ca6b0-128">Nyugodtan felvehet licenceket hozzájuk is.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-128">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="ca6b0-129">A felhasználók hozzáadása után a hitelesítő adatokat is megoszthatja a felvett új felhasználókkal.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-129">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="ca6b0-130">Ezeket kinyomtathatja, elküldheti e-mailben, vagy pedig letöltheti.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-130">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="ca6b0-131">Tartomány csatlakoztatása</span><span class="sxs-lookup"><span data-stu-id="ca6b0-131">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="ca6b0-132">Ha az .onmicrosoft tartományt választotta, vagy az Azure AD Connect segítségével beállította a felhasználókat, ez a lépés nem látható.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-132">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="ca6b0-133">A szolgáltatások beállításához frissítenie kell bizonyos rekordokat a DNS-szolgáltatónál vagy a tartományregisztrálónál.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-133">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="ca6b0-134">A beállítási varázsló általában felismeri a regisztrálóját, és részletes útmutatást jelenít meg arról, hogy miként frissítheti a névkiszolgálói rekordokat a regisztráló webhelyén.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-134">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="ca6b0-135">Ha nem, módosítsa a névkiszolgálókat úgy, hogy a [Microsoft 365-öt bármely tartományregisztrálónál beállítsa.](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md)</span><span class="sxs-lookup"><span data-stu-id="ca6b0-135">If it doesn't, [Change nameservers to set up Microsoft 365 with any domain registrar](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md).</span></span> 

    - <span data-ttu-id="ca6b0-136">Ha van meglévő DNS-rekordja, például egy meglévő webhelye, de a DNS-szolgáltató engedélyezve van a [tartományhoz](/office365/admin/get-help-with-domains/domain-connect)való csatlakozáshoz, válassza a Rekordok hozzáadása **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ca6b0-136">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="ca6b0-137">A Choose **your online services (Online szolgáltatások kiválasztása)** lapon fogadja el az összes alapértelmezett beállítást, és válassza a **Tovább**, majd az **Authorize** (Engedély) lehetőséget a DNS-szolgáltatója lapján.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-137">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="ca6b0-138">Ha más DNS-szolgáltatónál már van DNS-rekordja (a tartomány csatlakoztatása nem engedélyezett), akkor saját DNS-rekordjait kell kezelnie, hogy a meglévő szolgáltatások kapcsolatban maradjanak.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-138">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="ca6b0-139">További [információt a tartományokkal kapcsolatos alapismeretek](/office365/admin/get-help-with-domains/dns-basics) között található.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-139">See [domain basics](/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Rekordok aktiválása lap.](../media/activaterecords.png)

2. <span data-ttu-id="ca6b0-141">Kövesse a varázsló lépéseit, és állítsa be Önnek a levelezést és más szolgáltatásokat.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-141">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="ca6b0-142">A szervezet védelme</span><span class="sxs-lookup"><span data-stu-id="ca6b0-142">Protect your organization</span></span> 

<span data-ttu-id="ca6b0-143">A varázslóban beállított házirendek automatikusan vonatkoznak a Minden [felhasználó](/office365/admin/create-groups/compare-groups#security-groups) nevű biztonsági *csoportra.*</span><span class="sxs-lookup"><span data-stu-id="ca6b0-143">The policies you set up in the wizard are applied automatically to a [Security group](/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="ca6b0-144">További csoportokat is létrehozhat, amelyekhez házirendeket rendelhet hozzá a Felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-144">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="ca6b0-145">A speciális kiberfenyegetések elleni védelem növelése érdekében javasoljuk, hogy hagyja, hogy az [Office 365 Előzetes](../security/office-365-security/defender-for-office-365.md) veszélyforrások elleni védelem megvizsgálja az Office-appok fájljait és hivatkozásait.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-145">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](../security/office-365-security/defender-for-office-365.md) scan files and links in Office apps.</span></span>

    ![Képernyőkép a Védelem növelése lapról](../media/increasetreatprotection.png)


2. <span data-ttu-id="ca6b0-147">A  Bizalmas adatok kiszivárgásának megakadályozása lapon fogadja el az Office 365 Adatveszteség-megelőzés (DLP) alapértelmezett beállítását a bizalmas adatok nyomon követéséhez az Office-appokban, valamint annak érdekében, hogy megakadályozza ezeknek a szervezeten kívüli véletlen megosztását.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-147">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="ca6b0-148">Az Adatok **védelme az Office mobilappban** lapon hagyja be a mobilappok kezelését, bontsa ki a beállításokat, és tekintse át őket, majd válassza a Mobilappkezelési házirend **létrehozása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ca6b0-148">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Képernyőkép: Adatok védelme a mobil office-ban lap.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="ca6b0-150">Windows 10-es PC-k biztonságossá teve</span><span class="sxs-lookup"><span data-stu-id="ca6b0-150">Secure Windows 10 PCs</span></span>

<span data-ttu-id="ca6b0-151">A bal oldali  navigációs sávon válassza a Beállítás lehetőséget, majd a Bejelentkezés és biztonság alatt válassza A **Windows 10-es számítógépek biztonságának biztosítása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ca6b0-151">On the left nav, select **Setup** and then, under **Sign-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="ca6b0-152">Első **lépésekhez** válassza a Nézet lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-152">Choose **View** to get started.</span></span> <span data-ttu-id="ca6b0-153">Részletes útmutatásért olvassa el a [Windows 10-es](secure-win-10-pcs.md) számítógépek biztonságának biztosítása vonatkozó utasításokat.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-153">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="ca6b0-154">Office 365-ügyfélalkalmazások telepítése</span><span class="sxs-lookup"><span data-stu-id="ca6b0-154">Deploy Office 365 client apps</span></span>

<span data-ttu-id="ca6b0-155">Ha a telepítés során az Office-appok automatikus telepítését választotta, az appok a Windows 10-es eszközökre fognak telepíteni, miután a felhasználók bejelentkeztek az Azure AD szolgáltatásba a windowsos eszközükről a munkahelyi hitelesítő adataik használatával.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-155">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="ca6b0-156">Az Office mobil iOS- vagy Android-eszközökre való telepítéséhez lásd: Mobileszközök beállítása a [Microsoft 365 Business Premium felhasználóinak.](set-up-mobile-devices.md)</span><span class="sxs-lookup"><span data-stu-id="ca6b0-156">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="ca6b0-157">Az Office-t külön is telepítheti.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-157">You can also install Office individually.</span></span> <span data-ttu-id="ca6b0-158">Útmutatásért olvassa el Az [Office telepítése PC-re vagy Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) gépre.</span><span class="sxs-lookup"><span data-stu-id="ca6b0-158">See [install Office on a PC or Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="ca6b0-159">Lásd még</span><span class="sxs-lookup"><span data-stu-id="ca6b0-159">See also</span></span>

[<span data-ttu-id="ca6b0-160">Microsoft 365 Vállalati verzió – oktatóvideók</span><span class="sxs-lookup"><span data-stu-id="ca6b0-160">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)

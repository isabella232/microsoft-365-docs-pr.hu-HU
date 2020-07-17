---
title: A Microsoft 365 Vállalati Prémium verzió beállítása
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
description: Ismerje meg a Microsoft 365 Business Premium beállítási lépéseit, beleértve a tartomány és a felhasználók hozzáadását, a biztonsági házirendek beállítását és egyebeket.
ms.openlocfilehash: efa7934ece0dfeac3c4b20daa37da6f1160901e7
ms.sourcegitcommit: 5b769f74bcc76ac8d38aad815d1728824783cd9f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081902"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a><span data-ttu-id="2d94e-103">A Microsoft 365 Vállalati Prémium verzió beállítása a beállítási varázslóban</span><span class="sxs-lookup"><span data-stu-id="2d94e-103">Set up Microsoft 365 Business Premium in the setup wizard</span></span>

<span data-ttu-id="2d94e-104">Ebből a videóból megtudhatja, hogy miként tekintheti meg a Microsoft 365 Business Premium beállítását.</span><span class="sxs-lookup"><span data-stu-id="2d94e-104">Watch this video for an overview of Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

<span data-ttu-id="2d94e-105">Ha hasznosnak találta ezt a videót, tekintse meg a [teljes tanfolyamok kisvállalatoknak és Microsoft 365-újoncoknak](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) című cikket.</span><span class="sxs-lookup"><span data-stu-id="2d94e-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="2d94e-106">Tartomány, felhasználók hozzáadása és házirendek beállítása</span><span class="sxs-lookup"><span data-stu-id="2d94e-106">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="2d94e-107">A Microsoft 365 Business Premium megvásárlásakor lehetősége van arra, hogy saját tartományt használjon, vagy a [regisztráció](sign-up.md)során megvásárolja.</span><span class="sxs-lookup"><span data-stu-id="2d94e-107">When you purchase Microsoft 365 Business Premium, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="2d94e-108">Ha a regisztrált tartományban új tartományt vásárolt, a tartomány be van állítva, és áthelyezheti a Felhasználók hozzáadása és [a licencek hozzárendelése lehetőséget.](#add-users-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="2d94e-108">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="2d94e-109">A tartomány hozzáadása a bejelentkezés személyre szabásához</span><span class="sxs-lookup"><span data-stu-id="2d94e-109">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="2d94e-110">Jelentkezzen be a [Microsoft 365 Felügyeleti központba](https://admin.microsoft.com) a globális rendszergazdai hitelesítő adatok használatával.</span><span class="sxs-lookup"><span data-stu-id="2d94e-110">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="2d94e-111">A varázsló elindításához válassza **az Ugrás gombot** a beállításhoz.</span><span class="sxs-lookup"><span data-stu-id="2d94e-111">Choose **Go to setup** to start the wizard.</span></span>

    ![Válassza az Ugrás a beállításhoz lehetőséget.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="2d94e-113">Az **Office-alkalmazások telepítése** lapon igény szerint telepítheti az alkalmazásokat a saját számítógépére.</span><span class="sxs-lookup"><span data-stu-id="2d94e-113">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="2d94e-114">A **Tartomány hozzáadása** lépésben adja meg a használni kívánt tartománynevet (például contoso.com).</span><span class="sxs-lookup"><span data-stu-id="2d94e-114">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="2d94e-115">Ha a regisztráció során vásárolt egy tartományt, itt nem jelenik meg **a Tartomány hozzáadása** lépés.</span><span class="sxs-lookup"><span data-stu-id="2d94e-115">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="2d94e-116">Nyissa meg a [Felhasználók hozzáadása](#add-users-and-assign-licenses) lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="2d94e-116">Go to [Add users](#add-users-and-assign-licenses) instead.</span></span>

    ![Képernyőkép a Bejelentkezés testreszabása lapról.](../media/adddomain.png)

    
4. <span data-ttu-id="2d94e-118">Kövesse a varázsló lépéseit a [DNS-rekordok létrehozásához bármely Olyan Microsoft 365-alapú DNS-szolgáltatónál,](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) amely ellenőrzi a tartomány ön általi tulajdonát.</span><span class="sxs-lookup"><span data-stu-id="2d94e-118">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Microsoft 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="2d94e-119">Ha ismeri a tartományi állomást, olvassa el a [gazdagépspecifikus utasításokat](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)is.</span><span class="sxs-lookup"><span data-stu-id="2d94e-119">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="2d94e-120">Ha a tárhelyszolgáltatója A GoDaddy vagy a [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)egy másik állomása, a folyamat egyszerű, és a rendszer automatikusan kéri, hogy jelentkezzen be, és hagyja, hogy a Microsoft hitelesítse magát az Ön nevében.</span><span class="sxs-lookup"><span data-stu-id="2d94e-120">If your hosting provider is GoDaddy or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![A GoDaddy Hozzáférés megerősítése lapján válassza az Engedélyezés lehetőséget.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="2d94e-122">Felhasználók felvétele és licencek hozzárendelése</span><span class="sxs-lookup"><span data-stu-id="2d94e-122">Add users and assign licenses</span></span>

<span data-ttu-id="2d94e-123">A varázslóban hozzáadhat felhasználókat, de később a felügyeleti központban is [hozzáadhat felhasználókat.](add-users-m365b.md)</span><span class="sxs-lookup"><span data-stu-id="2d94e-123">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="2d94e-124">Továbbá, ha rendelkezik egy helyi tartományvezérlővel, hozzáadhat felhasználókat az [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)használatával.</span><span class="sxs-lookup"><span data-stu-id="2d94e-124">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="2d94e-125">Felhasználók felvétele a varázslóba</span><span class="sxs-lookup"><span data-stu-id="2d94e-125">Add users in the wizard</span></span>

<span data-ttu-id="2d94e-126">A varázslóban hozzáadott felhasználók automatikusan Microsoft 365 Business Premium licencet kapnak.</span><span class="sxs-lookup"><span data-stu-id="2d94e-126">Any users you add in the wizard get automatically assigned a Microsoft 365 Business Premium license.</span></span>

![Képernyőkép a varázsló Új felhasználók hozzáadása lapjáról](../media/addnewuserspage.png)

1. <span data-ttu-id="2d94e-128">Ha a Microsoft 365 Business Premium-előfizetése meglévő felhasználókkal rendelkezik (például ha az Azure AD Connectet használta), most lehetősége van licenceket rendelni hozzájuk.</span><span class="sxs-lookup"><span data-stu-id="2d94e-128">If your Microsoft 365 Business Premium subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="2d94e-129">Nyugodtan felvehet licenceket hozzájuk is.</span><span class="sxs-lookup"><span data-stu-id="2d94e-129">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="2d94e-130">Miután hozzáadta a felhasználókat, lehetősége van a hitelesítő adatok megosztására a hozzáadott új felhasználókkal.</span><span class="sxs-lookup"><span data-stu-id="2d94e-130">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="2d94e-131">Ezeket kinyomtathatja, elküldheti e-mailben, vagy pedig letöltheti.</span><span class="sxs-lookup"><span data-stu-id="2d94e-131">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="2d94e-132">Tartomány csatlakoztatása</span><span class="sxs-lookup"><span data-stu-id="2d94e-132">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="2d94e-133">Ha az .onmicrosoft tartomány t választotta, vagy az Azure AD Connect használatával állította be a felhasználókat, akkor ez a lépés nem jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="2d94e-133">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="2d94e-134">A szolgáltatások beállításához frissítenie kell bizonyos rekordokat a DNS-szolgáltatónál vagy a tartományregisztrálónál.</span><span class="sxs-lookup"><span data-stu-id="2d94e-134">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="2d94e-135">A beállítási varázsló általában felismeri a regisztrálóját, és részletes útmutatást jelenít meg arról, hogy miként frissítheti a névkiszolgálói rekordokat a regisztráló webhelyén.</span><span class="sxs-lookup"><span data-stu-id="2d94e-135">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="2d94e-136">Ha nem, módosítsa a [névkiszolgálókat, hogy a Microsoft 365-öt bármely tartományregisztrálóval állítsa be.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="2d94e-136">If it doesn't, [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar).</span></span> 

    - <span data-ttu-id="2d94e-137">Ha már rendelkezik meglévő DNS-rekordokkal, például egy meglévő webwebhelytel, de a DNS-szolgáltatója engedélyezve van a [tartománycsatlakozáshoz,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)válassza **a Rekordok hozzáadása nekem**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="2d94e-137">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="2d94e-138">Az **Online szolgáltatások kiválasztása** lapon fogadja el az összes alapértelmezést, és válassza a **Tovább**gombot, és válassza a DNS-szolgáltató lapján az **Engedélyezés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="2d94e-138">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="2d94e-139">Ha más DNS-állomásokkal is rendelkezik DNS-rekordokkal (nincs engedélyezve a tartománycsatlakozáshoz), akkor a meglévő szolgáltatások kapcsolatának biztosítása érdekében saját DNS-rekordjait kell kezelnie.</span><span class="sxs-lookup"><span data-stu-id="2d94e-139">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="2d94e-140">További információ a [tartományokkal kapcsolatos alapvető tudnivalókról.](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics)</span><span class="sxs-lookup"><span data-stu-id="2d94e-140">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Rekordok aktiválása lap.](../media/activaterecords.png)

2. <span data-ttu-id="2d94e-142">Kövesse a varázsló lépéseit, és az e-mail és egyéb szolgáltatások be lesznek állítva.</span><span class="sxs-lookup"><span data-stu-id="2d94e-142">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="2d94e-143">A szervezet védelme</span><span class="sxs-lookup"><span data-stu-id="2d94e-143">Protect your organization</span></span> 

<span data-ttu-id="2d94e-144">A varázslóban beállított házirendek automatikusan érvénybe lépnek a Minden felhasználó nevű [biztonsági](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) *csoportra.*</span><span class="sxs-lookup"><span data-stu-id="2d94e-144">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="2d94e-145">A felügyeleti központban további csoportokat is létrehozhat, amelyekhez házirendeket rendelhet.</span><span class="sxs-lookup"><span data-stu-id="2d94e-145">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="2d94e-146">A Fokozott védelem növelése a **fejlett kiberfenyegetésekkel**szembeni védelem beállításnál ajánlott elfogadni azokat az alapértelmezett beállításokat, amelyek lehetővé teszik, hogy az [Office 365 Előzetes veszélyforrások elleni védelem](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) fájlokat és hivatkozásokat késebősebben az Office-alkalmazásokban.</span><span class="sxs-lookup"><span data-stu-id="2d94e-146">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) scan files and links in Office apps.</span></span>

    ![Képernyőkép: Védelem növelése lap.](../media/increasetreatprotection.png)


2. <span data-ttu-id="2d94e-148">A **Bizalmas adatok kiszivárgásának megelőzése** lapon fogadja el az Office 365 adatveszteség-megelőzési (DLP) bekapcsolását a bizalmas adatok Office-alkalmazásokban való nyomon követéséhez és a szervezeten kívüli véletlen megosztás megakadályozásához.</span><span class="sxs-lookup"><span data-stu-id="2d94e-148">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="2d94e-149">Az Adatok védelme az **Office mobilszolgáltatásban** lapon hagyja bekapcsolva a mobilalkalmazás-kezelést, bontsa ki a beállításokat, és tekintse át őket, majd válassza **a Mobilalkalmazás-kezelési szabályzat létrehozása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="2d94e-149">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Képernyőkép: Adatok védelme az Office mobilon alkalmazásban lapról.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="2d94e-151">Biztonságos Windows 10-es számítógépek</span><span class="sxs-lookup"><span data-stu-id="2d94e-151">Secure Windows 10 PCs</span></span>

<span data-ttu-id="2d94e-152">A bal oldali navigációs sávon válassza a **Telepítés** lehetőséget, majd a Bejelentkezés és biztonság csoportban válassza **a Windows 10-es számítógépek védelme**lehetőséget. **Sign-in and security**</span><span class="sxs-lookup"><span data-stu-id="2d94e-152">On the left nav, select **Setup** and then, under **Sign-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="2d94e-153">A kezdéshez válassza a **Nézet** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="2d94e-153">Choose **View** to get started.</span></span> <span data-ttu-id="2d94e-154">A teljes körű útmutatásért tekintse meg [a Windows 10-es számítógépek biztonságossá](secure-win-10-pcs.md) tétele.</span><span class="sxs-lookup"><span data-stu-id="2d94e-154">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="2d94e-155">Office 365-ügyfélalkalmazások telepítése</span><span class="sxs-lookup"><span data-stu-id="2d94e-155">Deploy Office 365 client apps</span></span>

<span data-ttu-id="2d94e-156">Ha úgy döntött, hogy a telepítés során automatikusan telepíti az Office-alkalmazásokat, az alkalmazások akkor települnek a Windows 10-es eszközökre, amikor a felhasználók bejelentkeztek az Azure AD-be a Windows-eszközeikről, a munkahelyi hitelesítő adataik használatával.</span><span class="sxs-lookup"><span data-stu-id="2d94e-156">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="2d94e-157">Az Office mobilos iOS- vagy Android-eszközökre való telepítéséről a [Mobileszközök beállítása Microsoft 365 Vállalati Prémium verziófelhasználói számára című](set-up-mobile-devices.md)témakörben található.</span><span class="sxs-lookup"><span data-stu-id="2d94e-157">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="2d94e-158">Az Office-t külön is telepítheti.</span><span class="sxs-lookup"><span data-stu-id="2d94e-158">You can also install Office individually.</span></span> <span data-ttu-id="2d94e-159">További információt [az Office telepítése PC-re vagy Mac gépre](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="2d94e-159">See [install Office on a PC or Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="2d94e-160">Lásd még</span><span class="sxs-lookup"><span data-stu-id="2d94e-160">See also</span></span>

[<span data-ttu-id="2d94e-161">Microsoft 365 üzleti oktatóvideók</span><span class="sxs-lookup"><span data-stu-id="2d94e-161">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)

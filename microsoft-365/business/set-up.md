---
title: A Microsoft 365 Business beállítása
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Útmutató a Microsoft 365 Business beállításához.
ms.openlocfilehash: 0001c2b9962f6cce0be1f77cbf427c68f9ee3249
ms.sourcegitcommit: c5ca71d6feb0f033b50ccd4de816fd59b0925007
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/04/2019
ms.locfileid: "39831303"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="6ff3c-103">A Microsoft 365 Business beállítása a telepítővarázslóban</span><span class="sxs-lookup"><span data-stu-id="6ff3c-103">Set up Microsoft 365 Business in the setup wizard</span></span>

<span data-ttu-id="6ff3c-104">Tekintse meg a Microsoft 365 Business beállítását ismertető videót.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-104">Watch this video for an overview of Microsoft 365 Business setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

<span data-ttu-id="6ff3c-105">Ha Ön alapít ez video segíteni kész, kijelenti magát a [kiegészít képzés sor részére kicsi teendő és azok új-hoz mikroszkóp 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="6ff3c-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="6ff3c-106">A tartomány, a felhasználók és a házirendek beállítása</span><span class="sxs-lookup"><span data-stu-id="6ff3c-106">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="6ff3c-107">[![A megjelenő címke figyelmeztet a felügyeleti központ változásaira, további részleteket itt talál: aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="6ff3c-107">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="6ff3c-108">Amikor vagy megvásárol Mikroszkóp 365 teendő, Önnek van a választás-ból használ egy birtok Ön saját, vagy buying egy közben a [jel-megjelöl](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="6ff3c-108">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="6ff3c-109">Ha a feliratkozáskor új tartományt vásárolt, akkor a tartománya be van állítva, és segítségével [felhasználókat vehet fel és licenceket rendelhet](#add-users-and-assign-licenses)hozzá.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-109">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="6ff3c-110">Saját tartomány felvétele a bejelentkezés személyre szabásához</span><span class="sxs-lookup"><span data-stu-id="6ff3c-110">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="6ff3c-111">Jelentkezzen be a [Microsoft 365 felügyeleti központba](https://admin.microsoft.com) a globális rendszergazdai hitelesítő adatok használatával.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-111">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="6ff3c-112">A varázsló elindításához válassza a **mehet beállítást** .</span><span class="sxs-lookup"><span data-stu-id="6ff3c-112">Choose **Go to setup** to start the wizard.</span></span>

    ![Válassza az Ugrás a telepítéshez beállítást.](media/gotosetupinadmincenter.png)

3. <span data-ttu-id="6ff3c-114">Az **Office alkalmazások telepítése** lapon tetszés szerint telepítheti az alkalmazásokat a saját számítógépére.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-114">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="6ff3c-115">A **tartomány hozzáadása** lépésben adja meg a használni kívánt tartománynevet (például contoso.com).</span><span class="sxs-lookup"><span data-stu-id="6ff3c-115">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="6ff3c-116">Ha a regisztráció során tartományt vásárolt, akkor itt nem jelenik meg **a domainlépés hozzáadása** .</span><span class="sxs-lookup"><span data-stu-id="6ff3c-116">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="6ff3c-117">Tovább a [felhasználók hozzáadásához](#add-users-and-assign-licenses) helyette.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-117">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![Ernyőz-ból megszemélyesít-a jel--ban oldal.](media/adddomain.png)

    
4. <span data-ttu-id="6ff3c-119">A varázsló lépéseit követve [hozzon létre DNS-rekordokat az Office 365 olyan DNS-](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) szolgáltatójánál, amely igazolja, hogy Ön a tartomány tulajdonosa.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-119">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="6ff3c-120">Ha ismeri a domainnevét, akkor tekintse meg a [gazdagép utasításait](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)is.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-120">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="6ff3c-121">Ha a tárhely szolgáltató GoDaddy vagy más Host engedélyezve [domain Connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), a folyamat egyszerű, és akkor automatikusan felkérték, hogy jelentkezzen be, és hagyja, hogy a Microsoft hitelesít az Ön nevében.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-121">If your hosting provider is GoDaddy or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![-Ra GoDaddy igazol belépés oldal, kiválaszt engedélyez.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="6ff3c-123">Felhasználók felvétele és licencek hozzárendelése</span><span class="sxs-lookup"><span data-stu-id="6ff3c-123">Add users and assign licenses</span></span>

<span data-ttu-id="6ff3c-124">Felhasználókat felvehet a varázslóba, de később az admin központban is [hozzáadhat felhasználókat](add-users-m365b.md) .</span><span class="sxs-lookup"><span data-stu-id="6ff3c-124">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="6ff3c-125">Ezenkívül, ha van helyi tartományvezérlője, hozzáadhat felhasználókat a [Azure ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)segítségével.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-125">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="6ff3c-126">Felhasználók hozzáadása a varázslóhoz</span><span class="sxs-lookup"><span data-stu-id="6ff3c-126">Add users in the wizard</span></span>

<span data-ttu-id="6ff3c-127">A varázslóban hozzáadott felhasználók automatikusan Microsoft 365 üzleti licencet kapnak.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-127">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![Az új felhasználók hozzáadása lap képernyőképe a varázslóban](media/addnewuserspage.png)

1. <span data-ttu-id="6ff3c-129">Ha a Microsoft 365 üzleti előfizetés már meglévő felhasználókkal rendelkezik (például, ha a Azure AD Connect szolgáltatást használta), akkor most lehetősége van licencek kiosztésére.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-129">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="6ff3c-130">Nyugodtan felvehet licenceket hozzájuk is.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-130">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="6ff3c-131">A felhasználók hozzáadása után lehetőség van a hitelesítő adatok megosztására is az új felhasználókkal.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-131">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="6ff3c-132">Ezeket kinyomtathatja, elküldheti e-mailben, vagy pedig letöltheti.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-132">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="6ff3c-133">Tartomány csatlakoztatása</span><span class="sxs-lookup"><span data-stu-id="6ff3c-133">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="6ff3c-134">Ha az. onmicrosoft tartomány használata mellett döntött, vagy a felhasználók beállításához a Azure AD Connect szolgáltatást használja, akkor ezt a lépést nem fogja látni.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-134">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="6ff3c-135">A szolgáltatások beállításához frissítenie kell bizonyos rekordokat a DNS-szolgáltatónál vagy a tartományregisztrálónál.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-135">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="6ff3c-136">A beállítási varázsló általában felismeri a regisztrálóját, és részletes útmutatást jelenít meg arról, hogy miként frissítheti a névkiszolgálói rekordokat a regisztráló webhelyén.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-136">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="6ff3c-137">Ha nem, [módosítsa a névszervereket az Office 365 beállításához bármely tartományregisztrálóval](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="6ff3c-137">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="6ff3c-138">Ha vannak meglévő DNS-rekordjai, például egy meglévő webhely, de a DNS-állomás a tartományhoz történő [kapcsolódáshoz](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)engedélyezve van, válassza **a saját rekord hozzáadása**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-138">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="6ff3c-139">Az **online szolgáltatások kiválasztása** lapon fogadja el az összes alapértelmezett beállításokat, majd kattintson a **Tovább gombra**, és válassza az engedélyezés a DNS-állomás oldalán **engedélyt** .</span><span class="sxs-lookup"><span data-stu-id="6ff3c-139">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="6ff3c-140">Ha van meglévő DNS-rekordja más DNS-állomásokkal (nincs engedélyezve a tartomány csatlakoztatásához), saját DNS-rekordokat kell kezelnie annak érdekében, hogy a meglévő szolgáltatások ne maradjanak kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-140">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="6ff3c-141">További információ a [tartomány alapjai](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) című témakörben található.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-141">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![A rekordok oldal aktiválása.](media/activaterecords.png)

2. <span data-ttu-id="6ff3c-143">Kövesse a varázsló lépéseit, és az e-mail és egyéb szolgáltatások lesznek beállítva az Ön számára.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-143">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="6ff3c-144">A szervezet védelme</span><span class="sxs-lookup"><span data-stu-id="6ff3c-144">Protect your organization</span></span> 

<span data-ttu-id="6ff3c-145">A varázslóban beállított házirendek automatikusan alkalmazásra kerülnek a *minden felhasználó*nevű [biztonsági csoportra](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) .</span><span class="sxs-lookup"><span data-stu-id="6ff3c-145">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="6ff3c-146">További csoportokat is létrehozhat, ha házirendeket rendel az admin Centerhez.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-146">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="6ff3c-147">A **növekedés elleni védelem a fejlett számítógépes fenyegetések**, ajánlott, hogy fogadja el az alapértelmezett, hogy hagyja [Office 365 Advance fenyegetés védelem](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) Scan fájlokat és linkeket az Office alkalmazásokban.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-147">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) scan files and links in Office apps.</span></span>

    ![Ernyőz-ból növekszik védelem oldal.](media/increasetreatprotection.png)


2. <span data-ttu-id="6ff3c-149">-On **megakadályoz átereszt-ból érzékeny adat** oldal, elfogad a hiba-hoz megereszt Hivatal 365 adat elvesztés megakadályozás (DLP)-hoz nyom érzékeny adat-ban Hivatal apps és megakadályoz a esetleges cserépdarab-ból ezek külső rész-a szervezet.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-149">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="6ff3c-150">Az **Office mobileszközre szánt adatok védelme** lapon hagyja meg a mobilalkalmazás-kezelés beállítást, bontsa ki a beállításokat, és tekintse át őket, majd válassza a **mobilalkalmazás-kezelési házirend létrehozása**beállítást.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-150">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Ernyőz-ból megvéd adat-ban hivatal részére mozgatható oldal.](media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="6ff3c-152">Biztonságos Windows 10 PC-k</span><span class="sxs-lookup"><span data-stu-id="6ff3c-152">Secure Windows 10 PCs</span></span>

<span data-ttu-id="6ff3c-153">-On bal NAV, kiválaszt **beállít** aztán, alatt **énekel--ban és biztonság**, választ **biztosít-a Windows 10 számítógépek**.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-153">On the left nav, select **Setup** and then, under **Sing-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="6ff3c-154">A **megtekintéshez** válassza a nézet-t.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-154">Choose **View** to get started.</span></span> <span data-ttu-id="6ff3c-155">A [Windows 10 rendszerű számítógép biztonságossá tétele](secure-win-10-pcs.md) teljes körű utasításokért lásd:</span><span class="sxs-lookup"><span data-stu-id="6ff3c-155">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="6ff3c-156">Az Office 365 ügyfélalkalmazások telepítése</span><span class="sxs-lookup"><span data-stu-id="6ff3c-156">Deploy Office 365 client apps</span></span>

<span data-ttu-id="6ff3c-157">Ha úgy dönt, hogy telepítéskor automatikusan telepíti az Office-alkalmazásokat, az alkalmazások a Windows 10 eszközökre fognak telepíteni, amint a felhasználók a Azure AD rendszerbe be vannak jelentkezve a saját felhasználói hitelesítő adataik segítségével.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-157">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="6ff3c-158">Az Office mobil iOS vagy Android eszközökre történő telepítéséhez tekintse meg [a mobileszközök beállítása a Microsoft 365 üzleti felhasználók számára](set-up-mobile-devices.md)című témakört.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-158">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="6ff3c-159">Az Office programot egyenként is telepíthetjük.</span><span class="sxs-lookup"><span data-stu-id="6ff3c-159">You can also install Office individually.</span></span> <span data-ttu-id="6ff3c-160">Útmutatás: az [Office telepítése PC vagy Mac számítógépre](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) .</span><span class="sxs-lookup"><span data-stu-id="6ff3c-160">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="6ff3c-161">See also</span><span class="sxs-lookup"><span data-stu-id="6ff3c-161">See also</span></span>

[<span data-ttu-id="6ff3c-162">Microsoft 365 üzleti képzési videók</span><span class="sxs-lookup"><span data-stu-id="6ff3c-162">Microsoft 365 Business training videos</span></span>](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)

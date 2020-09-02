---
title: A Microsoft 365 vállalati prémium verzió beállítása
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
description: Ismerje meg a Microsoft 365 vállalati prémium verzió beállítási lépéseit, például a tartomány és a felhasználók hozzáadását, a biztonsági házirendek beállítását és sok mást.
ms.openlocfilehash: cc20637d7a78bd34ecb61a4ed46eb06d564d63df
ms.sourcegitcommit: 25afc0c34edc7f8a5eb389d8c701175256c58ec8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/01/2020
ms.locfileid: "47324496"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a><span data-ttu-id="0fee5-103">A Microsoft 365 vállalati prémium verzió beállítása a beállítási varázslóban</span><span class="sxs-lookup"><span data-stu-id="0fee5-103">Set up Microsoft 365 Business Premium in the setup wizard</span></span>

<span data-ttu-id="0fee5-104">Ebből a videóból áttekintést kaphat a Microsoft 365 vállalati prémium verzió telepítéséről.</span><span class="sxs-lookup"><span data-stu-id="0fee5-104">Watch this video for an overview of Microsoft 365 Business Premium setup.</span></span><br><br>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="0fee5-105">A tartomány, a felhasználók és a házirendek beállítása</span><span class="sxs-lookup"><span data-stu-id="0fee5-105">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="0fee5-106">Amikor megvásárolja a Microsoft 365 Business Premiumot, lehetősége van a saját tartomány használatára, vagy a [regisztráció](sign-up.md)során egyet vásárolni.</span><span class="sxs-lookup"><span data-stu-id="0fee5-106">When you purchase Microsoft 365 Business Premium, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="0fee5-107">Ha regisztrációkor új tartományt vásárolt, a tartománya minden beállítása, és áthelyezheti a [felhasználók hozzáadását és a licencek hozzárendelését](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="0fee5-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="0fee5-108">Saját tartomány hozzáadása a bejelentkezés személyre szabásához</span><span class="sxs-lookup"><span data-stu-id="0fee5-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="0fee5-109">A [Microsoft 365 felügyeleti központba](https://admin.microsoft.com) a globális rendszergazdai hitelesítő adataival jelentkezhet be.</span><span class="sxs-lookup"><span data-stu-id="0fee5-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="0fee5-110">A varázsló indításához válassza az **Ugrás a beállításra** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="0fee5-110">Choose **Go to setup** to start the wizard.</span></span>

    ![Kattintson az Ugrás a beállításra elemre.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="0fee5-112">Az **Office-alkalmazások telepítése** lapon igény szerint telepítheti az alkalmazásokat saját számítógépére.</span><span class="sxs-lookup"><span data-stu-id="0fee5-112">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="0fee5-113">A **tartomány hozzáadása** lépésben adja meg a használni kívánt tartománynevet (például contoso.com).</span><span class="sxs-lookup"><span data-stu-id="0fee5-113">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="0fee5-114">Ha a regisztráció során megvásárolt egy tartományt, itt nem jelenik meg **a tartomány felvétele** lépés.</span><span class="sxs-lookup"><span data-stu-id="0fee5-114">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="0fee5-115">Nyissa meg a [felhasználók felvétele](#add-users-and-assign-licenses) helyet.</span><span class="sxs-lookup"><span data-stu-id="0fee5-115">Go to [Add users](#add-users-and-assign-licenses) instead.</span></span>

    ![Képernyőkép: a bejelentkezési lap személyre szabása.](../media/adddomain.png)

    
4. <span data-ttu-id="0fee5-117">A varázsló lépéseit követve [hozzon létre DNS-rekordokat bármely DNS-szolgáltatónál a Microsoft 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) , amely igazolja, hogy Ön a tartomány tulajdonosa.</span><span class="sxs-lookup"><span data-stu-id="0fee5-117">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Microsoft 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="0fee5-118">Ha ismeri a tartomány szolgáltatóját, olvassa el a [Host-specifikus utasítások](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)című témakört is.</span><span class="sxs-lookup"><span data-stu-id="0fee5-118">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="0fee5-119">Ha szolgáltatójánál a GoDaddy vagy egy másik állomás engedélyezve van a [tartomány csatlakozásakor](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), a folyamat egyszerű, és automatikusan kéri a bejelentkezést, és hagyja, hogy a Microsoft hitelesítse az Ön nevében.</span><span class="sxs-lookup"><span data-stu-id="0fee5-119">If your hosting provider is GoDaddy or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![A GoDaddy hozzáférés megerősítése lapon válassza az Engedélyezés lehetőséget.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="0fee5-121">Felhasználók felvétele és licencek hozzárendelése</span><span class="sxs-lookup"><span data-stu-id="0fee5-121">Add users and assign licenses</span></span>

<span data-ttu-id="0fee5-122">Hozzáadhat felhasználókat a varázslóban, de [később is hozzáadhat felhasználókat](add-users-m365b.md) a felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="0fee5-122">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="0fee5-123">Ha helyi tartományvezérlőt használ, akkor az [Azure ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)segítségével felhasználókat vehet fel.</span><span class="sxs-lookup"><span data-stu-id="0fee5-123">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="0fee5-124">Felhasználók hozzáadása a varázslóban</span><span class="sxs-lookup"><span data-stu-id="0fee5-124">Add users in the wizard</span></span>

<span data-ttu-id="0fee5-125">A varázslóban hozzáadott minden felhasználó automatikusan hozzárendeli a Microsoft 365 vállalati prémium verzió licencét.</span><span class="sxs-lookup"><span data-stu-id="0fee5-125">Any users you add in the wizard get automatically assigned a Microsoft 365 Business Premium license.</span></span>

![Képernyőkép a varázsló új felhasználók hozzáadása lapjáról](../media/addnewuserspage.png)

1. <span data-ttu-id="0fee5-127">Ha a Microsoft 365 vállalati prémium verzióra szóló előfizetése meglévő felhasználókkal rendelkezik (például az Azure AD Connectt használta), akkor lehetősége van arra, hogy most rendelje hozzá a licenceket.</span><span class="sxs-lookup"><span data-stu-id="0fee5-127">If your Microsoft 365 Business Premium subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="0fee5-128">Nyugodtan felvehet licenceket hozzájuk is.</span><span class="sxs-lookup"><span data-stu-id="0fee5-128">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="0fee5-129">Miután hozzáadta a felhasználókat, megoszthatja a hitelesítő adatokat a hozzáadott új felhasználókkal.</span><span class="sxs-lookup"><span data-stu-id="0fee5-129">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="0fee5-130">Ezeket kinyomtathatja, elküldheti e-mailben, vagy pedig letöltheti.</span><span class="sxs-lookup"><span data-stu-id="0fee5-130">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="0fee5-131">Tartomány csatlakoztatása</span><span class="sxs-lookup"><span data-stu-id="0fee5-131">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="0fee5-132">Ha az. onmicrosoft tartomány használatát választotta, vagy az Azure AD Connectt használja a felhasználók beállításához, akkor nem fogja látni ezt a lépést.</span><span class="sxs-lookup"><span data-stu-id="0fee5-132">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="0fee5-133">A szolgáltatások beállításához frissítenie kell bizonyos rekordokat a DNS-szolgáltatónál vagy a tartományregisztrálónál.</span><span class="sxs-lookup"><span data-stu-id="0fee5-133">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="0fee5-134">A beállítási varázsló általában felismeri a regisztrálóját, és részletes útmutatást jelenít meg arról, hogy miként frissítheti a névkiszolgálói rekordokat a regisztráló webhelyén.</span><span class="sxs-lookup"><span data-stu-id="0fee5-134">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="0fee5-135">Ha nem, [módosítsa a névkiszolgálók beállítást a Microsoft 365 bármely tartományregisztrálónál való beállításához](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar).</span><span class="sxs-lookup"><span data-stu-id="0fee5-135">If it doesn't, [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar).</span></span> 

    - <span data-ttu-id="0fee5-136">Ha van meglévő DNS-rekordja (például egy meglévő webhely), de a DNS-szolgáltatója engedélyezve van a [tartomány csatlakoztatása](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)beállításnál, válassza a saját **rekordok hozzáadása**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="0fee5-136">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="0fee5-137">Az **online szolgáltatások kiválasztása** lapon fogadja el az összes alapértelmezett elemet, és válassza a **tovább**gombot, és válassza a DNS-szolgáltatója lapon az **Engedélyezés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="0fee5-137">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="0fee5-138">Ha meglévő DNS-rekordjait más DNS-szolgáltatókkal (nem engedélyezett a tartományhoz való csatlakozáskor) szeretné használni, kezelje saját DNS-rekordjait, és ellenőrizze, hogy a meglévő szolgáltatások maradnak-e csatlakoztatva.</span><span class="sxs-lookup"><span data-stu-id="0fee5-138">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="0fee5-139">További információt a [tartomány alapjai](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="0fee5-139">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![A rekordok aktiválása lap](../media/activaterecords.png)

2. <span data-ttu-id="0fee5-141">Kövesse a varázsló lépéseit, és az e-mailek és más szolgáltatások beállításra kerülnek.</span><span class="sxs-lookup"><span data-stu-id="0fee5-141">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="0fee5-142">A szervezet védelme</span><span class="sxs-lookup"><span data-stu-id="0fee5-142">Protect your organization</span></span> 

<span data-ttu-id="0fee5-143">A varázslóban beállított házirendeket a rendszer automatikusan alkalmazza az *összes felhasználó*nevű [biztonsági csoportba](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) .</span><span class="sxs-lookup"><span data-stu-id="0fee5-143">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="0fee5-144">Létrehozhat további csoportokat is, amelyekkel a felügyeleti központban megadhatja a házirendeket.</span><span class="sxs-lookup"><span data-stu-id="0fee5-144">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="0fee5-145">A **speciális Cyber-fenyegetések elleni védelem fokozása**érdekében ajánlott elfogadnia az alapértelmezett beállításokat, hogy az [Office 365 előzetes veszélyforrásokkal védett](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) fájlok és hivatkozások legyenek az Office-alkalmazásokban.</span><span class="sxs-lookup"><span data-stu-id="0fee5-145">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) scan files and links in Office apps.</span></span>

    ![Képernyőkép a védelem növelése lapról.](../media/increasetreatprotection.png)


2. <span data-ttu-id="0fee5-147">A **bizalmas adatok szivárgásának megakadályozása** lapon fogadja el az alapértelmezett adatokat az Office 365 adatvesztés-megelőzés (DLP) bekapcsolásához az Office-alkalmazásokban lévő bizalmas adatok nyomon követéséhez és a szervezeten kívüli adatok véletlenszerű megosztásához.</span><span class="sxs-lookup"><span data-stu-id="0fee5-147">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="0fee5-148">Az **Adatvédelem az Office Mobile-ban** lapon hagyja meg a mobil app-kezelés lehetőséget, bontsa ki a beállításokat, és tekintse át őket, és válassza a **mobil app-kezelési házirend létrehozása**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="0fee5-148">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Képernyőkép az adatvédelemről az Office for Mobile lapon.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="0fee5-150">Windows 10-es számítógépek biztonságossá tétele</span><span class="sxs-lookup"><span data-stu-id="0fee5-150">Secure Windows 10 PCs</span></span>

<span data-ttu-id="0fee5-151">A bal oldali navigációs sávon válassza a **Setup (beállítás** ) lehetőséget, majd a **Bejelentkezés és biztonság**csoportban válassza **a Windows 10-es számítógépek biztonságossá tétele**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="0fee5-151">On the left nav, select **Setup** and then, under **Sign-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="0fee5-152">A kezdéshez válassza a **nézet** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="0fee5-152">Choose **View** to get started.</span></span> <span data-ttu-id="0fee5-153">A teljes körű útmutatásért olvassa el a [Windows 10-es számítógépek biztonságossá tétele](secure-win-10-pcs.md) című témakört.</span><span class="sxs-lookup"><span data-stu-id="0fee5-153">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="0fee5-154">Az Office 365 ügyfélalkalmazás központi telepítése</span><span class="sxs-lookup"><span data-stu-id="0fee5-154">Deploy Office 365 client apps</span></span>

<span data-ttu-id="0fee5-155">Ha a telepítés során úgy döntött, hogy automatikusan telepíti az Office-alkalmazásokat, az alkalmazások a Windows 10-es eszközökön fognak megjelenni, amint a felhasználók a Windows-eszközökről bejelentkeznek az Azure AD szolgáltatásba, a munkahelyi hitelesítő adataikkal.</span><span class="sxs-lookup"><span data-stu-id="0fee5-155">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="0fee5-156">Ha az Office-t mobil iOS-vagy Android-eszközön szeretné telepíteni, olvassa el a [mobileszközök beállítása a Microsoft 365 vállalati prémium verzió felhasználóinak](set-up-mobile-devices.md)című témakört.</span><span class="sxs-lookup"><span data-stu-id="0fee5-156">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="0fee5-157">Az Office-t külön is telepítheti.</span><span class="sxs-lookup"><span data-stu-id="0fee5-157">You can also install Office individually.</span></span> <span data-ttu-id="0fee5-158">További információt az [Office telepítése PC-re vagy Mac gépre](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="0fee5-158">See [install Office on a PC or Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="0fee5-159">Lásd még</span><span class="sxs-lookup"><span data-stu-id="0fee5-159">See also</span></span>

[<span data-ttu-id="0fee5-160">Microsoft 365 vállalati verziós képzési videók</span><span class="sxs-lookup"><span data-stu-id="0fee5-160">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)

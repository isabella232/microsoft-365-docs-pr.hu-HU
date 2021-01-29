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
description: Megismerheti a Microsoft 365 Vállalati prémium verzió beállítási lépéseit, például tartomány és felhasználók hozzáadását, biztonsági házirendek beállítását és sok más lépést.
ms.openlocfilehash: e7ebe179c67077dc71ae4873b0711d0e810c701a
ms.sourcegitcommit: 1b30ac6e05906c8a014b1fed33fc71e1821f6ad2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/29/2021
ms.locfileid: "50044730"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a><span data-ttu-id="243fb-103">A Microsoft 365 Vállalati prémium verzió beállítása a beállítási varázslóban</span><span class="sxs-lookup"><span data-stu-id="243fb-103">Set up Microsoft 365 Business Premium in the setup wizard</span></span>

<span data-ttu-id="243fb-104">Ebből a videóból áttekintheti a Microsoft 365 Vállalati prémium verzió beállítását.</span><span class="sxs-lookup"><span data-stu-id="243fb-104">Watch this video for an overview of Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="243fb-105">Tartomány, felhasználók hozzáadása és házirendek beállítása</span><span class="sxs-lookup"><span data-stu-id="243fb-105">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="243fb-106">A Microsoft 365 Vállalati prémium verzió megvásárlásakor lehetősége van saját tartományt használni, vagy a regisztráció során vásárolni [egyet.](sign-up.md)</span><span class="sxs-lookup"><span data-stu-id="243fb-106">When you purchase Microsoft 365 Business Premium, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="243fb-107">Ha a feliratkozáskor új tartományt vásárolt, a tartománya be van állítva, és áthelyezheti a Felhasználók hozzáadása és licencek [hozzárendelése gombra.](#add-users-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="243fb-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="243fb-108">Tartomány hozzáadása a bejelentkezés személyre szabása</span><span class="sxs-lookup"><span data-stu-id="243fb-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="243fb-109">Jelentkezzen be a [Microsoft 365](https://admin.microsoft.com) Felügyeleti központba a globális rendszergazdai hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="243fb-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="243fb-110">A **varázslót az Ugrás** a beállításhoz gombra állítva indítsa el.</span><span class="sxs-lookup"><span data-stu-id="243fb-110">Choose **Go to setup** to start the wizard.</span></span>

    ![Válassza az Ugrás a beállításhoz lehetőséget.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="243fb-112">Az **Office-alkalmazások telepítése** lapon tetszés szerint telepítheti az appokat a saját számítógépére.</span><span class="sxs-lookup"><span data-stu-id="243fb-112">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="243fb-113">A Tartomány **hozzáadása lépésben** adja meg a használni kívánt tartománynevet (például contoso.com).</span><span class="sxs-lookup"><span data-stu-id="243fb-113">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="243fb-114">Ha a regisztráció során tartományt vásárolt, itt nem látható a Tartomány **hozzáadása** lépés.</span><span class="sxs-lookup"><span data-stu-id="243fb-114">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="243fb-115">Ehelyett a [Felhasználók hozzáadása gombra.](#add-users-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="243fb-115">Go to [Add users](#add-users-and-assign-licenses) instead.</span></span>

    ![Képernyőkép a Bejelentkezési lap személyre szabása lapról.](../media/adddomain.png)

    
4. <span data-ttu-id="243fb-117">A varázsló lépéseit követve hozza létre a DNS-rekordokat a [Microsoft 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) bármely OLYAN DNS-szolgáltatójánál, amely igazolja, hogy Öné a tartomány.</span><span class="sxs-lookup"><span data-stu-id="243fb-117">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Microsoft 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="243fb-118">Ha ismeri a tartománygazdát, olvassa el a [szolgáltatóra vonatkozó utasításokat is.](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)</span><span class="sxs-lookup"><span data-stu-id="243fb-118">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="243fb-119">Ha tárhelyszolgáltatója a GoDaddy vagy egy tartomány-csatlakozással engedélyezett másik [szolgáltató,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)a folyamat egyszerű, és a rendszer automatikusan kérni fogja, hogy jelentkezzen be, és hagyja, hogy a Microsoft hitelesítse magát az Ön nevében.</span><span class="sxs-lookup"><span data-stu-id="243fb-119">If your hosting provider is GoDaddy or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![On GoDaddy Confirm Access page, select Authorize.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="243fb-121">Felhasználók felvétele és licencek hozzárendelése</span><span class="sxs-lookup"><span data-stu-id="243fb-121">Add users and assign licenses</span></span>

<span data-ttu-id="243fb-122">Felvehet felhasználókat a varázslóba, de [](add-users-m365b.md) később a Felügyeleti központban is felvehet felhasználókat.</span><span class="sxs-lookup"><span data-stu-id="243fb-122">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="243fb-123">Ha pedig helyi tartományvezérlője van, felhasználókat is felvehet az [Azure AD Connect használatával.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="243fb-123">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="243fb-124">Felhasználók hozzáadása a varázslóban</span><span class="sxs-lookup"><span data-stu-id="243fb-124">Add users in the wizard</span></span>

<span data-ttu-id="243fb-125">A varázslóban hozzáadt felhasználók automatikusan hozzárendelnek egy Microsoft 365 Vállalati prémium verziós licencet.</span><span class="sxs-lookup"><span data-stu-id="243fb-125">Any users you add in the wizard get automatically assigned a Microsoft 365 Business Premium license.</span></span>

![Képernyőkép a varázsló Új felhasználók hozzáadása lapról](../media/addnewuserspage.png)

1. <span data-ttu-id="243fb-127">Ha Microsoft 365 Vállalati prémium verziós előfizetése meglévő felhasználókkal rendelkezik (például ha az Azure AD Connectet használta), akkor most lehetősége van licenceket rendelni hozzájuk.</span><span class="sxs-lookup"><span data-stu-id="243fb-127">If your Microsoft 365 Business Premium subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="243fb-128">Nyugodtan felvehet licenceket hozzájuk is.</span><span class="sxs-lookup"><span data-stu-id="243fb-128">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="243fb-129">A felhasználók hozzáadása után a hitelesítő adatokat is megoszthatja a felvett új felhasználókkal.</span><span class="sxs-lookup"><span data-stu-id="243fb-129">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="243fb-130">Ezeket kinyomtathatja, elküldheti e-mailben, vagy pedig letöltheti.</span><span class="sxs-lookup"><span data-stu-id="243fb-130">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="243fb-131">Tartomány csatlakoztatása</span><span class="sxs-lookup"><span data-stu-id="243fb-131">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="243fb-132">Ha az .onmicrosoft tartományt választotta, vagy az Azure AD Connectet használta a felhasználók beállítására, ez a lépés nem látható.</span><span class="sxs-lookup"><span data-stu-id="243fb-132">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="243fb-133">A szolgáltatások beállításához frissítenie kell bizonyos rekordokat a DNS-szolgáltatónál vagy a tartományregisztrálónál.</span><span class="sxs-lookup"><span data-stu-id="243fb-133">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="243fb-134">A beállítási varázsló általában felismeri a regisztrálóját, és részletes útmutatást jelenít meg arról, hogy miként frissítheti a névkiszolgálói rekordokat a regisztráló webhelyén.</span><span class="sxs-lookup"><span data-stu-id="243fb-134">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="243fb-135">Ha nem, módosítsa a névkiszolgálókat úgy, hogy a [Microsoft 365-öt bármely tartományregisztrálónál beállítsa.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="243fb-135">If it doesn't, [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar).</span></span> 

    - <span data-ttu-id="243fb-136">Ha már van DNS-rekordja, például egy meglévő webhelye, [](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)de a DNS-szolgáltató engedélyezte a tartományhoz való csatlakozást, válassza a Rekordok hozzáadása **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="243fb-136">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="243fb-137">Az Online **szolgáltatások kiválasztása** lapon fogadja el az összes alapértelmezett beállítást, válassza a Tovább **gombot,** és válassza az **Authorize** (Engedély) lehetőséget a DNS-szolgáltató lapján.</span><span class="sxs-lookup"><span data-stu-id="243fb-137">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="243fb-138">Ha már van DNS-rekordja más DNS-szolgáltatónál (a tartományhoz való csatlakozáshoz nincs engedélyezve), akkor saját DNS-rekordokat kell kezelnie, hogy a meglévő szolgáltatások kapcsolatban maradjanak.</span><span class="sxs-lookup"><span data-stu-id="243fb-138">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="243fb-139">További [információt a tartományi alapismeretek](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) között láthat.</span><span class="sxs-lookup"><span data-stu-id="243fb-139">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Rekordok aktiválása lap.](../media/activaterecords.png)

2. <span data-ttu-id="243fb-141">Kövesse a varázsló lépéseit, és állítsa be Önnek a levelezést és más szolgáltatásokat.</span><span class="sxs-lookup"><span data-stu-id="243fb-141">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="243fb-142">A szervezet védelme</span><span class="sxs-lookup"><span data-stu-id="243fb-142">Protect your organization</span></span> 

<span data-ttu-id="243fb-143">A varázslóban beállított házirendeket [a](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) program automatikusan alkalmazza a Minden felhasználó nevű biztonsági *csoportra.*</span><span class="sxs-lookup"><span data-stu-id="243fb-143">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="243fb-144">A felügyeleti központban további csoportokat is létrehozhat, amelyekhez házirendeket rendelhet hozzá.</span><span class="sxs-lookup"><span data-stu-id="243fb-144">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="243fb-145">A **speciális** kiberfenyegetések elleni védelem növelése érdekében javasoljuk, hogy hagyja, hogy az [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) átolvassa az Office-appokban lévő fájlokat és hivatkozásokat.</span><span class="sxs-lookup"><span data-stu-id="243fb-145">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) scan files and links in Office apps.</span></span>

    ![Képernyőkép a Védelem növelése lapról](../media/increasetreatprotection.png)


2. <span data-ttu-id="243fb-147">A  bizalmas adatok kiszivárgásának megelőzése lapon fogadja el az Office 365 Adatveszteség-megelőzés (DLP) alapértelmezett beállítását a bizalmas adatok nyomon követéséhez az Office-appokban, és megakadályozza, hogy a szervezeten kívüli adatok véletlenül meg is oszthatóak.</span><span class="sxs-lookup"><span data-stu-id="243fb-147">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="243fb-148">Az **Office** mobileszközökre vonatkozó adatainak védelme lapon hagyja be a mobilappok kezelését, bontsa ki a beállításokat, és tekintse át őket, majd válassza a Mobilappkezelési házirend **létrehozása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="243fb-148">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Képernyőkép az Adatok védelme lapról a Mobil Office-ban.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="243fb-150">Windows 10-es PC-k biztonságossá teve</span><span class="sxs-lookup"><span data-stu-id="243fb-150">Secure Windows 10 PCs</span></span>

<span data-ttu-id="243fb-151">A bal oldali navigációs sávon válassza a **Beállítás** lehetőséget, majd a Bejelentkezés és biztonság alatt válassza a **Windows 10-es számítógépek biztonságának biztosítása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="243fb-151">On the left nav, select **Setup** and then, under **Sign-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="243fb-152">Első **lépésekhez** válassza a Nézet lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="243fb-152">Choose **View** to get started.</span></span> <span data-ttu-id="243fb-153">A [teljes útmutatást a Windows 10-es](secure-win-10-pcs.md) számítógépek biztonságának biztosítása érdekében olvassa el.</span><span class="sxs-lookup"><span data-stu-id="243fb-153">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="243fb-154">Office 365-ügyfélalkalmazások telepítése</span><span class="sxs-lookup"><span data-stu-id="243fb-154">Deploy Office 365 client apps</span></span>

<span data-ttu-id="243fb-155">Ha a telepítés során úgy döntött, hogy automatikusan telepíti az Office-appokat, az appok a Windows 10-es eszközökre fognak telepíteni, miután a felhasználók bejelentkeztek az Azure AD-be a windowsos eszközükről a munkahelyi hitelesítő adataik használatával.</span><span class="sxs-lookup"><span data-stu-id="243fb-155">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="243fb-156">Az Office mobilos iOS- vagy Android-eszközökre való telepítéséhez lásd: Mobileszközök beállítása [a Microsoft 365 Vállalati prémium verzió felhasználóinak.](set-up-mobile-devices.md)</span><span class="sxs-lookup"><span data-stu-id="243fb-156">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="243fb-157">Az Office-t külön is telepítheti.</span><span class="sxs-lookup"><span data-stu-id="243fb-157">You can also install Office individually.</span></span> <span data-ttu-id="243fb-158">Útmutatásért [olvassa el az Office telepítése PC-re](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) vagy Mac gépre.</span><span class="sxs-lookup"><span data-stu-id="243fb-158">See [install Office on a PC or Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="243fb-159">Lásd még</span><span class="sxs-lookup"><span data-stu-id="243fb-159">See also</span></span>

[<span data-ttu-id="243fb-160">Microsoft 365 Vállalati verziós oktatóvideók</span><span class="sxs-lookup"><span data-stu-id="243fb-160">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)

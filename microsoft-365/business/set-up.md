---
title: A Microsoft 365 Business beállítása
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Fedezze fel a Microsoft 365 Vállalati verzió beállítási lépéseit, beleértve a tartomány és a felhasználók hozzáadását, a biztonsági házirendek beállítását stb.
ms.openlocfilehash: 99994b6f1e9e817b4858aeafe4ce3ceaaf4c3c37
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/07/2020
ms.locfileid: "42561183"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="c94b4-103">A Microsoft 365 Business beállítása a telepítővarázslóban</span><span class="sxs-lookup"><span data-stu-id="c94b4-103">Set up Microsoft 365 Business in the setup wizard</span></span>

<span data-ttu-id="c94b4-104">Ebből a videóból megtudhatja, hogy mik a Microsoft 365 Vállalati verzió beállítása.</span><span class="sxs-lookup"><span data-stu-id="c94b4-104">Watch this video for an overview of Microsoft 365 Business setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

<span data-ttu-id="c94b4-105">Ha hasznosnak találta ezt a videót, tekintse meg a [teljes tanfolyamok kisvállalatoknak és Microsoft 365-újoncoknak](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) című témakört.</span><span class="sxs-lookup"><span data-stu-id="c94b4-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="c94b4-106">Tartomány, felhasználók hozzáadása és házirendek beállítása</span><span class="sxs-lookup"><span data-stu-id="c94b4-106">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="c94b4-107">[![A megjelenő címke figyelmeztet a felügyeleti központ változásaira, további részleteket itt talál: aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="c94b4-107">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="c94b4-108">A Microsoft 365 Business megvásárlásakor lehetősége van arra, hogy a saját tartományát használja, vagy a [regisztráció](sign-up.md)során vásároljon egyet.</span><span class="sxs-lookup"><span data-stu-id="c94b4-108">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="c94b4-109">Ha regisztrált, új tartományt vásárolt, a tartomány teljesen be van állítva, és áthelyezheti a [Felhasználók hozzáadása és a licencek hozzárendelése](#add-users-and-assign-licenses)elemre.</span><span class="sxs-lookup"><span data-stu-id="c94b4-109">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="c94b4-110">A tartomány hozzáadása a bejelentkezés személyre szabásához</span><span class="sxs-lookup"><span data-stu-id="c94b4-110">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="c94b4-111">Jelentkezzen be a [Microsoft 365 Felügyeleti központba](https://admin.microsoft.com) a globális rendszergazdai hitelesítő adatok használatával.</span><span class="sxs-lookup"><span data-stu-id="c94b4-111">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="c94b4-112">A varázsló elindításához válassza az **Ugrás a beállításhoz** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c94b4-112">Choose **Go to setup** to start the wizard.</span></span>

    ![Válassza az Ugrás a beállításhoz lehetőséget.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="c94b4-114">Az **Office-alkalmazások telepítése** lapon igény szerint telepítheti az alkalmazásokat a saját számítógépére.</span><span class="sxs-lookup"><span data-stu-id="c94b4-114">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="c94b4-115">A **Tartomány hozzáadása** lépésben adja meg a használni kívánt tartománynevet (például contoso.com).</span><span class="sxs-lookup"><span data-stu-id="c94b4-115">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="c94b4-116">Ha a regisztráció során vásárolt tartományt, itt nem jelenik meg a **Tartomány hozzáadása** lépés.</span><span class="sxs-lookup"><span data-stu-id="c94b4-116">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="c94b4-117">Nyissa meg inkább a [Felhasználók hozzáadása](#add-users-and-assign-licenses) lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c94b4-117">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![Képernyőkép a Bejelentkezési oldal személyre szabása lapról.](../media/adddomain.png)

    
4. <span data-ttu-id="c94b4-119">A varázsló lépéseit [követve dns-rekordokat hozhat létre bármely Olyan OFFICE 365-ös DNS-szolgáltatónál,](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) amely ellenőrzi, hogy Ön a tartomány tulajdonosa.Follow the steps in the wizard to Create DNS records at any DNS hosting provider for Office 365 that verifies you own the domain.</span><span class="sxs-lookup"><span data-stu-id="c94b4-119">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="c94b4-120">Ha ismeri a tartományi állomást, olvassa el a [gazdagép specifikus utasításait.](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)</span><span class="sxs-lookup"><span data-stu-id="c94b4-120">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="c94b4-121">Ha a tárhelyszolgáltató godaddy vagy más, [tartományi kapcsolattal](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)rendelkező gazdagép, a folyamat egyszerű, és a rendszer automatikusan megkéri, hogy jelentkezzen be, és hagyja, hogy a Microsoft hitelesítse magát az Ön nevében.</span><span class="sxs-lookup"><span data-stu-id="c94b4-121">If your hosting provider is GoDaddy or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![A GoDaddy Access megerősítése lapon válassza az Engedélyezés lehetőséget.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="c94b4-123">Felhasználók felvétele és licencek hozzárendelése</span><span class="sxs-lookup"><span data-stu-id="c94b4-123">Add users and assign licenses</span></span>

<span data-ttu-id="c94b4-124">A varázslóban felhasználókat is felvehet, de később is [felvehet felhasználókat](add-users-m365b.md) a felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="c94b4-124">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="c94b4-125">Ha helyi tartományvezérlővel is rendelkezik, hozzáadhat felhasználókat az [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)szolgáltatással.</span><span class="sxs-lookup"><span data-stu-id="c94b4-125">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="c94b4-126">Felhasználók hozzáadása a varázslóban</span><span class="sxs-lookup"><span data-stu-id="c94b4-126">Add users in the wizard</span></span>

<span data-ttu-id="c94b4-127">A varázslóban hozzáadott felhasználók automatikusan Microsoft 365 Vállalati licencet kapnak.</span><span class="sxs-lookup"><span data-stu-id="c94b4-127">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![Képernyőkép az Új felhasználók hozzáadása lapról a varázslóban](../media/addnewuserspage.png)

1. <span data-ttu-id="c94b4-129">Ha a Microsoft 365 Business-előfizetése meglévő felhasználókkal rendelkezik (például ha az Azure AD Connectet használta), most lehetősége van licencek hozzárendelésére.</span><span class="sxs-lookup"><span data-stu-id="c94b4-129">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="c94b4-130">Nyugodtan felvehet licenceket hozzájuk is.</span><span class="sxs-lookup"><span data-stu-id="c94b4-130">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="c94b4-131">Miután felvette a felhasználókat, lehetőséget kap arra is, hogy megossza a hitelesítő adatokat a hozzáadott új felhasználókkal.</span><span class="sxs-lookup"><span data-stu-id="c94b4-131">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="c94b4-132">Ezeket kinyomtathatja, elküldheti e-mailben, vagy pedig letöltheti.</span><span class="sxs-lookup"><span data-stu-id="c94b4-132">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="c94b4-133">Tartomány csatlakoztatása</span><span class="sxs-lookup"><span data-stu-id="c94b4-133">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="c94b4-134">Ha az .onmicrosoft tartomány t használja, vagy az Azure AD Connectet használta a felhasználók beállításához, akkor ez a lépés nem jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="c94b4-134">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="c94b4-135">A szolgáltatások beállításához frissítenie kell bizonyos rekordokat a DNS-szolgáltatónál vagy a tartományregisztrálónál.</span><span class="sxs-lookup"><span data-stu-id="c94b4-135">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="c94b4-136">A beállítási varázsló általában felismeri a regisztrálóját, és részletes útmutatást jelenít meg arról, hogy miként frissítheti a névkiszolgálói rekordokat a regisztráló webhelyén.</span><span class="sxs-lookup"><span data-stu-id="c94b4-136">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="c94b4-137">Ha nem, módosítsa a [névkiszolgálókat, hogy az Office 365-öt bármely tartományregisztrálóval](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2)beállítsák.</span><span class="sxs-lookup"><span data-stu-id="c94b4-137">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="c94b4-138">Ha meglévő DNS-rekordokkal rendelkezik, például egy meglévő webhely, de a DNS-szolgáltató engedélyezve van a [tartománycsatlakozáshoz,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)válassza **a Rekordok hozzáadása számomra**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c94b4-138">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="c94b4-139">Az **Online szolgáltatások kiválasztása** lapon fogadja el az összes alapértelmezést, és válassza a **Tovább**gombot, és válassza a DNS-szolgáltató lapján az **Engedélyezés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c94b4-139">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="c94b4-140">Ha már rendelkezik DNS-rekordokkal más DNS-állomásokkal (nincs engedélyezve a tartománycsatlakozáshoz), akkor a meglévő szolgáltatások kapcsolatának biztosítása érdekében kezelje a saját DNS-rekordjait.</span><span class="sxs-lookup"><span data-stu-id="c94b4-140">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="c94b4-141">További információ a [tartomány alapjaiban.](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics)</span><span class="sxs-lookup"><span data-stu-id="c94b4-141">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Rekordok aktiválása lap.](../media/activaterecords.png)

2. <span data-ttu-id="c94b4-143">Kövesse a varázsló lépéseit, és az e-mailek és egyéb szolgáltatások beállítva lesznek.</span><span class="sxs-lookup"><span data-stu-id="c94b4-143">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="c94b4-144">A szervezet védelme</span><span class="sxs-lookup"><span data-stu-id="c94b4-144">Protect your organization</span></span> 

<span data-ttu-id="c94b4-145">A varázslóban beállított házirendek automatikusan érvénybe lépnek a *Minden felhasználó*nevű [biztonsági csoportra.](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups)</span><span class="sxs-lookup"><span data-stu-id="c94b4-145">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="c94b4-146">További csoportokat is létrehozhat, amelyekhez házirendeket rendelhet a felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="c94b4-146">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="c94b4-147">A **Fokozott védelem a fejlett kiberfenyegetésekkel kapcsolatban**ajánlott elfogadni az alapértelmezett beállításokat, hogy az [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) beszana fájlokat és hivatkozásokat az Office-alkalmazásokban.</span><span class="sxs-lookup"><span data-stu-id="c94b4-147">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) scan files and links in Office apps.</span></span>

    ![Képernyőkép: Védelem növelése lap.](../media/increasetreatprotection.png)


2. <span data-ttu-id="c94b4-149">A **Bizalmas adatok szivárgásának megakadályozása** lapon fogadja el az Office 365 adatveszteség-megelőzési (DLP) beállításának alapértelmezett beállításait a bizalmas adatok nyomon követéséhez az Office-alkalmazásokban, és megakadályozza ezek véletlen megosztását a szervezeten kívül.</span><span class="sxs-lookup"><span data-stu-id="c94b4-149">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="c94b4-150">Az **Adatok védelme mobiloffice-ban** lapon hagyja bekapcsolva a mobilalkalmazás-felügyeletet, bontsa ki a beállításokat és tekintse át őket, majd válassza a **Mobilalkalmazás-kezelési szabályzat létrehozása**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c94b4-150">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Képernyőkép: Adatok védelme a mobiloffice-ban lapon.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="c94b4-152">Windows 10-es számítógépek biztonságossá tétele</span><span class="sxs-lookup"><span data-stu-id="c94b4-152">Secure Windows 10 PCs</span></span>

<span data-ttu-id="c94b4-153">A bal oldali navigációs sávon válassza a **Telepítés** lehetőséget, majd a **Sin-in és a Biztonság**csoportban válassza a Windows **10-es számítógépek biztonsága**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c94b4-153">On the left nav, select **Setup** and then, under **Sing-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="c94b4-154">A kezdéshez válassza a **Nézet** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c94b4-154">Choose **View** to get started.</span></span> <span data-ttu-id="c94b4-155">A teljes útmutatóban a [Windows 10-es számítógépek biztonsága](secure-win-10-pcs.md) látható.</span><span class="sxs-lookup"><span data-stu-id="c94b4-155">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="c94b4-156">Az Office 365 ügyfélalkalmazásának telepítése</span><span class="sxs-lookup"><span data-stu-id="c94b4-156">Deploy Office 365 client apps</span></span>

<span data-ttu-id="c94b4-157">Ha úgy dönt, hogy a telepítés során automatikusan telepíti az Office-alkalmazásokat, az alkalmazások a Windows 10-es eszközökre települnek, miután a felhasználók bejelentkeztek az Azure AD-be a munkahelyi hitelesítő adataik használatával.</span><span class="sxs-lookup"><span data-stu-id="c94b4-157">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="c94b4-158">Az Office mobiliOS vagy Android rendszerű eszközökre való telepítéséhez olvassa el [a Mobileszközök beállítása a Microsoft 365 Vállalati verzió felhasználói számára](set-up-mobile-devices.md)című témakört.</span><span class="sxs-lookup"><span data-stu-id="c94b4-158">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="c94b4-159">Az Office-t külön is telepítheti.</span><span class="sxs-lookup"><span data-stu-id="c94b4-159">You can also install Office individually.</span></span> <span data-ttu-id="c94b4-160">Az [Office telepítése PC-re vagy Mac gépre](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) című témakörben talál további információt.</span><span class="sxs-lookup"><span data-stu-id="c94b4-160">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="c94b4-161">Lásd még</span><span class="sxs-lookup"><span data-stu-id="c94b4-161">See also</span></span>

[<span data-ttu-id="c94b4-162">Microsoft 365 Vállalati verziós oktatóvideók</span><span class="sxs-lookup"><span data-stu-id="c94b4-162">Microsoft 365 Business training videos</span></span>](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)

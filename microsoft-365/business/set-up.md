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
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Útmutató a Microsoft 365 Business beállításához.
ms.openlocfilehash: cd59570cbcb9b027780e160117b44be88770d6b9
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575548"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="02df4-103">A Microsoft 365 Business beállítása a telepítővarázslóban</span><span class="sxs-lookup"><span data-stu-id="02df4-103">Set up Microsoft 365 Business in the setup wizard</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="02df4-104">A tartomány, a felhasználók és a házirendek beállítása</span><span class="sxs-lookup"><span data-stu-id="02df4-104">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="02df4-105">[![Label, hogy tudd, az admin központ változik, és találsz további részleteket a aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="02df4-105">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="02df4-106">Amikor vagy megvásárol Mikroszkóp 365 teendő, Önnek van a választás-ból használ egy birtok Ön saját, vagy buying egy közben a [jel-megjelöl](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="02df4-106">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="02df4-107">Ha a feliratkozáskor új tartományt vásárolt, akkor a tartománya be van állítva, és segítségével [felhasználókat vehet fel és licenceket rendelhet](#add-users-and-assign-licenses)hozzá.</span><span class="sxs-lookup"><span data-stu-id="02df4-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="02df4-108">Saját tartomány felvétele a bejelentkezés személyre szabásához</span><span class="sxs-lookup"><span data-stu-id="02df4-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="02df4-109">Jelentkezzen be a [Microsoft 365 felügyeleti központba](https://admin.microsoft.com) a globális rendszergazdai hitelesítő adatok használatával.</span><span class="sxs-lookup"><span data-stu-id="02df4-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="02df4-110">Válassza a **tartomány hozzáadása** vagy a **felhasználók hozzáadása** a varázsló elindításához.</span><span class="sxs-lookup"><span data-stu-id="02df4-110">Choose **Add a domain** or **Add users** to start the wizard.</span></span>
    > [!IMPORTANT]
    > <span data-ttu-id="02df4-111">Ha a regisztráció során tartományt vásárolt, akkor itt nem jelenik meg **a domainlépés hozzáadása** .</span><span class="sxs-lookup"><span data-stu-id="02df4-111">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="02df4-112">Tovább a [felhasználók hozzáadásához](#add-users-and-assign-licenses) helyette.</span><span class="sxs-lookup"><span data-stu-id="02df4-112">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![Válassza az Ugrás a telepítéshez beállítást.](media/gotosetupinadmincenter.png)
    
3. <span data-ttu-id="02df4-114">A varázslóban adja meg a használni kívánt tartománynevet (például contoso.com).</span><span class="sxs-lookup"><span data-stu-id="02df4-114">In the wizard, enter the domain name you want to use (like contoso.com).</span></span>


    ![Ernyőz-ból megszemélyesít-a jel--ban oldal.](media/personalizesignin.png)

    
4. <span data-ttu-id="02df4-116">A varázsló lépéseit követve [hozzon létre DNS-rekordokat az Office 365 olyan DNS-](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) szolgáltatójánál, amely igazolja, hogy Ön a tartomány tulajdonosa.</span><span class="sxs-lookup"><span data-stu-id="02df4-116">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="02df4-117">Ha ismeri a domainnevét, akkor tekintse meg a [gazdagép utasításait](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)is.</span><span class="sxs-lookup"><span data-stu-id="02df4-117">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="02df4-118">Ha-a ellenséges eltartó van GoDaddy, vagy másik házigazda lehetővé tett-val [birtok összeköt](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), a folyamat van könnyű és lesz lenni keresztül keresztül-hoz jel-ban és enged Mikroszkóp hitelesít-ra-a nevében:</span><span class="sxs-lookup"><span data-stu-id="02df4-118">If your hosting provider is GoDaddy, or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you will be automatically asked to sign in and let Microsoft authenticate on your behalf:</span></span>

    ![-Ra GoDaddy igazol belépés oldal, kiválaszt engedélyez.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="02df4-120">Felhasználók felvétele és licencek hozzárendelése</span><span class="sxs-lookup"><span data-stu-id="02df4-120">Add users and assign licenses</span></span>

<span data-ttu-id="02df4-121">Felhasználókat felvehet a varázslóba, de később az admin központban is [hozzáadhat felhasználókat](add-users-m365b.md) .</span><span class="sxs-lookup"><span data-stu-id="02df4-121">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="02df4-122">Ezenkívül, ha van helyi tartományvezérlője, hozzáadhat felhasználókat a [Azure ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)segítségével.</span><span class="sxs-lookup"><span data-stu-id="02df4-122">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="02df4-123">Felhasználók hozzáadása a varázslóhoz</span><span class="sxs-lookup"><span data-stu-id="02df4-123">Add users in the wizard</span></span>

<span data-ttu-id="02df4-124">A varázslóban hozzáadott felhasználók automatikusan Microsoft 365 üzleti licencet kapnak.</span><span class="sxs-lookup"><span data-stu-id="02df4-124">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![Az új felhasználók hozzáadása lap képernyőképe a varázslóban](media/addnewuserspage.png)

1. <span data-ttu-id="02df4-126">Ha a Microsoft 365 üzleti előfizetés már meglévő felhasználókkal rendelkezik (például, ha a Azure AD Connect szolgáltatást használta), akkor most lehetősége van licencek kiosztésére.</span><span class="sxs-lookup"><span data-stu-id="02df4-126">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you get an option to assign licenses to them now.</span></span> <span data-ttu-id="02df4-127">Nyugodtan felvehet licenceket hozzájuk is.</span><span class="sxs-lookup"><span data-stu-id="02df4-127">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="02df4-128">A felhasználók hozzáadása után lehetősége van a hitelesítő adatok megosztására az új felhasználóknál is.</span><span class="sxs-lookup"><span data-stu-id="02df4-128">After you have added the users, you will also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="02df4-129">Ezeket kinyomtathatja, elküldheti e-mailben, vagy pedig letöltheti.</span><span class="sxs-lookup"><span data-stu-id="02df4-129">You can choose to print them out, email them, or download them.</span></span>

3. <span data-ttu-id="02df4-130">A csapatok létrehozása a szervezet számára csoport választhatja a csapatok hozzáadását és a felhasználók hozzáadását.</span><span class="sxs-lookup"><span data-stu-id="02df4-130">On the Create Teams for your organization, you can choose to add Teams and add users to them.</span></span> <span data-ttu-id="02df4-131">Ezt később is megteheti.</span><span class="sxs-lookup"><span data-stu-id="02df4-131">You can also do this later.</span></span> <span data-ttu-id="02df4-132">További információt a [vállalati szintű csapat létrehozása](https://support.office.com/article/037bb27a-bcc9-48fe-8d72-44d9482420a3)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="02df4-132">For more information, see [create a company-wide Team](https://support.office.com/article/037bb27a-bcc9-48fe-8d72-44d9482420a3).</span></span>

4. <span data-ttu-id="02df4-133">Hagyja ki az e-mail-üzenetek áttelepítését, és kattintson a **Tovább** gombra az **E-mail-üzenetek áttelepítése** lapon.</span><span class="sxs-lookup"><span data-stu-id="02df4-133">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 

    <span data-ttu-id="02df4-134">Ha egy másik e-mail szolgáltatótól költözik, és később át kívánja másolni az adatokat, akkor [áttelepítheti az e-maileket és a névjegyeket az Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span><span class="sxs-lookup"><span data-stu-id="02df4-134">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>


### <a name="connect-your-domain"></a><span data-ttu-id="02df4-135">Tartomány csatlakoztatása</span><span class="sxs-lookup"><span data-stu-id="02df4-135">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="02df4-136">Ha az. onmicrosoft tartomány használata mellett döntött, vagy a felhasználók beállításához a Azure AD Connect szolgáltatást használja, akkor ezt a lépést nem fogja látni.</span><span class="sxs-lookup"><span data-stu-id="02df4-136">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="02df4-137">A szolgáltatások beállításához frissítenie kell bizonyos rekordokat a DNS-szolgáltatónál vagy a tartományregisztrálónál.</span><span class="sxs-lookup"><span data-stu-id="02df4-137">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="02df4-138">A beállítási varázsló általában felismeri a regisztrálóját, és részletes útmutatást jelenít meg arról, hogy miként frissítheti a névkiszolgálói rekordokat a regisztráló webhelyén.</span><span class="sxs-lookup"><span data-stu-id="02df4-138">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="02df4-139">Ha nem, [módosítsa a névszervereket az Office 365 beállításához bármely tartományregisztrálóval](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="02df4-139">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="02df4-140">Ha vannak meglévő DNS-rekordjai, például egy meglévő webhely, de a DNS-állomás a tartományhoz történő [kapcsolódáshoz](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)engedélyezve van, válassza **a saját rekord hozzáadása**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="02df4-140">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="02df4-141">Az **online szolgáltatások kiválasztása** lapon fogadja el az összes alapértelmezett beállításokat, majd kattintson a **Tovább gombra**, és válassza az engedélyezés a DNS-állomás oldalán **engedélyt** .</span><span class="sxs-lookup"><span data-stu-id="02df4-141">On the **Choose your online services** page, accept all the defaults, and choose **Next**,and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="02df4-142">Ha van meglévő DNS-rekordja más DNS-állomásokkal (nincs engedélyezve a tartomány csatlakoztatásához), saját DNS-rekordokat kell kezelnie annak érdekében, hogy a meglévő szolgáltatások ne maradjanak kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="02df4-142">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you will want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="02df4-143">További információ a [tartomány alapjai](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) című témakörben található.</span><span class="sxs-lookup"><span data-stu-id="02df4-143">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Összeköt-a birtok oldal-val én ' kezel az én-m saját DNS hanglemezek.](media/connectyourdomainpage.png)

2. <span data-ttu-id="02df4-145">Kövesse a varázsló lépéseit, és az e-mail és egyéb szolgáltatások lesznek beállítva az Ön számára.</span><span class="sxs-lookup"><span data-stu-id="02df4-145">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-data-and-devices"></a><span data-ttu-id="02df4-146">Védjük az adatokat és az eszközöket</span><span class="sxs-lookup"><span data-stu-id="02df4-146">Protect data and devices</span></span> 

<span data-ttu-id="02df4-147">A varázslóban beállított házirendek automatikusan alkalmazásra kerülnek a *minden felhasználó*nevű [biztonsági csoportra](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) .</span><span class="sxs-lookup"><span data-stu-id="02df4-147">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="02df4-148">További csoportokat is létrehozhat, ha házirendeket rendel az admin Centerhez.</span><span class="sxs-lookup"><span data-stu-id="02df4-148">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="02df4-149">-Ra a **megvéd-a dolgozik fájlokat-ra mozgatható berendezés** a választás **megvéd dolgozik fájlokat mikor berendezés van elveszett vagy lopott** van válogatott mellett hiba.</span><span class="sxs-lookup"><span data-stu-id="02df4-149">On the **Protect your work files on mobile devices** the option **Protect work files when devices are lost or stolen** is selected by default.</span></span> <span data-ttu-id="02df4-150">Lehetősége van bekapcsolni annak **kezelését, hogy a felhasználók hogyan férhessék hozzá az Office-fájlokat a mobileszközökön**, és ez ajánlott.</span><span class="sxs-lookup"><span data-stu-id="02df4-150">You have an option to turn on **Manage how users access Office files on mobile devices**, and this is recommended.</span></span>

    ![Ernyőz-ból megvéd dolgozik fájlokat-ra mozgatható berendezés oldal.](media/protectworkfilesondevices.png)

     - <span data-ttu-id="02df4-152">Az [alapértelmezett értékek](protect-work-files-on-lost-or-stolen-device.md)megjelenítéséhez bontsa ki a **fájlvédelem a munkahelyi fájlokat, ha az eszköz elvész vagy ellopják** :</span><span class="sxs-lookup"><span data-stu-id="02df4-152">Expand **Protect work files when devices are lost or stolen** to display the [default values](protect-work-files-on-lost-or-stolen-device.md):</span></span>

        ![Képernyőkép az alapértelmezett értékekről az elveszett eszközökön lévő fájlok védelméhez.](media/protectworkfilesondevicesdefault.png)

    - <span data-ttu-id="02df4-154">Válassza a **kezelés, hogy a felhasználók hogyan férhetnek hozzá az Office-fájlokhoz a mobileszközökön** , és bontsa ki azt az [alapértelmezett értékek](manage-user-access-on-mobile-devices.md)megjelenítéséhez.</span><span class="sxs-lookup"><span data-stu-id="02df4-154">Select **Manage how users access Office files on mobile devices** and expand it to display the [default values](manage-user-access-on-mobile-devices.md).</span></span> <span data-ttu-id="02df4-155">Javasoljuk, hogy a telepítés során fogadja el az alapértelmezett értékeket, hogy az összes felhasználóra érvényes Android, iOS és Windows 10 alkalmazások házirendjeit hozza létre.</span><span class="sxs-lookup"><span data-stu-id="02df4-155">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="02df4-156">A telepítés után további házirendeket is létrehozhat majd.</span><span class="sxs-lookup"><span data-stu-id="02df4-156">You can create more policies after setup completes.</span></span>

        ![A mobil Office-fájlokhoz tartozó védelmi beállítások képernyőképe.](media/useraccessonmobile.png)

2. <span data-ttu-id="02df4-158">Az adatok és eszközök védelmének utolsó lépése lehetővé teszi a házirendek beállítására a Windows 10 eszközök biztonságossá tétele érdekében.</span><span class="sxs-lookup"><span data-stu-id="02df4-158">The last step on protect data and devices allows you to set up policies to secure Windows 10 devices.</span></span> <span data-ttu-id="02df4-159">Ezeket a beállításokat a rendszer automatikusan alkalmazza, amikor a felhasználó Windows 10-e csatlakozik a szervezethez.</span><span class="sxs-lookup"><span data-stu-id="02df4-159">These settings are applied automatically when a user's Windows 10 connects to your organization.</span></span> <span data-ttu-id="02df4-160">A **biztonságos Windows 10 eszközöket** kibonthatja az [alapértelmezett értékek](secure-windows-10-devices.md)megtekintéséhez és módosításához.</span><span class="sxs-lookup"><span data-stu-id="02df4-160">You can expand **Secure Windows 10 devices** to see and modify the [default values](secure-windows-10-devices.md).</span></span>
3. <span data-ttu-id="02df4-161">Azt is választhatja, hogy [automatikusan telepíti az Office](install-office-on-windows-10-during-setup.md) -t a Windows 10 eszközén.</span><span class="sxs-lookup"><span data-stu-id="02df4-161">You can also choose to [automatically install Office](install-office-on-windows-10-during-setup.md) on Windows 10 devices.</span></span>

    ![Képernyőkép beállítása a Windows 10 eszköz konfigurációs lapjáról.](media/setwin10config.png)


## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="02df4-163">Az Office 365 ügyfélalkalmazások telepítése</span><span class="sxs-lookup"><span data-stu-id="02df4-163">Deploy Office 365 client apps</span></span>

<span data-ttu-id="02df4-164">Ha úgy dönt, hogy a telepítés során automatikusan telepíti az Office-alkalmazásokat, az alkalmazások a Windows 10 eszközén telepíthetnek, amint a felhasználók az azúrkék HIRDETÉSRE be lettek jelentkezve a saját munkájukat hitelesítő adataikkal.</span><span class="sxs-lookup"><span data-stu-id="02df4-164">If you chose to automatically install Office apps in during the set up, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices with their work credentials.</span></span>
<span data-ttu-id="02df4-165">Az Office mobil iOS vagy Android eszközökre történő telepítéséhez tekintse meg [a mobileszközök beállítása a Microsoft 365 üzleti felhasználók számára](set-up-mobile-devices.md)című témakört.</span><span class="sxs-lookup"><span data-stu-id="02df4-165">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="02df4-166">Az Office programot egyenként is telepíthetjük.</span><span class="sxs-lookup"><span data-stu-id="02df4-166">You can also install Office individually.</span></span> <span data-ttu-id="02df4-167">Útmutatás: az [Office telepítése PC vagy Mac számítógépre](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) .</span><span class="sxs-lookup"><span data-stu-id="02df4-167">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

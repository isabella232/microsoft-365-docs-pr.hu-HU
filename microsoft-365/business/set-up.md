---
title: A Microsoft 365 Business beállítása
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Útmutató a Microsoft 365 üzleti beállítása.
ms.openlocfilehash: f3a9ad62f5ec8779296e800b9ecc8d6181d7aff7
ms.sourcegitcommit: f420a5cdedf3ec2babc6d8ad7e7c79da0b08e115
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33966978"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="ed696-103">A telepítővarázsló a Microsoft 365 üzleti beállítása</span><span class="sxs-lookup"><span data-stu-id="ed696-103">Set up Microsoft 365 Business in the setup wizard</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="ed696-104">Adja hozzá a tartományi felhasználók és a házirendek beállítása</span><span class="sxs-lookup"><span data-stu-id="ed696-104">Add your domain, users, and set up policies</span></span>

![Mutató transzparens https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

<span data-ttu-id="ed696-106">Microsoft 365 üzleti beszerzése esetén a saját tartomány használata, vagy a vásárlás során lehetőség van az [Internet-előfizetési](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="ed696-106">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="ed696-107">Ha új tartomány létrehozása során vásárolt, a tartomány összes fel, és Ugrás [felhasználók hozzáadása és a licencek hozzárendelése](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="ed696-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="ed696-108">Az egyéni bejelentkezési tartomány hozzáadása</span><span class="sxs-lookup"><span data-stu-id="ed696-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="ed696-109">Jelentkezzen be a [Microsoft 365 felügyeleti központ](https://admin.microsoft.com) a globális rendszergazdai hitelesítő adatok használatával.</span><span class="sxs-lookup"><span data-stu-id="ed696-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="ed696-110">Kattintson a **Hozzáadás a tartományhoz** vagy a **felhasználók hozzáadása** varázsló elindításához.</span><span class="sxs-lookup"><span data-stu-id="ed696-110">Choose **Add a domain** or **Add users** to start the wizard.</span></span>
    > [!IMPORTANT]
    > <span data-ttu-id="ed696-111">Ha a regisztráció során vásárolt egy tartomány, a program nem lásd: **tartomány hozzáadása** lépés itt.</span><span class="sxs-lookup"><span data-stu-id="ed696-111">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="ed696-112">Ugrás a [felhasználók hozzáadása](#add-users-and-assign-licenses) helyett.</span><span class="sxs-lookup"><span data-stu-id="ed696-112">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![Jelölje be a tartomány hozzáadása.](media/addadomainadmincenter.png)
    
3. <span data-ttu-id="ed696-114">A varázslóban adja meg a tartomány nevét (például contoso.com) használni kívánt.</span><span class="sxs-lookup"><span data-stu-id="ed696-114">In the wizard, enter the domain name you want to use (like contoso.com).</span></span>


    ![Képernyőkép a személyre szabás Bejelentkezés lapon.](media/personalizesignin.png)

    
4. <span data-ttu-id="ed696-116">Ellenőrzi a saját tartomány [létrehozása DNS-rekordokat az Office 365 bármely DNS-szolgáltatójánál,](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) kövesse a varázsló utasításait.</span><span class="sxs-lookup"><span data-stu-id="ed696-116">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="ed696-117">Ha ismeri a tartományi állomás, lásd még: [állomás konkrét utasításokat](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="ed696-117">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="ed696-118">Ha a videotár-szolgáltató GoDaddy, a folyamat egyszerű és program automatikusan kéri, jelentkezzen be, és hagyja, hogy a nevünkben hitelesíti a Microsoft:</span><span class="sxs-lookup"><span data-stu-id="ed696-118">If your hosting provider is GoDaddy, the process is easy and you will be automatically asked to sign in and let Microsoft authenticate on your behalf:</span></span>

    ![GoDaddy megerősítése adatelérési lapon jelölje be az engedélyezés.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="ed696-120">Felhasználók felvétele és licencek hozzárendelése</span><span class="sxs-lookup"><span data-stu-id="ed696-120">Add users and assign licenses</span></span>

<span data-ttu-id="ed696-121">A varázslóban hozzáadhat felhasználókat, de is [újabb felhasználók hozzáadása](add-users-m365b.md) a felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="ed696-121">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="ed696-122">Ezenkívül ha a helyi tartományvezérlő, hozzáadhat [Azure AD csatlakozás](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)rendelkező felhasználók.</span><span class="sxs-lookup"><span data-stu-id="ed696-122">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="ed696-123">Felhasználók hozzáadása varázsló</span><span class="sxs-lookup"><span data-stu-id="ed696-123">Add users in the wizard</span></span>

<span data-ttu-id="ed696-124">A varázsló felvett felhasználóknak Microsoft 365 üzleti licenc beszerzése automatikusan.</span><span class="sxs-lookup"><span data-stu-id="ed696-124">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![Képernyőkép a Hozzáadás új felhasználó lapon a varázsló](media/addnewuserspage.png)

1. <span data-ttu-id="ed696-126">Ha a Microsoft 365 üzleti előfizetés (például, ha Azure AD csatlakozás) a meglévő felhasználók, licencek hozzárendelése őket most lehetőséget kap.</span><span class="sxs-lookup"><span data-stu-id="ed696-126">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you get an option to assign licenses to them now.</span></span> <span data-ttu-id="ed696-127">Nyugodtan felvehet licenceket hozzájuk is.</span><span class="sxs-lookup"><span data-stu-id="ed696-127">Go ahead and add licenses to them as well.</span></span>

3. <span data-ttu-id="ed696-128">Miután hozzáadta a felhasználók, a hozzáadott új felhasználók hitelesítő adatok megosztása lehetőséget is fog kapni.</span><span class="sxs-lookup"><span data-stu-id="ed696-128">After you have added the users, you will also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="ed696-129">Ezeket kinyomtathatja, elküldheti e-mailben, vagy pedig letöltheti.</span><span class="sxs-lookup"><span data-stu-id="ed696-129">You can choose to print them out, email them, or download them.</span></span>

4. <span data-ttu-id="ed696-130">Hagyja ki az e-mail-üzenetek áttelepítését, és kattintson a **Tovább** gombra az **E-mail-üzenetek áttelepítése** lapon.</span><span class="sxs-lookup"><span data-stu-id="ed696-130">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 

    <span data-ttu-id="ed696-131">Ha áthelyezni egy másik e-mail szolgáltatójától, és később az adatok másolásához, akkor [e-mail áttelepítése és az Office 365 ügyfeleket](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span><span class="sxs-lookup"><span data-stu-id="ed696-131">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>


### <a name="connect-your-domain"></a><span data-ttu-id="ed696-132">Tartomány csatlakoztatása</span><span class="sxs-lookup"><span data-stu-id="ed696-132">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="ed696-133">Ha a .onmicrosoft tartomány használata mellett, vagy Azure AD csatlakozás segítségével a felhasználók beállítása, ez a lépés nem jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="ed696-133">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="ed696-134">A szolgáltatások beállításához frissítenie kell bizonyos rekordokat a DNS-szolgáltatónál vagy a tartományregisztrálónál.</span><span class="sxs-lookup"><span data-stu-id="ed696-134">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="ed696-135">A beállítási varázsló általában felismeri a regisztrálóját, és részletes útmutatást jelenít meg arról, hogy miként frissítheti a névkiszolgálói rekordokat a regisztráló webhelyén.</span><span class="sxs-lookup"><span data-stu-id="ed696-135">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="ed696-136">Ha nem, [Módosítás nameservers beállítása az Office 365 bármely tartomány tartományneveket regisztráló szervezetnél](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="ed696-136">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="ed696-137">Ha meglévő DNS-rekordok, például egy létező webhelyen, érdemes kapcsolattartásra a meglévő szolgáltatások biztosításához a saját DNS-rekordok kezeléséhez.</span><span class="sxs-lookup"><span data-stu-id="ed696-137">If you have existing DNS records, for example an existing web site, you will want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="ed696-138">További információ a [tartomány alapjai](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="ed696-138">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Csatlakozás a tartomány lap i. fogja kezelni a saját DNS-rekordokat.](media/connectyourdomainpage.png)

2. <span data-ttu-id="ed696-140">Kövesse a varázsló utasításait, és e-mail és egyéb szolgáltatások hoznak létre meg.</span><span class="sxs-lookup"><span data-stu-id="ed696-140">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="set-up-security-policies-and-device-configurations"></a><span data-ttu-id="ed696-141">Állítsa be a biztonsági házirendek és az eszközök konfigurációja</span><span class="sxs-lookup"><span data-stu-id="ed696-141">Set up security policies and device configurations</span></span> 

<span data-ttu-id="ed696-142">A házirendek beállítása varázsló automatikusan alkalmazni *Minden felhasználó*létrehoz egy [biztonsági csoportot](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) .</span><span class="sxs-lookup"><span data-stu-id="ed696-142">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="ed696-143">A felügyeleti központ házirendek hozzárendelése további csoportokat is létrehozhat.</span><span class="sxs-lookup"><span data-stu-id="ed696-143">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="ed696-144">A **mobil eszközökön a munka fájlok védelme** a beállítás **védelme Munkafájlok, ha elveszett vagy ellopott eszköz** alapértelmezés szerint van jelölve.</span><span class="sxs-lookup"><span data-stu-id="ed696-144">On the **Protect your work files on mobile devices** the option **Protect work files when devices are lost or stolen** is selected by default.</span></span> <span data-ttu-id="ed696-145">Akkor **kezelheti, hogy a felhasználók miként férhetnek hozzá a mobil eszközökön tárolt Office fájlokhoz**bekapcsolása lehetőséget, és ez ajánlott.</span><span class="sxs-lookup"><span data-stu-id="ed696-145">You have an option to turn on **Manage how users access Office files on mobile devices**, and this is recommended.</span></span>

    ![Munkafájlok védelme Képernyőkép a mobileszközök lapon.](media/protectworkfilesondevices.png)

     - <span data-ttu-id="ed696-147">Bontsa ki az [alapértelmezett értékek](protect-work-files-on-lost-or-stolen-device.md)megjelenítése **védelme Munkafájlok, ha elveszett vagy ellopott eszközök** :</span><span class="sxs-lookup"><span data-stu-id="ed696-147">Expand **Protect work files when devices are lost or stolen** to display the [default values](protect-work-files-on-lost-or-stolen-device.md):</span></span>

        ![Képernyőkép a elveszett eszköz fájlok védelme alapértelmezett értékeit.](media/protectworkfilesondevicesdefault.png)

    - <span data-ttu-id="ed696-149">Jelölje ki a **kezelni, hogy a felhasználók miként férhetnek hozzá a mobil eszközökön található Office-fájlokat** , és bontsa ki az [alapértelmezett értékeinek](manage-user-access-on-mobile-devices.md)megjelenítése.</span><span class="sxs-lookup"><span data-stu-id="ed696-149">Select **Manage how users access Office files on mobile devices** and expand it to display the [default values](manage-user-access-on-mobile-devices.md).</span></span> <span data-ttu-id="ed696-150">Azt javasoljuk, hogy elfogadja az alapértelmezett értékeket, Android, iOS és a Windows 10 alkalmazás-házirendek létrehozásához a telepítés során, amelyek minden felhasználóra vonatkoznak.</span><span class="sxs-lookup"><span data-stu-id="ed696-150">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="ed696-151">A telepítés után további házirendeket is létrehozhat majd.</span><span class="sxs-lookup"><span data-stu-id="ed696-151">You can create more policies after setup completes.</span></span>

        ![Képernyőkép a védelmi beállításait a hordozható Office-fájlokat.](media/useraccessonmobile.png)

2. <span data-ttu-id="ed696-153">Az utolsó lépés az adatok védelmét és az eszköz lehetővé teszi a házirendek beállítása Windows 10 eszközök biztonságos.</span><span class="sxs-lookup"><span data-stu-id="ed696-153">The last step on protect data and devices allows you to set up policies to secure Windows 10 devices.</span></span> <span data-ttu-id="ed696-154">Ezek a beállítások automatikusan érvényesek, ha a felhasználó Windows 10 csatlakozik a szervezet.</span><span class="sxs-lookup"><span data-stu-id="ed696-154">These settings are applied automatically when a user's Windows 10 connects to your organization.</span></span> <span data-ttu-id="ed696-155">Kibonthatja a **biztonságos Windows 10 eszközök** és az [alapértelmezett értékek](secure-windows-10-devices.md)módosíthatók.</span><span class="sxs-lookup"><span data-stu-id="ed696-155">You can expand **Secure Windows 10 devices** to see and modify the [default values](secure-windows-10-devices.md).</span></span>
3. <span data-ttu-id="ed696-156">Választhatja azt is, [automatikus telepítése az Office](install-office-on-windows-10-during-setup.md) eszközök a Windows 10.</span><span class="sxs-lookup"><span data-stu-id="ed696-156">You can also choose to [automatically install Office](install-office-on-windows-10-during-setup.md) on Windows 10 devices.</span></span>

    ![Képernyőkép a Windows 10 eszköz konfigurációs lapon állítsa be.](media/setwin10config.png)



## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="ed696-158">Telepítse az Office 365 ügyfélalkalmazások</span><span class="sxs-lookup"><span data-stu-id="ed696-158">Deploy Office 365 client apps</span></span>

<span data-ttu-id="ed696-159">Ha azt választotta, hogy automatikusan telepíti az Office-alkalmazások a telepítéskor ki, az apps telepíti a Windows 10 eszközök után a felhasználó bejelentkezett az Azure AD a munka hitelesítő adatokkal a Windows eszközök.</span><span class="sxs-lookup"><span data-stu-id="ed696-159">If you chose to automatically install Office apps in during the set up, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices with their work credentials.</span></span>
<span data-ttu-id="ed696-160">Office telepítése mobil iOS vagy Android-eszköz, lásd: [állítsa be a mobil eszközök Microsoft 365 üzleti felhasználók számára](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="ed696-160">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="ed696-161">Office külön-külön is telepíthető.</span><span class="sxs-lookup"><span data-stu-id="ed696-161">You can also install Office individually.</span></span> <span data-ttu-id="ed696-162">Lásd: [PC vagy Mac Office telepítéséhez](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) további útmutatást.</span><span class="sxs-lookup"><span data-stu-id="ed696-162">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) for instructions.</span></span>

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
ms.openlocfilehash: e635b828609fc47cd8b92bb179a25bcc43cb0a1a
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660809"
---
# <a name="set-up-microsoft-365-business"></a><span data-ttu-id="19cef-103">A Microsoft 365 Business beállítása</span><span class="sxs-lookup"><span data-stu-id="19cef-103">Set up Microsoft 365 Business</span></span>

<span data-ttu-id="19cef-104">Mielőtt elkezdené, előfizetési információt [Kaphat a Microsoft 365 üzleti](get-microsoft-365-business.md) talál.</span><span class="sxs-lookup"><span data-stu-id="19cef-104">Before you get started, see [Get Microsoft 365 Business](get-microsoft-365-business.md) for sign-up details.</span></span>

<span data-ttu-id="19cef-105">Tekintse meg egy [rövid videó a Microsoft 365 üzleti beállítása](https://support.office.com/article/38003e30-9d10-44cf-b596-f1b5f662bfa1) a készlet varázsló, és ha nem rendelkezünk a helyszíni Active Directory használatával</span><span class="sxs-lookup"><span data-stu-id="19cef-105">Watch a [short video on how to set up Microsoft 365 Business](https://support.office.com/article/38003e30-9d10-44cf-b596-f1b5f662bfa1) by using the set up wizard, and when you don't have an on-premises Active Directory</span></span>
  

## <a name="overview"></a><span data-ttu-id="19cef-106">Áttekintés</span><span class="sxs-lookup"><span data-stu-id="19cef-106">Overview</span></span>

<span data-ttu-id="19cef-107">Lépéseket beállítása a legtöbb elvégezhető a telepítő varázsló, de az egyéb beállítások is szerepelnek.</span><span class="sxs-lookup"><span data-stu-id="19cef-107">Most of the set up steps can be done in the setup wizard, but the other options are also listed.</span></span>

1. <span data-ttu-id="19cef-108">[A tartomány hozzáadása](#add-your-domain-to-personalize-sign-in) (a domain [regisztráció](sign-up.md)során vásárolt, ha ez a lépés már megtörtént.)</span><span class="sxs-lookup"><span data-stu-id="19cef-108">[Add your domain](#add-your-domain-to-personalize-sign-in) (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>
2. <span data-ttu-id="19cef-109">Felhasználók hozzáadása.</span><span class="sxs-lookup"><span data-stu-id="19cef-109">Add users.</span></span> <span data-ttu-id="19cef-110">Ez a három módokon teheti meg:</span><span class="sxs-lookup"><span data-stu-id="19cef-110">You can do this in any of the three ways:</span></span>
    - <span data-ttu-id="19cef-111">A [telepítő varázsló](#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="19cef-111">In the [setup wizard](#add-users-in-the-wizard).</span></span>
    - <span data-ttu-id="19cef-112">Ha a helyszíni Active directory [Azure AD csatlakozás segítségével a felhasználók](#add-users-by-using-azure-ad-connect) hozzáadása a címtárszinkronizálás használata</span><span class="sxs-lookup"><span data-stu-id="19cef-112">Use directory synchronization to [add users by using Azure AD Connect](#add-users-by-using-azure-ad-connect) if you have an on-premises Active directory.</span></span>
    - <span data-ttu-id="19cef-113">Is [újabb felhasználók hozzáadása](add-users-m365b.md) a felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="19cef-113">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
3. <span data-ttu-id="19cef-114">Biztonsági házirendek beállítása, és eszközök konfigurálása.</span><span class="sxs-lookup"><span data-stu-id="19cef-114">Set up security policies and configure devices.</span></span> <span data-ttu-id="19cef-115">Ez a három módokon teheti meg:</span><span class="sxs-lookup"><span data-stu-id="19cef-115">You can do this in any of the three ways:</span></span>
    - <span data-ttu-id="19cef-116">A [telepítő varázsló](#set-up-policies-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="19cef-116">In the [setup wizard](#set-up-policies-in-the-wizard).</span></span>  
    - <span data-ttu-id="19cef-117">A [felügyeleti központ](#modify-or-add-policies-in-the-admin-center).</span><span class="sxs-lookup"><span data-stu-id="19cef-117">In the [admin center](#modify-or-add-policies-in-the-admin-center).</span></span>
    - <span data-ttu-id="19cef-118">A [felügyeleti központ Intune](https://docs.microsoft.com/intune/what-is-device-management).</span><span class="sxs-lookup"><span data-stu-id="19cef-118">In the [Intune admin center](https://docs.microsoft.com/intune/what-is-device-management).</span></span>
4. <span data-ttu-id="19cef-119">Állítsa be és Eszközkezelés Windows 10.</span><span class="sxs-lookup"><span data-stu-id="19cef-119">Set up and manage Windows 10 devices.</span></span>

    <span data-ttu-id="19cef-120">Azure ad WIndows 10 eszköz csatlakoztatásakor a házirendeket a rendszer alkalmazza azt.</span><span class="sxs-lookup"><span data-stu-id="19cef-120">When you join a WIndows 10 device to Azure AD, all the policies get applied to it.</span></span>
    - <span data-ttu-id="19cef-121">A [telepítő varázsló](#set-up-policies-in-the-wizard)a Windows 10 eszköz konfigurációjának beállítása.</span><span class="sxs-lookup"><span data-stu-id="19cef-121">Set up Windows 10 device configurations in the [setup wizard](#set-up-policies-in-the-wizard).</span></span>
    - <span data-ttu-id="19cef-122">Borzas AD egy [új Windows 10 eszköz](set-up-windows-devices.md#for-a-brand-new-or-newly-upgraded-windows-10-pro-device) csatlakoztatása.</span><span class="sxs-lookup"><span data-stu-id="19cef-122">Join a [new Windows 10 device](set-up-windows-devices.md#for-a-brand-new-or-newly-upgraded-windows-10-pro-device) to Azure AD.</span></span>
    - <span data-ttu-id="19cef-123">Borzas AD egy [meglévő Windows 10 eszköz](set-up-windows-devices.md#for-a-device-already-set-up-and-running-windows-10-pro) csatlakoztatása.</span><span class="sxs-lookup"><span data-stu-id="19cef-123">Join an [existing Windows 10 device](set-up-windows-devices.md#for-a-device-already-set-up-and-running-windows-10-pro) to Azure AD.</span></span>
1. <span data-ttu-id="19cef-124">Telepítse az Office 365 üzleti.</span><span class="sxs-lookup"><span data-stu-id="19cef-124">Install Office 365 Business.</span></span>
    - <span data-ttu-id="19cef-125">A [telepítő varázsló](#set-up-policies-in-the-wizard)segítségével a Windows-eszközök automatikusan telepíthető Office.</span><span class="sxs-lookup"><span data-stu-id="19cef-125">You can automatically install Office in the Windows devices by using the [setup wizard](#set-up-policies-in-the-wizard).</span></span>
    - <span data-ttu-id="19cef-126">Automatikusan [az Office telepítése](auto-install-or-uninstall-office.md) az admin center.</span><span class="sxs-lookup"><span data-stu-id="19cef-126">Automatically [install Office](auto-install-or-uninstall-office.md) from the admin center.</span></span>
    - <span data-ttu-id="19cef-127">Lehetővé teszik a felhasználók [Office alkalmazások telepítése](https://docs.microsoft.com/office365/admin/setup/install-applications) a Windows és az eszközök.</span><span class="sxs-lookup"><span data-stu-id="19cef-127">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
1. <span data-ttu-id="19cef-128">További biztonsági beállítása.</span><span class="sxs-lookup"><span data-stu-id="19cef-128">Set up additional security.</span></span>
    - <span data-ttu-id="19cef-129">A telepítő varázsló az eszközök biztonságos házirendeket ad, de azt is kihasználhatják a [további biztonsági](#additional-security-settings) szolgáltatásainak segítségével biztonságos segít az adatok, partnerek és e-mailek.</span><span class="sxs-lookup"><span data-stu-id="19cef-129">The setup wizard adds policies to secure your devices, but you can also take advantage of [additional security](#additional-security-settings) capabilities to helps secure your data, accounts, and emails.</span></span> 

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="19cef-130">Adja hozzá a tartományi felhasználók és a házirendek beállítása</span><span class="sxs-lookup"><span data-stu-id="19cef-130">Add your domain, users and set up policies</span></span>

![Mutató transzparens https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

<span data-ttu-id="19cef-132">Microsoft 365 üzleti beszerzése esetén a saját tartomány használata, vagy a vásárlás során lehetőség van az [Internet-előfizetési](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="19cef-132">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="19cef-133">Ha új tartomány létrehozása során vásárolt, a tartomány összes fel, és Ugrás [felhasználók hozzáadása és a licencek hozzárendelése](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="19cef-133">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="19cef-134">Az egyéni bejelentkezési tartomány hozzáadása</span><span class="sxs-lookup"><span data-stu-id="19cef-134">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="19cef-135">Jelentkezzen be a [Microsoft 365 felügyeleti központ](https://admin.microsoft.com) a globális rendszergazdai hitelesítő adatok használatával.</span><span class="sxs-lookup"><span data-stu-id="19cef-135">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="19cef-136">Válassza ki **a tartomány hozzáadása** varázsló elindításához.</span><span class="sxs-lookup"><span data-stu-id="19cef-136">Choose **Add a domain** to start the wizard.</span></span>

    ![Jelölje be a tartomány hozzáadása.](media/addadomainadmincenter.png)
    
3. <span data-ttu-id="19cef-138">A varázslóban adja meg a tartomány nevét (például contoso.com) használni kívánt.</span><span class="sxs-lookup"><span data-stu-id="19cef-138">In the wizard, enter the domain name you want to use (like contoso.com).</span></span>


    ![Képernyőkép a személyre szabás Bejelentkezés lapon.](media/personalizesignin.png)

    
4. <span data-ttu-id="19cef-140">Ellenőrzi a saját tartomány [létrehozása DNS-rekordokat az Office 365 bármely DNS-szolgáltatójánál,](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) kövesse a varázsló utasításait.</span><span class="sxs-lookup"><span data-stu-id="19cef-140">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="19cef-141">Ha ismeri a tartományi állomás, lásd még: [állomás konkrét utasításokat](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="19cef-141">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="19cef-142">Ha a videotár-szolgáltató GoDaddy, a folyamat egyszerű és program automatikusan kéri, jelentkezzen be, és hagyja, hogy a nevünkben hitelesíti a Microsoft:</span><span class="sxs-lookup"><span data-stu-id="19cef-142">If your hosting provider is GoDaddy, the process is easy and you will be automatically asked to sign in and let Microsoft authenticate on your behalf:</span></span>

    ![GoDaddy megerősítése adatelérési lapon jelölje be az engedélyezés.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="19cef-144">Felhasználók felvétele és licencek hozzárendelése</span><span class="sxs-lookup"><span data-stu-id="19cef-144">Add users and assign licenses</span></span>

<span data-ttu-id="19cef-145">A varázslóban hozzáadhat felhasználókat, de is [újabb felhasználók hozzáadása](add-users-m365b.md) a felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="19cef-145">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="19cef-146">Ezenkívül ha a helyi tartományvezérlő, hozzáadhat [Azure AD csatlakozás](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)rendelkező felhasználók.</span><span class="sxs-lookup"><span data-stu-id="19cef-146">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="19cef-147">Felhasználók hozzáadása varázsló</span><span class="sxs-lookup"><span data-stu-id="19cef-147">Add users in the wizard</span></span>

<span data-ttu-id="19cef-148">A varázsló felvett felhasználóknak Microsoft 365 üzleti licenc beszerzése automatikusan.</span><span class="sxs-lookup"><span data-stu-id="19cef-148">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>
<span data-ttu-id="19cef-149">Ha tartomány tartományvezérlőjét, és az Active Directory használata, lásd: [ddd felhasználók Azure AD csatlakozás segítségével](#add-users-by-using-azure-ad-connect).</span><span class="sxs-lookup"><span data-stu-id="19cef-149">If you have a local domain controller, and are using Active Directory, see [how to ddd users by using Azure AD Connect](#add-users-by-using-azure-ad-connect).</span></span>

![Képernyőkép a Hozzáadás új felhasználó lapon a varázsló](media/addnewuserspage.png)

1. <span data-ttu-id="19cef-p106">Ha az Microsoft 365 Business-előfizetéshez tartoznak meglévő felhasználók (például ha az Azure AD Connect szolgáltatást használta), akkor itt lehetősége lesz licenceket rendelheti hozzájuk. Nyugodtan felvehet licenceket hozzájuk is.</span><span class="sxs-lookup"><span data-stu-id="19cef-p106">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you will get an option to assign licenses to them now. Go ahead and add licenses to them as well.</span></span>

3. <span data-ttu-id="19cef-153">Miután hozzáadta a felhasználók, a hozzáadott új felhasználók hitelesítő adatok megosztása lehetőséget is fog kapni.</span><span class="sxs-lookup"><span data-stu-id="19cef-153">After you have added the users, you will also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="19cef-154">Ezeket kinyomtathatja, elküldheti e-mailben, vagy pedig letöltheti.</span><span class="sxs-lookup"><span data-stu-id="19cef-154">You can choose to print them out, email them, or download them.</span></span>

4. <span data-ttu-id="19cef-155">Hagyja ki az e-mail-üzenetek áttelepítését, és kattintson a **Tovább** gombra az **E-mail-üzenetek áttelepítése** lapon.</span><span class="sxs-lookup"><span data-stu-id="19cef-155">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 

    <span data-ttu-id="19cef-156">Ha áthelyezni egy másik e-mail szolgáltatójától, és később az adatok másolásához, akkor [e-mail áttelepítése és az Office 365 ügyfeleket](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span><span class="sxs-lookup"><span data-stu-id="19cef-156">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>

#### <a name="add-users-by-using-azure-ad-connect"></a><span data-ttu-id="19cef-157">Borzas AD csatlakozás segítségével a felhasználók hozzáadása</span><span class="sxs-lookup"><span data-stu-id="19cef-157">Add users by using Azure AD Connect</span></span>

 <span data-ttu-id="19cef-158">Ha az Active Directory tartomány tartományvezérlőjét, a felhasználók és szinkronizálása Microsoft 365 üzleti [Azure AD csatlakozás](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)segítségével.</span><span class="sxs-lookup"><span data-stu-id="19cef-158">If you have a local domain controller with Active Directory, you synchronize your users with Microsoft 365 Business by using [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span> <span data-ttu-id="19cef-159">Végezze el ezt a telepítő varázsló elindítása előtt.</span><span class="sxs-lookup"><span data-stu-id="19cef-159">Complete this before you start the setup wizard.</span></span> <span data-ttu-id="19cef-160">A felügyeleti központ letölthető:</span><span class="sxs-lookup"><span data-stu-id="19cef-160">You can download it in the admin center:</span></span>

- <span data-ttu-id="19cef-161">Keresse fel **a felhasználók** \> **aktív felhasználók**, az oldal tetején található az ellipszisek válassza, majd **a címtárszinkronizálás** Azure AD csatlakozás letöltése.</span><span class="sxs-lookup"><span data-stu-id="19cef-161">Go to **Users** \> **Active users**, select the ellipses on the top of the page and then select **Directory synchronization** to download Azure AD Connect.</span></span>

    ![Az aktív felhasználók lapján válassza ki az ellipszisek > könyvtár snchronization.](media/setupdirsync.png)

    > [!IMPORTANT]
    > <span data-ttu-id="19cef-163">Ha ezzel a módszerrel hoz létre a felhasználók, még akkor rendelhet licenceket azokat a felügyeleti központ.</span><span class="sxs-lookup"><span data-stu-id="19cef-163">If you create users this way, you will still have to assign licenses to them in the admin center.</span></span>

##### <a name="continue-to-access-domain-joined-apps-and-devices"></a><span data-ttu-id="19cef-164">Továbbra is elérhető a tartományhoz tartozó alkalmazások és eszközök</span><span class="sxs-lookup"><span data-stu-id="19cef-164">Continue to access domain-joined apps and devices</span></span>

<span data-ttu-id="19cef-165">Ha továbbra is elérhető a tartományhoz tartozó alkalmazások és eszközök, olvassa el az alábbi cikkekből, amelyek lehetővé teszik, hogy két különböző módon:</span><span class="sxs-lookup"><span data-stu-id="19cef-165">If you want to continue to access domain-joined apps and devices, read the following articles for two different way of enabling that:</span></span>
  
- [<span data-ttu-id="19cef-166">A tartományhoz csatlakoztatott Windows 10-es eszközök kezelésének engedélyezése a Microsoft 365 Vállalati verzió számára</span><span class="sxs-lookup"><span data-stu-id="19cef-166">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>](manage-windows-devices.md)
    - <span data-ttu-id="19cef-167">Ez az ajánlott módja.</span><span class="sxs-lookup"><span data-stu-id="19cef-167">This is the recommended way.</span></span>

- [<span data-ttu-id="19cef-168">Hozzáférés a helyi erőforrások egy Azure AD csatlakozott eszközről a Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="19cef-168">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>](access-resources.md)

### <a name="connect-your-domain"></a><span data-ttu-id="19cef-169">Tartomány csatlakoztatása</span><span class="sxs-lookup"><span data-stu-id="19cef-169">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="19cef-170">Ha a .onmicrosoft tartomány használata mellett, vagy Azure AD csatlakozás segítségével a felhasználók beállítása, ez a lépés nem jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="19cef-170">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="19cef-171">A szolgáltatások beállításához frissítenie kell bizonyos rekordokat a DNS-szolgáltatónál vagy a tartományregisztrálónál.</span><span class="sxs-lookup"><span data-stu-id="19cef-171">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="19cef-172">A beállítási varázsló általában felismeri a regisztrálóját, és részletes útmutatást jelenít meg arról, hogy miként frissítheti a névkiszolgálói rekordokat a regisztráló webhelyén.</span><span class="sxs-lookup"><span data-stu-id="19cef-172">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="19cef-173">Ha nem, [Módosítás nameservers beállítása az Office 365 bármely tartomány tartományneveket regisztráló szervezetnél](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="19cef-173">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="19cef-174">Ha meglévő DNS-rekordok, például egy létező webhelyen, érdemes kapcsolattartásra a meglévő szolgáltatások biztosításához a saját DNS-rekordok kezeléséhez.</span><span class="sxs-lookup"><span data-stu-id="19cef-174">If you have existing DNS records, for example an existing web site, you will want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="19cef-175">További információ a [tartomány alapjai](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="19cef-175">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Csatlakozás a tartomány lap i. fogja kezelni a saját DNS-rekordokat.](media/connectyourdomainpage.png)

2. <span data-ttu-id="19cef-177">Kövesse a varázsló utasításait, és e-mail és egyéb szolgáltatások hoznak létre meg.</span><span class="sxs-lookup"><span data-stu-id="19cef-177">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="set-up-security-policies-and-device-configurations"></a><span data-ttu-id="19cef-178">Állítsa be a biztonsági házirendek és az eszközök konfigurációja</span><span class="sxs-lookup"><span data-stu-id="19cef-178">Set up security policies and device configurations</span></span> 

<span data-ttu-id="19cef-179">Ezek a házirendek vonatkoznak minden felhasználó adhat a licencet, vagy a felhasználók egy csoportja, ha úgy dönt, hogy a felhasználók egy csoportja különböző házirendek hozzárendelése.</span><span class="sxs-lookup"><span data-stu-id="19cef-179">These policies apply to every user you give a license to, or to a group of users if you decide to assign different policies to a set of users.</span></span>

#### <a name="set-up-policies-in-the-wizard"></a><span data-ttu-id="19cef-180">A varázsló házirendek beállítása</span><span class="sxs-lookup"><span data-stu-id="19cef-180">Set up policies in the wizard</span></span>

<span data-ttu-id="19cef-181">A házirendek beállítása varázsló automatikusan alkalmazni *Minden felhasználó*létrehoz egy [biztonsági csoportot](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) .</span><span class="sxs-lookup"><span data-stu-id="19cef-181">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span>

1. <span data-ttu-id="19cef-182">A **mobil eszközökön a munka fájlok védelme** a beállítás **védelme Munkafájlok, ha elveszett vagy ellopott eszköz** alapértelmezés szerint van jelölve.</span><span class="sxs-lookup"><span data-stu-id="19cef-182">On the **Protect your work files on mobile devices** the option **Protect work files when devices are lost or stolen** is selected by default.</span></span> <span data-ttu-id="19cef-183">Akkor **kezelheti, hogy a felhasználók miként férhetnek hozzá a mobil eszközökön tárolt Office fájlokhoz**bekapcsolása lehetőséget, és ez ajánlott.</span><span class="sxs-lookup"><span data-stu-id="19cef-183">You have an option to turn on **Manage how users access Office files on mobile devices**, and this is recommended.</span></span>

    ![Munkafájlok védelme Képernyőkép a mobileszközök lapon.](media/protectworkfilesondevices.png)

     - <span data-ttu-id="19cef-185">Bontsa ki a **védelem Munkafájlok, ha az eszköz elveszett vagy ellopott**, ha az [alapértelmezett értékek](protect-work-files-on-lost-or-stolen-device.md) előre kiválasztott:</span><span class="sxs-lookup"><span data-stu-id="19cef-185">If you expand **Protect work files when devices are lost or stolen**, the [default values](protect-work-files-on-lost-or-stolen-device.md) are pre-selected:</span></span>

        ![Képernyőkép a elveszett eszköz fájlok védelme alapértelmezett értékeit.](media/protectworkfilesondevicesdefault.png)

    - <span data-ttu-id="19cef-187">Ha bejelöli a **kezelése, hogy a felhasználók miként férhetnek hozzá a mobil eszközökön található Office-fájlok** kibontásához, az [alapértelmezett értékek](manage-user-access-on-mobile-devices.md) jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="19cef-187">If you select **Manage how users access Office files on mobile devices** and expand it, the [default values](manage-user-access-on-mobile-devices.md) are shown.</span></span> <span data-ttu-id="19cef-188">Azt javasoljuk, hogy a telepítés során fogadja el azokat az alapértelmezett értékeket, amelyekkel minden felhasználóra vonatkozó alkalmazásházirendeket hozhat létre Android, iOS és Windows 10 rendszerekre.</span><span class="sxs-lookup"><span data-stu-id="19cef-188">We recommend you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="19cef-189">A telepítés után további házirendeket is létrehozhat majd.</span><span class="sxs-lookup"><span data-stu-id="19cef-189">You can create more policies after setup completes.</span></span>

        ![Képernyőkép a védelmi beállításait a hordozható Office-fájlokat.](media/useraccessonmobile.png)

2. <span data-ttu-id="19cef-191">Az utolsó lépés az adatok védelmét és az eszköz lehetővé teszi a házirendek beállítása Windows 10 eszközök biztonságos.</span><span class="sxs-lookup"><span data-stu-id="19cef-191">The last step on protect data and devices allows you to set up policies to secure Windows 10 devices.</span></span> <span data-ttu-id="19cef-192">Ezek a beállítások automatikusan érvényesek, ha a felhasználó Windows 10 csatlakozik a szervezet.</span><span class="sxs-lookup"><span data-stu-id="19cef-192">These settings are applied automatically when a user's Windows 10 connects to your organization.</span></span> <span data-ttu-id="19cef-193">Kibonthatja a **biztonságos Windows 10 eszközök** és az [alapértelmezett értékek](secure-windows-10-devices.md)módosíthatók.</span><span class="sxs-lookup"><span data-stu-id="19cef-193">You can expand **Secure Windows 10 devices** to see and modify the [default values](secure-windows-10-devices.md).</span></span>
3. <span data-ttu-id="19cef-194">Választhatja azt is, [automatikus telepítése az Office](install-office-on-windows-10-during-setup.md) eszközök a Windows 10.</span><span class="sxs-lookup"><span data-stu-id="19cef-194">You can also choose to [automatically install Office](install-office-on-windows-10-during-setup.md) on Windows 10 devices.</span></span>

    ![Képernyőkép a Windows 10 eszköz konfigurációs lapon állítsa be.](media/setwin10config.png)

#### <a name="modify-or-add-policies-in-the-admin-center"></a><span data-ttu-id="19cef-196">Módosítsa vagy adja hozzá a házirendek a felügyeleti központ</span><span class="sxs-lookup"><span data-stu-id="19cef-196">Modify or add policies in the admin center</span></span>

<span data-ttu-id="19cef-197">Lásd a [Microsoft 365 tevékenység kezelésére](manage.md) vonatkozó házirendek hogyan lehet megtekinteni és módosítani az eszköz-és app témakörökre mutató hivatkozásokat, és hogyan adatainak eltávolítása vagy visszaállítása a felhasználói eszközök.</span><span class="sxs-lookup"><span data-stu-id="19cef-197">See [manage Microsoft 365 Business](manage.md) for links to topics on how to view and modify device and app protection polices, and how to remove data from, or reset user devices.</span></span>

## <a name="deploy-and-manage-windows-10"></a><span data-ttu-id="19cef-198">Telepítését és kezelését a Windows 10</span><span class="sxs-lookup"><span data-stu-id="19cef-198">Deploy and manage Windows 10</span></span>
<span data-ttu-id="19cef-199">Manuális csatlakoztatása Azure AD, vagy új számítógépek, illetve a meglévő számítógépek bejelentkezési profil módosításával a telepítés során a [Microsoft 365 üzleti felhasználók számára a Windows-eszközök beállítása](set-up-windows-devices.md) témakörben található.</span><span class="sxs-lookup"><span data-stu-id="19cef-199">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) to manually connect to Azure AD, either during setup for new computers, or by changing sign-in profile for existing computers.</span></span> 

### <a name="use-autopilot-to-set-up-new-devices"></a><span data-ttu-id="19cef-200">Automata segítségével állítsa be az új eszközök</span><span class="sxs-lookup"><span data-stu-id="19cef-200">Use Autopilot to set up new devices</span></span>

<span data-ttu-id="19cef-201">[Windows automata](add-autopilot-devices-and-profile.md) segítségével automatikusan előre konfigurálja egy felhasználó **Új** Windows 10 eszközök, de lehet egyszerűbben, egy [partner](https://www.microsoft.com/solution-providers/search) , aki teheti meg.</span><span class="sxs-lookup"><span data-stu-id="19cef-201">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="19cef-202">Ugrás a [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) is, és kérje meg a felhő technológia szakértői vásárol meg az új eszközök beállítása.</span><span class="sxs-lookup"><span data-stu-id="19cef-202">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) and ask a cloud technology expert set up new devices you purchase for you.</span></span>

### <a name="access-on-premises-resources"></a><span data-ttu-id="19cef-203">Helyi erőforrások eléréséhez.</span><span class="sxs-lookup"><span data-stu-id="19cef-203">Access on-premises resources</span></span>

<span data-ttu-id="19cef-204">Ha a szervezet használja a Windows Server Active Directory helyszíni, állíthat be Microsoft 365 üzleti védelme érdekében a Windows 10 eszközök továbbra is fenntartva helyi hitelesítést igénylő helyszíni erőforrásokhoz való hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="19cef-204">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="19cef-205">Kövesse a [Microsoft 365 üzleti által kezelt tartományhoz tartozó Windows 10 eszközök engedélyezése](manage-windows-devices.md) meg.</span><span class="sxs-lookup"><span data-stu-id="19cef-205">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="19cef-206">Ez a javasolt módszer és eszközök ebben az állapotban úgynevezett hibrid Azure AD eszközöket csatlakozott.</span><span class="sxs-lookup"><span data-stu-id="19cef-206">This is the preferred method and devices in this state are called Hybrid Azure AD joined devices.</span></span>

<span data-ttu-id="19cef-207">Ha a vállalatnál a helyi Active Directory, amely tartalmazza az egyes helyi erőforrásokat (például fájlmegosztásokat és nyomtatókat), a Borzas AD csatlakoztatott eszközök hozzáférést biztosíthat a forrásokhoz való lépések itt: [Access helyszíni erőforrásokat egy 365 üzleti Microsoft Azure AD csatlakozott eszköz](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="19cef-207">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers) , you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="19cef-208">Telepítse az Office 365 ügyfélalkalmazások</span><span class="sxs-lookup"><span data-stu-id="19cef-208">Deploy Office 365 client apps</span></span>

<span data-ttu-id="19cef-209">Ha azt választotta, hogy automatikusan telepíti az Office-alkalmazások a telepítéskor ki, az apps telepíti a Windows 10 eszközök után a felhasználó bejelentkezett az Azure AD a munka hitelesítő adatokkal a Windows eszközök.</span><span class="sxs-lookup"><span data-stu-id="19cef-209">If you chose to automatically install Office apps in during the set up, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices with their work credentials.</span></span>
<span data-ttu-id="19cef-210">Office telepítése mobil iOS vagy Android-eszköz, lásd: [állítsa be a mobil eszközök Microsoft 365 üzleti felhasználók számára](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="19cef-210">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="19cef-211">Office külön-külön is telepíthető.</span><span class="sxs-lookup"><span data-stu-id="19cef-211">You can also install Office individually.</span></span> <span data-ttu-id="19cef-212">Lásd: [PC vagy Mac Office telepítéséhez](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) további útmutatást.</span><span class="sxs-lookup"><span data-stu-id="19cef-212">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) for instructions.</span></span>

## <a name="additional-security-settings"></a><span data-ttu-id="19cef-213">További biztonsági beállítások</span><span class="sxs-lookup"><span data-stu-id="19cef-213">Additional security settings</span></span>

<span data-ttu-id="19cef-214">A biztonsági és kompatibilitási beállítást a telepítő varázsló mellett a következő további beállításokat is meg lehet:</span><span class="sxs-lookup"><span data-stu-id="19cef-214">In addition to the security and compliance setting in the setup wizard, you can also set up the following additional settings:</span></span>
  
- <span data-ttu-id="19cef-215">**E-mail rosszindulatú programok elleni védekezés**</span><span class="sxs-lookup"><span data-stu-id="19cef-215">**Email malware protection**</span></span>
- <span data-ttu-id="19cef-216">**Speciális veszély védelmi (ATP) biztonságos mellékletek**</span><span class="sxs-lookup"><span data-stu-id="19cef-216">**Advanced Threat Protection (ATP) Safe Attachments**</span></span>
- <span data-ttu-id="19cef-217">**ATP ajánlott hivatkozások**</span><span class="sxs-lookup"><span data-stu-id="19cef-217">**ATP Safe Links**</span></span>
- <span data-ttu-id="19cef-218">**APT adatlopás**</span><span class="sxs-lookup"><span data-stu-id="19cef-218">**APT anti-phishing**</span></span>
- <span data-ttu-id="19cef-219">**Exchange Online Archiválás**</span><span class="sxs-lookup"><span data-stu-id="19cef-219">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="19cef-220">**Adatvesztés megelőzése (DLP)**</span><span class="sxs-lookup"><span data-stu-id="19cef-220">**Data loss prevention (DLP)**</span></span>
- <span data-ttu-id="19cef-221">**Borzas információk védelméről** (1 terv)</span><span class="sxs-lookup"><span data-stu-id="19cef-221">**Azure Information Protection** (Plan 1)</span></span>
- <span data-ttu-id="19cef-222">**Intune portál elérhetősége**</span><span class="sxs-lookup"><span data-stu-id="19cef-222">**Intune portal availability**</span></span>

<span data-ttu-id="19cef-223">Get elindítani a [Speciális biztonsági házirendek beállítása](set-up-advanced-security.md)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="19cef-223">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

<span data-ttu-id="19cef-224">Lásd még: [365 a Microsoft üzleti biztonságos felső 10 mód](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) a legjobb biztonsági gyakorlatok ütemterv.</span><span class="sxs-lookup"><span data-stu-id="19cef-224">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>
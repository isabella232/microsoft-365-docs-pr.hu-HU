---
title: A Microsoft 365 Business beállítása a beállítási varázslóval
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
description: Útmutató a Microsoft 365 üzleti beállítása négy lépés végrehajtásával.
ms.openlocfilehash: a1c8a41c3e291983276280a063248bdd10a7f85a
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32283911"
---
# <a name="set-up-microsoft-365-business-by-using-the-setup-wizard"></a><span data-ttu-id="33036-103">A Microsoft 365 Business beállítása a beállítási varázslóval</span><span class="sxs-lookup"><span data-stu-id="33036-103">Set up Microsoft 365 Business by using the setup wizard</span></span>

<span data-ttu-id="33036-104">Hajtsa végre az alábbi 1 – 4.</span><span class="sxs-lookup"><span data-stu-id="33036-104">Complete steps 1-4 below.</span></span>
  
### <a name="set-up-microsoft-365-business"></a><span data-ttu-id="33036-105">A Microsoft 365 Business beállítása</span><span class="sxs-lookup"><span data-stu-id="33036-105">Set up Microsoft 365 Business</span></span>

<span data-ttu-id="33036-106">Ha helyszíni Active Directory nincs Microsoft 365 üzleti beállítása a videó megtekintése:</span><span class="sxs-lookup"><span data-stu-id="33036-106">Watch a video on how to set up Microsoft 365 Business when you don't have an on-premises Active Directory:</span></span>
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/0705c337-f3e8-4d28-bb6c-530cd28e99f2?autoplay=false]
  
<span data-ttu-id="33036-107">A beállítási lépéseket a telepítéshez, amely tartalmazza a helyi Active Directory információkat tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="33036-107">The set-up steps include information for setups that include local Active Directory.</span></span> <span data-ttu-id="33036-108">Ha továbbra is elérhető a tartományhoz csatlakoztatott eszközök, olvassa el az alábbi cikkekből, amelyek lehetővé teszik, hogy két különböző módon, és hajtsa végre a varázsló futtatása előtt:</span><span class="sxs-lookup"><span data-stu-id="33036-108">If you want to continue to access domain-joined devices, read the following articles for two different way of enabling that, and complete the steps before you run the Setup wizard:</span></span>
  
- [<span data-ttu-id="33036-109">A tartományhoz csatlakoztatott Windows 10-es eszközök kezelésének engedélyezése a Microsoft 365 Vállalati verzió számára</span><span class="sxs-lookup"><span data-stu-id="33036-109">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>](manage-windows-devices.md)
    
    <span data-ttu-id="33036-110">-Ez az ajánlott módja.</span><span class="sxs-lookup"><span data-stu-id="33036-110">-This is the recommended way.</span></span>
    
- [<span data-ttu-id="33036-111">Hozzáférés a helyi erőforrások egy Azure AD csatlakozott eszközről a Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="33036-111">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>](access-resources.md)
    
### <a name="step-1-personalize-sign-in"></a><span data-ttu-id="33036-112">1. lépés: A bejelentkezés testreszabása</span><span class="sxs-lookup"><span data-stu-id="33036-112">Step 1: Personalize sign-in</span></span>

1. <span data-ttu-id="33036-p102">Jelentkezzen be a [Microsoft 365 Business](https://portal.microsoft.com) szolgáltatásba a globális rendszergazdai hitelesítő adataival. A **Felügyelet** csempét választva lépjen a felügyeleti központba.</span><span class="sxs-lookup"><span data-stu-id="33036-p102">Sign in to [Microsoft 365 Business](https://portal.microsoft.com) by using your global admin credentials. Choose the **Admin** tile to go to the admin center.</span></span> 
    
2. <span data-ttu-id="33036-115">Válassza a **Beállítás indítása** lehetőséget (az állapotától függően előfordulhat, hogy ehelyett a **Beállítás folytatása** elem látható) a felügyeleti központban a varázsló elindításához.</span><span class="sxs-lookup"><span data-stu-id="33036-115">Choose **Start setup** (depending on your state you may see **Continue setup** instead) in the admin center to start the wizard.</span></span> 
    
3. <span data-ttu-id="33036-116">Adja meg a használni kívánt tartomány nevét (például contoso.com).</span><span class="sxs-lookup"><span data-stu-id="33036-116">Enter the domain name you want to use (like contoso.com).</span></span>
    
    <span data-ttu-id="33036-117">Nyugodtan megadhatja a tartományt akkor is, ha már ellenőrizte például az Azure AD Connect használata során.</span><span class="sxs-lookup"><span data-stu-id="33036-117">Go ahead and enter your domain even if you have verified it while using Azure AD Connect, for example.</span></span> <span data-ttu-id="33036-118">A következő két lépést nem vonatkoznak, ha Azure AD csatlakozás segítségével ellenőrizze a tartomány.</span><span class="sxs-lookup"><span data-stu-id="33036-118">The following two steps do not apply to you if you used Azure AD Connect to verify your domain.</span></span>
    
4. <span data-ttu-id="33036-119">Ellenőrzi a saját tartomány [létrehozása DNS-rekordokat az Office 365 bármely DNS-szolgáltatójánál,](https://support.office.com/article/7b7b075d-79f9-4e37-8a9e-fb60c1d95166) kövesse a varázsló utasításait.</span><span class="sxs-lookup"><span data-stu-id="33036-119">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://support.office.com/article/7b7b075d-79f9-4e37-8a9e-fb60c1d95166) that verifies you own the domain.</span></span> 
    
    <span data-ttu-id="33036-120">Megtekintheti egy példa videó [Videó: telepítés Office 365 az új Admin központban](https://support.office.com/article/a8c2002a-34bc-4ab3-93d8-9b5156c48bf8).</span><span class="sxs-lookup"><span data-stu-id="33036-120">You can view an example video of [Video: Setup Office 365 in the new Admin Center](https://support.office.com/article/a8c2002a-34bc-4ab3-93d8-9b5156c48bf8).</span></span> <span data-ttu-id="33036-121">Fontos megjegyezni, hogy a videóban nem szerepelnek az Microsoft 365 Business adatvédelmi lépései.</span><span class="sxs-lookup"><span data-stu-id="33036-121">Note that this video does not include the data protection steps of Microsoft 365 Business.</span></span>
    
    ![Screenshot of the Business Cloud Suite setup wizard.](media/3c4fd40c-2de1-4a87-8ee0-78d3928c7bb7.png)
  
### <a name="step-2-add-users-and-assign-licenses"></a><span data-ttu-id="33036-123">2. lépés: Felhasználók hozzáadása és a licencek hozzárendelése</span><span class="sxs-lookup"><span data-stu-id="33036-123">Step 2: Add users and assign licenses</span></span>

1. <span data-ttu-id="33036-124">A felhasználókat felveheti itt, vagy [később is](add-users-m365b.md) a felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="33036-124">You can add users here, or you can [add users later](add-users-m365b.md) in the admin center.</span></span> 
    
    <span data-ttu-id="33036-125">A rendszer minden felvett felhasználóhoz automatikusan hozzárendel egy Microsoft 365 Business-licencet.</span><span class="sxs-lookup"><span data-stu-id="33036-125">Any users you add get automatically assigned a Microsoft 365 Business license.</span></span>
    
2. <span data-ttu-id="33036-p105">Ha az Microsoft 365 Business-előfizetéshez tartoznak meglévő felhasználók (például ha az Azure AD Connect szolgáltatást használta), akkor itt lehetősége lesz licenceket rendelheti hozzájuk. Nyugodtan felvehet licenceket hozzájuk is.</span><span class="sxs-lookup"><span data-stu-id="33036-p105">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you will get an option to assign licenses to them now. Go ahead and add licenses to them as well.</span></span>
    
3. <span data-ttu-id="33036-p106">Emellett arra is lesz lehetősége, hogy megossza a hitelesítő adatokat a felvett új felhasználókkal. Ezeket kinyomtathatja, elküldheti e-mailben, vagy pedig letöltheti.</span><span class="sxs-lookup"><span data-stu-id="33036-p106">You will also get an option to share credentials with the new users you added. You can choose to print them out, email them, or download them.</span></span>
    
4. <span data-ttu-id="33036-130">Hagyja ki az e-mail-üzenetek áttelepítését, és kattintson a **Tovább** gombra az **E-mail-üzenetek áttelepítése** lapon.</span><span class="sxs-lookup"><span data-stu-id="33036-130">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 
    
    <span data-ttu-id="33036-131">Ha áthelyezni egy másik e-mail szolgáltatójától, és később az adatok másolásához, akkor [e-mail áttelepítése és az Office 365 ügyfeleket](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span><span class="sxs-lookup"><span data-stu-id="33036-131">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>
    
    ![Screenshot of two new users added in the setup wizard](media/8f729967-5c65-4ceb-b737-18119db40564.png)
  
### <a name="step-3-connect-your-domain"></a><span data-ttu-id="33036-133">3. lépés: Csatlakozás a tartomány</span><span class="sxs-lookup"><span data-stu-id="33036-133">Step 3: Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="33036-134">Ha a .onmicrosoft tartomány használata mellett, vagy Azure AD csatlakozás használt, ez a lépés nem jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="33036-134">If you chose to use the .onmicrosoft domain, or used Azure AD Connect, you will not see this step.</span></span> 
  
<span data-ttu-id="33036-135">A szolgáltatások beállításához frissítenie kell bizonyos rekordokat a DNS-szolgáltatónál vagy a tartományregisztrálónál.</span><span class="sxs-lookup"><span data-stu-id="33036-135">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="33036-136">A beállítási varázsló általában felismeri a regisztrálóját, és részletes útmutatást jelenít meg arról, hogy miként frissítheti a névkiszolgálói rekordokat a regisztráló webhelyén.</span><span class="sxs-lookup"><span data-stu-id="33036-136">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="33036-137">Ha nem, [Módosítás nameservers beállítása az Office 365 bármely tartomány tartományneveket regisztráló szervezetnél](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="33036-137">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span>
    
2. <span data-ttu-id="33036-138">A levelezési és egyéb szolgáltatásokat a rendszer beállítja Önnek</span><span class="sxs-lookup"><span data-stu-id="33036-138">Email and other services will be set up for you</span></span>
    
### <a name="step-4-manage-devices-and-work-files"></a><span data-ttu-id="33036-139">4. lépés: Eszközök kezelése és fájlok használata</span><span class="sxs-lookup"><span data-stu-id="33036-139">Step 4: Manage devices and work files</span></span>

1. <span data-ttu-id="33036-140">A **Munkafájlok védelme a mobileszközök** lap beállítása **védelme Munkafájlok, ha elveszett vagy ellopott eszközök** és a beállítások **kezelése, hogy a felhasználók miként férhetnek hozzá a mobil eszközökön tárolt Office fájlokhoz** **a**.</span><span class="sxs-lookup"><span data-stu-id="33036-140">On the **Protect work files on your mobile devices** page set both **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** settings to **On**.</span></span> <span data-ttu-id="33036-141">Minden rész beállításra kattintva minden beállítás a chevron is elérhető.</span><span class="sxs-lookup"><span data-stu-id="33036-141">You can also access each sub-setting by clicking the chevrons next to each setting.</span></span>
  
  <span data-ttu-id="33036-142">A licenccel rendelkező felhasználók munka fájlokat most védett iOS és Android-eszköz, azokat a lehető leghamarabb [telepítse az Office alkalmazások](set-up-mobile-devices.md) (és azok Microsoft 365 üzleti hitelesítő adatokkal hitelesítik).</span><span class="sxs-lookup"><span data-stu-id="33036-142">All of your licensed users' work files are now protected on iOS and Android devices, as soon as they [install Office apps](set-up-mobile-devices.md) (and authenticate with their Microsoft 365 Business credentials).</span></span> 
  
  ![Screenshot of protect work files on your mobile devices page](media/3139a9aa-6228-4e74-8166-c6a886d7319f.PNG)
  
2. <span data-ttu-id="33036-144">A **Windows 10 beállítása eszköz konfigurációs** lapon állítsa be a **Windows 10 eszközök biztonságos** **meg**.</span><span class="sxs-lookup"><span data-stu-id="33036-144">On the **Set Windows 10 device configuration** page, set **Secure Windows 10 Devices** setting to **On**.</span></span>
  
   <span data-ttu-id="33036-145">Minden rész beállítás mellett a francia idézőjelre kattintva is elérheti.</span><span class="sxs-lookup"><span data-stu-id="33036-145">You can also access each sub-setting by clicking the chevron next to it.</span></span>
  
3. <span data-ttu-id="33036-146">Állítsa be az **Office telepítése Windows 10 eszközök** **Igen** Ha minden felhasználó Windows 10 számítógéppel rendelkezik, és telepíti vagy nem létező Office vagy Office-telepítések való kattintásra.</span><span class="sxs-lookup"><span data-stu-id="33036-146">Set the **Install Office on Windows 10 Devices** setting to **Yes** if all of your users have Windows 10 computers, and either no existing Office installs, or click-to-run Office installs.</span></span> <span data-ttu-id="33036-147">Ha nem ez a helyzet, ez a beállítás **nem**értékre.</span><span class="sxs-lookup"><span data-stu-id="33036-147">If this is not the case, set this option to **No**.</span></span> <span data-ttu-id="33036-148">Lehetőség van [automatikus telepítése az Office](auto-install-or-uninstall-office.md) újabb admin közepétől már rendelkezésre állnak a felhasználó számítógépére.</span><span class="sxs-lookup"><span data-stu-id="33036-148">You can [automatically install Office](auto-install-or-uninstall-office.md) later from the admin center after you have prepared the user computers.</span></span> <span data-ttu-id="33036-149">Útmutatásért lásd: az [Office ügyfél telepítésének előkészítéséhez](prepare-for-office-client-deployment.md).</span><span class="sxs-lookup"><span data-stu-id="33036-149">For instructions, see [prepare for Office client installation](prepare-for-office-client-deployment.md).</span></span>
  
    <span data-ttu-id="33036-150">Munkafájlok licenccel rendelkező felhasználók a Windows 10 eszközök, amint azok tervezett fog [csatlakozni a Windows 10 eszköz](set-up-windows-devices.md) Microsoft 365 Business Azure AD tartomány vagy [Windows 10 új számítógépre telepíti](https://support.office.com/article/c654bd23-d256-4ac7-8fba-0c993bf5a771.aspx) a Microsoft 365 egyidejűleg csatlakozó Üzleti Azure Active Directory-tartománynak.</span><span class="sxs-lookup"><span data-stu-id="33036-150">The licensed users' work files on Windows 10 devices will be projected as soon as they [join their Windows 10 device](set-up-windows-devices.md) to a Microsoft 365 Business Azure AD domain or [install Windows 10 on a new computer](https://support.office.com/article/c654bd23-d256-4ac7-8fba-0c993bf5a771.aspx) while simultaneously joining the Microsoft 365 Business Azure AD domain.</span></span> 
  
4. <span data-ttu-id="33036-151">Kattintson a **Tovább** gombra, és a telepítő befejezte.</span><span class="sxs-lookup"><span data-stu-id="33036-151">Click **Next** and you are done with setup.</span></span> 
  
    <span data-ttu-id="33036-152">Kérjük visszajelzés nekünk ennél a lépésnél segítheti a tapasztalat.</span><span class="sxs-lookup"><span data-stu-id="33036-152">Please leave us feedback at this step to help us improve the experience.</span></span>
  
    ![Screenshot of Prepare Windows 10 devices page](media/bff701c1-48a3-44f4-aa95-9d959d57c85b.PNG)
  
## <a name="additional-security-settings"></a><span data-ttu-id="33036-154">További biztonsági beállítások</span><span class="sxs-lookup"><span data-stu-id="33036-154">Additional security settings</span></span>

<span data-ttu-id="33036-155">A biztonsági és kompatibilitási beállítást a telepítő varázsló mellett a következő további beállításokat is meg lehet:</span><span class="sxs-lookup"><span data-stu-id="33036-155">In addition to the security and compliance setting in the setup wizard, you can also set up the following additional settings:</span></span>
  
- <span data-ttu-id="33036-156">Állítsa be a nem biztonságos mellékletek elleni védelem.</span><span class="sxs-lookup"><span data-stu-id="33036-156">Set up protection against unsafe attachments.</span></span> <span data-ttu-id="33036-157">**Speciális veszély védelmi** (ATP) azonosítja a rosszindulatú tartalmat, és adathalászó sémák és ransomware fertőzések elleni védelme, majd blokkolja a nem biztonságos mellékletek, szállítás.</span><span class="sxs-lookup"><span data-stu-id="33036-157">**Advanced Threat Protection** (ATP) identifies malicious content and then blocks delivery of unsafe attachments, helping protect you against phishing schemes and ransomware infections.</span></span> <span data-ttu-id="33036-158">Melléklet védelem aktiválása, lásd: [Office 365 ATP biztonságos mellékletek házirendek beállítása](https://support.office.com/article/078eb946-819a-4e13-8673-fe0c0ad3a775#setpolicy).</span><span class="sxs-lookup"><span data-stu-id="33036-158">To activate attachment protection, see [Set up Office 365 ATP Safe Attachments policies](https://support.office.com/article/078eb946-819a-4e13-8673-fe0c0ad3a775#setpolicy).</span></span>
    
- <span data-ttu-id="33036-159">A környezet védelme, amikor a felhasználó a rosszindulatú hivatkozások kattint.</span><span class="sxs-lookup"><span data-stu-id="33036-159">Protect your environment when users click malicious links.</span></span> <span data-ttu-id="33036-160">ATP megvizsgálja e-mailben található hivatkozásokra, amikor a felhasználó rájuk kattint.</span><span class="sxs-lookup"><span data-stu-id="33036-160">ATP examines links in email at the time a user clicks them.</span></span> <span data-ttu-id="33036-161">Ha a kapcsolat nem biztonságos, a felhasználó figyelmeztetést arról, hogy nem a webhelyen vagy tájékoztatták, hogy a hely le van tiltva.</span><span class="sxs-lookup"><span data-stu-id="33036-161">If a link is unsafe, the user is warned not to visit the site or informed that the site has been blocked.</span></span> <span data-ttu-id="33036-162">Ez segít az adatlopás elleni védelem.</span><span class="sxs-lookup"><span data-stu-id="33036-162">This helps protect against phishing schemes.</span></span> <span data-ttu-id="33036-163">[Office 365 ATP biztonságos csatolások házirendek beállítása](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#reveddefaultscc) , vagy [Office 365 ATP biztonságos csatolások házirendek beállítása](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#addemailpolscc).</span><span class="sxs-lookup"><span data-stu-id="33036-163">[Set up Office 365 ATP Safe Links policies](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#reveddefaultscc) or [Set up Office 365 ATP Safe Links policies](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#addemailpolscc).</span></span>
    
- <span data-ttu-id="33036-164">Minden postaláda tartalom, beleértve a törölt elemek helyezi a felhasználó teljes postaláda **peres eljárás tartsa**megőrizhető.</span><span class="sxs-lookup"><span data-stu-id="33036-164">You can preserve all mailbox content including deleted items by putting a user's entire mailbox on **litigation hold**.</span></span> <span data-ttu-id="33036-165">Útmutatásért lásd:</span><span class="sxs-lookup"><span data-stu-id="33036-165">For instructions, see</span></span> 
- <span data-ttu-id="33036-166">[E-mail adatmegőrzési az Exchange Online archiválás beállítása](security-features.md#set-up-email-retention-with-exchange-online-archiving).</span><span class="sxs-lookup"><span data-stu-id="33036-166">[Set up email retention with Exchange Online Archiving](security-features.md#set-up-email-retention-with-exchange-online-archiving).</span></span>
    
- <span data-ttu-id="33036-167">Állítsa be egyéni **adatmegőrzési szabályok**, például egy bizonyos meghatározott ideig megőrizni és tartalom véglegesen törli a birtokon tartási időszak végén.</span><span class="sxs-lookup"><span data-stu-id="33036-167">Set up customized **retention policies**, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="33036-168">Engedélyezheti az értékpapírok és a Megfelelési központba, keresse fel az **adatok kormányzás** egyéni adatmegőrzési \> **fenntartását**, és kövesse a varázsló utasításait.</span><span class="sxs-lookup"><span data-stu-id="33036-168">You can enable customized retention policies in the Securities and compliance center, go to **Data governance** \> **Retention**, and then follow the steps in the wizard.</span></span> <span data-ttu-id="33036-169">További [adatmegőrzési szabályok – áttekintés](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="33036-169">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>
    
## <a name="next-steps"></a><span data-ttu-id="33036-170">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="33036-170">Next steps</span></span>

<span data-ttu-id="33036-171">A licencekkel már rendelkező felhasználóknak következő lépésként be kell állítaniuk az eszközeiket.</span><span class="sxs-lookup"><span data-stu-id="33036-171">For the users that have their licenses, the next step is to set up devices.</span></span><br/> <span data-ttu-id="33036-172">Lásd: [Windows rendszerű eszközök beállítása a Microsoft 365 Business felhasználóinak](set-up-windows-devices.md) és [Mobileszközök beállítása a Microsoft 365 Business felhasználóinak](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="33036-172">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) and [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span> <br/><span data-ttu-id="33036-173">[A Microsoft 365 Business kezelése](manage.md) című témakörben olyan hivatkozásokat talál, amelyekre kattintva az eszköz és az appvédelmi házirendek beállításával és az adatok felhasználói eszközökről történő eltávolításával foglalkozó cikkek érhetők el.</span><span class="sxs-lookup"><span data-stu-id="33036-173">See [Manage Microsoft 365 Business](manage.md) for links to topics on how to set device and app protection polices, and how to remove data from user devices.</span></span> 
  



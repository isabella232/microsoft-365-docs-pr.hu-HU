---
title: Windows-eszközök beállítása a Microsoft 365 vállalati prémium verzió felhasználóinak
f1.keywords:
- CSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: Megtudhatja, hogy miként állíthatja be a Windows 10 Pro rendszert futtató Windows-eszközöket a Microsoft 365 vállalati prémium verzió felhasználóinak, és engedélyezze a központi felügyeletet és a biztonsági vezérlőket.
ms.openlocfilehash: c95b9e51c7ec3c440509fe34084d2a030c7f2eec
ms.sourcegitcommit: e56894917d2aae05705c3b9447388d10e2156183
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48841259"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a><span data-ttu-id="b82c9-103">Windows-eszközök beállítása a Microsoft 365 vállalati prémium verzió felhasználóinak</span><span class="sxs-lookup"><span data-stu-id="b82c9-103">Set up Windows devices for Microsoft 365 Business Premium users</span></span>

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-premium-users"></a><span data-ttu-id="b82c9-104">A Windows-eszközök Microsoft 365 vállalati prémium verziós felhasználóknak való beállításának előfeltételei</span><span class="sxs-lookup"><span data-stu-id="b82c9-104">Prerequisites for setting up Windows devices for Microsoft 365 Business Premium users</span></span>

<span data-ttu-id="b82c9-105">Mielőtt beállíthatja a Windows-eszközöket a Microsoft 365 vállalati prémium verzió felhasználóinak, győződjön meg arról, hogy minden Windows-eszközön Windows 10 Pro, 1703-es verzió (alkotók frissítése) fut.</span><span class="sxs-lookup"><span data-stu-id="b82c9-105">Before you can set up Windows devices for Microsoft 365 Business Premium users, make sure all the Windows devices are running Windows 10 Pro, version 1703 (Creators Update).</span></span> <span data-ttu-id="b82c9-106">Windows 10 Pro a Windows 10 Business központi telepítésének előfeltétele, amely a Windows 10 Pro rendszerhez készült felhőalapú szolgáltatások és eszközkezelés, valamint a Microsoft 365 vállalati prémium verzió központi kezelési és biztonsági ellenőrzésének engedélyezése.</span><span class="sxs-lookup"><span data-stu-id="b82c9-106">Windows 10 Pro is a prerequisite for deploying Windows 10 Business, which is a set of cloud services and device management capabilities that complement Windows 10 Pro and enable the centralized management and security controls of Microsoft 365 Business Premium.</span></span>
  
<span data-ttu-id="b82c9-107">Ha Windows 7 Pro, Windows 8 Pro vagy Windows 8,1 Pro rendszerű Windows-eszközökkel rendelkezik, Microsoft 365 vállalati prémium verzióra szóló előfizetése feljogosítja a Windows 10-es frissítésre.</span><span class="sxs-lookup"><span data-stu-id="b82c9-107">If you have Windows devices running Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your Microsoft 365 Business Premium subscription entitles you to a Windows 10 upgrade.</span></span>
  
<span data-ttu-id="b82c9-108">Ha többet szeretne megtudni arról, hogy hogyan frissítheti Windows-eszközeit a Windows 10 Pro alkotói frissítésére, kövesse a következő témakörben szereplő lépéseket: [Windows-eszközök frissítése a Windows Pro alkotói frissítésére](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="b82c9-108">For more information on how to upgrade Windows devices to Windows 10 Pro Creators Update, follow the steps in this topic: [Upgrade Windows devices to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
  
<span data-ttu-id="b82c9-109">Ellenőrizze, hogy az [eszköz csatlakoztatva van](#verify-the-device-is-connected-to-azure-ad) -e az Azure ad-hoz, és ellenőrizze, hogy rendelkezik-e a frissítéssel, vagy hogy biztosan működött-e a frissítés.</span><span class="sxs-lookup"><span data-stu-id="b82c9-109">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to verify you have the upgrade, or to make sure the upgrade worked.</span></span>

<span data-ttu-id="b82c9-110">Nézze meg ezt a rövid videót a Windows csatlakoztatásáról a Microsoft 365-ra.</span><span class="sxs-lookup"><span data-stu-id="b82c9-110">Watch a short video about connecting Windows to Microsoft 365.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

<span data-ttu-id="b82c9-111">Ha hasznosnak találta ezt a videót, tekintse meg a [teljes tanfolyamok kisvállalatoknak és Microsoft 365-újoncoknak](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) című cikket.</span><span class="sxs-lookup"><span data-stu-id="b82c9-111">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a><span data-ttu-id="b82c9-112">Windows 10-es eszközök csatlakoztatása a szervezet Azure AD szolgáltatásához</span><span class="sxs-lookup"><span data-stu-id="b82c9-112">Join Windows 10 devices to your organization's Azure AD</span></span>

<span data-ttu-id="b82c9-113">Ha a szervezet minden Windows-eszköze frissítve lett a Windows 10-es Pro-készítők frissítésére, vagy már Windows 10-es Pro Creators frissítést futtat, ezek az eszközök a szervezet Azure Active Directoryhoz is bekapcsolódnak.</span><span class="sxs-lookup"><span data-stu-id="b82c9-113">When all Windows devices in your organization have either been upgraded to Windows 10 Pro Creators Update or are already running Windows 10 Pro Creators Update, you can join these devices to your organization's Azure Active Directory.</span></span> <span data-ttu-id="b82c9-114">Az eszközök csatlakoztatása után a rendszer automatikusan frissíti őket a Windows 10 Business verzióra, amely része a Microsoft 365 vállalati prémium verziós előfizetésnek.</span><span class="sxs-lookup"><span data-stu-id="b82c9-114">Once the devices are joined, they'll be automatically upgraded to Windows 10 Business, which is part of your Microsoft 365 Business Premium subscription.</span></span>
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a><span data-ttu-id="b82c9-115">Vadonatúj vagy újonnan frissített Windows 10 Pro-eszköz esetén</span><span class="sxs-lookup"><span data-stu-id="b82c9-115">For a brand new, or newly upgraded, Windows 10 Pro device</span></span>

<span data-ttu-id="b82c9-116">A Windows 10 Pro alkotói frissítését futtató vadonatúj eszköz, illetve egy olyan eszköz esetén, amely frissítve lett ugyan a Windows 10 Pro alkotói frissítésére, de még nem lett elvégezve rajta a Windows 10-es eszköz beállítása, kövesse az alábbi lépéseket.</span><span class="sxs-lookup"><span data-stu-id="b82c9-116">For a brand new device running Windows 10 Pro Creators Update, or for a device that was upgraded to Windows 10 Pro Creators Update but has not gone through Windows 10 device setup, follow these steps.</span></span>
  
1. <span data-ttu-id="b82c9-117">Kezdje meg a Windows 10-es eszköz beállítását, amíg a **Hogyan szeretné beállítani?** lapra nem jut.</span><span class="sxs-lookup"><span data-stu-id="b82c9-117">Go through Windows 10 device setup until you get to the **How would you like to set up?** page.</span></span> 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. <span data-ttu-id="b82c9-119">Itt válassza a **beállítás szervezethez** lehetőséget, majd adja meg a Microsoft 365 vállalati prémium verzió felhasználónevét és jelszavát.</span><span class="sxs-lookup"><span data-stu-id="b82c9-119">Here, choose **Set up for an organization** and then enter your username and password for Microsoft 365 Business Premium.</span></span> 
    
3. <span data-ttu-id="b82c9-120">Fejezze be a Windows 10-es eszköz beállítását.</span><span class="sxs-lookup"><span data-stu-id="b82c9-120">Finish Windows 10 device setup.</span></span>
    
   <span data-ttu-id="b82c9-p103">Ha végzett, a felhasználó csatlakoztatva lesz a szervezet Azure AD szolgáltatásához. Ha meg szeretne győződni arról, hogy sikerült-e a csatlakoztatás, olvassa el az [Annak ellenőrzése, hogy az eszköz csatlakoztatva van-e az Azure AD szolgáltatáshoz](#verify-the-device-is-connected-to-azure-ad) című szakaszt.</span><span class="sxs-lookup"><span data-stu-id="b82c9-p103">Once you're done, the user will be connected to your organization's Azure AD. See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to make sure.</span></span> 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a><span data-ttu-id="b82c9-123">Már beállított és a Windows 10 Prót futtató eszköz esetén</span><span class="sxs-lookup"><span data-stu-id="b82c9-123">For a device already set up and running Windows 10 Pro</span></span>

 <span data-ttu-id="b82c9-124">**Felhasználók csatlakoztatása az Azure AD-hez:**</span><span class="sxs-lookup"><span data-stu-id="b82c9-124">**Connect users to Azure AD:**</span></span>
  
1. <span data-ttu-id="b82c9-125">A felhasználó Windows rendszerű PC-jén, amelyen a Windows 10 Pro 1703-as verziója (alkotói frissítés) fut (lásd [előfeltételek](pre-requisites-for-data-protection.md)), kattintson a Windows emblémára, majd a Beállítások ikonra.</span><span class="sxs-lookup"><span data-stu-id="b82c9-125">In your user's Windows PC, that is running Windows 10 Pro, version 1703 (Creators Update) (see [pre-requisites](pre-requisites-for-data-protection.md)), click the Windows logo, and then the Settings icon.</span></span>
  
   ![In the Start menu, click Windows Settings icon](../media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. <span data-ttu-id="b82c9-127">A **Beállítások** lapon válassza a **Fiókok** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b82c9-127">In **Settings** , go to **Accounts**.</span></span>
  
   ![In Windows Settings, go to Accounts](../media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. <span data-ttu-id="b82c9-129">**Az Ön adatai** lapon kattintson a **Hozzáférés munkahelyi vagy iskolai rendszerhez** \> **Csatlakozás** elemre.</span><span class="sxs-lookup"><span data-stu-id="b82c9-129">On **Your info** page, click **Access work or school** \> **Connect**.</span></span>
  
   ![Choose Connect under Access work or school](../media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. <span data-ttu-id="b82c9-131">A **Munkahelyi vagy iskolai fiók beállítása** párbeszédpanel **Más műveletek** csoportjában válassza **Az eszköz csatlakoztatása az Azure Active Directoryhoz** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b82c9-131">On the **Set up a work or school account** dialog, under **Alternate actions** , choose **Join this device to Azure Active Directory**.</span></span>
  
   ![Click Join this device to Azure Active Directory](../media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. <span data-ttu-id="b82c9-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span><span class="sxs-lookup"><span data-stu-id="b82c9-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span></span>
  
   <span data-ttu-id="b82c9-134">On the **Enter password** page, enter your password \> **Sign in**.</span><span class="sxs-lookup"><span data-stu-id="b82c9-134">On the **Enter password** page, enter your password \> **Sign in**.</span></span>
  
   ![Enter your work or school email on the Let's get you signed in page](../media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. <span data-ttu-id="b82c9-136">A győződjön meg arról, hogy **Ez a szervezet** lapja, ellenőrizze, hogy az adatok helyesek-e, és válassza a **Csatlakozás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b82c9-136">On the **Make sure this is your organization** page, verify that the information is correct, and choose **Join**.</span></span>
  
   <span data-ttu-id="b82c9-137">A minden készen áll **!**</span><span class="sxs-lookup"><span data-stu-id="b82c9-137">On the **You're all set!**</span></span> <span data-ttu-id="b82c9-138">Lap, válasszon másikat **végzett**.</span><span class="sxs-lookup"><span data-stu-id="b82c9-138">page, chosse **Done**.</span></span>
  
   ![A győződjön meg róla, hogy a szervezet képernyőjén van, válassza a csatlakozás lehetőséget.](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
<span data-ttu-id="b82c9-140">Szinkronizálja újból a OneDrive Vállalati verzióba esetleg feltöltött fájlokat.</span><span class="sxs-lookup"><span data-stu-id="b82c9-140">If you uploaded files to OneDrive for Business, sync them back down.</span></span> <span data-ttu-id="b82c9-141">Ha harmadik féltől származó eszközt használ a profil és a fájlok áttelepítéséhez, az új profilba is szinkronizálja őket.</span><span class="sxs-lookup"><span data-stu-id="b82c9-141">If you used a third-party tool to migrate profile and files, also sync those to the new profile.</span></span>
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a><span data-ttu-id="b82c9-142">Annak ellenőrzése, hogy az eszköz csatlakoztatva van-e az Azure AD szolgáltatáshoz</span><span class="sxs-lookup"><span data-stu-id="b82c9-142">Verify the device is connected to Azure AD</span></span>

<span data-ttu-id="b82c9-143">A szinkronizálás állapotának ellenőrzéséhez a **beállításokban** a **hozzáférés munkahelyi vagy iskolai** lapján jelölje be a **kapcsolat** _ \<organization name\> _ területhez választógombot, és válassza ki a gombok **adatait** , majd **válassza a leválasztás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b82c9-143">To verify your sync status, on the **Access work or school** page in **Settings** , select the **Connected to** _ \<organization name\> _ area to expose the buttons **Info** and **Disconnect**.</span></span> <span data-ttu-id="b82c9-144">A szinkronizálási állapot eléréséhez válassza az **információ** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b82c9-144">Choose **Info** to get your synchronization status.</span></span> 
  
<span data-ttu-id="b82c9-145">A **szinkronizálás állapota** lapon a **szinkronizálás** gombra koppintva nyissa meg a legújabb mobileszköz-kezelési házirendeket a PC-re.</span><span class="sxs-lookup"><span data-stu-id="b82c9-145">On the **Sync status** page, choose **Sync** to get the latest mobile device management policies onto the PC.</span></span>
  
<span data-ttu-id="b82c9-146">A Microsoft 365 vállalati prémium verzió használatának megkezdéséhez lépjen a Windows **Start** gombjára, kattintson a jobb gombbal az aktuális fiók képére, és válassza a **fiók váltása** parancsot.</span><span class="sxs-lookup"><span data-stu-id="b82c9-146">To start using the Microsoft 365 Business Premium account, go to the Windows **Start** button, right-click your current account picture, and then **Switch account**.</span></span> <span data-ttu-id="b82c9-147">Jelentkezzen be a szervezeti e-mail-címével és jelszavával.</span><span class="sxs-lookup"><span data-stu-id="b82c9-147">Sign in by using your organization email and password.</span></span>
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-pc-is-upgraded-to-windows-10-business"></a><span data-ttu-id="b82c9-149">Annak ellenőrzése, hogy a számítógép frissítve lett-e a Windows 10 Business verzióra</span><span class="sxs-lookup"><span data-stu-id="b82c9-149">Verify the PC is upgraded to Windows 10 Business</span></span>

<span data-ttu-id="b82c9-150">Győződjön meg arról, hogy a Microsoft 365 vállalati prémium verzióra szóló előfizetése részeként az Azure AD csatlakozik Windows 10-es eszközeit a Windows 10 Business verzióra frissítette.</span><span class="sxs-lookup"><span data-stu-id="b82c9-150">Verify that your Azure AD joined Windows 10 devices are upgraded to Windows 10 Business as part of your Microsoft 365 Business Premium subscription.</span></span>
  
1. <span data-ttu-id="b82c9-151">Válassza a **Beállítások** \> **Rendszer** \> **Névjegy** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b82c9-151">Go to **Settings** \> **System** \> **About**.</span></span>
    
2. <span data-ttu-id="b82c9-152">Győződjön meg arról, hogy a **Kiadás** feliratnál a **Windows 10 Business** terméknév szerepel.</span><span class="sxs-lookup"><span data-stu-id="b82c9-152">Confirm that the **Edition** shows **Windows 10 Business**.</span></span>
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a><span data-ttu-id="b82c9-154">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="b82c9-154">Next steps</span></span>

<span data-ttu-id="b82c9-155">A mobileszközök beállításáról a [mobileszközök beállítása a microsoft 365 vállalati prémium verzió felhasználóinak](set-up-mobile-devices.md)című témakörben olvashat a [Microsoft 365 vállalati verzió kezelése](manage.md)című témakörben.</span><span class="sxs-lookup"><span data-stu-id="b82c9-155">To set up your mobile devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md), To set device protection or app protection policies, see [Manage Microsoft 365 for business](manage.md).</span></span>
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a><span data-ttu-id="b82c9-156">További információ a Microsoft 365 Business Premium beállításáról és használatáról</span><span class="sxs-lookup"><span data-stu-id="b82c9-156">For more on setting up and using Microsoft 365 Business Premium</span></span>

[<span data-ttu-id="b82c9-157">Microsoft 365 vállalati verziós képzési videók</span><span class="sxs-lookup"><span data-stu-id="b82c9-157">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)

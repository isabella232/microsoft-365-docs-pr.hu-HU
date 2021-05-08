---
title: Az eszköz Windows beállítása a Microsoft 365 Vállalati prémium verzió számára
f1.keywords:
- CSH
ms.author: sharik
author: skjerland
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
- okr_smb
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: Megtudhatja, hogy miként állíthatja Windows a Windows 10 Pro-et futtató Microsoft 365 Vállalati prémium verzió központi felügyelet és biztonsági vezérlők engedélyezésével.
ms.openlocfilehash: 3e268d81ff6fb7113b7e0b0fe5d0545ff5c72b1e
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52244776"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a><span data-ttu-id="d8596-103">Az eszköz Windows beállítása a Microsoft 365 Vállalati prémium verzió számára</span><span class="sxs-lookup"><span data-stu-id="d8596-103">Set up Windows devices for Microsoft 365 Business Premium users</span></span>

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-premium-users"></a><span data-ttu-id="d8596-104">A mobileszközök beállításának előfeltételei Windows felhasználóknak Microsoft 365 Vállalati prémium verzió számára</span><span class="sxs-lookup"><span data-stu-id="d8596-104">Prerequisites for setting up Windows devices for Microsoft 365 Business Premium users</span></span>

<span data-ttu-id="d8596-105">Mielőtt Windows eszközét Microsoft 365 Vállalati prémium verzió, győződjön meg arról, hogy az összes Windows-eszközön az 1703-as verzió (alkotói frissítés) Windows 10 Pro fut.</span><span class="sxs-lookup"><span data-stu-id="d8596-105">Before you can set up Windows devices for Microsoft 365 Business Premium users, make sure all the Windows devices are running Windows 10 Pro, version 1703 (Creators Update).</span></span> <span data-ttu-id="d8596-106">Windows 10 Pro a Windows 10 Business üzembe helyezésének előfeltétele, amely a Windows 10 Pro-et kiegészítő felhőalapú szolgáltatások és eszközkezelési képességek készlete, amely lehetővé teszi az Microsoft 365 Vállalati prémium verzió központi felügyeletét és Microsoft 365 Vállalati prémium verzió.</span><span class="sxs-lookup"><span data-stu-id="d8596-106">Windows 10 Pro is a prerequisite for deploying Windows 10 Business, which is a set of cloud services and device management capabilities that complement Windows 10 Pro and enable the centralized management and security controls of Microsoft 365 Business Premium.</span></span>
  
<span data-ttu-id="d8596-107">Ha 7 Pro, Windows 8 Pro vagy Windows 8.1 Pro-t futtató Windows Windows-es eszközével rendelkezik, az Microsoft 365 Vállalati prémium verzió-előfizetés feljogosítja a Windows 10 frissítésére.</span><span class="sxs-lookup"><span data-stu-id="d8596-107">If you have Windows devices running Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your Microsoft 365 Business Premium subscription entitles you to a Windows 10 upgrade.</span></span>
  
<span data-ttu-id="d8596-108">Ha többet szeretne megtudni arról, hogy hogyan frissítheti Windows-eszközeit a Windows 10 Pro alkotói frissítésére, kövesse a következő témakörben szereplő lépéseket: [Windows-eszközök frissítése a Windows Pro alkotói frissítésére](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="d8596-108">For more information on how to upgrade Windows devices to Windows 10 Pro Creators Update, follow the steps in this topic: [Upgrade Windows devices to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
  
<span data-ttu-id="d8596-109">Az [Annak ellenőrzése, hogy az eszköz](#verify-the-device-is-connected-to-azure-ad) csatlakoztatva van-e az Azure AD szolgáltatáshoz? vagy a frissítés megfelelő voltának ellenőrzéséhez lásd: Az eszköz csatlakoztatva van az Azure AD szolgáltatáshoz.</span><span class="sxs-lookup"><span data-stu-id="d8596-109">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to verify you have the upgrade, or to make sure the upgrade worked.</span></span>

<span data-ttu-id="d8596-110">Tekintsen meg egy rövid videót arról, hogy hogyan Windows a Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d8596-110">Watch a short video about connecting Windows to Microsoft 365.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

<span data-ttu-id="d8596-111">Ha hasznosnak találta ezt a videót, tekintse meg a [teljes tanfolyamok kisvállalatoknak és Microsoft 365-újoncoknak](../business-video/index.yml) című cikket.</span><span class="sxs-lookup"><span data-stu-id="d8596-111">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](../business-video/index.yml).</span></span>
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a><span data-ttu-id="d8596-112">Windows 10-es eszközök csatlakoztatása a szervezet Azure AD szolgáltatásához</span><span class="sxs-lookup"><span data-stu-id="d8596-112">Join Windows 10 devices to your organization's Azure AD</span></span>

<span data-ttu-id="d8596-113">Ha a Windows összes eszközét frissítette az Windows 10 Pro alkotói frissítésre, vagy már futtatja az Windows 10 Pro alkotói frissítést, csatlakozhat ezekhez az eszközökhez a szervezet Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d8596-113">When all Windows devices in your organization have either been upgraded to Windows 10 Pro Creators Update or are already running Windows 10 Pro Creators Update, you can join these devices to your organization's Azure Active Directory.</span></span> <span data-ttu-id="d8596-114">Miután csatlakozott az eszközökhez, a rendszer automatikusan frissíti őket a Windows 10 Business verzióra, amely az Ön Microsoft 365 Vállalati prémium verzió része.</span><span class="sxs-lookup"><span data-stu-id="d8596-114">Once the devices are joined, they'll be automatically upgraded to Windows 10 Business, which is part of your Microsoft 365 Business Premium subscription.</span></span>
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a><span data-ttu-id="d8596-115">Vadonatúj vagy újonnan frissített Windows 10 Pro-eszköz esetén</span><span class="sxs-lookup"><span data-stu-id="d8596-115">For a brand new, or newly upgraded, Windows 10 Pro device</span></span>

<span data-ttu-id="d8596-116">A Windows 10 Pro alkotói frissítését futtató vadonatúj eszköz, illetve egy olyan eszköz esetén, amely frissítve lett ugyan a Windows 10 Pro alkotói frissítésére, de még nem lett elvégezve rajta a Windows 10-es eszköz beállítása, kövesse az alábbi lépéseket.</span><span class="sxs-lookup"><span data-stu-id="d8596-116">For a brand new device running Windows 10 Pro Creators Update, or for a device that was upgraded to Windows 10 Pro Creators Update but has not gone through Windows 10 device setup, follow these steps.</span></span>
  
1. <span data-ttu-id="d8596-117">Kezdje meg a Windows 10-es eszköz beállítását, amíg a **Hogyan szeretné beállítani?** lapra nem jut.</span><span class="sxs-lookup"><span data-stu-id="d8596-117">Go through Windows 10 device setup until you get to the **How would you like to set up?** page.</span></span> 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. <span data-ttu-id="d8596-119">Itt válassza a **Beállítás szervezet számára lehetőséget,** majd adja meg a szervezethez tartozó felhasználónevét és Microsoft 365 Vállalati prémium verzió.</span><span class="sxs-lookup"><span data-stu-id="d8596-119">Here, choose **Set up for an organization** and then enter your username and password for Microsoft 365 Business Premium.</span></span> 
    
3. <span data-ttu-id="d8596-120">Fejezze be a Windows 10-es eszköz beállítását.</span><span class="sxs-lookup"><span data-stu-id="d8596-120">Finish Windows 10 device setup.</span></span>
    
   <span data-ttu-id="d8596-p103">Ha végzett, a felhasználó csatlakoztatva lesz a szervezet Azure AD szolgáltatásához. Ha meg szeretne győződni arról, hogy sikerült-e a csatlakoztatás, olvassa el az [Annak ellenőrzése, hogy az eszköz csatlakoztatva van-e az Azure AD szolgáltatáshoz](#verify-the-device-is-connected-to-azure-ad) című szakaszt.</span><span class="sxs-lookup"><span data-stu-id="d8596-p103">Once you're done, the user will be connected to your organization's Azure AD. See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to make sure.</span></span> 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a><span data-ttu-id="d8596-123">Már beállított és a Windows 10 Prót futtató eszköz esetén</span><span class="sxs-lookup"><span data-stu-id="d8596-123">For a device already set up and running Windows 10 Pro</span></span>

 <span data-ttu-id="d8596-124">**Felhasználók csatlakoztatása az Azure AD-hez:**</span><span class="sxs-lookup"><span data-stu-id="d8596-124">**Connect users to Azure AD:**</span></span>
  
1. <span data-ttu-id="d8596-125">A felhasználó Windows rendszerű PC-jén, amelyen a Windows 10 Pro 1703-as verziója (alkotói frissítés) fut (lásd [előfeltételek](pre-requisites-for-data-protection.md)), kattintson a Windows emblémára, majd a Beállítások ikonra.</span><span class="sxs-lookup"><span data-stu-id="d8596-125">In your user's Windows PC, that is running Windows 10 Pro, version 1703 (Creators Update) (see [pre-requisites](pre-requisites-for-data-protection.md)), click the Windows logo, and then the Settings icon.</span></span>
  
   ![In the Start menu, click Windows Settings icon](../media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. <span data-ttu-id="d8596-127">A **Beállítások** lapon válassza a **Fiókok** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="d8596-127">In **Settings**, go to **Accounts**.</span></span>
  
   ![In Windows Settings, go to Accounts](../media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. <span data-ttu-id="d8596-129">**Az Ön adatai** lapon kattintson a **Hozzáférés munkahelyi vagy iskolai rendszerhez** \> **Csatlakozás** elemre.</span><span class="sxs-lookup"><span data-stu-id="d8596-129">On **Your info** page, click **Access work or school** \> **Connect**.</span></span>
  
   ![Choose Connect under Access work or school](../media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. <span data-ttu-id="d8596-131">A **Munkahelyi vagy iskolai fiók beállítása** párbeszédpanel **Más műveletek** csoportjában válassza **Az eszköz csatlakoztatása az Azure Active Directoryhoz** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="d8596-131">On the **Set up a work or school account** dialog, under **Alternate actions**, choose **Join this device to Azure Active Directory**.</span></span>
  
   ![Click Join this device to Azure Active Directory](../media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. <span data-ttu-id="d8596-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span><span class="sxs-lookup"><span data-stu-id="d8596-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span></span>
  
   <span data-ttu-id="d8596-134">On the **Enter password** page, enter your password \> **Sign in**.</span><span class="sxs-lookup"><span data-stu-id="d8596-134">On the **Enter password** page, enter your password \> **Sign in**.</span></span>
  
   ![Enter your work or school email on the Let's get you signed in page](../media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. <span data-ttu-id="d8596-136">Az **Ez az Ön szervezete?** lapon ellenőrizze, hogy helyesek-e az adatok, és válassza a Csatlakozás **gombot.**</span><span class="sxs-lookup"><span data-stu-id="d8596-136">On the **Make sure this is your organization** page, verify that the information is correct, and choose **Join**.</span></span>
  
   <span data-ttu-id="d8596-137">A **Minden beállítás meg van állítva!**</span><span class="sxs-lookup"><span data-stu-id="d8596-137">On the **You're all set!**</span></span> <span data-ttu-id="d8596-138">lap, **ékes** Kész .</span><span class="sxs-lookup"><span data-stu-id="d8596-138">page, chosse **Done**.</span></span>
  
   ![A Legyen ez az Ön szervezete képernyőn válassza a Csatlakozás gombot.](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
<span data-ttu-id="d8596-140">Szinkronizálja újból a OneDrive Vállalati verzióba esetleg feltöltött fájlokat.</span><span class="sxs-lookup"><span data-stu-id="d8596-140">If you uploaded files to OneDrive for Business, sync them back down.</span></span> <span data-ttu-id="d8596-141">Ha egy külső eszközt használt a profil és a fájlok áttelepítéséhez, azokat is szinkronizálja az új profilba.</span><span class="sxs-lookup"><span data-stu-id="d8596-141">If you used a third-party tool to migrate profile and files, also sync those to the new profile.</span></span>
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a><span data-ttu-id="d8596-142">Annak ellenőrzése, hogy az eszköz csatlakoztatva van-e az Azure AD szolgáltatáshoz</span><span class="sxs-lookup"><span data-stu-id="d8596-142">Verify the device is connected to Azure AD</span></span>

<span data-ttu-id="d8596-143">A szinkronizálási állapot ellenőrzéséhez az Access munkahelyi vagy iskolai Gépház **területén** válassza a Csatlakoztatva **_** _ terület lehetőséget az Információ és a Kapcsolat bontása gomb  \<organization name\> **eléréséhez.** </span><span class="sxs-lookup"><span data-stu-id="d8596-143">To verify your sync status, on the **Access work or school** page in **Settings**, select the **Connected to** _ \<organization name\> _ area to expose the buttons **Info** and **Disconnect**.</span></span> <span data-ttu-id="d8596-144">Az **Információ lehetőséget** választva lekérte a szinkronizálás állapotát.</span><span class="sxs-lookup"><span data-stu-id="d8596-144">Choose **Info** to get your synchronization status.</span></span> 
  
<span data-ttu-id="d8596-145">A Szinkronizálás **állapota** lapon  a Szinkronizálás lehetőséget választva szerezze be a legújabb mobileszköz-kezelési házirendeket a pc-re.</span><span class="sxs-lookup"><span data-stu-id="d8596-145">On the **Sync status** page, choose **Sync** to get the latest mobile device management policies onto the PC.</span></span>
  
<span data-ttu-id="d8596-146">A fiók használatának Microsoft 365 Vállalati prémium verzió kattintson a Windows **Start** gombra, kattintson a jobb gombbal az aktuális fiókképre, és válassza a **Fiókváltás gombra.**</span><span class="sxs-lookup"><span data-stu-id="d8596-146">To start using the Microsoft 365 Business Premium account, go to the Windows **Start** button, right-click your current account picture, and then **Switch account**.</span></span> <span data-ttu-id="d8596-147">Jelentkezzen be a szervezeti e-mail-címével és jelszavával.</span><span class="sxs-lookup"><span data-stu-id="d8596-147">Sign in by using your organization email and password.</span></span>
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-pc-is-upgraded-to-windows-10-business"></a><span data-ttu-id="d8596-149">Ellenőrizze, hogy a számítógép frissítve van-e Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="d8596-149">Verify the PC is upgraded to Windows 10 Business</span></span>

<span data-ttu-id="d8596-150">Ellenőrizze, hogy az Azure AD-hez Windows 10 eszközén a Windows 10 Business előfizetése részeként Microsoft 365 Vállalati prémium verzió-e.</span><span class="sxs-lookup"><span data-stu-id="d8596-150">Verify that your Azure AD joined Windows 10 devices are upgraded to Windows 10 Business as part of your Microsoft 365 Business Premium subscription.</span></span>
  
1. <span data-ttu-id="d8596-151">Válassza a **Beállítások** \> **Rendszer** \> **Névjegy** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="d8596-151">Go to **Settings** \> **System** \> **About**.</span></span>
    
2. <span data-ttu-id="d8596-152">Győződjön meg arról, hogy a **Kiadás** feliratnál a **Windows 10 Business** terméknév szerepel.</span><span class="sxs-lookup"><span data-stu-id="d8596-152">Confirm that the **Edition** shows **Windows 10 Business**.</span></span>
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a><span data-ttu-id="d8596-154">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="d8596-154">Next steps</span></span>

<span data-ttu-id="d8596-155">A mobileszközök beállításához lásd: Mobileszközök beállítása Microsoft 365 Vállalati prémium verzió [felhasználóknak](set-up-mobile-devices.md), eszközvédelmi és alkalmazásvédelmi házirendek beállításához lásd: Vállalati Microsoft 365 [kezelése.](manage.md)</span><span class="sxs-lookup"><span data-stu-id="d8596-155">To set up your mobile devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md), To set device protection or app protection policies, see [Manage Microsoft 365 for business](manage.md).</span></span>
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a><span data-ttu-id="d8596-156">További információ a beállításokról és a Microsoft 365 Vállalati prémium verzió</span><span class="sxs-lookup"><span data-stu-id="d8596-156">For more on setting up and using Microsoft 365 Business Premium</span></span>

[<span data-ttu-id="d8596-157">Microsoft 365 vállalati verziós oktatóvideók</span><span class="sxs-lookup"><span data-stu-id="d8596-157">Microsoft 365 for business training videos</span></span>](../business-video/index.yml)

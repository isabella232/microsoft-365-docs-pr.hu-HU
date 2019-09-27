---
title: Windows rendszerű eszközök beállítása a Microsoft 365 Business felhasználóinak
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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: 'Útmutató a Windows 10 Pro és a Microsoft 365 üzleti felhasználók számára működő Windows-eszközök beállításához. '
ms.openlocfilehash: c4edd09d952ed1c98be8f41f6bcbaff8a16319a7
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288475"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-users"></a><span data-ttu-id="a5774-103">Windows rendszerű eszközök beállítása a Microsoft 365 Business felhasználóinak</span><span class="sxs-lookup"><span data-stu-id="a5774-103">Set up Windows devices for Microsoft 365 Business users</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5774-104">Előfeltételek</span><span class="sxs-lookup"><span data-stu-id="a5774-104">Prerequisites</span></span>

<span data-ttu-id="a5774-p101">Mielőtt beállítaná a Windows-eszközöket a Microsoft 365 Business felhasználóinál, győződjön meg arról, hogy az összes Windows-eszközön a Windows 10 Pro 1703-as verziója (alkotói frissítés) fut. A Windows 10 Pro megléte előfeltétele a Windows 10 Business üzembe helyezésének, amely a Windows 10 Prót kiegészítő felhőszolgáltatásokat és eszközkezelési lehetőségeket tartalmaz, és lehetővé teszi a Microsoft 365 Business központi kezelését és biztonsági szabályozását.</span><span class="sxs-lookup"><span data-stu-id="a5774-p101">Before you can set up Windows devices for Microsoft 365 Business users, make sure all the Windows devices are running Windows 10 Pro, version 1703 (Creators Update). Windows 10 Pro is a prerequisite for deploying Windows 10 Business, which is a set of cloud services and device management capabilities that complement Windows 10 Pro and enable the centralized management and security controls of Microsoft 365 Business.</span></span>
  
<span data-ttu-id="a5774-107">Ha Ön Windows 7 Pro, Windows 8 Pro vagy Windows 8.1 Pro rendszerű Windows-eszközökkel rendelkezik, akkor Microsoft 365 Business-előfizetése feljogosítja a Windows 10-re való frissítésre.</span><span class="sxs-lookup"><span data-stu-id="a5774-107">If you have Windows devices running Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your Microsoft 365 Business subscription entitles you to a Windows 10 upgrade.</span></span>
  
<span data-ttu-id="a5774-108">Ha többet szeretne megtudni arról, hogy hogyan frissítheti Windows-eszközeit a Windows 10 Pro alkotói frissítésére, kövesse a következő témakörben szereplő lépéseket: [Windows-eszközök frissítése a Windows Pro alkotói frissítésére](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="a5774-108">For more information on how to upgrade Windows devices to Windows 10 Pro Creators Update, follow the steps in this topic: [Upgrade Windows devices to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
  
<span data-ttu-id="a5774-109">Lásd: [az eszköz ellenőrzése csatlakoztatva van azúrkék HIRDETÉSRE](#verify-the-device-is-connected-to-azure-ad) , hogy ellenőrizze, rendelkezik-e a frissítéssel, vagy hogy működik-e a frissítés.</span><span class="sxs-lookup"><span data-stu-id="a5774-109">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to verify you have the upgrade, or to make sure the upgrade worked.</span></span> 
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a><span data-ttu-id="a5774-110">Windows 10-es eszközök csatlakoztatása a szervezet Azure AD szolgáltatásához</span><span class="sxs-lookup"><span data-stu-id="a5774-110">Join Windows 10 devices to your organization's Azure AD</span></span>

<span data-ttu-id="a5774-p102">Ha már a szervezet összes Windows-eszköze frissítve lett a Windows 10 Pro alkotói frissítésére, vagy már eleve a Windows 10 Pro alkotói frissítését futtatja, csatlakoztathatja az eszközöket a szervezet Azure Active Directory szolgáltatásához. A csatlakoztatott eszközök automatikusan a Windows 10 Business verzióra frissülnek, amely része a Microsoft 365 Business-előfizetésnek.</span><span class="sxs-lookup"><span data-stu-id="a5774-p102">Once all Windows devices in your organization have either been upgraded to Windows 10 Pro Creators Update or are already running Windows 10 Pro Creators Update, you can join these devices to your organization's Azure Active Directory. Once the devices are joined, they will automatically be upgraded to Windows 10 Business, which is part of your Microsoft 365 Business subscription.</span></span>
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a><span data-ttu-id="a5774-113">Vadonatúj vagy újonnan frissített Windows 10 Pro-eszköz esetén</span><span class="sxs-lookup"><span data-stu-id="a5774-113">For a brand new, or newly upgraded, Windows 10 Pro device</span></span>

<span data-ttu-id="a5774-114">A Windows 10 Pro alkotói frissítését futtató vadonatúj eszköz, illetve egy olyan eszköz esetén, amely frissítve lett ugyan a Windows 10 Pro alkotói frissítésére, de még nem lett elvégezve rajta a Windows 10-es eszköz beállítása, kövesse az alábbi lépéseket.</span><span class="sxs-lookup"><span data-stu-id="a5774-114">For a brand new device running Windows 10 Pro Creators Update, or for a device that was upgraded to Windows 10 Pro Creators Update but has not gone through Windows 10 device setup, follow these steps.</span></span>
  
1. <span data-ttu-id="a5774-115">Kezdje meg a Windows 10-es eszköz beállítását, amíg a **Hogyan szeretné beállítani?** lapra nem jut.</span><span class="sxs-lookup"><span data-stu-id="a5774-115">Go through Windows 10 device setup until you get to the **How would you like to set up?** page.</span></span> 
    
    ![On the How would you like to set up page, choose Set up for an organization](media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. <span data-ttu-id="a5774-117">Itt válassza a **Beállítás szervezeti használatra** lehetőséget, és adja meg a Microsoft 365 Businesshez használt felhasználónevét és jelszavát.</span><span class="sxs-lookup"><span data-stu-id="a5774-117">Here, choose **Set up for an organization** and then enter your username and password for Microsoft 365 Business.</span></span> 
    
3. <span data-ttu-id="a5774-118">Fejezze be a Windows 10-es eszköz beállítását.</span><span class="sxs-lookup"><span data-stu-id="a5774-118">Finish Windows 10 device setup.</span></span>
    
   <span data-ttu-id="a5774-p103">Ha végzett, a felhasználó csatlakoztatva lesz a szervezet Azure AD szolgáltatásához. Ha meg szeretne győződni arról, hogy sikerült-e a csatlakoztatás, olvassa el az [Annak ellenőrzése, hogy az eszköz csatlakoztatva van-e az Azure AD szolgáltatáshoz](#verify-the-device-is-connected-to-azure-ad) című szakaszt.</span><span class="sxs-lookup"><span data-stu-id="a5774-p103">Once you're done, the user will be connected to your organization's Azure AD. See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to make sure.</span></span> 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a><span data-ttu-id="a5774-121">Már beállított és a Windows 10 Prót futtató eszköz esetén</span><span class="sxs-lookup"><span data-stu-id="a5774-121">For a device already set up and running Windows 10 Pro</span></span>

 <span data-ttu-id="a5774-122">**Felhasználók csatlakoztatása az Azure AD-hez:**</span><span class="sxs-lookup"><span data-stu-id="a5774-122">**Connect users to Azure AD:**</span></span>
  
1. <span data-ttu-id="a5774-123">A felhasználó Windows rendszerű PC-jén, amelyen a Windows 10 Pro 1703-as verziója (alkotói frissítés) fut (lásd [előfeltételek](pre-requisites-for-data-protection.md)), kattintson a Windows emblémára, majd a Beállítások ikonra.</span><span class="sxs-lookup"><span data-stu-id="a5774-123">In your user's Windows PC, that is running Windows 10 Pro, version 1703 (Creators Update) (see [pre-requisites](pre-requisites-for-data-protection.md)), click the Windows logo, and then the Settings icon.</span></span>
  
   ![In the Start menu, click Windows Settings icon](media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. <span data-ttu-id="a5774-125">A **Beállítások** lapon válassza a **Fiókok** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="a5774-125">In **Settings**, go to **Accounts**.</span></span>
  
   ![In Windows Settings, go to Accounts](media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. <span data-ttu-id="a5774-127">**Az Ön adatai** lapon kattintson a **Hozzáférés munkahelyi vagy iskolai rendszerhez** \> **Csatlakozás** elemre.</span><span class="sxs-lookup"><span data-stu-id="a5774-127">On **Your info** page, click **Access work or school** \> **Connect**.</span></span>
  
   ![Choose Connect under Access work or school](media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. <span data-ttu-id="a5774-129">A **Munkahelyi vagy iskolai fiók beállítása** párbeszédpanel **Más műveletek** csoportjában válassza **Az eszköz csatlakoztatása az Azure Active Directoryhoz** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="a5774-129">On the **Set up a work or school account** dialog, under **Alternate actions**, choose **Join this device to Azure Active Directory**.</span></span>
  
   ![Click Join this device to Azure Active Directory](media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. <span data-ttu-id="a5774-131">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span><span class="sxs-lookup"><span data-stu-id="a5774-131">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span></span>
  
   <span data-ttu-id="a5774-132">On the **Enter password** page, enter your password \> **Sign in**.</span><span class="sxs-lookup"><span data-stu-id="a5774-132">On the **Enter password** page, enter your password \> **Sign in**.</span></span>
  
   ![Enter your work or school email on the Let's get you signed in page](media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. <span data-ttu-id="a5774-134">A győződjön meg róla, hogy **Ez a szervezet** lapja, ellenőrizze, hogy az adatok helyesek-e, majd kattintson a **Csatlakozás**gombra.</span><span class="sxs-lookup"><span data-stu-id="a5774-134">On the **Make sure this is your organization** page, verify that the information is correct, and click **Join**.</span></span>
  
   <span data-ttu-id="a5774-p104">A **Minden készen áll** lapon kattintson a **Kész** elemre.</span><span class="sxs-lookup"><span data-stu-id="a5774-p104">On the **You're all set!** page, click **Done**.</span></span>
  
   ![On the Make sure this is your organization screen, click Join](media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
<span data-ttu-id="a5774-p105">Szinkronizálja újból a OneDrive Vállalati verzióba esetleg feltöltött fájlokat. Ha egy külső eszközt vett igénybe a profil és a fájlok áttelepítéséhez, ezeket is szinkronizálja az új profilba.</span><span class="sxs-lookup"><span data-stu-id="a5774-p105">If you uploaded files to OneDrive for Business, sync them back down. If you used a third party tool to migrate profile and files, sync those also to the new profile.</span></span>
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a><span data-ttu-id="a5774-140">Annak ellenőrzése, hogy az eszköz csatlakoztatva van-e az Azure AD szolgáltatáshoz</span><span class="sxs-lookup"><span data-stu-id="a5774-140">Verify the device is connected to Azure AD</span></span>

<span data-ttu-id="a5774-p106">A szinkronizálási állapot ellenőrzéséhez a **Hozzáférés munkahelyi vagy iskolai rendszerhez** lap **Beállítások** csoportjában kattintson a **Csatlakoztatva** _ \<organization name\> _ területre az **Információ** és a **Leválasztás** gomb megjelenítéséhez. Kattintson az **Információ** gombra a szinkronizálás állapotának megjelenítéséhez.</span><span class="sxs-lookup"><span data-stu-id="a5774-p106">To verify your sync status, on the **Access work or school** page in **Settings**, click in the **Connected to** _ \<organization name\> _ area to expose the buttons **Info** and **Disconnect**. Click on **Info** to get your synchronization status.</span></span> 
  
<span data-ttu-id="a5774-143">A Szinkronizálás állapota lapon a Szinkronizálás elemre kattintva beszerezheti a legújabb mobileszköz-kezelési házirendeket a PC-re.</span><span class="sxs-lookup"><span data-stu-id="a5774-143">On the Sync status page, click Sync to get the latest mobile device management policies onto the PC.</span></span>
  
<span data-ttu-id="a5774-p107">A Microsoft 365 Business-fiók használatának megkezdéséhez kattintson a Windows **Start** gombjára, kattintson a jobb gombbal az aktuális fiókjának a képére, és válassza a **Fiókváltás** parancsot. Jelentkezzen be a szervezeti e-mail-címével és jelszavával.</span><span class="sxs-lookup"><span data-stu-id="a5774-p107">To start using the Microsoft 365 Business account, go to the Windows **Start** button, right-click your current account picture and then **Switch account**. Sign in by using your organization email and password.</span></span>
  
![Click Info button to view synchronization status](media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-device-is-upgraded-to-windows-10-business"></a><span data-ttu-id="a5774-147">Annak ellenőrzése, hogy az eszköz frissítve lett-e a Windows 10 Business verzióra</span><span class="sxs-lookup"><span data-stu-id="a5774-147">Verify the device is upgraded to Windows 10 Business</span></span>

<span data-ttu-id="a5774-148">Ellenőrizheti, hogy megtörtént-e az Azure AD szolgáltatáshoz csatlakoztatott Windows 10-es eszközök frissítése Windows 10 Business verzióra, a Microsoft 365 Business-előfizetése részeként.</span><span class="sxs-lookup"><span data-stu-id="a5774-148">Verify that your Azure AD joined Windows 10 devices were upgraded to Windows 10 Business as part of your Microsoft 365 Business subscription.</span></span>
  
1. <span data-ttu-id="a5774-149">Válassza a **Beállítások** \> **Rendszer** \> **Névjegy** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="a5774-149">Go to **Settings** \> **System** \> **About**.</span></span>
    
2. <span data-ttu-id="a5774-150">Győződjön meg arról, hogy a **Kiadás** feliratnál a **Windows 10 Business** terméknév szerepel.</span><span class="sxs-lookup"><span data-stu-id="a5774-150">Confirm that the **Edition** shows **Windows 10 Business**.</span></span>
    
    ![Verify that Windows edition is Windows 10 Business.](media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a><span data-ttu-id="a5774-152">Következő lépések</span><span class="sxs-lookup"><span data-stu-id="a5774-152">Next steps</span></span>

<span data-ttu-id="a5774-153">A mobileszközök beállításáról a [Mobileszközök beállítása a Microsoft 365 Business felhasználóinak](set-up-mobile-devices.md), az eszközvédelmi vagy appvédelmi beállítások megadásáról pedig [A Microsoft 365 Business kezelése](manage.md) című témakörben tájékozódhat.</span><span class="sxs-lookup"><span data-stu-id="a5774-153">To set up your mobile devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md), To set device protection or app protection policies, see [Manage Microsoft 365 Business](manage.md).</span></span>
  

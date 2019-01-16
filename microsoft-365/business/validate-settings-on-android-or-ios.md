---
title: Android vagy iOS eszközökön app védelmi beállítások ellenőrzése
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: f3433b6b-02f7-447f-9d62-306bf03638b0
description: 'Learn how to validate the Microsoft 365 Business app protection settings in your Android or iOS devices.  '
ms.openlocfilehash: 300f59e81a93cc3dfc03fd1d98891be1ac4f7795
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/16/2019
ms.locfileid: "26983675"
---
# <a name="validate-app-protection-settings-on-android-or-ios-devices"></a><span data-ttu-id="54242-103">Android vagy iOS eszközökön app védelmi beállítások ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="54242-103">Validate app protection settings on Android or iOS devices</span></span>

<span data-ttu-id="54242-104">Kövesse az utasításokat a lapokon Android vagy iOS eszközökön app védelmi beállítások érvényesítése.</span><span class="sxs-lookup"><span data-stu-id="54242-104">Follow the instructions in the tabs to validate app protection settings on Android or iOS devices.</span></span>
  
## <a name="androidtab"></a>[<span data-ttu-id="54242-105">Android</span><span class="sxs-lookup"><span data-stu-id="54242-105">Android</span></span>](#tab/)
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="54242-106">Az appkezelési beállítások működésének ellenőrzése a felhasználói eszközökön</span><span class="sxs-lookup"><span data-stu-id="54242-106">Check that the App protection settings are working on user devices</span></span>

<span data-ttu-id="54242-107">Miután [konfigurálta az Android-eszközök beállításait](app-protection-settings-for-android-and-ios.md) az appok védelmére, az alábbi lépésekkel ellenőrizheti, hogy működnek-e a kiválasztott beállítások.</span><span class="sxs-lookup"><span data-stu-id="54242-107">After you [set app configurations for Android devices](app-protection-settings-for-android-and-ios.md) to protect the apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="54242-108">Elsőként győződjön meg arról, hogy a házirend arra az appra vonatkozik, amelyben az ellenőrzését végezni készül.</span><span class="sxs-lookup"><span data-stu-id="54242-108">First, make sure that the policy applies to the app in which you are going to validate it.</span></span>
  
1. <span data-ttu-id="54242-109">A Microsoft 365 Business [felügyeleti központjában](https://portal.office.com) válassza a **Házirendek** \> **Házirend szerkesztése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="54242-109">In the Microsoft 365 Business [admin center](https://portal.office.com) go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="54242-110">Válassza az **Alkalmazás-házirend Android-eszközökhöz** lehetőséget a telepítéskor létrehozott beállításokhoz, illetve egy másik Ön által létrehozott házirendet, és ellenőrizze, hogy az kényszerítve van-e, például az Outlookhoz.</span><span class="sxs-lookup"><span data-stu-id="54242-110">Choose **Application policy for Android** for the settings you created at setup, or another policy you created, and verify that it is enforced for Outlook for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](media/b3be3ddd-f683-4073-8d7a-9c639a636a2c.png)
  
### <a name="validate-require-a-pin-or-a-fingerprint-to-access-office-apps"></a><span data-ttu-id="54242-112">A „PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez" beállítás ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="54242-112">Validate Require a PIN or a fingerprint to access Office apps</span></span>

<span data-ttu-id="54242-113">A **Házirend szerkesztése** ablaktáblában válassza a **Szerkesztés** elemet az **Office-dokumentumok elérésének szabályozása** elem mellett, bontsa ki az **Office-fájlok felhasználói mobileszközökön történő elérésének felügyelete** csomópontot, és győződjön meg arról, hogy a **PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez** beállítás értéke **Be**.</span><span class="sxs-lookup"><span data-stu-id="54242-113">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Make sure that the Require a PIN or fingerprint to acces Office apps is set to On.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="54242-115">A felhasználó Android-eszközén nyissa meg az Outlookot, és jelentkezzen be a felhasználó Microsoft 365 Businesshez használt hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="54242-115">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="54242-116">A rendszer PIN-kód megadására vagy ujjlenyomat használatára is kérni fogja.</span><span class="sxs-lookup"><span data-stu-id="54242-116">You will also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your Android device to access Office apps.](media/9e8ecfee-8122-4a3a-8918-eece80344310.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="54242-118">A „PIN-kód alaphelyzetbe állítása ennyi sikertelen kísérlet után" beállítás ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="54242-118">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="54242-119">A **Házirend szerkesztése** ablaktáblában válassza a **Szerkesztés** elemet az **Office-dokumentumok elérésének szabályozása** elem mellett, bontsa ki az **Office-fájlok felhasználói mobileszközökön történő elérésének felügyelete** csomópontot, és győződjön meg arról, hogy a **PIN-kód alaphelyzetbe állítása ennyi sikertelen kísérlet után** beállítás értéke egy szám - alapértelmezés szerint 5.</span><span class="sxs-lookup"><span data-stu-id="54242-119">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number - this is 5 by default.</span></span> 
  
1. <span data-ttu-id="54242-120">A felhasználó Android-eszközén nyissa meg az Outlookot, és jelentkezzen be a felhasználó Microsoft 365 Businesshez használt hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="54242-120">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="54242-p101">Írjon be egy helytelen PIN-kódot a házirendben megadott alkalommal. Megjelenik egy üzenet a **Több PIN-kódot már nem adhat meg** szöveggel, amelyen alaphelyzetbe állíthatja a PIN-kódot.</span><span class="sxs-lookup"><span data-stu-id="54242-p101">Enter an incorrect PIN as many times as specified by the policy. You will see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fca6fcb4-bb5c-477f-af5e-5dc937e8b835.png)
  
3. <span data-ttu-id="54242-p102">Válassza a **PIN-kód visszaállítása** elemet. Ekkor a rendszer arra kéri, hogy jelentkezzen be a felhasználó Microsoft 365 Businesshez használt hitelesítő adataival, majd állítson be egy új PIN-kódot.</span><span class="sxs-lookup"><span data-stu-id="54242-p102">Press **Reset PIN**. You will be prompted to sign in with the user's Microsoft 365 Business credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="54242-126">„A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió" beállítás ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="54242-126">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="54242-127">A **Házirend szerkesztése** ablaktáblában válassza a **Szerkesztés** elemet az **Elveszett vagy ellopott eszközök elleni védelem** elem mellett, bontsa ki a **Munkahelyi fájlok védelme az eszköz elvesztése vagy ellopása esetén** csomópontot, és győződjön meg arról, hogy **A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió** beállítás értéke **Be**.</span><span class="sxs-lookup"><span data-stu-id="54242-127">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="54242-129">A felhasználó Android-eszközén nyissa meg az Outlookot, jelentkezzen be a felhasználó Microsoft 365 Businesshez használt hitelesítő adataival, és szükség esetén adja meg a PIN-kódot.</span><span class="sxs-lookup"><span data-stu-id="54242-129">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="54242-130">Nyisson meg egy mellékletet tartalmazó e-mailt, és koppintson a lefelé mutató nyíl ikonra a melléklet adatai mellett.</span><span class="sxs-lookup"><span data-stu-id="54242-130">Open an email that contains an attachment and tap the down arrow icon next to the attachment's information.</span></span>
    
    ![Tap the down arrow next to an attachment to try to save it.](media/b22573bb-91ce-455f-84fa-8feb2846b117.png)
  
    <span data-ttu-id="54242-132">A képernyő alján megjelenik **A fájl nem menthető az eszközre** felirat.</span><span class="sxs-lookup"><span data-stu-id="54242-132">You will see **Cannot save to device** on the bottom of the screen.</span></span> 
    
    ![Warning text that indicates cannot save a file locally to an Android.](media/52ca3f3d-7ed0-4a52-9621-4872da6ea9c5.png)
  
    > [!NOTE]
    > <span data-ttu-id="54242-134">A OneDrive Vállalati verzióba való mentés jelenleg nem engedélyezett az Android rendszerben, így csak annyi látható, hogy a helyi mentés le van tiltva.</span><span class="sxs-lookup"><span data-stu-id="54242-134">Saving to OneDrive for Business is not enabled for Android at this time, so you can only see that saving locally is blocked.</span></span> 
  
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="54242-135">„A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után" beállítás ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="54242-135">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="54242-136">A **Házirend szerkesztése** ablaktáblában válassza a **Szerkesztés** elemet az **Office-dokumentumok elérésének szabályozása** elem mellett, bontsa ki az **Office-fájlok felhasználói mobileszközökön történő elérésének felügyelete** csomópontot, és győződjön meg arról, hogy **A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után** beállítás értéke egy szám - alapértelmezés szerint 30 perc.</span><span class="sxs-lookup"><span data-stu-id="54242-136">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes - this is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="54242-137">A felhasználó Android-eszközén nyissa meg az Outlookot, jelentkezzen be a felhasználó Microsoft 365 Businesshez használt hitelesítő adataival, és szükség esetén adja meg a PIN-kódot.</span><span class="sxs-lookup"><span data-stu-id="54242-137">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="54242-p103">Ekkor megjelenik az Outlook Beérkezett üzenetek mappája. Hagyja az Android-eszközt üresjáratban legalább 30 percig (vagy más időtartamig, az a lényeg, hogy hosszabb legyen a házirendben meghatározottnál). Az eszköz valószínűleg elsötétül.</span><span class="sxs-lookup"><span data-stu-id="54242-p103">You should now see Outlook's inbox. Let the Android device idle untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="54242-141">Nyissa meg újra az Outlookot az Android-eszközön.</span><span class="sxs-lookup"><span data-stu-id="54242-141">Re-access Outlook on the Android device.</span></span>
    
4. <span data-ttu-id="54242-142">A rendszer arra fogja kérni, hogy adja meg a PIN-kódot az Outlook ismételt eléréséhez.</span><span class="sxs-lookup"><span data-stu-id="54242-142">You will be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="54242-143">A „Munkahelyi fájlok védelme titkosítással" beállítás ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="54242-143">Validate Protect work files with encryption</span></span>

<span data-ttu-id="54242-144">A **Házirend szerkesztése** ablaktáblában válassza a **Szerkesztés** elemet az **Elveszett vagy ellopott eszközök elleni védelem** elem mellett, bontsa ki a **Munkahelyi fájlok védelme az eszköz elvesztése vagy ellopása esetén** csomópontot, és győződjön meg arról, hogy a **Munkahelyi fájlok védelme titkosítással** beállítás értéke **Be**, **A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió** beállításé pedig **Ki**.</span><span class="sxs-lookup"><span data-stu-id="54242-144">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="54242-145">A felhasználó Android-eszközén nyissa meg az Outlookot, jelentkezzen be a felhasználó Microsoft 365 Businesshez használt hitelesítő adataival, és szükség esetén adja meg a PIN-kódot.</span><span class="sxs-lookup"><span data-stu-id="54242-145">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="54242-146">Nyisson meg egy olyan e-mailt, amely tartalmaz néhány képfájlt mellékletként.</span><span class="sxs-lookup"><span data-stu-id="54242-146">Open an email which contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="54242-147">Koppintson a lefelé mutató nyílra a melléklet adatai mellett a mentéséhez.</span><span class="sxs-lookup"><span data-stu-id="54242-147">Tap the down arrow icon next to the attachment's info to save it.</span></span>
    
    ![Tap the down arrow to save the figure file to the Android device.](media/08a9e21e-4022-45d5-acff-59cface651e7.png)
  
4. <span data-ttu-id="54242-p104">Ekkor a rendszer arra kérheti, hogy engedélyezze a hozzáférést az Outlooknak a fényképekhez, médiatartalmakhoz és más fájlokhoz. Koppintson az **Engedélyezés** gombra.</span><span class="sxs-lookup"><span data-stu-id="54242-p104">You may be prompted to allow Outlook to access photos, media, and files on your device. Tap **Allow**.</span></span>
    
5. <span data-ttu-id="54242-151">A képernyő alján válassza a **Mentés helye: Eszköz** lehetőséget, majd nyissa meg a **Galéria** appot.</span><span class="sxs-lookup"><span data-stu-id="54242-151">At the bottom of the screen, choose to **Save to Device** and then open the **Gallery** app.</span></span> 
    
6. <span data-ttu-id="54242-p105">A listában látható lehet egy (vagy - ha több, képfájlt tartalmazó mellékletet mentett - több) titkosított fájl. Egy szürke négyzetként jelenhet meg a Képek listában, amelyben középen egy fehér felkiáltójel látható egy fehér körön belül.</span><span class="sxs-lookup"><span data-stu-id="54242-p105">You should see an encrypted photo (or more, if you saved multiple image file attachments) in the list. It may appear in the Pictures list as a gray square with a white exclamation point within a white circle in the center of the gray square.</span></span>
    
    ![An encrypted image file in the Gallery app.](media/25936414-bd7e-421d-824e-6e59b877722d.png)
  
## <a name="iostab"></a>[<span data-ttu-id="54242-155">iOS</span><span class="sxs-lookup"><span data-stu-id="54242-155">iOS</span></span>](#tab/)
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="54242-156">Az appkezelési beállítások működésének ellenőrzése a felhasználói eszközökön</span><span class="sxs-lookup"><span data-stu-id="54242-156">Check that the App protection settings are working on user devices</span></span>

<span data-ttu-id="54242-157">Miután [konfigurálta az iOS-eszközök beállításait](app-protection-settings-for-android-and-ios.md) az appok védelmére, az alábbi lépésekkel ellenőrizheti, hogy működnek-e a kiválasztott beállítások.</span><span class="sxs-lookup"><span data-stu-id="54242-157">After you [set app configurations for iOS devices](app-protection-settings-for-android-and-ios.md) to protect apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="54242-158">Elsőként győződjön meg arról, hogy a házirend arra az appra vonatkozik, amelyben az ellenőrzését végezni készül.</span><span class="sxs-lookup"><span data-stu-id="54242-158">First, make sure that the policy applies to the app in which you are going to validate it.</span></span>
  
1. <span data-ttu-id="54242-159">A Microsoft 365 Business [felügyeleti központjában](https://portal.office.com) válassza a **Házirendek** \> **Házirend szerkesztése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="54242-159">In the Microsoft 365 Business [admin center](https://portal.office.com), go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="54242-160">Válassza az **Alkalmazás-házirend iOS-eszközökhöz** lehetőséget a telepítéskor létrehozott beállításokhoz, illetve egy másik Ön által létrehozott házirendet, és ellenőrizze, hogy az kényszerítve van-e, például az Outlookhoz.</span><span class="sxs-lookup"><span data-stu-id="54242-160">Choose **Application policy for iOS** for the settings you created at setup, or another policy you created, and verify that it is enforced for Outlook for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](media/842441b8-e7b1-4b86-9edd-d94d1f77b6f4.png)
  
### <a name="validate-require-a-pin-to-access-office-apps"></a><span data-ttu-id="54242-162">A „PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez" beállítás ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="54242-162">Validate Require a PIN to access Office apps</span></span>

<span data-ttu-id="54242-163">A **Házirend szerkesztése** ablaktáblában válassza a **Szerkesztés** elemet az **Office-dokumentumok elérésének szabályozása** elem mellett, bontsa ki az **Office-fájlok felhasználói mobileszközökön történő elérésének felügyelete** csomópontot, és győződjön meg arról, hogy a **PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez** beállítás értéke **Be**.</span><span class="sxs-lookup"><span data-stu-id="54242-163">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Make sure that the Require a PIN or fingerprint to acces Office apps is set to On.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="54242-165">A felhasználó iOS-eszközén nyissa meg az Outlookot, és jelentkezzen be a felhasználó Microsoft 365 Businesshez használt hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="54242-165">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="54242-166">A rendszer PIN-kód megadására vagy ujjlenyomat használatára is kérni fogja.</span><span class="sxs-lookup"><span data-stu-id="54242-166">You will also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your IOS device to access Office apps.](media/06fc5cf3-9f19-4090-b23c-14bb59805b7a.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="54242-168">A „PIN-kód alaphelyzetbe állítása ennyi sikertelen kísérlet után" beállítás ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="54242-168">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="54242-169">A **Házirend szerkesztése** ablaktáblában válassza a **Szerkesztés** elemet az **Office-dokumentumok elérésének szabályozása** elem mellett, bontsa ki az **Office-fájlok felhasználói mobileszközökön történő elérésének felügyelete** csomópontot, és győződjön meg arról, hogy a **PIN-kód alaphelyzetbe állítása ennyi sikertelen kísérlet után** beállítás értéke egy szám - alapértelmezés szerint 5.</span><span class="sxs-lookup"><span data-stu-id="54242-169">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number - this is 5 by default.</span></span> 
  
1. <span data-ttu-id="54242-170">A felhasználó iOS-eszközén nyissa meg az Outlookot, és jelentkezzen be a felhasználó Microsoft 365 Businesshez használt hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="54242-170">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="54242-p106">Írjon be egy helytelen PIN-kódot a házirendben megadott alkalommal. Megjelenik egy üzenet a **Több PIN-kódot már nem adhat meg** szöveggel, amelyen alaphelyzetbe állíthatja a PIN-kódot.</span><span class="sxs-lookup"><span data-stu-id="54242-p106">Enter an incorrect PIN as many times as specified by the policy. You will see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fab5c089-a4a5-4e8d-8c95-b8eed1dfa262.png)
  
3. <span data-ttu-id="54242-p107">Válassza az **OK** gombot. Ekkor a rendszer arra kéri, hogy jelentkezzen be a felhasználó Microsoft 365 Businesshez használt hitelesítő adataival, majd állítson be egy új PIN-kódot.</span><span class="sxs-lookup"><span data-stu-id="54242-p107">Press **OK**. You will be prompted to sign in with the user's Microsoft 365 Business credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="54242-176">„A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió" beállítás ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="54242-176">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="54242-177">A **Házirend szerkesztése** ablaktáblában válassza a **Szerkesztés** elemet az **Elveszett vagy ellopott eszközök elleni védelem** elem mellett, bontsa ki a **Munkahelyi fájlok védelme az eszköz elvesztése vagy ellopása esetén** csomópontot, és győződjön meg arról, hogy **A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió** beállítás értéke **Be**.</span><span class="sxs-lookup"><span data-stu-id="54242-177">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="54242-179">A felhasználó iOS-eszközén nyissa meg az Outlookot, jelentkezzen be a felhasználó Microsoft 365 Businesshez használt hitelesítő adataival, és szükség esetén adja meg a PIN-kódot.</span><span class="sxs-lookup"><span data-stu-id="54242-179">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="54242-180">Nyisson meg egy mellékletet tartalmazó e-mailt, nyissa meg a mellékletet, és válassza a **Mentés** elemet a képernyő alján.</span><span class="sxs-lookup"><span data-stu-id="54242-180">Open an email that contains an attachment, open the attachment and choose **Save** on the bottom of the screen.</span></span> 
    
    ![Tap the Save option after you open an attachment to try to save it.](media/b419b070-1530-4f14-86a8-8d89933a2b25.png)
  
3. <span data-ttu-id="54242-p108">Elvileg csak a OneDrive Vállalati verzió beállítás látható. Ha nem így van, koppintson a **Fiók hozzáadása** elemre, és válassza a **OneDrive Vállalati verzió** lehetőséget a **Tárhelyfiók hozzáadása** képernyőn. Amikor szükséges, adja meg a végfelhasználó Microsoft 365 Businesshez használt adatait a bejelentkezéshez.</span><span class="sxs-lookup"><span data-stu-id="54242-p108">You should only see an option for OneDrive for Business. If not If not, tap **Add Account** and select **OneDrive for Business** from the **Add Storage Account** screen. Provide the end user's Microsoft 365 Business to sign in when prompted.</span></span> 
    
    <span data-ttu-id="54242-185">Koppintson a **Mentés** elemre, és válassza a **OneDrive Vállalati verzió** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="54242-185">Tap **Save** and select **OneDrive for Business**.</span></span>
    
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="54242-186">„A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után" beállítás ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="54242-186">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="54242-187">A **Házirend szerkesztése** ablaktáblában válassza a **Szerkesztés** elemet az **Office-dokumentumok elérésének szabályozása** elem mellett, bontsa ki az **Office-fájlok felhasználói mobileszközökön történő elérésének felügyelete** csomópontot, és győződjön meg arról, hogy **A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után** beállítás értéke egy szám - alapértelmezés szerint 30 perc.</span><span class="sxs-lookup"><span data-stu-id="54242-187">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes - this is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="54242-188">A felhasználó iOS-eszközén nyissa meg az Outlookot, jelentkezzen be a felhasználó Microsoft 365 Businesshez használt hitelesítő adataival, és szükség esetén adja meg a PIN-kódot.</span><span class="sxs-lookup"><span data-stu-id="54242-188">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="54242-p109">Ekkor megjelenik az Outlook Beérkezett üzenetek mappája. Hagyja az iOS-eszközt érintetlenül legalább 30 percig (vagy más időtartamig, az a lényeg, hogy hosszabb legyen a házirendben meghatározottnál). Az eszköz valószínűleg elsötétül.</span><span class="sxs-lookup"><span data-stu-id="54242-p109">You should now see Outlook's inbox. Let the iOS device untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="54242-192">Nyissa meg újra az Outlookot az iOS-eszközön.</span><span class="sxs-lookup"><span data-stu-id="54242-192">Re-access Outlook on the iOS device.</span></span>
    
4. <span data-ttu-id="54242-193">A rendszer arra fogja kérni, hogy adja meg a PIN-kódot az Outlook ismételt eléréséhez.</span><span class="sxs-lookup"><span data-stu-id="54242-193">You will be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="54242-194">A „Munkahelyi fájlok védelme titkosítással" beállítás ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="54242-194">Validate Protect work files with encryption</span></span>

<span data-ttu-id="54242-195">A **Házirend szerkesztése** ablaktáblában válassza a **Szerkesztés** elemet az **Elveszett vagy ellopott eszközök elleni védelem** elem mellett, bontsa ki a **Munkahelyi fájlok védelme az eszköz elvesztése vagy ellopása esetén** csomópontot, és győződjön meg arról, hogy a **Munkahelyi fájlok védelme titkosítással** beállítás értéke **Be**, **A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió** beállításé pedig **Ki**.</span><span class="sxs-lookup"><span data-stu-id="54242-195">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="54242-196">A felhasználó iOS-eszközén nyissa meg az Outlookot, jelentkezzen be a felhasználó Microsoft 365 Businesshez használt hitelesítő adataival, és szükség esetén adja meg a PIN-kódot.</span><span class="sxs-lookup"><span data-stu-id="54242-196">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="54242-197">Nyisson meg egy olyan e-mailt, amely tartalmaz néhány képfájlt mellékletként.</span><span class="sxs-lookup"><span data-stu-id="54242-197">Open an email which contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="54242-198">Koppintson a mellékletre, majd alatta a **Mentés** elemre.</span><span class="sxs-lookup"><span data-stu-id="54242-198">Tap the attachment and then tap the **Save** option under it.</span></span> 
    
4. <span data-ttu-id="54242-p110">Nyissa meg a **Fotók** appot a kezdőképernyőről. Ekkor egy (vagy - ha több, képfájlt tartalmazó mellékletet mentett - több) mentett, ám titkosított fényképet kell látnia.</span><span class="sxs-lookup"><span data-stu-id="54242-p110">Open **Photos** app from the home screen. You should see an encrypted photo (or more, if you saved multiple image file attachments) saved, but encrypted.</span></span> 
    
---


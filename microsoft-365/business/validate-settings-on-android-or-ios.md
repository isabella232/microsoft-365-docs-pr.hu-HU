---
title: Appvédelmi beállítások ellenőrzése Android- vagy iOS-eszközökön
f1.keywords:
- NOCSH
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
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: f3433b6b-02f7-447f-9d62-306bf03638b0
description: Megtudhatja, hogy miként ellenőrizheti a Microsoft 365 Vállalati prémium verzió appvédelmi beállításait Android- vagy iOS-eszközein.
ms.openlocfilehash: d4b8ec3ff3a15c25133b20d437249611530977a5
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403370"
---
# <a name="validate-app-protection-settings-on-android-or-ios-devices"></a><span data-ttu-id="bcfe8-103">Appvédelmi beállítások ellenőrzése Android- vagy iOS-eszközökön</span><span class="sxs-lookup"><span data-stu-id="bcfe8-103">Validate app protection settings on Android or iOS devices</span></span>

<span data-ttu-id="bcfe8-104">Az alábbi szakaszokban található utasításokat követve érvényesítheti az appvédelmi beállításokat Android- vagy iOS-eszközökön.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-104">Follow the instructions in the following sections to validate app protection settings on Android or iOS devices.</span></span>
  
## <a name="android"></a><span data-ttu-id="bcfe8-105">Android</span><span class="sxs-lookup"><span data-stu-id="bcfe8-105">Android</span></span>
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="bcfe8-106">Annak ellenőrzése, hogy működnek-e az appvédelmi beállítások a felhasználói eszközökön</span><span class="sxs-lookup"><span data-stu-id="bcfe8-106">Check that the app protection settings are working on user devices</span></span>

<span data-ttu-id="bcfe8-107">Miután [konfigurálta az Android-eszközök beállításait](app-protection-settings-for-android-and-ios.md) az appok védelmére, az alábbi lépésekkel ellenőrizheti, hogy működnek-e a kiválasztott beállítások.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-107">After you [set app configurations for Android devices](app-protection-settings-for-android-and-ios.md) to protect the apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="bcfe8-108">Először győződjön meg arról, hogy a házirend arra az appra vonatkozik, amelyben érvényesíteni fogja azt.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-108">First, make sure that the policy applies to the app in which you're going to validate it.</span></span>
  
1. <span data-ttu-id="bcfe8-109">A Microsoft 365 Vállalati prémium verzió [felügyeleti](https://portal.office.com)központjában kattintson a **Házirendek** szerkesztése \> **házirendre.**</span><span class="sxs-lookup"><span data-stu-id="bcfe8-109">In the Microsoft 365 Business Premium [admin center](https://portal.office.com), go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="bcfe8-110">Válassza **az Android** alkalmazás-házirendet a beállításkor létrehozott beállításokhoz, vagy egy másik, Ön által létrehozott házirendet, és ellenőrizze, hogy az kényszerítve van-e az Outlookban.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-110">Choose **Application policy for Android** for the settings you created at setup, or another policy you created, and verify that it's enforced for Outlook, for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](../media/b3be3ddd-f683-4073-8d7a-9c639a636a2c.png)
  
### <a name="validate-require-a-pin-or-a-fingerprint-to-access-office-apps"></a><span data-ttu-id="bcfe8-112">A „PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez" beállítás ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="bcfe8-112">Validate Require a PIN or a fingerprint to access Office apps</span></span>

<span data-ttu-id="bcfe8-113">A **Házirend szerkesztése** ablaktáblában válassza a **Szerkesztés** elemet az **Office-dokumentumok elérésének szabályozása** elem mellett, bontsa ki az **Office-fájlok felhasználói mobileszközökön történő elérésének felügyelete** csomópontot, és győződjön meg arról, hogy a **PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez** beállítás értéke **Be**.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-113">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Győződjön meg arról, hogy a PIN-kód vagy ujjlenyomat megkövetelve az Office-appok eléréséhez be van állítva.](../media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="bcfe8-115">A felhasználó Android-eszközén nyissa meg az Outlookot, és jelentkezzen be a felhasználó Microsoft 365 Vállalati prémium verziós hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-115">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="bcfe8-116">A rendszer PIN-kód beíratára vagy ujjlenyomat használatára is kérni fogja.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-116">You'll also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your Android device to access Office apps.](../media/9e8ecfee-8122-4a3a-8918-eece80344310.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="bcfe8-118">A „PIN-kód alaphelyzetbe állítása ennyi sikertelen kísérlet után" beállítás ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="bcfe8-118">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="bcfe8-119">A  Házirend szerkesztése ablaktáblában válassza a Szerkesztés az **Office-dokumentumok** hozzáférés-vezérlése mellett lehetőséget, bontsa ki a Felhasználók **Office-fájlok** mobileszközökön való elérésének kezelése lehetőséget, és győződjön meg arról, hogy a **PIN-kód** alaphelyzetbe állítása a sikertelen kísérletek száma után számra van állítva. </span><span class="sxs-lookup"><span data-stu-id="bcfe8-119">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number.</span></span> <span data-ttu-id="bcfe8-120">Ez alapértelmezés szerint 5.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-120">This is 5 by default.</span></span> 
  
1. <span data-ttu-id="bcfe8-121">A felhasználó Android-eszközén nyissa meg az Outlookot, és jelentkezzen be a felhasználó Microsoft 365 Vállalati prémium verziós hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-121">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="bcfe8-122">Írjon be egy helytelen PIN-kódot a házirendben megadott alkalommal.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-122">Enter an incorrect PIN as many times as specified by the policy.</span></span> <span data-ttu-id="bcfe8-123">A PIN-kód visszaállításához  egy üzenet arról fogja kérni, hogy a PIN-kódra vonatkozó korlát elérve.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-123">You'll see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](../media/fca6fcb4-bb5c-477f-af5e-5dc937e8b835.png)
  
3. <span data-ttu-id="bcfe8-125">Válassza a **PIN-kód visszaállítása** elemet.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-125">Press **Reset PIN**.</span></span> <span data-ttu-id="bcfe8-126">A rendszer kérni fogja, hogy jelentkezzen be a felhasználó Microsoft 365 Vállalati prémium verziós hitelesítő adataival, majd állítson be egy új PIN-kódot.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-126">You'll be prompted to sign in with the user's Microsoft 365 Business Premium credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="bcfe8-127">„A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió" beállítás ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="bcfe8-127">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="bcfe8-128">A **Házirend szerkesztése** ablaktáblában válassza a **Szerkesztés** elemet az **Elveszett vagy ellopott eszközök elleni védelem** elem mellett, bontsa ki a **Munkahelyi fájlok védelme az eszköz elvesztése vagy ellopása esetén** csomópontot, és győződjön meg arról, hogy **A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió** beállítás értéke **Be**.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-128">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](../media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="bcfe8-130">A felhasználó Android-eszközén nyissa meg az Outlookot, jelentkezzen be a felhasználó Microsoft 365 Vállalati prémium verziós hitelesítő adataival, és szükség esetén adjon meg egy PIN-kódot.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-130">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="bcfe8-131">Nyisson meg egy mellékletet tartalmazó e-mailt, és koppintson a lefelé mutató nyíl ikonra a melléklet adatai mellett.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-131">Open an email that contains an attachment and tap the down arrow icon next to the attachment's information.</span></span>
    
    ![Tap the down arrow next to an attachment to try to save it.](../media/b22573bb-91ce-455f-84fa-8feb2846b117.png)
  
    <span data-ttu-id="bcfe8-133">A képernyő alján a **Nem** menthető az eszközre jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-133">You'll see **Cannot save to device** on the bottom of the screen.</span></span> 
    
    ![Warning text that indicates cannot save a file locally to an Android.](../media/52ca3f3d-7ed0-4a52-9621-4872da6ea9c5.png)
  
    > [!NOTE]
    > <span data-ttu-id="bcfe8-135">A OneDrive Vállalati verzióba való mentés jelenleg nem engedélyezett az Android rendszerben, így csak annyi látható, hogy a helyi mentés le van tiltva.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-135">Saving to OneDrive for Business is not enabled for Android at this time, so you can only see that saving locally is blocked.</span></span> 
  
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="bcfe8-136">„A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után" beállítás ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="bcfe8-136">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="bcfe8-137">A  Házirend szerkesztése ablaktáblában válassza a Szerkesztés az **Office-dokumentumok** hozzáférés-vezérlése mellett lehetőséget, bontsa ki a Felhasználók **Office-fájlok** mobileszközökön való elérésének kezelése lehetőséget, és győződjön meg arról, hogy a felhasználóknak ismét be kell jelentkezniük, miután az **Office-appok** inaktívak voltak, néhány percnyire van beállítva. </span><span class="sxs-lookup"><span data-stu-id="bcfe8-137">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes.</span></span> <span data-ttu-id="bcfe8-138">Ez alapértelmezés szerint 30 perc.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-138">This is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="bcfe8-139">A felhasználó Android-eszközén nyissa meg az Outlookot, jelentkezzen be a felhasználó Microsoft 365 Vállalati prémium verziós hitelesítő adataival, és szükség esetén adjon meg egy PIN-kódot.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-139">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="bcfe8-p105">Ekkor megjelenik az Outlook Beérkezett üzenetek mappája. Hagyja az Android-eszközt üresjáratban legalább 30 percig (vagy más időtartamig, az a lényeg, hogy hosszabb legyen a házirendben meghatározottnál). Az eszköz valószínűleg elsötétül.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-p105">You should now see Outlook's inbox. Let the Android device idle untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="bcfe8-143">Az Android-eszközön ismét elérheti az Outlookot.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-143">Access Outlook on the Android device again.</span></span>
    
4. <span data-ttu-id="bcfe8-144">Mielőtt újból hozzáférhet az Outlookhoz, a rendszer kérni fogja, hogy adja meg a PIN-kódját.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-144">You'll be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="bcfe8-145">A „Munkahelyi fájlok védelme titkosítással" beállítás ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="bcfe8-145">Validate Protect work files with encryption</span></span>

<span data-ttu-id="bcfe8-146">A **Házirend szerkesztése** ablaktáblában válassza a **Szerkesztés** elemet az **Elveszett vagy ellopott eszközök elleni védelem** elem mellett, bontsa ki a **Munkahelyi fájlok védelme az eszköz elvesztése vagy ellopása esetén** csomópontot, és győződjön meg arról, hogy a **Munkahelyi fájlok védelme titkosítással** beállítás értéke **Be**, **A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió** beállításé pedig **Ki**.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-146">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="bcfe8-147">A felhasználó Android-eszközén nyissa meg az Outlookot, jelentkezzen be a felhasználó Microsoft 365 Vállalati prémium verziós hitelesítő adataival, és szükség esetén adjon meg egy PIN-kódot.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-147">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="bcfe8-148">Nyisson meg egy olyan e-mailt, amely néhány képfájlmellékletet tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-148">Open an email that contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="bcfe8-149">Koppintson a lefelé mutató nyílra a melléklet adatai mellett a mentéséhez.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-149">Tap the down arrow icon next to the attachment's info to save it.</span></span>
    
    ![Tap the down arrow to save the figure file to the Android device.](../media/08a9e21e-4022-45d5-acff-59cface651e7.png)
  
4. <span data-ttu-id="bcfe8-p106">Ekkor a rendszer arra kérheti, hogy engedélyezze a hozzáférést az Outlooknak a fényképekhez, médiatartalmakhoz és más fájlokhoz. Koppintson az **Engedélyezés** gombra.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-p106">You may be prompted to allow Outlook to access photos, media, and files on your device. Tap **Allow**.</span></span>
    
5. <span data-ttu-id="bcfe8-153">A képernyő alján válassza a **Mentés helye: Eszköz** lehetőséget, majd nyissa meg a **Galéria** appot.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-153">At the bottom of the screen, choose to **Save to Device** and then open the **Gallery** app.</span></span> 
    
6. <span data-ttu-id="bcfe8-p107">A listában látható lehet egy (vagy - ha több, képfájlt tartalmazó mellékletet mentett - több) titkosított fájl. Egy szürke négyzetként jelenhet meg a Képek listában, amelyben középen egy fehér felkiáltójel látható egy fehér körön belül.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-p107">You should see an encrypted photo (or more, if you saved multiple image file attachments) in the list. It may appear in the Pictures list as a gray square with a white exclamation point within a white circle in the center of the gray square.</span></span>
    
    ![An encrypted image file in the Gallery app.](../media/25936414-bd7e-421d-824e-6e59b877722d.png)
  
## <a name="ios"></a><span data-ttu-id="bcfe8-157">iOS</span><span class="sxs-lookup"><span data-stu-id="bcfe8-157">iOS</span></span>
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="bcfe8-158">Az appkezelési beállítások működésének ellenőrzése a felhasználói eszközökön</span><span class="sxs-lookup"><span data-stu-id="bcfe8-158">Check that the App protection settings are working on user devices</span></span>

<span data-ttu-id="bcfe8-159">Miután [konfigurálta az iOS-eszközök beállításait](app-protection-settings-for-android-and-ios.md) az appok védelmére, az alábbi lépésekkel ellenőrizheti, hogy működnek-e a kiválasztott beállítások.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-159">After you [set app configurations for iOS devices](app-protection-settings-for-android-and-ios.md) to protect apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="bcfe8-160">Először győződjön meg arról, hogy a házirend arra az appra vonatkozik, amelyben érvényesíteni fogja azt.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-160">First, make sure that the policy applies to the app in which you're going to validate it.</span></span>
  
1. <span data-ttu-id="bcfe8-161">A Microsoft 365 Vállalati prémium verzió [felügyeleti](https://portal.office.com)központjában kattintson a **Házirendek** szerkesztése \> **házirendre.**</span><span class="sxs-lookup"><span data-stu-id="bcfe8-161">In the Microsoft 365 Business Premium [admin center](https://portal.office.com), go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="bcfe8-162">Válassza **az iOS** alkalmazás-házirendet a beállításkor létrehozott beállításokhoz, vagy egy másik Ön által létrehozott házirendet, és ellenőrizze, hogy az kényszerítve van-e az Outlookban.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-162">Choose **Application policy for iOS** for the settings you created at setup, or another policy you created, and verify that it's enforced for Outlook for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](../media/842441b8-e7b1-4b86-9edd-d94d1f77b6f4.png)
  
### <a name="validate-require-a-pin-to-access-office-apps"></a><span data-ttu-id="bcfe8-164">A „PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez" beállítás ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="bcfe8-164">Validate Require a PIN to access Office apps</span></span>

<span data-ttu-id="bcfe8-165">A **Házirend szerkesztése** ablaktáblában válassza a **Szerkesztés** elemet az **Office-dokumentumok elérésének szabályozása** elem mellett, bontsa ki az **Office-fájlok felhasználói mobileszközökön történő elérésének felügyelete** csomópontot, és győződjön meg arról, hogy a **PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez** beállítás értéke **Be**.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-165">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Győződjön meg arról, hogy a PIN-kód vagy ujjlenyomat megkövetelve az Office-appok eléréséhez be van állítva.](../media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="bcfe8-167">A felhasználó iOS-eszközén nyissa meg az Outlookot, és jelentkezzen be a felhasználó Microsoft 365 Vállalati prémium verziós hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-167">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="bcfe8-168">A rendszer PIN-kód beíratára vagy ujjlenyomat használatára is kérni fogja.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-168">You'll also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your IOS device to access Office apps.](../media/06fc5cf3-9f19-4090-b23c-14bb59805b7a.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="bcfe8-170">A „PIN-kód alaphelyzetbe állítása ennyi sikertelen kísérlet után" beállítás ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="bcfe8-170">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="bcfe8-171">A  Házirend szerkesztése ablaktáblában válassza a Szerkesztés az **Office-dokumentumok** hozzáférés-vezérlése mellett lehetőséget, bontsa ki a Felhasználók **Office-fájlok** mobileszközökön való elérésének kezelése lehetőséget, és győződjön meg arról, hogy a **PIN-kód** alaphelyzetbe állítása a sikertelen kísérletek száma után számra van állítva. </span><span class="sxs-lookup"><span data-stu-id="bcfe8-171">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number.</span></span> <span data-ttu-id="bcfe8-172">Ez alapértelmezés szerint 5.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-172">This is 5 by default.</span></span> 
  
1. <span data-ttu-id="bcfe8-173">A felhasználó iOS-eszközén nyissa meg az Outlookot, és jelentkezzen be a felhasználó Microsoft 365 Vállalati prémium verziós hitelesítő adataival.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-173">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="bcfe8-174">Írjon be egy helytelen PIN-kódot a házirendben megadott alkalommal.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-174">Enter an incorrect PIN as many times as specified by the policy.</span></span> <span data-ttu-id="bcfe8-175">A PIN-kód visszaállításához  egy üzenet arról fogja kérni, hogy a PIN-kódra vonatkozó korlát elérve.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-175">You'll see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](../media/fab5c089-a4a5-4e8d-8c95-b8eed1dfa262.png)
  
3. <span data-ttu-id="bcfe8-177">Válassza az **OK** gombot.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-177">Press **OK**.</span></span> <span data-ttu-id="bcfe8-178">A rendszer kérni fogja, hogy jelentkezzen be a felhasználó Microsoft 365 Vállalati prémium verziós hitelesítő adataival, majd állítson be egy új PIN-kódot.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-178">You'll be prompted to sign in with the user's Microsoft 365 Business Premium credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="bcfe8-179">„A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió" beállítás ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="bcfe8-179">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="bcfe8-180">A **Házirend szerkesztése** ablaktáblában válassza a **Szerkesztés** elemet az **Elveszett vagy ellopott eszközök elleni védelem** elem mellett, bontsa ki a **Munkahelyi fájlok védelme az eszköz elvesztése vagy ellopása esetén** csomópontot, és győződjön meg arról, hogy **A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió** beállítás értéke **Be**.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-180">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](../media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="bcfe8-182">A felhasználó iOS-eszközén nyissa meg az Outlookot, jelentkezzen be a felhasználó Microsoft 365 Vállalati prémium verziós hitelesítő adataival, és szükség esetén adjon meg egy PIN-kódot.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-182">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="bcfe8-183">Nyisson meg egy mellékletet tartalmazó e-mailt, nyissa meg a mellékletet, és válassza a **Mentés** elemet a képernyő alján.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-183">Open an email that contains an attachment, open the attachment and choose **Save** on the bottom of the screen.</span></span> 
    
    ![Tap the Save option after you open an attachment to try to save it.](../media/b419b070-1530-4f14-86a8-8d89933a2b25.png)
  
3. <span data-ttu-id="bcfe8-185">Elvileg csak a OneDrive Vállalati verzió beállítás látható.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-185">You should only see an option for OneDrive for Business.</span></span> <span data-ttu-id="bcfe8-186">Ha nem, **koppintson** a Fiók hozzáadása elemre, és válassza a **OneDrive** Vállalati verzió lehetőséget a Tárfiók **hozzáadása** képernyőn.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-186">If not, tap **Add Account** and select **OneDrive for Business** from the **Add Storage Account** screen.</span></span> <span data-ttu-id="bcfe8-187">Adja meg a végfelhasználó Microsoft 365 Vállalati prémium verziós előfizetését, hogy amikor a rendszer kéri, jelentkezzen be.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-187">Provide the end user's Microsoft 365 Business Premium to sign in when prompted.</span></span> 
    
    <span data-ttu-id="bcfe8-188">Koppintson a **Mentés** elemre, és válassza a **OneDrive Vállalati verzió** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-188">Tap **Save** and select **OneDrive for Business**.</span></span>
    
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="bcfe8-189">„A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után" beállítás ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="bcfe8-189">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="bcfe8-190">A  Házirend szerkesztése ablaktáblában válassza a Szerkesztés az **Office-dokumentumok** hozzáférés-vezérlése mellett lehetőséget, bontsa ki a Felhasználók **Office-fájlok** mobileszközökön való elérésének kezelése lehetőséget, és győződjön meg arról, hogy a felhasználóknak ismét be kell jelentkezniük, miután az **Office-appok** inaktívak voltak, néhány percnyire van beállítva. </span><span class="sxs-lookup"><span data-stu-id="bcfe8-190">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes.</span></span> <span data-ttu-id="bcfe8-191">Ez alapértelmezés szerint 30 perc.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-191">This is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="bcfe8-192">A felhasználó iOS-eszközén nyissa meg az Outlookot, jelentkezzen be a felhasználó Microsoft 365 Vállalati prémium verziós hitelesítő adataival, és szükség esetén adjon meg egy PIN-kódot.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-192">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="bcfe8-p113">Ekkor megjelenik az Outlook Beérkezett üzenetek mappája. Hagyja az iOS-eszközt érintetlenül legalább 30 percig (vagy más időtartamig, az a lényeg, hogy hosszabb legyen a házirendben meghatározottnál). Az eszköz valószínűleg elsötétül.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-p113">You should now see Outlook's inbox. Let the iOS device untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="bcfe8-196">Az iOS-eszközön újból elérheti az Outlookot.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-196">Access Outlook on the iOS device again.</span></span>
    
4. <span data-ttu-id="bcfe8-197">Mielőtt újból hozzáférhet az Outlookhoz, a rendszer kérni fogja, hogy adja meg a PIN-kódját.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-197">You'll be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="bcfe8-198">A „Munkahelyi fájlok védelme titkosítással" beállítás ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="bcfe8-198">Validate Protect work files with encryption</span></span>

<span data-ttu-id="bcfe8-199">A **Házirend szerkesztése** ablaktáblában válassza a **Szerkesztés** elemet az **Elveszett vagy ellopott eszközök elleni védelem** elem mellett, bontsa ki a **Munkahelyi fájlok védelme az eszköz elvesztése vagy ellopása esetén** csomópontot, és győződjön meg arról, hogy a **Munkahelyi fájlok védelme titkosítással** beállítás értéke **Be**, **A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió** beállításé pedig **Ki**.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-199">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="bcfe8-200">A felhasználó iOS-eszközén nyissa meg az Outlookot, jelentkezzen be a felhasználó Microsoft 365 Vállalati prémium verziós hitelesítő adataival, és szükség esetén adjon meg egy PIN-kódot.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-200">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business Premium credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="bcfe8-201">Nyisson meg egy olyan e-mailt, amely néhány képfájlmellékletet tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-201">Open an email that contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="bcfe8-202">Koppintson a mellékletre, majd alatta a **Mentés** elemre.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-202">Tap the attachment and then tap the **Save** option under it.</span></span> 
    
4. <span data-ttu-id="bcfe8-p114">Nyissa meg a **Fotók** appot a kezdőképernyőről. Ekkor egy (vagy - ha több, képfájlt tartalmazó mellékletet mentett - több) mentett, ám titkosított fényképet kell látnia.</span><span class="sxs-lookup"><span data-stu-id="bcfe8-p114">Open **Photos** app from the home screen. You should see an encrypted photo (or more, if you saved multiple image file attachments) saved, but encrypted.</span></span> 
    
---


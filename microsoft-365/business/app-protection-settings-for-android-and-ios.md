---
title: Appvédelmi beállítások megadása androidos vagy iOS-es eszközökhöz
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Útmutató létrehozása, szerkesztése, vagy app kezelési házirend törlése és Android vagy iOS eszközökön Munkafájlok védelme.
ms.openlocfilehash: e81ff8a4bd71dbbbf7ccc31249d450e03f4bd241
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32277451"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a><span data-ttu-id="704ab-103">Appvédelmi beállítások megadása androidos vagy iOS-es eszközökhöz</span><span class="sxs-lookup"><span data-stu-id="704ab-103">Set app protection settings for Android or iOS devices</span></span>

## <a name="create-an-app-management-policy"></a><span data-ttu-id="704ab-104">Appkezelési házirend létrehozása</span><span class="sxs-lookup"><span data-stu-id="704ab-104">Create an app management policy</span></span>

1. <span data-ttu-id="704ab-105">Jelentkezzen be a [Microsoft 365 üzleti admin center](https://go.microsoft.com/fwlink/p/?linkid=837890) globális rendszergazdai hitelesítő adatokkal.</span><span class="sxs-lookup"><span data-stu-id="704ab-105">Sign in to [Microsoft 365 Business admin center ](https://go.microsoft.com/fwlink/p/?linkid=837890) with global admin credentials.</span></span> 
    
2. <span data-ttu-id="704ab-106">A felügyeleti központban válassza az **eszközök** \> **politika** \> **házirend hozzáadása**.</span><span class="sxs-lookup"><span data-stu-id="704ab-106">In the admin center, choose **Devices** \> **Policies** \> **Add policy**.</span></span>
  
3. <span data-ttu-id="704ab-107">A **Házirend felvétele** ablaktáblában adja meg a házirend egyedi nevét.</span><span class="sxs-lookup"><span data-stu-id="704ab-107">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="704ab-108">A **Házirend típusa** csoportban válassza az **Alkalmazáskezelés Android-eszközökhöz** vagy az **Alkalmazáskezelés iOS-eszközökhöz** lehetőséget attól függően, hogy milyen házirendkészletet szeretne létrehozni.</span><span class="sxs-lookup"><span data-stu-id="704ab-108">Under **Policy type**, choose **Application Management for Android** or **Application Management for iOS** depending on which set of policies you want to create.</span></span> 
    
5. <span data-ttu-id="704ab-109">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** \> configure the settings how you would like.</span><span class="sxs-lookup"><span data-stu-id="704ab-109">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** \> configure the settings how you would like.</span></span> <span data-ttu-id="704ab-110">The **Manage how users access Office files on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values.</span><span class="sxs-lookup"><span data-stu-id="704ab-110">The **Manage how users access Office files on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values.</span></span> <span data-ttu-id="704ab-111">További tudnivalókért tanulmányozza a [rendelkezésre álló beállításokat](#available-settings) .</span><span class="sxs-lookup"><span data-stu-id="704ab-111">See [Available settings](#available-settings)  for more information.</span></span> 
    
    <span data-ttu-id="704ab-112">Az **Alapértelmezett beállítások visszaállítása** hivatkozásra kattintva bármikor visszatérhet az alapértelmezett beállításokhoz.</span><span class="sxs-lookup"><span data-stu-id="704ab-112">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. <span data-ttu-id="704ab-p102">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span><span class="sxs-lookup"><span data-stu-id="704ab-p102">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="704ab-116">Végül válassza a **Kész** lehetőséget a házirend mentéséhez és eszközökhöz való hozzárendeléséhez.</span><span class="sxs-lookup"><span data-stu-id="704ab-116">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="edit-an-app-management-policy"></a><span data-ttu-id="704ab-117">Appkezelési házirend szerkesztése</span><span class="sxs-lookup"><span data-stu-id="704ab-117">Edit an app management policy</span></span>

1. <span data-ttu-id="704ab-118">A **házirendek** kartonon válassza a **házirend szerkesztése**.</span><span class="sxs-lookup"><span data-stu-id="704ab-118">On the **Policies** card, choose **Edit policy**.</span></span>
    
2. <span data-ttu-id="704ab-119">A **Házirend szerkesztése** ablaktáblában válassza ki a módosítani kívánt házirendet.</span><span class="sxs-lookup"><span data-stu-id="704ab-119">On the **Edit policy** pane, choose the policy you want to change</span></span> 
    
3. <span data-ttu-id="704ab-p103">Válassza a **Szerkesztés** elemet az egyes beállítások mellett a házirend értékeinek módosításához. Amikor módosít egy értéket, azt a rendszer automatikusan menti a házirendben.</span><span class="sxs-lookup"><span data-stu-id="704ab-p103">Choose **Edit** next to each setting to change the values in the policy. When you change a value, it is automatically saved into the policy</span></span> 
    
4. <span data-ttu-id="704ab-122">Ha végzett, zárja be a **Házirend szerkesztése** ablaktáblát.</span><span class="sxs-lookup"><span data-stu-id="704ab-122">When you are finished, close the **Edit policy** pane.</span></span> 
    
## <a name="delete-an-app-management-policy"></a><span data-ttu-id="704ab-123">Appkezelési házirend törlése</span><span class="sxs-lookup"><span data-stu-id="704ab-123">Delete an app management policy</span></span>

1. <span data-ttu-id="704ab-124">A **Házirendek** kártyán válassza a **Házirend törlése** elemet.</span><span class="sxs-lookup"><span data-stu-id="704ab-124">On the **Policies** card, choose **Delete policy**.</span></span>
    
2. <span data-ttu-id="704ab-125">On the **Delete policy** pane, choose the policies you want to delete \> **Select**, then **Confirm** to delete the policy or policies you chose.</span><span class="sxs-lookup"><span data-stu-id="704ab-125">On the **Delete policy** pane, choose the policies you want to delete \> **Select**, then **Confirm** to delete the policy or policies you chose.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="704ab-126">Rendelkezésre álló beállítások</span><span class="sxs-lookup"><span data-stu-id="704ab-126">Available settings</span></span>

<span data-ttu-id="704ab-127">Az alábbi táblázatok részletes információkkal szolgálnak azokról a beállításokról, amelyekkel védelmet nyújthat az eszközökön lévő fájloknak, valamint azokról is, amelyekkel szabályozhatja, hogy a felhasználók hogyan férhessenek hozzá az Office-fájlokhoz mobileszközükről.</span><span class="sxs-lookup"><span data-stu-id="704ab-127">The following tables give detailed information about the available settings to protect work files on devices and the settings that control how users access Office files from their mobile devices.</span></span>
  
 <span data-ttu-id="704ab-128">További információt [A Microsoft 365 Vállalati verzió védelmi funkcióinak megfelelő Intune-beállítások](map-protection-features-to-intune-settings.md) című témakör tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="704ab-128">See [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md) for more information.</span></span> 
  
### <a name="settings-that-protect-work-files"></a><span data-ttu-id="704ab-129">Munkahelyi fájlok védelmére szolgáló beállítások</span><span class="sxs-lookup"><span data-stu-id="704ab-129">Settings that protect work files</span></span>

<span data-ttu-id="704ab-130">Az alábbi beállításokkal védhetők meg a munkahelyi fájlok, ha az eszköz elveszett vagy ellopták:</span><span class="sxs-lookup"><span data-stu-id="704ab-130">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="704ab-131">Beállítás</span><span class="sxs-lookup"><span data-stu-id="704ab-131">Setting</span></span>  <br/> |<span data-ttu-id="704ab-132">Leírás</span><span class="sxs-lookup"><span data-stu-id="704ab-132">Description</span></span>  <br/> |
|<span data-ttu-id="704ab-133">Munkahelyi fájlok törlése az inaktív eszközökről ennyi nap után</span><span class="sxs-lookup"><span data-stu-id="704ab-133">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="704ab-134">Ha az eszközt az itt megadott számú napig nem használják, akkor a rajta tárolt összes munkahelyi fájl automatikusan törlődik.</span><span class="sxs-lookup"><span data-stu-id="704ab-134">If a device is not used for the number of days that you specify here, any work files stored on the device will automatically be deleted.</span></span>  <br/> |
|<span data-ttu-id="704ab-135">A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió</span><span class="sxs-lookup"><span data-stu-id="704ab-135">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="704ab-136">Ha ez a beállítás **Be** állapotban van, akkor a munkahelyi fájlok mentési helye kizárólag a OneDrive Vállalati verzió lehet.</span><span class="sxs-lookup"><span data-stu-id="704ab-136">If this setting is **On**, the only available save location for work files will be OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="704ab-137">Munkahelyi fájlok titkosítása</span><span class="sxs-lookup"><span data-stu-id="704ab-137">Encrypt work files</span></span>  <br/> |<span data-ttu-id="704ab-p104">A munkahelyi fájlok titkosítással való védelméhez ezt a beállítást tartsa **Be** állapotban. A céges adatokat még akkor sem tudják majd elolvasni, ha az eszköz elvész vagy ellopják.  </span><span class="sxs-lookup"><span data-stu-id="704ab-p104">Keep this setting **On** so that work files are protected by encryption. Even if the device is lost or stolen, no one will be able to read your company data.  </span></span><br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="704ab-140">Az Office-fájlok mobileszközökön való elérését szabályozó beállítások</span><span class="sxs-lookup"><span data-stu-id="704ab-140">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="704ab-141">Az alábbi beállítások használhatók a munkahelyi Office-fájlok elérésének kezelésére:</span><span class="sxs-lookup"><span data-stu-id="704ab-141">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="704ab-142">Beállítás</span><span class="sxs-lookup"><span data-stu-id="704ab-142">Setting</span></span>  <br/> |<span data-ttu-id="704ab-143">Leírás</span><span class="sxs-lookup"><span data-stu-id="704ab-143">Description</span></span>  <br/> |
|<span data-ttu-id="704ab-144">PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez</span><span class="sxs-lookup"><span data-stu-id="704ab-144">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="704ab-145">Ha ez a beállítás **Be** állapotban van, a mobileszközön lévő Office-appok használatához a felhasználónéven és a jelszón kívül a felhasználóknak további hitelesítési módszert is használniuk kell.</span><span class="sxs-lookup"><span data-stu-id="704ab-145">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="704ab-146">PIN-kód visszaállítása ennyi sikertelen bejelentkezési kísérlet után</span><span class="sxs-lookup"><span data-stu-id="704ab-146">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="704ab-147">Annak érdekében, hogy ne lehessen a PIN-kódot véletlenszerű próbálkozásokkal megfejteni, az Ön által megadott számú téves próbálkozás után a PIN-kód alaphelyzetbe áll.</span><span class="sxs-lookup"><span data-stu-id="704ab-147">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="704ab-148">A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után</span><span class="sxs-lookup"><span data-stu-id="704ab-148">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="704ab-149">Ezzel a beállítással azt határozhatja meg, hogy a felhasználó mennyi ideig maradhat inaktív, mielőtt újra be kellene jelentkeznie.</span><span class="sxs-lookup"><span data-stu-id="704ab-149">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="704ab-150">Hozzáférés letiltása a munkahelyi fájlokhoz a feltört vagy rootolással feltört eszközökön</span><span class="sxs-lookup"><span data-stu-id="704ab-150">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="704ab-p105">A hozzáértő felhasználók esetleg feltört vagy rootolással feltört eszközzel is rendelkezhetnek. Ez azt jelenti, hogy a felhasználó módosíthatja az operációs rendszert, ami viszont kártevők által sebezhetőbbé teheti az eszközt. Ha ez a beállítás **Be** állapotban van, az ilyen eszközök le lesznek tiltva.  </span><span class="sxs-lookup"><span data-stu-id="704ab-p105">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="704ab-154">A felhasználók másolhatnak tartalmakat az Office-appokból személyes appokba</span><span class="sxs-lookup"><span data-stu-id="704ab-154">Allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="704ab-155">Azt alapértelmezés szerint engedélyezi, de ha a beállítás be **kapcsolva**, a felhasználó tudta átmásolni információk munkafájlt a személyes fájlok.</span><span class="sxs-lookup"><span data-stu-id="704ab-155">We do allow this by default, but if the setting is **On**, the user could copy information in a work file to a personal file.</span></span> <span data-ttu-id="704ab-156">Ha a beállítás ki **kapcsolva**, a felhasználói információ másolása egy munka fiókból személyes app vagy személyes fiók nem lesz.</span><span class="sxs-lookup"><span data-stu-id="704ab-156">If the setting is **Off**, the user will be unable to copy information from a work account into a personal app or personal account.</span></span>  <br/> |
   

  


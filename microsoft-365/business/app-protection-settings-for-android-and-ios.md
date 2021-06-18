---
title: Appvédelmi beállítások megadása androidos vagy iOS-es eszközökhöz
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
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
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Megtudhatja, hogy miként hozhat létre, szerkeszthet és törölhet appkezelési házirendeket, és hogyan védheti meg a munkahelyi fájlokat Android- vagy iOS-eszközökön.
ms.openlocfilehash: 92dce1e8761e53b85df85f2a84f30ab307f63e6d
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/14/2021
ms.locfileid: "52925063"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a><span data-ttu-id="3ec21-103">Appvédelmi beállítások megadása androidos vagy iOS-es eszközökhöz</span><span class="sxs-lookup"><span data-stu-id="3ec21-103">Set app protection settings for Android or iOS devices</span></span>

<span data-ttu-id="3ec21-104">Ez a cikk a Microsoft 365 Vállalati prémium verzió.</span><span class="sxs-lookup"><span data-stu-id="3ec21-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="create-an-app-management-policy"></a><span data-ttu-id="3ec21-105">Appkezelési házirend létrehozása</span><span class="sxs-lookup"><span data-stu-id="3ec21-105">Create an app management policy</span></span>

1. <span data-ttu-id="3ec21-106">A felügyeleti központ megnyitásához: <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="3ec21-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="3ec21-107">A bal oldali navigációs sávon válassza az **Eszköz** \> **házirendek** \> **hozzáadása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="3ec21-107">In the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
  
3. <span data-ttu-id="3ec21-108">A **Házirend felvétele** ablaktáblában adja meg a házirend egyedi nevét.</span><span class="sxs-lookup"><span data-stu-id="3ec21-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="3ec21-109">A **Házirend típusa csoportban** válassza az **Alkalmazáskezelés Androidhoz** vagy **az Alkalmazáskezelés iOS** rendszerhez lehetőséget attól függően, hogy milyen házirendkészletet szeretne létrehozni.</span><span class="sxs-lookup"><span data-stu-id="3ec21-109">Under **Policy type**, choose **Application Management for Android** or **Application Management for iOS**, depending on which set of policies you want to create.</span></span> 
    
5. <span data-ttu-id="3ec21-110">Bontsa ki a **Munkahelyi fájlok védelme az eszközök** elveszett vagy ellopása esetén és a Felhasználók mobileszközökön Office fájlokhoz való **hozzáférésének kezelése ot.**</span><span class="sxs-lookup"><span data-stu-id="3ec21-110">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices**.</span></span> <span data-ttu-id="3ec21-111">Adja meg a beállításokat a megfelelő módon.</span><span class="sxs-lookup"><span data-stu-id="3ec21-111">Configure the settings how you would like.</span></span> <span data-ttu-id="3ec21-112">**A mobileszközökön Office** felhasználók hozzáférésének  beállítása Alapértelmezés szerint Ki, de  azt javasoljuk, hogy kapcsolja be, és fogadja el az alapértelmezett értékeket.</span><span class="sxs-lookup"><span data-stu-id="3ec21-112">**Manage how users access Office files on mobile devices** is **Off** by default, but we recommend that you turn it **On** and accept the default values.</span></span> <span data-ttu-id="3ec21-113">További információt a Rendelkezésre álló [beállítások lapon található.](#available-settings)</span><span class="sxs-lookup"><span data-stu-id="3ec21-113">For more information, see [Available settings](#available-settings).</span></span> 
    
    <span data-ttu-id="3ec21-114">Az **Alapértelmezett beállítások visszaállítása** hivatkozásra kattintva bármikor visszatérhet az alapértelmezett beállításokhoz.</span><span class="sxs-lookup"><span data-stu-id="3ec21-114">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Screenshot of Create a policy with Application management for Android selected](../media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. <span data-ttu-id="3ec21-116">Next decide **Who will get these settings?**</span><span class="sxs-lookup"><span data-stu-id="3ec21-116">Next decide **Who will get these settings?**</span></span> <span data-ttu-id="3ec21-117">Ha nem szeretné az alapértelmezett  Minden felhasználó biztonsági csoportot használni, válassza a Módosítás gombot, és válassza ki azokat a biztonsági csoportokat, amelyekben meg vannak jelölve ezek a \> **beállítások. Válassza a lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="3ec21-117">If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups that get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="3ec21-118">Végül válassza a **Kész** lehetőséget a házirend mentéséhez és eszközökhöz való hozzárendeléséhez.</span><span class="sxs-lookup"><span data-stu-id="3ec21-118">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="edit-an-app-management-policy"></a><span data-ttu-id="3ec21-119">Appkezelési házirend szerkesztése</span><span class="sxs-lookup"><span data-stu-id="3ec21-119">Edit an app management policy</span></span>

1. <span data-ttu-id="3ec21-120">A **Házirendek kártyán** válassza a **Házirend szerkesztése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="3ec21-120">On the **Policies** card, choose **Edit policy**.</span></span>
    
2. <span data-ttu-id="3ec21-121">A **Házirend szerkesztése** ablaktáblában válassza ki a módosítani kívánt házirendet.</span><span class="sxs-lookup"><span data-stu-id="3ec21-121">On the **Edit policy** pane, choose the policy you want to change</span></span> 
    
3. <span data-ttu-id="3ec21-122">Válassza a **Szerkesztés** elemet az egyes beállítások mellett a házirend értékeinek módosításához.</span><span class="sxs-lookup"><span data-stu-id="3ec21-122">Choose **Edit** next to each setting to change the values in the policy.</span></span> <span data-ttu-id="3ec21-123">Amikor módosít egy értéket, a rendszer automatikusan menti azt a házirendben.</span><span class="sxs-lookup"><span data-stu-id="3ec21-123">When you change a value, it's automatically saved in the policy.</span></span>
    
4. <span data-ttu-id="3ec21-124">Ha végzett, zárja be a Házirend szerkesztése **ablaktáblát.**</span><span class="sxs-lookup"><span data-stu-id="3ec21-124">When you're finished, close the **Edit policy** pane.</span></span> 
    
## <a name="delete-an-app-management-policy"></a><span data-ttu-id="3ec21-125">Appkezelési házirend törlése</span><span class="sxs-lookup"><span data-stu-id="3ec21-125">Delete an app management policy</span></span>

1. <span data-ttu-id="3ec21-126">A **Házirendek lapon** válasszon ki egy házirendet, majd kattintson a **Törlés gombra.**</span><span class="sxs-lookup"><span data-stu-id="3ec21-126">On the **Policies** page, choose a policy and then **Delete**.</span></span>
    
2. <span data-ttu-id="3ec21-127">A Házirend **törlése ablaktáblában** válassza a Megerősítés gombot a választott házirend vagy házirendek törléséhez. </span><span class="sxs-lookup"><span data-stu-id="3ec21-127">On the **Delete policy** pane, choose **Confirm** to delete the policy or policies you chose.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="3ec21-128">Rendelkezésre álló beállítások</span><span class="sxs-lookup"><span data-stu-id="3ec21-128">Available settings</span></span>

<span data-ttu-id="3ec21-129">Az alábbi táblázatok részletes információkat tartalmaznak az eszközök munkahelyi fájljainak védelmére vonatkozó beállításokról, valamint arról, hogy a felhasználók hogyan férhetnek hozzá Office fájlokhoz mobileszközükről.</span><span class="sxs-lookup"><span data-stu-id="3ec21-129">The following tables give detailed information about settings available to protect work files on devices and the settings that control how users access Office files from their mobile devices.</span></span>
  
 <span data-ttu-id="3ec21-130">További információt a Hogyan használhatja a védelmi funkciókat az Microsoft 365 Vállalati prémium verzió [Intune-beállításoknak?](map-protection-features-to-intune-settings.md)</span><span class="sxs-lookup"><span data-stu-id="3ec21-130">For more information, see [How do protection features in Microsoft 365 Business Premium map to Intune settings](map-protection-features-to-intune-settings.md).</span></span> 
  
### <a name="settings-that-protect-work-files"></a><span data-ttu-id="3ec21-131">Munkahelyi fájlok védelmére szolgáló beállítások</span><span class="sxs-lookup"><span data-stu-id="3ec21-131">Settings that protect work files</span></span>

<span data-ttu-id="3ec21-132">Az alábbi beállításokkal védhetők meg a munkahelyi fájlok, ha az eszköz elveszett vagy ellopták:</span><span class="sxs-lookup"><span data-stu-id="3ec21-132">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>


|<span data-ttu-id="3ec21-133">Beállítás</span><span class="sxs-lookup"><span data-stu-id="3ec21-133">Setting</span></span>  <br/> |<span data-ttu-id="3ec21-134">Leírás</span><span class="sxs-lookup"><span data-stu-id="3ec21-134">Description</span></span>  <br/> |
|:-----|:-----|
|<span data-ttu-id="3ec21-135">Munkahelyi fájlok törlése az inaktív eszközökről ennyi nap után</span><span class="sxs-lookup"><span data-stu-id="3ec21-135">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="3ec21-136">Ha az itt megadott számú napig nem használ egy eszközt, az eszközön tárolt munkahelyi fájlok automatikusan törlődnek.</span><span class="sxs-lookup"><span data-stu-id="3ec21-136">If a device isn't used for the number of days that you specify here, any work files stored on the device will be deleted automatically.</span></span>  <br/> |
|<span data-ttu-id="3ec21-137">A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió</span><span class="sxs-lookup"><span data-stu-id="3ec21-137">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="3ec21-138">Ha ez a beállítás **Be,** a munkahelyi fájlok mentésének egyedül a helye OneDrive vállalati verzió.</span><span class="sxs-lookup"><span data-stu-id="3ec21-138">If this setting is **On**, the only available save location for work files is OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="3ec21-139">Munkahelyi fájlok titkosítása</span><span class="sxs-lookup"><span data-stu-id="3ec21-139">Encrypt work files</span></span>  <br/> |<span data-ttu-id="3ec21-140">A munkahelyi fájlok titkosítással való védelméhez ezt a beállítást tartsa **Be** állapotban.</span><span class="sxs-lookup"><span data-stu-id="3ec21-140">Keep this setting **On** so that work files are protected by encryption.</span></span> <span data-ttu-id="3ec21-141">A céges adatokat még akkor sem olvashatják el, ha az eszközt ellopják vagy ellopják.</span><span class="sxs-lookup"><span data-stu-id="3ec21-141">Even if the device is lost or stolen, no one can read your company data.</span></span>  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="3ec21-142">Az Office-fájlok mobileszközökön történő elérésének felügyeletét meghatározó beállítások</span><span class="sxs-lookup"><span data-stu-id="3ec21-142">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="3ec21-143">Az alábbi beállítások használhatók a munkahelyi Office-fájlok elérésének kezelésére:</span><span class="sxs-lookup"><span data-stu-id="3ec21-143">The following settings are available to manage how users access Office work files:</span></span>


|<span data-ttu-id="3ec21-144">Beállítás</span><span class="sxs-lookup"><span data-stu-id="3ec21-144">Setting</span></span>  <br/> |<span data-ttu-id="3ec21-145">Leírás</span><span class="sxs-lookup"><span data-stu-id="3ec21-145">Description</span></span>  <br/> |
|:-----|:-----|
|<span data-ttu-id="3ec21-146">PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez</span><span class="sxs-lookup"><span data-stu-id="3ec21-146">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="3ec21-147">Ha ez a beállítás **Be,** a felhasználóknak a felhasználónéven és a jelszavukon kívül más hitelesítési módszert is meg kell adniuk ahhoz, hogy a mobileszközökön Office használják a hitelesítő alkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="3ec21-147">If this setting is **On** users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile devices.</span></span><br/> |
|<span data-ttu-id="3ec21-148">PIN-kód visszaállítása ennyi sikertelen bejelentkezési kísérlet után</span><span class="sxs-lookup"><span data-stu-id="3ec21-148">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="3ec21-149">Annak érdekében, hogy ne lehessen a PIN-kódot véletlenszerű próbálkozásokkal megfejteni, az Ön által megadott számú téves próbálkozás után a PIN-kód alaphelyzetbe áll.</span><span class="sxs-lookup"><span data-stu-id="3ec21-149">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="3ec21-150">A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után</span><span class="sxs-lookup"><span data-stu-id="3ec21-150">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="3ec21-151">Ez a beállítás azt határozza meg, hogy a felhasználó mennyi ideig inaktív, mielőtt a rendszer ismét arra kéri, hogy jelentkezzen be.</span><span class="sxs-lookup"><span data-stu-id="3ec21-151">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="3ec21-152">Hozzáférés letiltása a munkahelyi fájlokhoz a feltört vagy rootolással feltört eszközökön</span><span class="sxs-lookup"><span data-stu-id="3ec21-152">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="3ec21-p105">A hozzáértő felhasználók esetleg feltört vagy rootolással feltört eszközzel is rendelkezhetnek. Ez azt jelenti, hogy a felhasználó módosíthatja az operációs rendszert, ami viszont kártevők által sebezhetőbbé teheti az eszközt. Ha ez a beállítás **Be** állapotban van, az ilyen eszközök le lesznek tiltva.  </span><span class="sxs-lookup"><span data-stu-id="3ec21-p105">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="3ec21-156">Nem engedélyezem a felhasználóknak, hogy tartalmakat másoljanak Office-alkalmazásokból a személyes alkalmazásokba</span><span class="sxs-lookup"><span data-stu-id="3ec21-156">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="3ec21-157">Ez alapértelmezés szerint engedélyezett, de ha a beállítás Be van kapcsolva, a felhasználó átmásolhatja egy munkahelyi fájl adatait egy személyes fájlba.</span><span class="sxs-lookup"><span data-stu-id="3ec21-157">We do allow this by default, but if the setting is **On**, the user could copy information in a work file to a personal file.</span></span> <span data-ttu-id="3ec21-158">Ha a beállítás **Ki** van kapcsolva, a felhasználó nem tud adatokat másolni egy munkahelyi fiókból egy személyes appba vagy személyes fiókba.</span><span class="sxs-lookup"><span data-stu-id="3ec21-158">If the setting is **Off**, the user will be unable to copy information from a work account into a personal app or personal account.</span></span>  <br/> |

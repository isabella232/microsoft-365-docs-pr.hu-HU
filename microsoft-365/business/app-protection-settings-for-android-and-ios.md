---
title: Appvédelmi beállítások megadása androidos vagy iOS-es eszközökhöz
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Itt megtudhatja, hogyan hozhat létre, szerkeszthet és törölhet egy Alkalmazáskezelési házirendet, és hogyan védheti meg a munkahelyi fájlokat az Android vagy iOS rendszerű eszközökön.
ms.openlocfilehash: 2eebe5b603837d7e4125ab7e88b61792ca3a1e5d
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/14/2019
ms.locfileid: "38321845"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a><span data-ttu-id="ec94f-103">Appvédelmi beállítások megadása androidos vagy iOS-es eszközökhöz</span><span class="sxs-lookup"><span data-stu-id="ec94f-103">Set app protection settings for Android or iOS devices</span></span>

![Banner, hogy pont https://aka.ms/aboutM365preview-hoz.](media/m365admincenterchanging.png)

## <a name="create-an-app-management-policy"></a><span data-ttu-id="ec94f-105">Appkezelési házirend létrehozása</span><span class="sxs-lookup"><span data-stu-id="ec94f-105">Create an app management policy</span></span>

1. <span data-ttu-id="ec94f-106">Menj az admin központba <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span><span class="sxs-lookup"><span data-stu-id="ec94f-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="ec94f-107">Kattintson a bal oldali NAV \> **eszközházirendek** \> **hozzáadása**parancsára. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="ec94f-107">In the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
  
3. <span data-ttu-id="ec94f-108">A **Házirend felvétele** ablaktáblában adja meg a házirend egyedi nevét.</span><span class="sxs-lookup"><span data-stu-id="ec94f-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="ec94f-109">A **házirendtípus**területen válassza az **Alkalmazáskezelés az Android rendszerhez** vagy **az Alkalmazáskezelés az iOS rendszerhez**típust, attól függően, hogy milyen házirendeket szeretne létrehozni.</span><span class="sxs-lookup"><span data-stu-id="ec94f-109">Under **Policy type**, choose **Application Management for Android** or **Application Management for iOS**, depending on which set of policies you want to create.</span></span> 
    
5. <span data-ttu-id="ec94f-110">Bontsa ki a **munkahelyi fájlok védelmét az eszközök elvesztése vagy ellopása esetén** , és **kezelje a felhasználók által a mobileszközökön elérhető Office-fájlokat**.</span><span class="sxs-lookup"><span data-stu-id="ec94f-110">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices**.</span></span> <span data-ttu-id="ec94f-111">Konfigurálja a beállításokat, hogy hogyan szeretné.</span><span class="sxs-lookup"><span data-stu-id="ec94f-111">Configure the settings how you would like.</span></span> <span data-ttu-id="ec94f-112">Annak kezelése, hogy a **felhasználók hogyan férhetnek hozzá a mobileszközökön található Office-fájlokhoz** , alapértelmezés szerint **ki van kapcsolva** , de azt javasoljuk, hogy kapcsolja **be és fogadja** el az alapértelmezett értékeket.</span><span class="sxs-lookup"><span data-stu-id="ec94f-112">**Manage how users access Office files on mobile devices** is **Off** by default, but we recommend that you turn it **On** and accept the default values.</span></span> <span data-ttu-id="ec94f-113">További tudnivalókért tanulmányozza az [elérhető beállítások](#available-settings)című témakört.</span><span class="sxs-lookup"><span data-stu-id="ec94f-113">For more information, see [Available settings](#available-settings).</span></span> 
    
    <span data-ttu-id="ec94f-114">Az **Alapértelmezett beállítások visszaállítása** hivatkozásra kattintva bármikor visszatérhet az alapértelmezett beállításokhoz.</span><span class="sxs-lookup"><span data-stu-id="ec94f-114">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. <span data-ttu-id="ec94f-116">Next decide **Who will get these settings?**</span><span class="sxs-lookup"><span data-stu-id="ec94f-116">Next decide **Who will get these settings?**</span></span> <span data-ttu-id="ec94f-117">Ha nem kívánja használni az alapértelmezett **minden felhasználó** biztonsági csoportot, válassza a **módosítás**beállítást, válassza ki azokat a biztonsági csoportokat, amelyek \> ezeket **a beállításokat**megkapnak.</span><span class="sxs-lookup"><span data-stu-id="ec94f-117">If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups that get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="ec94f-118">Végül válassza a **Kész** lehetőséget a házirend mentéséhez és eszközökhöz való hozzárendeléséhez.</span><span class="sxs-lookup"><span data-stu-id="ec94f-118">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="edit-an-app-management-policy"></a><span data-ttu-id="ec94f-119">Appkezelési házirend szerkesztése</span><span class="sxs-lookup"><span data-stu-id="ec94f-119">Edit an app management policy</span></span>

1. <span data-ttu-id="ec94f-120">A **házirendek** kartonon kattintson a **házirend szerkesztése**lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="ec94f-120">On the **Policies** card, choose **Edit policy**.</span></span>
    
2. <span data-ttu-id="ec94f-121">A **Házirend szerkesztése** ablaktáblában válassza ki a módosítani kívánt házirendet.</span><span class="sxs-lookup"><span data-stu-id="ec94f-121">On the **Edit policy** pane, choose the policy you want to change</span></span> 
    
3. <span data-ttu-id="ec94f-122">Válassza a **Szerkesztés** elemet az egyes beállítások mellett a házirend értékeinek módosításához.</span><span class="sxs-lookup"><span data-stu-id="ec94f-122">Choose **Edit** next to each setting to change the values in the policy.</span></span> <span data-ttu-id="ec94f-123">Az érték módosítása automatikusan a házirendbe kerül.</span><span class="sxs-lookup"><span data-stu-id="ec94f-123">When you change a value, it's automatically saved in the policy.</span></span>
    
4. <span data-ttu-id="ec94f-124">Ha végzett, zárja be a **házirend szerkesztése** ablaktáblát.</span><span class="sxs-lookup"><span data-stu-id="ec94f-124">When you're finished, close the **Edit policy** pane.</span></span> 
    
## <a name="delete-an-app-management-policy"></a><span data-ttu-id="ec94f-125">Appkezelési házirend törlése</span><span class="sxs-lookup"><span data-stu-id="ec94f-125">Delete an app management policy</span></span>

1. <span data-ttu-id="ec94f-126">A **házirendek** lapon válasszon egy házirendet, majd **törölje**.</span><span class="sxs-lookup"><span data-stu-id="ec94f-126">On the **Policies** page, choose a policy and then **Delete**.</span></span>
    
2. <span data-ttu-id="ec94f-127">A **házirend törlése** párbeszédpanelen kattintson a **megerősítés** elemre a kiválasztott házirend vagy házirendek törléséhez.</span><span class="sxs-lookup"><span data-stu-id="ec94f-127">On the **Delete policy** pane, choose **Confirm** to delete the policy or policies you chose.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="ec94f-128">Rendelkezésre álló beállítások</span><span class="sxs-lookup"><span data-stu-id="ec94f-128">Available settings</span></span>

<span data-ttu-id="ec94f-129">A következő táblázatok részletes információt adnak azokról a beállításokról, amelyek az eszközök munkafájlok védelmére használhatók, valamint azok a beállítások, amelyek a felhasználók számára az Office fájlokhoz való hozzáférést a mobileszköztől vezérelhetik.</span><span class="sxs-lookup"><span data-stu-id="ec94f-129">The following tables give detailed information about settings available to protect work files on devices and the settings that control how users access Office files from their mobile devices.</span></span>
  
 <span data-ttu-id="ec94f-130">További információt [A Microsoft 365 Vállalati verzió védelmi funkcióinak megfelelő Intune-beállítások](map-protection-features-to-intune-settings.md) című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="ec94f-130">For more information, see [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md).</span></span> 
  
### <a name="settings-that-protect-work-files"></a><span data-ttu-id="ec94f-131">Munkahelyi fájlok védelmére szolgáló beállítások</span><span class="sxs-lookup"><span data-stu-id="ec94f-131">Settings that protect work files</span></span>

<span data-ttu-id="ec94f-132">Az alábbi beállításokkal védhetők meg a munkahelyi fájlok, ha az eszköz elveszett vagy ellopták:</span><span class="sxs-lookup"><span data-stu-id="ec94f-132">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="ec94f-133">Beállítás</span><span class="sxs-lookup"><span data-stu-id="ec94f-133">Setting</span></span>  <br/> |<span data-ttu-id="ec94f-134">Leírás</span><span class="sxs-lookup"><span data-stu-id="ec94f-134">Description</span></span>  <br/> |
|<span data-ttu-id="ec94f-135">Munkahelyi fájlok törlése az inaktív eszközökről ennyi nap után</span><span class="sxs-lookup"><span data-stu-id="ec94f-135">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="ec94f-136">Ha egy eszköz nem az itt megadott számú napra van használatban, akkor az eszközön tárolt minden munka automatikusan törlődik.</span><span class="sxs-lookup"><span data-stu-id="ec94f-136">If a device isn't used for the number of days that you specify here, any work files stored on the device will be deleted automatically.</span></span>  <br/> |
|<span data-ttu-id="ec94f-137">A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió</span><span class="sxs-lookup"><span data-stu-id="ec94f-137">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="ec94f-138">Ha ez elintézés van- **on**, egyetlen elérhető megment elhelyezés részére dolgozik fájlokat van OneDrive részére teendő.</span><span class="sxs-lookup"><span data-stu-id="ec94f-138">If this setting is **On**, the only available save location for work files is OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="ec94f-139">Munkahelyi fájlok titkosítása</span><span class="sxs-lookup"><span data-stu-id="ec94f-139">Encrypt work files</span></span>  <br/> |<span data-ttu-id="ec94f-140">A munkahelyi fájlok titkosítással való védelméhez ezt a beállítást tartsa **Be** állapotban.</span><span class="sxs-lookup"><span data-stu-id="ec94f-140">Keep this setting **On** so that work files are protected by encryption.</span></span> <span data-ttu-id="ec94f-141">Még ha az eszköz elvész vagy ellopják is, senki nem tudja elolvasni a vállalat adatait.</span><span class="sxs-lookup"><span data-stu-id="ec94f-141">Even if the device is lost or stolen, no one can read your company data.</span></span>  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="ec94f-142">Az Office-fájlok mobileszközökön történő elérésének felügyeletét meghatározó beállítások</span><span class="sxs-lookup"><span data-stu-id="ec94f-142">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="ec94f-143">Az alábbi beállítások használhatók a munkahelyi Office-fájlok elérésének kezelésére:</span><span class="sxs-lookup"><span data-stu-id="ec94f-143">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="ec94f-144">Beállítás</span><span class="sxs-lookup"><span data-stu-id="ec94f-144">Setting</span></span>  <br/> |<span data-ttu-id="ec94f-145">Leírás</span><span class="sxs-lookup"><span data-stu-id="ec94f-145">Description</span></span>  <br/> |
|<span data-ttu-id="ec94f-146">PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez</span><span class="sxs-lookup"><span data-stu-id="ec94f-146">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="ec94f-147">Ha **a felhasználónak a felhasználónévvel** és a jelszóval kapcsolatban egy másik hitelesítési formát kell adnia, akkor az Office alkalmazások mobileszközökön való használata előtt.</span><span class="sxs-lookup"><span data-stu-id="ec94f-147">If this setting is **On** users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile devices.</span></span><br/> |
|<span data-ttu-id="ec94f-148">PIN-kód visszaállítása ennyi sikertelen bejelentkezési kísérlet után</span><span class="sxs-lookup"><span data-stu-id="ec94f-148">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="ec94f-149">Annak érdekében, hogy ne lehessen a PIN-kódot véletlenszerű próbálkozásokkal megfejteni, az Ön által megadott számú téves próbálkozás után a PIN-kód alaphelyzetbe áll.</span><span class="sxs-lookup"><span data-stu-id="ec94f-149">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="ec94f-150">A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után</span><span class="sxs-lookup"><span data-stu-id="ec94f-150">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="ec94f-151">Ez a beállítás határozza meg, hogy a felhasználók mennyi ideig lehetnek üresjáratban, mielőtt a rendszer újra bejelentkezne.</span><span class="sxs-lookup"><span data-stu-id="ec94f-151">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="ec94f-152">Hozzáférés letiltása a munkahelyi fájlokhoz a feltört vagy rootolással feltört eszközökön</span><span class="sxs-lookup"><span data-stu-id="ec94f-152">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="ec94f-p105">A hozzáértő felhasználók esetleg feltört vagy rootolással feltört eszközzel is rendelkezhetnek. Ez azt jelenti, hogy a felhasználó módosíthatja az operációs rendszert, ami viszont kártevők által sebezhetőbbé teheti az eszközt. Ha ez a beállítás **Be** állapotban van, az ilyen eszközök le lesznek tiltva.  </span><span class="sxs-lookup"><span data-stu-id="ec94f-p105">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="ec94f-156">A felhasználók másolhatnak tartalmakat az Office-appokból személyes appokba</span><span class="sxs-lookup"><span data-stu-id="ec94f-156">Allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="ec94f-157">Ezt alapértelmezésben engedélyezi, de ha a beállítás **be van kapcsolva**, a felhasználó egy munkahelyi fájlban lévő információt átmásolhatja egy személyes fájlba.</span><span class="sxs-lookup"><span data-stu-id="ec94f-157">We do allow this by default, but if the setting is **On**, the user could copy information in a work file to a personal file.</span></span> <span data-ttu-id="ec94f-158">Ha a beállítás **ki van kapcsolva**, a felhasználó nem tud adatokat másolni munkahelyi fiókból személyes alkalmazásba vagy személyes fiókba.</span><span class="sxs-lookup"><span data-stu-id="ec94f-158">If the setting is **Off**, the user will be unable to copy information from a work account into a personal app or personal account.</span></span>  <br/> |

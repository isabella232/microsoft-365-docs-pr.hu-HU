---
title: Appvédelmi beállítások megadása androidos vagy iOS-es eszközökhöz
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
description: Megtudhatja, hogy miként hozhat létre, szerkeszthet vagy törölhet alkalmazáskezelési szabályzatot, és hogyan védheti meg a munkahelyi fájlokat Android vagy iOS rendszerű eszközökön.
ms.openlocfilehash: c0c8883fb120db90d81e57fbb80206d6ce4eccbf
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593313"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a><span data-ttu-id="d6bb3-103">Appvédelmi beállítások megadása androidos vagy iOS-es eszközökhöz</span><span class="sxs-lookup"><span data-stu-id="d6bb3-103">Set app protection settings for Android or iOS devices</span></span>

![Banner, hogy https://aka.ms/aboutM365previewpont .](media/m365admincenterchanging.png)

## <a name="create-an-app-management-policy"></a><span data-ttu-id="d6bb3-105">Appkezelési házirend létrehozása</span><span class="sxs-lookup"><span data-stu-id="d6bb3-105">Create an app management policy</span></span>

1. <span data-ttu-id="d6bb3-106">Nyissa meg a <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>felügyeleti központot a .</span><span class="sxs-lookup"><span data-stu-id="d6bb3-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="d6bb3-107">A bal oldali navigációs sávon válassza az **Eszközök** \> **házirendek** \> **hozzáadása**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="d6bb3-107">In the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
  
3. <span data-ttu-id="d6bb3-108">A **Házirend felvétele** ablaktáblában adja meg a házirend egyedi nevét.</span><span class="sxs-lookup"><span data-stu-id="d6bb3-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="d6bb3-109">A **Házirend típusa**csoportban válassza az Android **alkalmazáskezelés** vagy az **iOS alkalmazáskezelés**lehetőséget, attól függően, hogy mely házirendeket szeretné létrehozni.</span><span class="sxs-lookup"><span data-stu-id="d6bb3-109">Under **Policy type**, choose **Application Management for Android** or **Application Management for iOS**, depending on which set of policies you want to create.</span></span> 
    
5. <span data-ttu-id="d6bb3-110">Bontsa ki a Munkahelyi fájlok védelme az **eszközök ellopása vagy ellopása** esetén, és **kezelje, hogy a felhasználók hogyan férnek hozzá az Office-fájlokhoz mobileszközökön.**</span><span class="sxs-lookup"><span data-stu-id="d6bb3-110">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices**.</span></span> <span data-ttu-id="d6bb3-111">Adja meg a beállításokat, hogyan szeretné.</span><span class="sxs-lookup"><span data-stu-id="d6bb3-111">Configure the settings how you would like.</span></span> <span data-ttu-id="d6bb3-112">**A felhasználók mobileszközökön** való \*\*\*\* hozzáférésének alapértelmezett beállítását kezelheti, de azt javasoljuk, hogy kapcsolja be **és** fogadja el az alapértelmezett értékeket.</span><span class="sxs-lookup"><span data-stu-id="d6bb3-112">**Manage how users access Office files on mobile devices** is **Off** by default, but we recommend that you turn it **On** and accept the default values.</span></span> <span data-ttu-id="d6bb3-113">További információ: [Elérhető beállítások](#available-settings).</span><span class="sxs-lookup"><span data-stu-id="d6bb3-113">For more information, see [Available settings](#available-settings).</span></span> 
    
    <span data-ttu-id="d6bb3-114">Az **Alapértelmezett beállítások visszaállítása** hivatkozásra kattintva bármikor visszatérhet az alapértelmezett beállításokhoz.</span><span class="sxs-lookup"><span data-stu-id="d6bb3-114">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. <span data-ttu-id="d6bb3-116">Next decide **Who will get these settings?**</span><span class="sxs-lookup"><span data-stu-id="d6bb3-116">Next decide **Who will get these settings?**</span></span> <span data-ttu-id="d6bb3-117">Ha nem szeretné használni az alapértelmezett **Minden felhasználó** biztonsági csoportot, válassza a **Módosítás**lehetőséget, válassza a beállításokat \> bekapó biztonsági csoportokat **Válassza.**</span><span class="sxs-lookup"><span data-stu-id="d6bb3-117">If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups that get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="d6bb3-118">Végül válassza a **Kész** lehetőséget a házirend mentéséhez és eszközökhöz való hozzárendeléséhez.</span><span class="sxs-lookup"><span data-stu-id="d6bb3-118">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="edit-an-app-management-policy"></a><span data-ttu-id="d6bb3-119">Appkezelési házirend szerkesztése</span><span class="sxs-lookup"><span data-stu-id="d6bb3-119">Edit an app management policy</span></span>

1. <span data-ttu-id="d6bb3-120">A **Házirendek** kartonon válassza a **Házirend szerkesztése**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="d6bb3-120">On the **Policies** card, choose **Edit policy**.</span></span>
    
2. <span data-ttu-id="d6bb3-121">A **Házirend szerkesztése** ablaktáblában válassza ki a módosítani kívánt házirendet.</span><span class="sxs-lookup"><span data-stu-id="d6bb3-121">On the **Edit policy** pane, choose the policy you want to change</span></span> 
    
3. <span data-ttu-id="d6bb3-122">Válassza a **Szerkesztés** elemet az egyes beállítások mellett a házirend értékeinek módosításához.</span><span class="sxs-lookup"><span data-stu-id="d6bb3-122">Choose **Edit** next to each setting to change the values in the policy.</span></span> <span data-ttu-id="d6bb3-123">Ha módosít egy értéket, az automatikusan mentésre kerül a házirendbe.</span><span class="sxs-lookup"><span data-stu-id="d6bb3-123">When you change a value, it's automatically saved in the policy.</span></span>
    
4. <span data-ttu-id="d6bb3-124">Ha végzett, zárja be a **Házirend szerkesztése** ablaktáblát.</span><span class="sxs-lookup"><span data-stu-id="d6bb3-124">When you're finished, close the **Edit policy** pane.</span></span> 
    
## <a name="delete-an-app-management-policy"></a><span data-ttu-id="d6bb3-125">Appkezelési házirend törlése</span><span class="sxs-lookup"><span data-stu-id="d6bb3-125">Delete an app management policy</span></span>

1. <span data-ttu-id="d6bb3-126">A **Házirendek** lapon válasszon egy házirendet, majd törölje a **fájlt.**</span><span class="sxs-lookup"><span data-stu-id="d6bb3-126">On the **Policies** page, choose a policy and then **Delete**.</span></span>
    
2. <span data-ttu-id="d6bb3-127">A **Házirend törlése** ablaktáblán válassza a **Megerősítés** lehetőséget a választott házirend vagy házirendek törléséhez.</span><span class="sxs-lookup"><span data-stu-id="d6bb3-127">On the **Delete policy** pane, choose **Confirm** to delete the policy or policies you chose.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="d6bb3-128">Rendelkezésre álló beállítások</span><span class="sxs-lookup"><span data-stu-id="d6bb3-128">Available settings</span></span>

<span data-ttu-id="d6bb3-129">Az alábbi táblázatok részletes információkat nyújtanak az eszközökön lévő munkahelyi fájlok védelmére rendelkezésre álló beállításokról, valamint azokról a beállításokról, amelyek szabályozzák, hogy a felhasználók hogyan férnek hozzá az Office-fájlokhoz a mobileszközükről.</span><span class="sxs-lookup"><span data-stu-id="d6bb3-129">The following tables give detailed information about settings available to protect work files on devices and the settings that control how users access Office files from their mobile devices.</span></span>
  
 <span data-ttu-id="d6bb3-130">További információt [A Microsoft 365 Vállalati verzió védelmi funkcióinak megfelelő Intune-beállítások](map-protection-features-to-intune-settings.md) című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="d6bb3-130">For more information, see [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md).</span></span> 
  
### <a name="settings-that-protect-work-files"></a><span data-ttu-id="d6bb3-131">Munkahelyi fájlok védelmére szolgáló beállítások</span><span class="sxs-lookup"><span data-stu-id="d6bb3-131">Settings that protect work files</span></span>

<span data-ttu-id="d6bb3-132">Az alábbi beállításokkal védhetők meg a munkahelyi fájlok, ha az eszköz elveszett vagy ellopták:</span><span class="sxs-lookup"><span data-stu-id="d6bb3-132">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="d6bb3-133">Beállítás</span><span class="sxs-lookup"><span data-stu-id="d6bb3-133">Setting</span></span>  <br/> |<span data-ttu-id="d6bb3-134">Leírás</span><span class="sxs-lookup"><span data-stu-id="d6bb3-134">Description</span></span>  <br/> |
|<span data-ttu-id="d6bb3-135">Munkahelyi fájlok törlése az inaktív eszközökről ennyi nap után</span><span class="sxs-lookup"><span data-stu-id="d6bb3-135">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="d6bb3-136">Ha egy eszközt nem használ az itt megadott számú napig, az eszközön tárolt munkafájlok automatikusan törlődnek.</span><span class="sxs-lookup"><span data-stu-id="d6bb3-136">If a device isn't used for the number of days that you specify here, any work files stored on the device will be deleted automatically.</span></span>  <br/> |
|<span data-ttu-id="d6bb3-137">A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió</span><span class="sxs-lookup"><span data-stu-id="d6bb3-137">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="d6bb3-138">Ha ez a beállítás **Be van,** a munkahelyi fájlok csak a OneDrive Vállalati verzió számára érhető el mentési hely.</span><span class="sxs-lookup"><span data-stu-id="d6bb3-138">If this setting is **On**, the only available save location for work files is OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="d6bb3-139">Munkahelyi fájlok titkosítása</span><span class="sxs-lookup"><span data-stu-id="d6bb3-139">Encrypt work files</span></span>  <br/> |<span data-ttu-id="d6bb3-140">A munkahelyi fájlok titkosítással való védelméhez ezt a beállítást tartsa **Be** állapotban.</span><span class="sxs-lookup"><span data-stu-id="d6bb3-140">Keep this setting **On** so that work files are protected by encryption.</span></span> <span data-ttu-id="d6bb3-141">Még akkor is, ha az eszköz elveszett vagy ellopták, senki sem tudja olvasni a vállalati adatokat.</span><span class="sxs-lookup"><span data-stu-id="d6bb3-141">Even if the device is lost or stolen, no one can read your company data.</span></span>  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="d6bb3-142">Az Office-fájlok mobileszközökön történő elérésének felügyeletét meghatározó beállítások</span><span class="sxs-lookup"><span data-stu-id="d6bb3-142">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="d6bb3-143">Az alábbi beállítások használhatók a munkahelyi Office-fájlok elérésének kezelésére:</span><span class="sxs-lookup"><span data-stu-id="d6bb3-143">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="d6bb3-144">Beállítás</span><span class="sxs-lookup"><span data-stu-id="d6bb3-144">Setting</span></span>  <br/> |<span data-ttu-id="d6bb3-145">Leírás</span><span class="sxs-lookup"><span data-stu-id="d6bb3-145">Description</span></span>  <br/> |
|<span data-ttu-id="d6bb3-146">PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez</span><span class="sxs-lookup"><span data-stu-id="d6bb3-146">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="d6bb3-147">Ha ez a beállítás **A** felhasználónak a felhasználónévés jelszava mellett más hitelesítési formát is meg kell adnia ahhoz, hogy mobileszközeiken használhassák az Office-alkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="d6bb3-147">If this setting is **On** users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile devices.</span></span><br/> |
|<span data-ttu-id="d6bb3-148">PIN-kód visszaállítása ennyi sikertelen bejelentkezési kísérlet után</span><span class="sxs-lookup"><span data-stu-id="d6bb3-148">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="d6bb3-149">Annak érdekében, hogy ne lehessen a PIN-kódot véletlenszerű próbálkozásokkal megfejteni, az Ön által megadott számú téves próbálkozás után a PIN-kód alaphelyzetbe áll.</span><span class="sxs-lookup"><span data-stu-id="d6bb3-149">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="d6bb3-150">A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után</span><span class="sxs-lookup"><span data-stu-id="d6bb3-150">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="d6bb3-151">Ez a beállítás határozza meg, hogy a felhasználó mennyi ideig lehet tétlen, mielőtt a rendszer ismételten bejelentkezne.</span><span class="sxs-lookup"><span data-stu-id="d6bb3-151">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="d6bb3-152">Hozzáférés letiltása a munkahelyi fájlokhoz a feltört vagy rootolással feltört eszközökön</span><span class="sxs-lookup"><span data-stu-id="d6bb3-152">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="d6bb3-p105">A hozzáértő felhasználók esetleg feltört vagy rootolással feltört eszközzel is rendelkezhetnek. Ez azt jelenti, hogy a felhasználó módosíthatja az operációs rendszert, ami viszont kártevők által sebezhetőbbé teheti az eszközt. Ha ez a beállítás **Be** állapotban van, az ilyen eszközök le lesznek tiltva.  </span><span class="sxs-lookup"><span data-stu-id="d6bb3-p105">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="d6bb3-156">A felhasználók másolhatnak tartalmakat az Office-appokból személyes appokba</span><span class="sxs-lookup"><span data-stu-id="d6bb3-156">Allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="d6bb3-157">Alapértelmezés szerint engedélyezieztünk, de ha a beállítás Be van **kapcsolva,** a felhasználó átmásolhatja a munkahelyi fájlban lévő adatokat egy személyes fájlba.</span><span class="sxs-lookup"><span data-stu-id="d6bb3-157">We do allow this by default, but if the setting is **On**, the user could copy information in a work file to a personal file.</span></span> <span data-ttu-id="d6bb3-158">Ha a beállítás ki van **kapcsolva,** a felhasználó nem tudja átmásolni az adatokat egy munkahelyi fiókból egy személyes alkalmazásba vagy személyes fiókba.</span><span class="sxs-lookup"><span data-stu-id="d6bb3-158">If the setting is **Off**, the user will be unable to copy information from a work account into a personal app or personal account.</span></span>  <br/> |

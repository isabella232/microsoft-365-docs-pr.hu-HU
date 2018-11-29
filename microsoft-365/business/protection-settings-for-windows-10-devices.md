---
title: Alkalmazásvédelmi beállítások megadása Windows 10-es eszközökhöz
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
f1_keywords:
- Win10AppPolicy
- O365E_Win10AppPolicy
- BCS365_Win10AppPolicy
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Útmutató az app adatkezelési házirend létrehozása és munka fájlok Windows 10 eszközök védelme.
ms.openlocfilehash: acf19a72d994185a35b2e425f8334a73a121ee10
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982825"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="5866a-103">Alkalmazásvédelmi beállítások megadása Windows 10-es eszközökhöz</span><span class="sxs-lookup"><span data-stu-id="5866a-103">Set application protection settings for Windows 10 devices</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="5866a-104">Appkezelési házirend létrehozása Windows 10-es eszközhöz</span><span class="sxs-lookup"><span data-stu-id="5866a-104">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="5866a-105">Ha a felhasználók munkahelyi feladatokra is használják saját Windows 10-es eszközeiket, az azokon tárolt munkahelyi adatok is védhetők.</span><span class="sxs-lookup"><span data-stu-id="5866a-105">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="5866a-p101">Jelentkezzen be a [Microsoft 365 Vállalati verzióba](https://portal.office.com) globális rendszergazdai hitelesítő adatokkal. Az **Admin** csempét választva lépjen a felügyeleti központba.</span><span class="sxs-lookup"><span data-stu-id="5866a-p101">Sign in to [Microsoft 365 Business](https://portal.office.com) with global admin credentials. Choose the **Admin** tile to go to the admin center.</span></span> 
    
2. <span data-ttu-id="5866a-108">A felügyeleti portál **Eszközházirendek** kártyáján válassza a **Házirend felvétele** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="5866a-108">On the **Device policies** card of the admin portal, choose **Add policy**.</span></span>
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. <span data-ttu-id="5866a-110">A **Házirend felvétele** ablaktáblában adja meg a házirend egyedi nevét.</span><span class="sxs-lookup"><span data-stu-id="5866a-110">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="5866a-111">A **Házirend típusa** beállításnál válassza az **Alkalmazáskezelés Windows 10-es eszközökhöz** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="5866a-111">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
    
5. <span data-ttu-id="5866a-112">A \*\* eszköztípus \*\*, válassza a **személyes** vagy a **Vállalat birtokában**.</span><span class="sxs-lookup"><span data-stu-id="5866a-112">Under \*\* Device type \*\*, choose either **Personal** or **Company Owned**.</span></span>
    
6. <span data-ttu-id="5866a-113">A **Munkahelyi fájlok titkosítása** lehetőség automatikusan be van kapcsolva.</span><span class="sxs-lookup"><span data-stu-id="5866a-113">The **Encrypt work files** is turned on automatically.</span></span> 
    
7. <span data-ttu-id="5866a-114">Ha nem szeretné, hogy a felhasználók a saját számítógépükre mentsék a munkahelyi fájlokat, állítsa **A felhasználók nem másolhatnak céges adatokat saját fájljaikba, a munkahelyi fájlokat pedig csak a OneDrive Vállalati verzióba menthetik** beállítást **Be** értékre.</span><span class="sxs-lookup"><span data-stu-id="5866a-114">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
    
8. <span data-ttu-id="5866a-p102">Bontsa ki a **kezelése, hogy a felhasználók miként férhetnek hozzá a eszközök Office fájlok** \> hogyan szeretné a beállításokat. Alapértelmezés szerint nincs **bekapcsolva** a **kezelése, hogy a felhasználók miként férhetnek hozzá a mobil eszközökön található Office-eszközöket** , de ajánlott, hogy kapcsolja **be** , és elfogadhatja az alapértelmezett értékeket. További tudnivalókért tanulmányozza a [rendelkezésre álló beállításokat](protection-settings-for-windows-10-devices.md#bkmk_settings) .</span><span class="sxs-lookup"><span data-stu-id="5866a-p102">Expand **Manage how users access Office files on devices** \> configure the settings how you would like. The **Manage how users access Office devices on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values. See [Available settings](protection-settings-for-windows-10-devices.md#bkmk_settings) for more information.</span></span> 
    
    <span data-ttu-id="5866a-118">Az **Alapértelmezett beállítások visszaállítása** hivatkozásra kattintva bármikor visszatérhet az alapértelmezett beállításokhoz.</span><span class="sxs-lookup"><span data-stu-id="5866a-118">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
9. <span data-ttu-id="5866a-119">Bontsa ki a **Windowsos eszközökön lévő adatok helyreállítása** beállítást, és ajánlott, hogy azt állítsa **Be** értékre.</span><span class="sxs-lookup"><span data-stu-id="5866a-119">Expand **Recover data on Windows devices** and it is recommended that you turn it **On**.</span></span>
    
    <span data-ttu-id="5866a-p103">Ahhoz, hogy megkereshesse az adat-helyreállítási megbízott tanúsítványának helyét, először létre kell hoznia egyet. Pontos utasításokat [A titkosított fájlrendszer (EFS) adat-helyreállítási megbízottja (DRA) tanúsítványának létrehozása és ellenőrzése](https://go.microsoft.com/fwlink/p/?linkid=853700) című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="5866a-p103">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one. For instructions see, [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](https://go.microsoft.com/fwlink/p/?linkid=853700).</span></span>
    
    <span data-ttu-id="5866a-p104">A munkahelyi fájlok alapértelmezés szerint egy az eszközön tárolt és a felhasználó profiljához társított titkos kulccsal vannak titkosítva. Csak a felhasználó tudja megnyitni és visszafejteni a fájlt. Így tehát, ha valaki elveszít egy eszközt, vagy törölnek egy felhasználót, egy szükséges fájl titkosított állapotban ragadhat. A kizárólag rendszergazda által használható adat-helyreállítási megbízott (DRA) tanúsítvánnyal visszafejthető a fájl.</span><span class="sxs-lookup"><span data-stu-id="5866a-p104">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile. Only the user can open and decrypt the file. However, if a device is lost or a user is removed, a file can be stuck in an encrypted state. The Data Recovery Agent (DRA) certificate can be used by an admin to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="5866a-p105">Bontsa ki a **További hálózati és felhőbeli helyek védelme** beállítást, ha szeretne további tartományokat vagy SharePoint Online-helyeket felvenni a felsorolt appokban lévő fájlok védelmének biztosítása érdekében. Ha bármelyik mezőben egynél több elemet kell megadnia, pontosvesszővel (;) válassza el őket egymástól.</span><span class="sxs-lookup"><span data-stu-id="5866a-p105">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps will be protected. If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span> 
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="5866a-p106">Ezután döntse el, **fog kapni, akik ezeket a beállításokat?** Ha nem szeretné az alapértelmezett **Felhasználók** biztonsági csoporthoz, választhat **módosítása**, a biztonsági csoportok, akik ezeket a beállításokat kap \> **kiválasztása**.</span><span class="sxs-lookup"><span data-stu-id="5866a-p106">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
12. <span data-ttu-id="5866a-132">Végül válassza a **Hozzáadás** lehetőséget a házirend mentéséhez és eszközökhöz való hozzárendeléséhez.</span><span class="sxs-lookup"><span data-stu-id="5866a-132">Finally, choose **Add** to save the policy, and assign it to devices.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="5866a-133">Rendelkezésre álló beállítások</span><span class="sxs-lookup"><span data-stu-id="5866a-133">Available settings</span></span>

<span data-ttu-id="5866a-134">Az alábbi beállítások használhatók a munkahelyi Office-fájlok elérésének kezelésére.</span><span class="sxs-lookup"><span data-stu-id="5866a-134">The following settings are available to manage how users access Office work files.</span></span>
  
<span data-ttu-id="5866a-135">További információt [A Microsoft 365 Vállalati verzió védelmi funkcióinak megfelelő Intune-beállítások](map-protection-features-to-intune-settings.md) című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="5866a-135">For more information, see [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md).</span></span>
  
|<span data-ttu-id="5866a-136">**Beállítás**</span><span class="sxs-lookup"><span data-stu-id="5866a-136">**Setting**</span></span>|<span data-ttu-id="5866a-137">**Leírás**</span><span class="sxs-lookup"><span data-stu-id="5866a-137">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5866a-138">PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez</span><span class="sxs-lookup"><span data-stu-id="5866a-138">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="5866a-139">Ha ez a beállítás **Be** állapotban van, a mobileszközön lévő Office-appok használatához a felhasználónéven és a jelszón kívül a felhasználóknak további hitelesítési módszert is használniuk kell.</span><span class="sxs-lookup"><span data-stu-id="5866a-139">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="5866a-140">PIN-kód visszaállítása ennyi sikertelen bejelentkezési kísérlet után</span><span class="sxs-lookup"><span data-stu-id="5866a-140">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="5866a-141">Annak érdekében, hogy ne lehessen a PIN-kódot véletlenszerű próbálkozásokkal megfejteni, az Ön által megadott számú téves próbálkozás után a PIN-kód alaphelyzetbe áll.</span><span class="sxs-lookup"><span data-stu-id="5866a-141">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="5866a-142">A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után</span><span class="sxs-lookup"><span data-stu-id="5866a-142">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="5866a-143">Ezzel a beállítással azt határozhatja meg, hogy a felhasználó mennyi ideig maradhat inaktív, mielőtt újra be kellene jelentkeznie.</span><span class="sxs-lookup"><span data-stu-id="5866a-143">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
   


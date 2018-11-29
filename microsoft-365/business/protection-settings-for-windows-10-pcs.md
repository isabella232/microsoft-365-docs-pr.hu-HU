---
title: Eszközvédelmi beállítások megadása Windows 10-es PC-khez
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: bd66c26c-73a4-45a8-8642-3ea4ee7cd89d
description: Alapértelmezett és más Microsoft 365 üzleti Windows 10 eszközök biztonságos beállítások ismertetése
ms.openlocfilehash: ebfe5f59e544b67e5a4f2ecd990031e9221ff8e5
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982145"
---
# <a name="set-device-protection-settings-for-windows-10-pcs"></a><span data-ttu-id="8c240-103">Eszközvédelmi beállítások megadása Windows 10-es PC-khez</span><span class="sxs-lookup"><span data-stu-id="8c240-103">Set device protection settings for Windows 10 PCs</span></span>

## <a name="secure-windows-10-devices"></a><span data-ttu-id="8c240-104">Windows 10-es eszközök védelme</span><span class="sxs-lookup"><span data-stu-id="8c240-104">Secure Windows 10 devices</span></span>

<span data-ttu-id="8c240-105">Nézze meg ezt a videót a Windows 10-es eszközök biztonságos használatáról a Microsoft 365 Business-szel:</span><span class="sxs-lookup"><span data-stu-id="8c240-105">View a video on how to secure Windows 10 devices with Microsoft 365 Business:</span></span>
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. <span data-ttu-id="8c240-106">Jelentkezzen be a [Microsoft 365 Business](https://portal.office.com) szolgáltatásba globális rendszergazdai hitelesítő adatokkal.</span><span class="sxs-lookup"><span data-stu-id="8c240-106">Sign in to [Microsoft 365 Business](https://portal.office.com) with global admin credentials.</span></span> 
    
2. <span data-ttu-id="8c240-107">A felügyeleti központ **Eszközházirendek** kártyáján válassza a **Házirend felvétele** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="8c240-107">in the admin center, on the **Device policies** card, choose **Add policy**.</span></span>
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. <span data-ttu-id="8c240-109">A **Házirend felvétele** ablaktáblában adja meg a házirend egyedi nevét.</span><span class="sxs-lookup"><span data-stu-id="8c240-109">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="8c240-110">A **Házirend típusa** csoportban válassza a **Windows 10-es eszközök konfigurálása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="8c240-110">Under **Policy type**, choose **Windows 10 Device Configuration**.</span></span>
    
5. <span data-ttu-id="8c240-p101">Bontsa ki a **Windows 10 eszközök biztonságos** \> hogyan szeretné a beállításokat. További tudnivalókért tanulmányozza a [rendelkezésre álló beállításokat](protection-settings-for-windows-10-pcs.md#bkmk_availablesettings) .</span><span class="sxs-lookup"><span data-stu-id="8c240-p101">Expand **Secure Windows 10 Devices** \> configure the settings how you would like. See [Available settings](protection-settings-for-windows-10-pcs.md#bkmk_availablesettings) for more information.</span></span> 
    
    <span data-ttu-id="8c240-113">Az **Alapértelmezett beállítások visszaállítása** hivatkozásra kattintva bármikor visszatérhet az alapértelmezett beállításokhoz.</span><span class="sxs-lookup"><span data-stu-id="8c240-113">You can alway use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Add policy pane with Windows 10 Device configuration selected](media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. <span data-ttu-id="8c240-p102">Ezután döntse el, **fog kapni, akik ezeket a beállításokat?** Ha nem szeretné használni az alapértelmezett **minden felhasználó** biztonsági csoport, válassza ki a **Módosítás**, keresse meg a biztonsági csoportot, akik ezeket a beállításokat kap \> **kiválasztása**.</span><span class="sxs-lookup"><span data-stu-id="8c240-p102">Next decide **Who will get these settings?** If you don't want to use the default **All users** security group, Choose **Change**, search for the security group who will get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="8c240-117">Végül válassza a **Kész** lehetőséget a házirend mentéséhez és eszközökhöz való hozzárendeléséhez.</span><span class="sxs-lookup"><span data-stu-id="8c240-117">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="8c240-118">Rendelkezésre álló beállítások</span><span class="sxs-lookup"><span data-stu-id="8c240-118">Available settings</span></span>

<span data-ttu-id="8c240-p103">Alapértelmezés szerint minden beállítás **be van kapcsolva**. Az alábbi beállítások érhetők el.</span><span class="sxs-lookup"><span data-stu-id="8c240-p103">By default all settings are **On**. The following settings are available.</span></span>
  
<span data-ttu-id="8c240-121">További információt [A Microsoft 365 Vállalati verzió védelmi funkcióinak megfelelő Intune-beállítások](map-protection-features-to-intune-settings.md) című cikk tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="8c240-121">See [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md) for more information.</span></span> 
  
|||
|:-----|:-----|
|<span data-ttu-id="8c240-122">Beállítás</span><span class="sxs-lookup"><span data-stu-id="8c240-122">Setting</span></span>  <br/> |<span data-ttu-id="8c240-123">Leírás</span><span class="sxs-lookup"><span data-stu-id="8c240-123">Description</span></span>  <br/> |
|<span data-ttu-id="8c240-124">PC-k védelme a vírusokkal és más fenyegetésekkel szemben a Windows Defender víruskereső használatával</span><span class="sxs-lookup"><span data-stu-id="8c240-124">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="8c240-125">Használatához a Windows Defender víruskeresőnek bekapcsolt állapotban kell lennie, hogy védelmet nyújthasson a PC-knek az internethez csatlakozva jelentkező veszélyekkel szemben.</span><span class="sxs-lookup"><span data-stu-id="8c240-125">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="8c240-126">PC-k védelme a webes fenyegetésekkel szemben a Microsoft Edge böngészőben</span><span class="sxs-lookup"><span data-stu-id="8c240-126">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="8c240-127">Bekapcsolja a Microsoft Edge böngészőben azokat a beállításokat, amelyek segítenek megvédeni a felhasználót a kártékony webhelyek és letöltések által okozott veszélyektől.</span><span class="sxs-lookup"><span data-stu-id="8c240-127">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="8c240-128">Eszközök támadási felületét csökkentő szabályok használata</span><span class="sxs-lookup"><span data-stu-id="8c240-128">Use rules that reduce the attack surface of devices</span></span>  <br/> |<span data-ttu-id="8c240-p104">A támadásifelület-csökkentés bekapcsolásával letilthatók azok a műveletek és appok, amelyekkel a kártevők rendszerint megfertőzik az eszközöket. Ez a beállítás csak akkor használható, ha be van kapcsolva a Windows Defender víruskereső. További információ a [támadásifelület-csökkentésről](https://go.microsoft.com/fwlink/?linkid=870417).  </span><span class="sxs-lookup"><span data-stu-id="8c240-p104">When turned On, attack surface reduction helps block actions and apps typically used by malware to infect devices. This setting is only available if Windows Defender Antivirus is set to On. See [Reduce attack surfaces](https://go.microsoft.com/fwlink/?linkid=870417) to learn more.  </span></span><br/> |
|<span data-ttu-id="8c240-132">Mappák védelme a veszélyforrásokkal (például a zsarolóvírusokkal) szemben</span><span class="sxs-lookup"><span data-stu-id="8c240-132">Protect folders from threats such as ransomware</span></span>  <br/> |<span data-ttu-id="8c240-p105">Ez a beállítás szabályozott mappahozzáféréssel védi a céges adatokat a gyanús vagy kártékony appok (például a zsarolóvírusok) általi módosítástól azáltal, hogy nem engedélyezi nekik a védett mappákban tárolt adatok módosítását. Ez a beállítás csak akkor használható, ha be van kapcsolva a Windows Defender víruskereső. További információt a [Mappák védelme szabályozott mappahozzáféréssel](https://go.microsoft.com/fwlink/?linkid=870418) című cikkben talál.  </span><span class="sxs-lookup"><span data-stu-id="8c240-p105">This setting uses controlled folder access to protect company data from modification by suspicious or malicious apps, such as ransomware. These types of apps are blocked from making changes in protected folders. This setting is only available if Windows Defender Antivirus is set to On. See [Protect folders with COntrolled folder access](https://go.microsoft.com/fwlink/?linkid=870418) to learn more.  </span></span><br/> |
|<span data-ttu-id="8c240-137">Vélhetően kártékony internetes tartalmakhoz történő hálózati hozzáférés megakadályozása</span><span class="sxs-lookup"><span data-stu-id="8c240-137">Prevent network access to potentially malicious content on the Internet</span></span>  <br/> |<span data-ttu-id="8c240-p106">Ezzel a beállítással letilthatja a felhasználók kevésbé megbízható internetes helyekre irányuló kimenő kapcsolatait. Az ilyen helyeken adathalász kísérletekre, biztonsági résekre vagy más kártékony tartalmakra lehet számítani. Ez a beállítás csak akkor használható, ha be van kapcsolva a Windows Defender víruskereső. További információt [A hálózat védelme](https://go.microsoft.com/fwlink/?linkid=870419) című cikk tartalmaz.  </span><span class="sxs-lookup"><span data-stu-id="8c240-p106">Use this setting to block outbound user connections to low-reputation Internet locations that may host phishing scams, exploits or other malicious content. This setting is only available if Windows Defender Antivirus is set to On. See [Protect your network](https://go.microsoft.com/fwlink/?linkid=870419) for more information.  </span></span><br/> |
|<span data-ttu-id="8c240-141">PC-ken lévő fájlok és mappák illetéktelen hozzáféréssel szembeni védelme BitLocker-titkosítással</span><span class="sxs-lookup"><span data-stu-id="8c240-141">Help protect files and folders on PCs from unauthorized access with BitLocker</span></span>  <br/> |<span data-ttu-id="8c240-p107">A Bitlocker a számítógép merevlemezének titkosításával és a számítógép elvesztése vagy ellopása esetén az adatok kinyerése elleni védelemmel biztosítja adatai védelmét. További információt a [Bitlocker - gyakori kérdések](https://go.microsoft.com/fwlink/?linkid=871000) című cikk tartalmaz.  </span><span class="sxs-lookup"><span data-stu-id="8c240-p107">Bitlocker protects data by encrypting the computer hard drives and protect against data exposure if a computer is lost or stolen. See [Bitlocker FAQ](https://go.microsoft.com/fwlink/?linkid=871000) for more information.  </span></span><br/> |
|<span data-ttu-id="8c240-144">A felhasználók letölthetnek appokat innen: Microsoft Áruház</span><span class="sxs-lookup"><span data-stu-id="8c240-144">Allow users to download apps from Microsoft Store</span></span>  <br/> |<span data-ttu-id="8c240-p108">Lehetővé teszi, hogy a felhasználók appokat tölthessenek le és telepíthessenek a Microsoft Áruházból. Az appok között játékok és munkára használható eszközök egyaránt lehetnek, ezért ez a beállítás **Be** állapotban van, de a fokozott biztonság érdekében ki is kapcsolhatja.  </span><span class="sxs-lookup"><span data-stu-id="8c240-p108">Lets users download and install apps from the Microsoft Store. Apps include everything from games to productivity tools, so we leave this setting **On**, but you can turn it off for extra security.  </span></span><br/> |
|<span data-ttu-id="8c240-147">A felhasználók igénybe vehetik Cortana segítségét</span><span class="sxs-lookup"><span data-stu-id="8c240-147">Allow users to access Cortana</span></span>  <br/> |<span data-ttu-id="8c240-p109">Cortana nagyon hasznos lehet. Beállításokat képes be- és kikapcsolni, útbaigazítást tud adni, és ügyelni tud arra, hogy Ön ne késsen el a megbeszéléseiről, ezért ez a beállítás alapértelmezés szerint **Be** állapotban van.  </span><span class="sxs-lookup"><span data-stu-id="8c240-p109">Cortana can be very helpful! She can turn settings on or off for you, give directions, and make sure you're on time for appointments, so we keep this **On** by default.  </span></span><br/> |
|<span data-ttu-id="8c240-150">A felhasználók kaphatnak tippeket és hirdetéseket a Windowszal kapcsolatban a Microsofttól</span><span class="sxs-lookup"><span data-stu-id="8c240-150">Allow users to receive Windows tips and advertisements from Microsoft</span></span>  <br/> |<span data-ttu-id="8c240-151">A Windows-tippek hasznosak lehetnek, és új funkciók megjelenésekor segíthetnek a felhasználóknak a funkciók megismerésében.</span><span class="sxs-lookup"><span data-stu-id="8c240-151">Windows tips can be handy and help orient users when new features are released.</span></span>  <br/> |
|<span data-ttu-id="8c240-152">A Windows 10-es eszközök automatikus naprakészen tartása</span><span class="sxs-lookup"><span data-stu-id="8c240-152">Keep Windows 10 devices up to date automatically</span></span>  <br/> |<span data-ttu-id="8c240-153">Biztosítja, hogy a Windows 10-es eszközök automatikusan megkapják a legújabb frissítéseket.</span><span class="sxs-lookup"><span data-stu-id="8c240-153">Makes sure that Windows 10 devices automatically receive the latest updates.</span></span>  <br/> |
|<span data-ttu-id="8c240-154">Az eszköz képernyőjének kikapcsolása ennyi üresjárati idő után</span><span class="sxs-lookup"><span data-stu-id="8c240-154">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="8c240-p110">Biztosítja a céges adatok védelmét, amikor a felhasználó inaktív. Tegyük fel például, hogy a felhasználó nyilvános helyen, például egy kávézóban dolgozik. Ilyenkor, ha akár csak rövid időre is, de elvonhatják a figyelmét, és így illetéktelen személyek is láthatják az eszköz kijelzőjét. Ezzel a beállítással szabályozhatja, hogy a felhasználó mennyi ideig maradhat inaktív, mielőtt a kijelző kikapcsol.</span><span class="sxs-lookup"><span data-stu-id="8c240-p110">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
   
  


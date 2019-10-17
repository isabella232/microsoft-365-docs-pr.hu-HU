---
title: Eszközvédelmi beállítások megadása Windows 10-es PC-khez
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
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: bd66c26c-73a4-45a8-8642-3ea4ee7cd89d
description: Ismerje meg a Microsoft 365 Business rendszerben elérhető alapértelmezett és egyéb beállításokat a Windows 10 eszközök biztonságossá tétele érdekében.
ms.openlocfilehash: ab306e3d5a6011a0e7d537c98ecca6ef49ff82d9
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575758"
---
# <a name="set-device-protection-settings-for-windows-10-pcs"></a><span data-ttu-id="7252b-103">Eszközvédelmi beállítások megadása Windows 10-es PC-khez</span><span class="sxs-lookup"><span data-stu-id="7252b-103">Set device protection settings for Windows 10 PCs</span></span>

## <a name="secure-windows-10-devices"></a><span data-ttu-id="7252b-104">Windows 10-es eszközök védelme</span><span class="sxs-lookup"><span data-stu-id="7252b-104">Secure Windows 10 devices</span></span>

<span data-ttu-id="7252b-105">Nézze meg ezt a videót a Windows 10-es eszközök biztonságos használatáról a Microsoft 365 Business-szel:</span><span class="sxs-lookup"><span data-stu-id="7252b-105">View a video on how to secure Windows 10 devices with Microsoft 365 Business:</span></span>
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. <span data-ttu-id="7252b-106">Menj az admin központba <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span><span class="sxs-lookup"><span data-stu-id="7252b-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="7252b-107">Kattintson a bal oldali NAV \> **eszközházirendek** \> **hozzáadása**parancsára. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="7252b-107">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
  
3. <span data-ttu-id="7252b-108">A **Házirend felvétele** ablaktáblában adja meg a házirend egyedi nevét.</span><span class="sxs-lookup"><span data-stu-id="7252b-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="7252b-109">A **Házirend típusa** csoportban válassza a **Windows 10-es eszközök konfigurálása** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7252b-109">Under **Policy type**, choose **Windows 10 Device Configuration**.</span></span>
    
5. <span data-ttu-id="7252b-p101">Expand **Secure Windows 10 Devices** \> configure the settings how you would like. See [Available settings](#available-settings) for more information.</span><span class="sxs-lookup"><span data-stu-id="7252b-p101">Expand **Secure Windows 10 Devices** \> configure the settings how you would like. See [Available settings](#available-settings) for more information.</span></span> 
    
    <span data-ttu-id="7252b-112">Az **Alapértelmezett beállítások visszaállítása** hivatkozásra kattintva bármikor visszatérhet az alapértelmezett beállításokhoz.</span><span class="sxs-lookup"><span data-stu-id="7252b-112">You can alway use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Add policy pane with Windows 10 Device configuration selected](media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. <span data-ttu-id="7252b-p102">Next decide **Who will get these settings?** If you don't want to use the default **All users** security group, Choose **Change**, search for the security group who will get these settings \> **Select**.</span><span class="sxs-lookup"><span data-stu-id="7252b-p102">Next decide **Who will get these settings?** If you don't want to use the default **All users** security group, Choose **Change**, search for the security group who will get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="7252b-116">Végül válassza a **Kész** lehetőséget a házirend mentéséhez és eszközökhöz való hozzárendeléséhez.</span><span class="sxs-lookup"><span data-stu-id="7252b-116">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="7252b-117">Rendelkezésre álló beállítások</span><span class="sxs-lookup"><span data-stu-id="7252b-117">Available settings</span></span>

<span data-ttu-id="7252b-p103">Alapértelmezés szerint minden beállítás **be van kapcsolva**. Az alábbi beállítások érhetők el.</span><span class="sxs-lookup"><span data-stu-id="7252b-p103">By default all settings are **On**. The following settings are available.</span></span>
  
<span data-ttu-id="7252b-120">További információt [A Microsoft 365 Vállalati verzió védelmi funkcióinak megfelelő Intune-beállítások](map-protection-features-to-intune-settings.md) című cikk tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="7252b-120">See [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md) for more information.</span></span> 
  
|||
|:-----|:-----|
|<span data-ttu-id="7252b-121">Beállítás</span><span class="sxs-lookup"><span data-stu-id="7252b-121">Setting</span></span>  <br/> |<span data-ttu-id="7252b-122">Leírás</span><span class="sxs-lookup"><span data-stu-id="7252b-122">Description</span></span>  <br/> |
|<span data-ttu-id="7252b-123">PC-k védelme a vírusokkal és más fenyegetésekkel szemben a Windows Defender víruskereső használatával</span><span class="sxs-lookup"><span data-stu-id="7252b-123">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="7252b-124">Használatához a Windows Defender víruskeresőnek bekapcsolt állapotban kell lennie, hogy a PC-ket védeni lehessen az internetes kapcsolat során előforduló fenyegetésekkel szemben.</span><span class="sxs-lookup"><span data-stu-id="7252b-124">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="7252b-125">PC-k védelme a webes fenyegetésekkel szemben a Microsoft Edge böngészőben</span><span class="sxs-lookup"><span data-stu-id="7252b-125">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="7252b-126">Bekapcsolja a Microsoft Edge böngészőben azokat a beállításokat, amelyek segítenek megvédeni a felhasználót a kártékony webhelyek és letöltések által okozott veszélyektől.</span><span class="sxs-lookup"><span data-stu-id="7252b-126">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="7252b-127">Eszközök támadási felületét csökkentő szabályok használata</span><span class="sxs-lookup"><span data-stu-id="7252b-127">Use rules that reduce the attack surface of devices</span></span>  <br/> |<span data-ttu-id="7252b-p104">A támadásifelület-csökkentés bekapcsolásával letilthatók azok a műveletek és appok, amelyekkel a kártevők rendszerint megfertőzik az eszközöket. Ez a beállítás csak akkor használható, ha be van kapcsolva a Windows Defender víruskereső. További információ a [támadásifelület-csökkentésről](https://go.microsoft.com/fwlink/?linkid=870417).  </span><span class="sxs-lookup"><span data-stu-id="7252b-p104">When turned On, attack surface reduction helps block actions and apps typically used by malware to infect devices. This setting is only available if Windows Defender Antivirus is set to On. See [Reduce attack surfaces](https://go.microsoft.com/fwlink/?linkid=870417) to learn more.  </span></span><br/> |
|<span data-ttu-id="7252b-131">Mappák védelme a veszélyforrásokkal (például a zsarolóvírusokkal) szemben</span><span class="sxs-lookup"><span data-stu-id="7252b-131">Protect folders from threats such as ransomware</span></span>  <br/> |<span data-ttu-id="7252b-p105">Ez a beállítás szabályozott mappahozzáféréssel védi a céges adatokat a gyanús vagy kártékony appok (például a zsarolóvírusok) általi módosítástól azáltal, hogy nem engedélyezi nekik a védett mappákban tárolt adatok módosítását. Ez a beállítás csak akkor használható, ha be van kapcsolva a Windows Defender víruskereső. További információt a [Mappák védelme szabályozott mappahozzáféréssel](https://go.microsoft.com/fwlink/?linkid=870418) című cikkben talál.  </span><span class="sxs-lookup"><span data-stu-id="7252b-p105">This setting uses controlled folder access to protect company data from modification by suspicious or malicious apps, such as ransomware. These types of apps are blocked from making changes in protected folders. This setting is only available if Windows Defender Antivirus is set to On. See [Protect folders with COntrolled folder access](https://go.microsoft.com/fwlink/?linkid=870418) to learn more.  </span></span><br/> |
|<span data-ttu-id="7252b-136">Vélhetően kártékony internetes tartalmakhoz történő hálózati hozzáférés megakadályozása</span><span class="sxs-lookup"><span data-stu-id="7252b-136">Prevent network access to potentially malicious content on the Internet</span></span>  <br/> |<span data-ttu-id="7252b-p106">Ezzel a beállítással letilthatja a felhasználók kevésbé megbízható internetes helyekre irányuló kimenő kapcsolatait. Az ilyen helyeken adathalász kísérletekre, biztonsági résekre vagy más kártékony tartalmakra lehet számítani. Ez a beállítás csak akkor használható, ha be van kapcsolva a Windows Defender víruskereső. További információt [A hálózat védelme](https://go.microsoft.com/fwlink/?linkid=870419) című cikk tartalmaz.  </span><span class="sxs-lookup"><span data-stu-id="7252b-p106">Use this setting to block outbound user connections to low-reputation Internet locations that may host phishing scams, exploits or other malicious content. This setting is only available if Windows Defender Antivirus is set to On. See [Protect your network](https://go.microsoft.com/fwlink/?linkid=870419) for more information.  </span></span><br/> |
|<span data-ttu-id="7252b-140">PC-ken lévő fájlok és mappák illetéktelen hozzáféréssel szembeni védelme BitLocker-titkosítással</span><span class="sxs-lookup"><span data-stu-id="7252b-140">Help protect files and folders on PCs from unauthorized access with BitLocker</span></span>  <br/> |<span data-ttu-id="7252b-p107">A Bitlocker a számítógép merevlemezének titkosításával és a számítógép elvesztése vagy ellopása esetén az adatok kinyerése elleni védelemmel biztosítja adatai védelmét. További információt a [Bitlocker - gyakori kérdések](https://go.microsoft.com/fwlink/?linkid=871000) című cikk tartalmaz.  </span><span class="sxs-lookup"><span data-stu-id="7252b-p107">Bitlocker protects data by encrypting the computer hard drives and protect against data exposure if a computer is lost or stolen. See [Bitlocker FAQ](https://go.microsoft.com/fwlink/?linkid=871000) for more information.  </span></span><br/> |
|<span data-ttu-id="7252b-143">A felhasználók letölthetnek appokat innen: Microsoft Áruház</span><span class="sxs-lookup"><span data-stu-id="7252b-143">Allow users to download apps from Microsoft Store</span></span>  <br/> |<span data-ttu-id="7252b-p108">Lehetővé teszi, hogy a felhasználók appokat tölthessenek le és telepíthessenek a Microsoft Áruházból. Az appok között játékok és munkára használható eszközök egyaránt lehetnek, ezért ez a beállítás **Be** állapotban van, de a fokozott biztonság érdekében ki is kapcsolhatja.  </span><span class="sxs-lookup"><span data-stu-id="7252b-p108">Lets users download and install apps from the Microsoft Store. Apps include everything from games to productivity tools, so we leave this setting **On**, but you can turn it off for extra security.  </span></span><br/> |
|<span data-ttu-id="7252b-146">A felhasználók igénybe vehetik Cortana segítségét</span><span class="sxs-lookup"><span data-stu-id="7252b-146">Allow users to access Cortana</span></span>  <br/> |<span data-ttu-id="7252b-p109">Cortana nagyon hasznos lehet. Beállításokat képes be- és kikapcsolni, útbaigazítást tud adni, és ügyelni tud arra, hogy Ön ne késsen el a megbeszéléseiről, ezért ez a beállítás alapértelmezés szerint **Be** állapotban van.  </span><span class="sxs-lookup"><span data-stu-id="7252b-p109">Cortana can be very helpful! She can turn settings on or off for you, give directions, and make sure you're on time for appointments, so we keep this **On** by default.  </span></span><br/> |
|<span data-ttu-id="7252b-149">A felhasználók kaphatnak tippeket és hirdetéseket a Windowszal kapcsolatban a Microsofttól</span><span class="sxs-lookup"><span data-stu-id="7252b-149">Allow users to receive Windows tips and advertisements from Microsoft</span></span>  <br/> |<span data-ttu-id="7252b-150">A Windows-tippek hasznosak lehetnek, és új funkciók megjelenésekor segíthetnek a felhasználóknak a funkciók megismerésében.</span><span class="sxs-lookup"><span data-stu-id="7252b-150">Windows tips can be handy and help orient users when new features are released.</span></span>  <br/> |
|<span data-ttu-id="7252b-151">A Windows 10-es eszközök automatikus naprakészen tartása</span><span class="sxs-lookup"><span data-stu-id="7252b-151">Keep Windows 10 devices up to date automatically</span></span>  <br/> |<span data-ttu-id="7252b-152">Biztosítja, hogy a Windows 10-es eszközök automatikusan megkapják a legújabb frissítéseket.</span><span class="sxs-lookup"><span data-stu-id="7252b-152">Makes sure that Windows 10 devices automatically receive the latest updates.</span></span>  <br/> |
|<span data-ttu-id="7252b-153">Az eszköz képernyőjének kikapcsolása ennyi üresjárati idő után</span><span class="sxs-lookup"><span data-stu-id="7252b-153">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="7252b-p110">Biztosítja a céges adatok védelmét, amikor a felhasználó inaktív. Előfordulhat, hogy a felhasználó nyilvános helyen, például egy kávézóban végez munkát, és ilyenkor ha csak rövid időre is elvonják a figyelmét az eszközről, akkor annak kijelzőjét illetéktelen személyek is láthatják. Ezzel a beállítással azt határozhatja meg, hogy a felhasználó mennyi ideig maradhat inaktív, mielőtt az eszköz kijelzője kikapcsol.</span><span class="sxs-lookup"><span data-stu-id="7252b-p110">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
   
  


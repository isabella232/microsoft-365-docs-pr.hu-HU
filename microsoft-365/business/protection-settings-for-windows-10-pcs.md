---
title: Eszközvédelmi beállítások megadása Windows 10-es PC-khez
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
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: bd66c26c-73a4-45a8-8642-3ea4ee7cd89d
description: Ismerje meg a Microsoft 365 vállalati verzióban a Windows 10-es eszközök védelmére szolgáló alapértelmezett és egyéb beállításokat.
ms.openlocfilehash: a3b7f0a8572a215491b32101a30c306b54571b6f
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/21/2020
ms.locfileid: "43633017"
---
# <a name="set-device-protection-settings-for-windows-10-pcs"></a>Eszközvédelmi beállítások megadása Windows 10-es PC-khez

## <a name="secure-windows-10-devices"></a>Windows 10-es eszközök védelme

Tekintse meg a Windows 10-eszközök microsoft 365 vállalati verzióval való védelméről szóló videót:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. Nyissa meg a <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>felügyeleti központot a alkalmazásban. 
    
2. A bal oldali navigációs sávon válassza az \> **Eszközházirendek** \> **hozzáadása lehetőséget.** **Devices**
  
3. A **Házirend felvétele** ablaktáblában adja meg a házirend egyedi nevét. 
    
4. A **Házirend típusa** csoportban válassza a **Windows 10-es eszközök konfigurálása** lehetőséget.
    
5. Expand **Secure Windows 10 Devices** \> configure the settings how you would like. További információt az [Elérhető beállítások című témakörben talál.](#available-settings) 
    
    Az **Alapértelmezett beállítások visszaállítása** hivatkozásra kattintva bármikor visszatérhet az alapértelmezett beállításokhoz. 
    
    ![Add policy pane with Windows 10 Device configuration selected](../media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. Next decide **Who will get these settings?** If you don't want to use the default **All users** security group, Choose **Change**, search for the security group who will get these settings \> **Select**.
    
7. Végül válassza a **Kész** lehetőséget a házirend mentéséhez és eszközökhöz való hozzárendeléséhez. 
    
## <a name="available-settings"></a>Rendelkezésre álló beállítások

Alapértelmezés szerint minden beállítás **be van kapcsolva**. Az alábbi beállítások érhetők el.
  
További információt a [Microsoft 365 Premium szolgáltatás védelmi szolgáltatásai nak az Intune beállításaihoz című témakörben talál.](map-protection-features-to-intune-settings.md) 
  
|||
|:-----|:-----|
|Beállítás  <br/> |Leírás  <br/> |
|PC-k védelme a vírusokkal és más fenyegetésekkel szemben a Windows Defender víruskereső használatával  <br/> |Használatához a Windows Defender víruskeresőnek bekapcsolt állapotban kell lennie, hogy a PC-ket védeni lehessen az internetes kapcsolat során előforduló fenyegetésekkel szemben.  <br/> |
|PC-k védelme a webes fenyegetésekkel szemben a Microsoft Edge böngészőben  <br/> |Bekapcsolja a Microsoft Edge böngészőben azokat a beállításokat, amelyek segítenek megvédeni a felhasználót a kártékony webhelyek és letöltések által okozott veszélyektől.  <br/> |
|Eszközök támadási felületét csökkentő szabályok használata  <br/> |A támadásifelület-csökkentés bekapcsolásával letilthatók azok a műveletek és appok, amelyekkel a kártevők rendszerint megfertőzik az eszközöket. Ez a beállítás csak akkor használható, ha be van kapcsolva a Windows Defender víruskereső. További információ a [támadásifelület-csökkentésről](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/exploit-protection).  <br/> |
|Mappák védelme a veszélyforrásokkal (például a zsarolóvírusokkal) szemben  <br/> |Ez a beállítás ellenőrzött mappahozzáférést használ, hogy megvédje a vállalati adatokat a gyanús vagy rosszindulatú alkalmazások, például zsarolóprogramok általi módosításokkal szemben. Az ilyen típusú alkalmazások nem módosíthatják a védett mappákat. Ez a beállítás csak akkor használható, ha be van kapcsolva a Windows Defender víruskereső. További [információ: Mappák védelme ellenőrzött mappákkal.](https://docs.microsoft.com/configmgr/protect/deploy-use/create-deploy-exploit-guard-policy#bkmk_CFA)  <br/> |
|Vélhetően kártékony internetes tartalmakhoz történő hálózati hozzáférés megakadályozása  <br/> |Ezzel a beállítással letilthatja a kimenő felhasználói kapcsolatokat az alacsony hírnévvel rendelkező internetes helyekre, amelyek adathalász csalásokat, biztonsági réseket vagy más rosszindulatú tartalmat tartalmazhatnak. Ez a beállítás csak akkor érhető **On**el, ha a Windows Defender víruskereső be van kapcsolva. További információt [a Hálózat védelme](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/configure-real-time-protection-windows-defender-antivirus)című témakörben talál.  <br/> |
|PC-ken lévő fájlok és mappák illetéktelen hozzáféréssel szembeni védelme BitLocker-titkosítással  <br/> |A Bitlocker a számítógép merevlemezének titkosításával és a számítógép elvesztése vagy ellopása esetén az adatok kinyerése elleni védelemmel biztosítja adatai védelmét. További információ: [Bitlocker GYIK](https://go.microsoft.com/fwlink/?linkid=871000).  <br/> |
|A felhasználók letölthetnek appokat innen: Microsoft Áruház  <br/> |Lehetővé teszi, hogy a felhasználók appokat tölthessenek le és telepíthessenek a Microsoft Áruházból. Az appok között játékok és munkára használható eszközök egyaránt lehetnek, ezért ez a beállítás **Be** állapotban van, de a fokozott biztonság érdekében ki is kapcsolhatja.  <br/> |
|A felhasználók igénybe vehetik Cortana segítségét  <br/> |Cortana nagyon hasznos lehet. Cortana be- és kikapcsolhatja a beállításokat, útbaigazítást adhat, és meggyőződhet arról, hogy időben van a találkozókhoz, ezért alapértelmezés szerint **bekapcsolva** tartjuk ezt a beállítást.  <br/> |
|A felhasználók kaphatnak tippeket és hirdetéseket a Windowszal kapcsolatban a Microsofttól  <br/> |A Windows-tippek hasznosak lehetnek, és új funkciók megjelenésekor segíthetnek a felhasználóknak a funkciók megismerésében.  <br/> |
|A Windows 10-es eszközök automatikus naprakészen tartása  <br/> |Biztosítja, hogy a Windows 10-es eszközök automatikusan megkapják a legújabb frissítéseket.  <br/> |
|Az eszköz képernyőjének kikapcsolása ennyi üresjárati idő után  <br/> |Biztosítja a céges adatok védelmét, amikor a felhasználó inaktív. Előfordulhat, hogy a felhasználó nyilvános helyen, például egy kávézóban végez munkát, és ilyenkor ha csak rövid időre is elvonják a figyelmét az eszközről, akkor annak kijelzőjét illetéktelen személyek is láthatják. Ezzel a beállítással azt határozhatja meg, hogy a felhasználó mennyi ideig maradhat inaktív, mielőtt az eszköz kijelzője kikapcsol.  <br/> |

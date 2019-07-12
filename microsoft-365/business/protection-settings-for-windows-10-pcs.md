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
search.appverid:
- BCS160
- MET150
ms.assetid: bd66c26c-73a4-45a8-8642-3ea4ee7cd89d
description: Alapértelmezett és más Microsoft 365 üzleti Windows 10 eszközök biztonságos beállítások ismertetése
ms.openlocfilehash: 844bddc4b93c7dc543ad6c6a79f5cf92c96ceff0
ms.sourcegitcommit: 0c1227dc79b66bab529bf178c5672791369ba471
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35630609"
---
# <a name="set-device-protection-settings-for-windows-10-pcs"></a>Eszközvédelmi beállítások megadása Windows 10-es PC-khez

## <a name="secure-windows-10-devices"></a>Windows 10-es eszközök védelme

Nézze meg ezt a videót a Windows 10-es eszközök biztonságos használatáról a Microsoft 365 Business-szel:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. Ugrás az admin center <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>. 
    
2. A bal oldali navigációs sáv, válassza az **eszközök** \> **politika** \> **hozzáadása**.
  
3. A **Házirend felvétele** ablaktáblában adja meg a házirend egyedi nevét. 
    
4. A **Házirend típusa** csoportban válassza a **Windows 10-es eszközök konfigurálása** lehetőséget.
    
5. Expand **Secure Windows 10 Devices** \> configure the settings how you would like. See [Available settings](#available-settings) for more information. 
    
    Az **Alapértelmezett beállítások visszaállítása** hivatkozásra kattintva bármikor visszatérhet az alapértelmezett beállításokhoz. 
    
    ![Add policy pane with Windows 10 Device configuration selected](media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. Next decide **Who will get these settings?** If you don't want to use the default **All users** security group, Choose **Change**, search for the security group who will get these settings \> **Select**.
    
7. Végül válassza a **Kész** lehetőséget a házirend mentéséhez és eszközökhöz való hozzárendeléséhez. 
    
## <a name="available-settings"></a>Rendelkezésre álló beállítások

Alapértelmezés szerint minden beállítás **be van kapcsolva**. Az alábbi beállítások érhetők el.
  
További információt [A Microsoft 365 Vállalati verzió védelmi funkcióinak megfelelő Intune-beállítások](map-protection-features-to-intune-settings.md) című cikk tartalmaz. 
  
|||
|:-----|:-----|
|Beállítás  <br/> |Leírás  <br/> |
|PC-k védelme a vírusokkal és más fenyegetésekkel szemben a Windows Defender víruskereső használatával  <br/> |Használatához a Windows Defender víruskeresőnek bekapcsolt állapotban kell lennie, hogy a PC-ket védeni lehessen az internetes kapcsolat során előforduló fenyegetésekkel szemben.  <br/> |
|PC-k védelme a webes fenyegetésekkel szemben a Microsoft Edge böngészőben  <br/> |Bekapcsolja a Microsoft Edge böngészőben azokat a beállításokat, amelyek segítenek megvédeni a felhasználót a kártékony webhelyek és letöltések által okozott veszélyektől.  <br/> |
|Eszközök támadási felületét csökkentő szabályok használata  <br/> |A támadásifelület-csökkentés bekapcsolásával letilthatók azok a műveletek és appok, amelyekkel a kártevők rendszerint megfertőzik az eszközöket. Ez a beállítás csak akkor használható, ha be van kapcsolva a Windows Defender víruskereső. További információ a [támadásifelület-csökkentésről](https://go.microsoft.com/fwlink/?linkid=870417).  <br/> |
|Mappák védelme a veszélyforrásokkal (például a zsarolóvírusokkal) szemben  <br/> |Ez a beállítás szabályozott mappahozzáféréssel védi a céges adatokat a gyanús vagy kártékony appok (például a zsarolóvírusok) általi módosítástól azáltal, hogy nem engedélyezi nekik a védett mappákban tárolt adatok módosítását. Ez a beállítás csak akkor használható, ha be van kapcsolva a Windows Defender víruskereső. További információt a [Mappák védelme szabályozott mappahozzáféréssel](https://go.microsoft.com/fwlink/?linkid=870418) című cikkben talál.  <br/> |
|Vélhetően kártékony internetes tartalmakhoz történő hálózati hozzáférés megakadályozása  <br/> |Ezzel a beállítással letilthatja a felhasználók kevésbé megbízható internetes helyekre irányuló kimenő kapcsolatait. Az ilyen helyeken adathalász kísérletekre, biztonsági résekre vagy más kártékony tartalmakra lehet számítani. Ez a beállítás csak akkor használható, ha be van kapcsolva a Windows Defender víruskereső. További információt [A hálózat védelme](https://go.microsoft.com/fwlink/?linkid=870419) című cikk tartalmaz.  <br/> |
|PC-ken lévő fájlok és mappák illetéktelen hozzáféréssel szembeni védelme BitLocker-titkosítással  <br/> |A Bitlocker a számítógép merevlemezének titkosításával és a számítógép elvesztése vagy ellopása esetén az adatok kinyerése elleni védelemmel biztosítja adatai védelmét. További információt a [Bitlocker - gyakori kérdések](https://go.microsoft.com/fwlink/?linkid=871000) című cikk tartalmaz.  <br/> |
|A felhasználók letölthetnek appokat innen: Microsoft Áruház  <br/> |Lehetővé teszi, hogy a felhasználók appokat tölthessenek le és telepíthessenek a Microsoft Áruházból. Az appok között játékok és munkára használható eszközök egyaránt lehetnek, ezért ez a beállítás **Be** állapotban van, de a fokozott biztonság érdekében ki is kapcsolhatja.  <br/> |
|A felhasználók igénybe vehetik Cortana segítségét  <br/> |Cortana nagyon hasznos lehet. Beállításokat képes be- és kikapcsolni, útbaigazítást tud adni, és ügyelni tud arra, hogy Ön ne késsen el a megbeszéléseiről, ezért ez a beállítás alapértelmezés szerint **Be** állapotban van.  <br/> |
|A felhasználók kaphatnak tippeket és hirdetéseket a Windowszal kapcsolatban a Microsofttól  <br/> |A Windows-tippek hasznosak lehetnek, és új funkciók megjelenésekor segíthetnek a felhasználóknak a funkciók megismerésében.  <br/> |
|A Windows 10-es eszközök automatikus naprakészen tartása  <br/> |Biztosítja, hogy a Windows 10-es eszközök automatikusan megkapják a legújabb frissítéseket.  <br/> |
|Az eszköz képernyőjének kikapcsolása ennyi üresjárati idő után  <br/> |Biztosítja a céges adatok védelmét, amikor a felhasználó inaktív. Előfordulhat, hogy a felhasználó nyilvános helyen, például egy kávézóban végez munkát, és ilyenkor ha csak rövid időre is elvonják a figyelmét az eszközről, akkor annak kijelzőjét illetéktelen személyek is láthatják. Ezzel a beállítással azt határozhatja meg, hogy a felhasználó mennyi ideig maradhat inaktív, mielőtt az eszköz kijelzője kikapcsol.  <br/> |
   
  


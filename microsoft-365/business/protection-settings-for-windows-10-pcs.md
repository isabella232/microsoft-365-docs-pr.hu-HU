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
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982145"
---
# <a name="set-device-protection-settings-for-windows-10-pcs"></a>Eszközvédelmi beállítások megadása Windows 10-es PC-khez

## <a name="secure-windows-10-devices"></a>Windows 10-es eszközök védelme

Nézze meg ezt a videót a Windows 10-es eszközök biztonságos használatáról a Microsoft 365 Business-szel:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. Jelentkezzen be a [Microsoft 365 Business](https://portal.office.com) szolgáltatásba globális rendszergazdai hitelesítő adatokkal. 
    
2. A felügyeleti központ **Eszközházirendek** kártyáján válassza a **Házirend felvétele** lehetőséget.
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. A **Házirend felvétele** ablaktáblában adja meg a házirend egyedi nevét. 
    
4. A **Házirend típusa** csoportban válassza a **Windows 10-es eszközök konfigurálása** lehetőséget.
    
5. Bontsa ki a **Windows 10 eszközök biztonságos** \> hogyan szeretné a beállításokat. További tudnivalókért tanulmányozza a [rendelkezésre álló beállításokat](protection-settings-for-windows-10-pcs.md#bkmk_availablesettings) . 
    
    Az **Alapértelmezett beállítások visszaállítása** hivatkozásra kattintva bármikor visszatérhet az alapértelmezett beállításokhoz. 
    
    ![Add policy pane with Windows 10 Device configuration selected](media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. Ezután döntse el, **fog kapni, akik ezeket a beállításokat?** Ha nem szeretné használni az alapértelmezett **minden felhasználó** biztonsági csoport, válassza ki a **Módosítás**, keresse meg a biztonsági csoportot, akik ezeket a beállításokat kap \> **kiválasztása**.
    
7. Végül válassza a **Kész** lehetőséget a házirend mentéséhez és eszközökhöz való hozzárendeléséhez. 
    
## <a name="available-settings"></a>Rendelkezésre álló beállítások

Alapértelmezés szerint minden beállítás **be van kapcsolva**. Az alábbi beállítások érhetők el.
  
További információt [A Microsoft 365 Vállalati verzió védelmi funkcióinak megfelelő Intune-beállítások](map-protection-features-to-intune-settings.md) című cikk tartalmaz. 
  
|||
|:-----|:-----|
|Beállítás  <br/> |Leírás  <br/> |
|PC-k védelme a vírusokkal és más fenyegetésekkel szemben a Windows Defender víruskereső használatával  <br/> |Használatához a Windows Defender víruskeresőnek bekapcsolt állapotban kell lennie, hogy védelmet nyújthasson a PC-knek az internethez csatlakozva jelentkező veszélyekkel szemben.  <br/> |
|PC-k védelme a webes fenyegetésekkel szemben a Microsoft Edge böngészőben  <br/> |Bekapcsolja a Microsoft Edge böngészőben azokat a beállításokat, amelyek segítenek megvédeni a felhasználót a kártékony webhelyek és letöltések által okozott veszélyektől.  <br/> |
|Eszközök támadási felületét csökkentő szabályok használata  <br/> |A támadásifelület-csökkentés bekapcsolásával letilthatók azok a műveletek és appok, amelyekkel a kártevők rendszerint megfertőzik az eszközöket. Ez a beállítás csak akkor használható, ha be van kapcsolva a Windows Defender víruskereső. További információ a [támadásifelület-csökkentésről](https://go.microsoft.com/fwlink/?linkid=870417).  <br/> |
|Mappák védelme a veszélyforrásokkal (például a zsarolóvírusokkal) szemben  <br/> |Ez a beállítás szabályozott mappahozzáféréssel védi a céges adatokat a gyanús vagy kártékony appok (például a zsarolóvírusok) általi módosítástól azáltal, hogy nem engedélyezi nekik a védett mappákban tárolt adatok módosítását. Ez a beállítás csak akkor használható, ha be van kapcsolva a Windows Defender víruskereső. További információt a [Mappák védelme szabályozott mappahozzáféréssel](https://go.microsoft.com/fwlink/?linkid=870418) című cikkben talál.  <br/> |
|Vélhetően kártékony internetes tartalmakhoz történő hálózati hozzáférés megakadályozása  <br/> |Ezzel a beállítással letilthatja a felhasználók kevésbé megbízható internetes helyekre irányuló kimenő kapcsolatait. Az ilyen helyeken adathalász kísérletekre, biztonsági résekre vagy más kártékony tartalmakra lehet számítani. Ez a beállítás csak akkor használható, ha be van kapcsolva a Windows Defender víruskereső. További információt [A hálózat védelme](https://go.microsoft.com/fwlink/?linkid=870419) című cikk tartalmaz.  <br/> |
|PC-ken lévő fájlok és mappák illetéktelen hozzáféréssel szembeni védelme BitLocker-titkosítással  <br/> |A Bitlocker a számítógép merevlemezének titkosításával és a számítógép elvesztése vagy ellopása esetén az adatok kinyerése elleni védelemmel biztosítja adatai védelmét. További információt a [Bitlocker - gyakori kérdések](https://go.microsoft.com/fwlink/?linkid=871000) című cikk tartalmaz.  <br/> |
|A felhasználók letölthetnek appokat innen: Microsoft Áruház  <br/> |Lehetővé teszi, hogy a felhasználók appokat tölthessenek le és telepíthessenek a Microsoft Áruházból. Az appok között játékok és munkára használható eszközök egyaránt lehetnek, ezért ez a beállítás **Be** állapotban van, de a fokozott biztonság érdekében ki is kapcsolhatja.  <br/> |
|A felhasználók igénybe vehetik Cortana segítségét  <br/> |Cortana nagyon hasznos lehet. Beállításokat képes be- és kikapcsolni, útbaigazítást tud adni, és ügyelni tud arra, hogy Ön ne késsen el a megbeszéléseiről, ezért ez a beállítás alapértelmezés szerint **Be** állapotban van.  <br/> |
|A felhasználók kaphatnak tippeket és hirdetéseket a Windowszal kapcsolatban a Microsofttól  <br/> |A Windows-tippek hasznosak lehetnek, és új funkciók megjelenésekor segíthetnek a felhasználóknak a funkciók megismerésében.  <br/> |
|A Windows 10-es eszközök automatikus naprakészen tartása  <br/> |Biztosítja, hogy a Windows 10-es eszközök automatikusan megkapják a legújabb frissítéseket.  <br/> |
|Az eszköz képernyőjének kikapcsolása ennyi üresjárati idő után  <br/> |Biztosítja a céges adatok védelmét, amikor a felhasználó inaktív. Tegyük fel például, hogy a felhasználó nyilvános helyen, például egy kávézóban dolgozik. Ilyenkor, ha akár csak rövid időre is, de elvonhatják a figyelmét, és így illetéktelen személyek is láthatják az eszköz kijelzőjét. Ezzel a beállítással szabályozhatja, hogy a felhasználó mennyi ideig maradhat inaktív, mielőtt a kijelző kikapcsol.  <br/> |
   
  


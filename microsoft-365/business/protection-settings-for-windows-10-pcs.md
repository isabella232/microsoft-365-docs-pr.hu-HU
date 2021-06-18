---
title: Eszközvédelmi beállítások szerkesztése vagy létrehozása Windows 10 PC-khez
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: bd66c26c-73a4-45a8-8642-3ea4ee7cd89d
description: Ismerje meg a Vállalati verzióban Microsoft 365 beállításokat az Windows 10 biztonságának érdekében.
ms.openlocfilehash: 4859681d5e71a61b8a5dd58114bce899f485967a
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/14/2021
ms.locfileid: "52925319"
---
# <a name="edit-or-create-device-protection-settings-for-windows-10-pcs"></a>Eszközvédelmi beállítások szerkesztése vagy létrehozása Windows 10 PC-khez

Ez a cikk a Microsoft 365 Vállalati prémium verzió.

Miután beállította az alapértelmezett Windows beállítási beállításokat a Beállítás lapon, felvehet újakat, amelyek az összes felhasználóra vagy egy felhasználókészletre vonatkoznak. A létrehozottakat szerkesztheti is.

## <a name="create-protection-settings-for-windows-10-devices"></a>Védelmi beállítások létrehozása Windows 10 eszközökhöz

Nézze meg ezt a videót, amely bemutatja, hogy miként Windows 10 eszközökhöz a Microsoft 365 Vállalati prémium verzió:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. A felügyeleti központ megnyitásához: <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> . 
2. A bal oldali navigációs sávon válassza az **Eszköz** \> **házirendek hozzáadása** \> **lehetőséget.**
3. A **Házirend felvétele** ablaktáblában adja meg a házirend egyedi nevét. 
4. A **Házirend típusa** csoportban válassza a **Windows 10-es eszközök konfigurálása** lehetőséget.
5. Expand **Secure Windows 10 Devices** \> configure the settings how you would like. További információt a Rendelkezésre álló [beállítások lapon található.](#available-settings) 
    
    Az **Alapértelmezett beállítások visszaállítása** hivatkozásra kattintva bármikor visszatérhet az alapértelmezett beállításokhoz. 
    
    ![Add policy pane with Windows 10 Device configuration selected](../media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. Next decide **Who will get these settings?** If you don't want to use the default **All users** security group, Choose **Change**, search for the security group who will get these settings \> **Select**.
7. Végül válassza a **Kész** lehetőséget a házirend mentéséhez és eszközökhöz való hozzárendeléséhez. 

## <a name="edit-windows-10-protection-settings"></a>A Windows 10 védelmi beállítások szerkesztése
 
1. A felügyeleti központ megnyitásához: <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .     
2. A bal oldali  navigációs sávon válassza az Eszköz \> **házirendek lehetőséget.**
1. Válasszon ki egy meglévő Windows eszköz házirendet, majd a **Szerkesztés gombra.**
1. Válassza **a Szerkesztés** lehetőséget a módosítani kívánt beállítás mellett, majd a Mentés **gombra.**

## <a name="available-settings"></a>Rendelkezésre álló beállítások

Alapértelmezés szerint minden beállítás **be van kapcsolva**. Az alábbi beállítások érhetők el.
  
További információt a Hogyan használhatja a védelmi funkciókat az [Microsoft 365 Prémium Intune-beállításoknak?](map-protection-features-to-intune-settings.md)lapon található. 


|Beállítás  <br/> |Leírás  <br/> |
|:-----|:-----|
|PC-k védelme a vírusokkal és más fenyegetésekkel szemben a Windows Defender víruskereső használatával  <br/> |Használatához a Windows Defender víruskeresőnek bekapcsolt állapotban kell lennie, hogy a PC-ket védeni lehessen az internetes kapcsolat során előforduló fenyegetésekkel szemben.  <br/> |
|PC-k védelme a webes fenyegetésekkel szemben a Microsoft Edge böngészőben  <br/> |Bekapcsolja a Microsoft Edge böngészőben azokat a beállításokat, amelyek segítenek megvédeni a felhasználót a kártékony webhelyek és letöltések által okozott veszélyektől.  <br/> |
|Eszközök támadási felületét csökkentő szabályok használata  <br/> |A támadásifelület-csökkentés bekapcsolásával letilthatók azok a műveletek és appok, amelyekkel a kártevők rendszerint megfertőzik az eszközöket. Ez a beállítás csak akkor használható, ha be van kapcsolva a Windows Defender víruskereső. További információ a [támadásifelület-csökkentésről](/windows/security/threat-protection/microsoft-defender-atp/exploit-protection).  <br/> |
|Mappák védelme a veszélyforrásokkal (például a zsarolóvírusokkal) szemben  <br/> |Ez a beállítás szabályozott mappaelérést használva védi a céges adatokat a gyanús vagy kártékony appok, például a zsarolóvírusok módosításaitól. Az ilyen típusú alkalmazások nem módosíthatnak védett mappákat. Ez a beállítás csak akkor használható, ha be van kapcsolva a Windows Defender víruskereső. További [információt a Mappák védelme mappaelérés szabályozott](/mem/configmgr/protect/deploy-use/create-deploy-exploit-guard-policy#bkmk_CFA) hozzáféréssel.  <br/> |
|Vélhetően kártékony internetes tartalmakhoz történő hálózati hozzáférés megakadályozása  <br/> |Ezzel a beállítással letilthatja az adathalászatot, biztonsági rést vagy más kártékony tartalmat tároló, alacsony jó hírű internetes helyekre irányuló kimenő felhasználói kapcsolatokat. Ez a beállítás csak akkor érhető el, Windows Defender víruskereső be van **állítva.** További információ: [A hálózat védelme.](/windows/security/threat-protection/windows-defender-antivirus/configure-real-time-protection-windows-defender-antivirus)  <br/> |
|PC-ken lévő fájlok és mappák illetéktelen hozzáféréssel szembeni védelme BitLocker-titkosítással  <br/> |A Bitlocker a számítógép merevlemezének titkosításával és a számítógép elvesztése vagy ellopása esetén az adatok kinyerése elleni védelemmel biztosítja adatai védelmét. További információt a Bitlocker – gyakori [kérdések című témakörben talál.](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions)  <br/> |
|A felhasználók letölthetnek appokat innen: Microsoft Áruház  <br/> |Lehetővé teszi, hogy a felhasználók appokat tölthessenek le és telepíthessenek a Microsoft Áruházból. Az appok között játékok és munkára használható eszközök egyaránt lehetnek, ezért ez a beállítás **Be** állapotban van, de a fokozott biztonság érdekében ki is kapcsolhatja.  <br/> |
|A felhasználók igénybe vehetik Cortana segítségét  <br/> |Cortana nagyon hasznos lehet. Cortana be- és kikapcsolhatja a beállításokat, útvonaltervet adhat, és biztosíthatja, hogy időben legyen  a találkozókhoz, ezért ez a beállítás alapértelmezés szerint Be van kapcsolva.  <br/> |
|A felhasználók kaphatnak tippeket és hirdetéseket a Windowszal kapcsolatban a Microsofttól  <br/> |A Windows-tippek hasznosak lehetnek, és új funkciók megjelenésekor segíthetnek a felhasználóknak a funkciók megismerésében.  <br/> |
|A Windows 10-es eszközök automatikus naprakészen tartása  <br/> |Biztosítja, hogy a Windows 10-es eszközök automatikusan megkapják a legújabb frissítéseket.  <br/> |
|Az eszköz képernyőjének kikapcsolása ennyi üresjárati idő után  <br/> |Biztosítja a céges adatok védelmét, amikor a felhasználó inaktív. Előfordulhat, hogy a felhasználó nyilvános helyen, például egy kávézóban végez munkát, és ilyenkor ha csak rövid időre is elvonják a figyelmét az eszközről, akkor annak kijelzőjét illetéktelen személyek is láthatják. Ezzel a beállítással azt határozhatja meg, hogy a felhasználó mennyi ideig maradhat inaktív, mielőtt az eszköz kijelzője kikapcsol.  <br/> |
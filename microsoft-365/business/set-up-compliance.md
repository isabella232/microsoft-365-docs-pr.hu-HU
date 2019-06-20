---
title: Fenyegetés növelhető a Microsoft 365 üzleti
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
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
description: Állítsa be az Office 365 speciális veszély védelmi, és a bizalmas adatok védelme.
ms.openlocfilehash: 53741a7726222bb32329a401953be72257df95cc
ms.sourcegitcommit: 7ac06563c6ff034358e8fd3f9298fc426187ade2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/31/2019
ms.locfileid: "35086342"
---
# <a name="set-up-compliance-features"></a>E szolgáltatások beállítása

A Microsoft 365 üzleti adatok és berendezések védelmét, és folyamatosan, Ön és a felhasználók bizalmas adatok biztonságos szolgáltatásokat tartalmaz.

## <a name="set-up-dlp-features"></a>DLP szolgáltatások beállítása

[Sablonból DLP házirend létrehozása](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) ellen személyhez köthető adatot Gyűjtenek a házirend beállításával kapcsolatos példát talál. 
  
DLP számos kész használható sablonok számos különböző nyelvhez tartalmaz. Például a pénzügyi adatok Ausztrália, Kanada személyes információ törvény, amerikai pénzügyi adatok, stb. Teljes listájához lásd a [Mi a DLP sablonokat tartalmazza](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) . Az összes ezeket a sablonokat lehet engedélyezni a Gyűjtenek sablon példára hasonlít. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>E-mail adatmegőrzési az Exchange Online archiválás beállítása

 **Exchange Online archiválás** licencéhez tartozó szolgáltatások fenntartása érdekében megfelelőségi és szabályozási előírások által e-mail megőrzésére szánt elektronikus adatok feltárása. Is csökkenthető a kockázat esetén peres és biztosítja az adatbiztonság megsértése után, vagy ha a törölt elemek kell helyreállítani az adatokat. Per tartsa használja az összes felhasználói tartalom megőrzése érdekében, vagy testre szeretné megőrizni az adatmegőrzési szabályok segítségével.
  
**Per tartás:** Minden postaláda-tartalom helyezi a felhasználó teljes postaláda peres eljárás beleértve törölt elemek tárolására képes megőrizni. 
    
Helyezze egy postaláda peres eljárás felfüggesztése a felügyeleti központ:
    
1. A bal oldali navigációs sáv, keresse meg **a felhasználók** \> **aktív felhasználók**.
    
2. Jelöljön ki egy felhasználót, akinek el szeretné helyezni a per postaláda tartsa és a felhasználó ablaktáblában bontsa ki a **levelezési beállításokat** , és **További beállítások** mellett válassza a **Tulajdonságok szerkesztése Exchange**.
    
3. A felhasználó postaláda lapon válassza ki ** postaláda szolgáltatások ** kattintson a bal oldali navigációs sáv, és válassza ki a **per tartsa** **engedélyezése** hivatkozásra.
    
4. **Per tartsa** párbeszédpanelen megadhatja, hogy a per tartás időtartama a **per tartás időtartama** mezőben, a mezőt hagyja üresen, ha el szeretné helyezni egy végtelen tartsa. Is megjegyzéseket és közvetlen mail lista tulajdonosa egy webhelyre, előfordulhat, hogy tartsa a per bővebben magyarázatot kell \> **mentése**.
    
**Retenciós:** Egyéni adatmegőrzési szabályok, például engedélyezheti egy adott meghatározott ideig megőrizni és tartalom véglegesen törli a birtokon tartási időszak végén. További [adatmegőrzési szabályok – áttekintés](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423)című témakörben talál.

## <a name="set-up-azure-information-protection-features"></a>Információvédelem Azure szolgáltatások beállítása

Borzas információk védelme (AIP) segít osztályozására és a dokumentumok és e-mailek, esetleg védelme címkék alkalmazásával. Címkék automatikusan alkalmazhatók, a rendszergazdák, akik a szabályokat és feltételeket határozza meg, kézzel felhasználók, vagy együttesének felhasználásával, ahol a felhasználók kapnak ajánlásokat.

Az Outlook programban a weben alkalmazhatja az e-mailek a következő beépített feliratok és korlátozások:
  
- **Nem továbbítandó**: címzettek is olvashassák az üzenetet, de nem továbbíthatják, nyomtatás, másolhatják a tartalmat
    
- **Titkosítás**: A teljes üzenet titkosítva van. Címzettek a titkosított tartalom elérése előtt meg kell erősítenie az identitásukat és titkosítása nem távolítható el.
    
- **Bizalmas**: a szervezet alkalmazottainak teljes engedélyt ad az e-mail tartalom és mellékletek, de nem a szervezeten kívülieknek. Adatok tulajdonosai nyomon követheti és tartalmat bármikor visszavonhatja.
    
- **Nagyon bizalmas**: Ez a korlátozás nagyon bizalmas adatok, amely lehetővé teszi az alkalmazottak megtekintése, szerkesztése, és válaszolni, de nem továbbítása, nyomtatása vagy másolja az adatokat lehet alkalmazni. Adatok tulajdonosai nyomon követheti és tartalmat bármikor visszavonhatja.

### <a name="make-sure-azure-information-protection-is-activated"></a>Ellenőrizze, hogy aktív Azure információk védelméről

Ellenőrizze, hogy aktiválva van-e az AIP:

1. [Borzas portal](https://portal.azure.com/)bejelentkezni.

2. Jelölje be a **minden szolgáltatás** és típus *Azure információk védelméről* a **Keresés mezőbe**.

3. Után az eredmények megjelenítéséhez kattintson a következő teszi a kedvenc **Azure információk védelméről** és könnyen megjegyezhető kezdete.

4. Válassza ki az **Azure információk védelméről** \> **védelem aktiválás** , és győződjön meg arról, hogy ez a beállítás, aktivált. 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a>Az információk védelméről Azure házirendet és az alapértelmezett címkék megjelenítése 

Megtekintése és módosítása, hogy a meglévő címkék:

1. Válassza az Azure információvédelem irányítópult **osztályozások** \> **címkék**. <br/>![Szabványos címkék Azure információ védelme.](media/AIPLabels.png)

2. Megadhatja, hogy minden címke beállításainak megtekintéséhez, megváltoztathatja a megjelenítési név, szín, stb.
 
3. Lásd: [Módosítás, és hozzon létre új címkéket](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) Ha szeretne létrehozni a saját. 

### <a name="install-the-azure-information-protection-client-manually"></a>Az információk védelméről Azure ügyfél telepítése manuálisan

Az AIP ügyfél manuális telepítéséhez:

1. **AzInfoProtection.exe** letölthető [a Microsoft letöltőközpontból](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Ellenőrizheti, hogy a telepítés egy Word dokumentum megtekintése, és ügyelve arra, hogy a **védelem** beállítás érhető el a **Kezdőlap** lap dolgozott. <br/>![Védelem lapon legördülő Word dokumentumban.](media/Word_Protect.png)

További tájékoztatás, [az ügyfél telepítése](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).

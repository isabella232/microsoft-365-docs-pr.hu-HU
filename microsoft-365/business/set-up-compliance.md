---
title: Növelje a Microsoft 365 Business fenyegetettség elleni védelmét
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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
description: A megfelelőségi funkciók beállítása az adatvesztést és a címkeérzékeny adatok megelőzésére.
ms.openlocfilehash: 6fae95e8c5e6d133e3163dbdfd3c09cfede11382
ms.sourcegitcommit: 5d11f516e78ea4a74145e19ba2300f0792c8bac1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38715122"
---
# <a name="set-up-compliance-features"></a>Megfelelőségi funkciók beállítása

A Microsoft 365 üzleti szolgáltatásai védik az adatokat és az eszközöket, és segítenek megőrizni az Ön és ügyfelei kényes információit.

## <a name="set-up-dlp-features"></a>DLP-szolgáltatások beállítása

Lásd a [DLP-házirend létrehozása sablonból](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) példát a személyes azonosításra alkalmas adatok (PII) elleni védelemre vonatkozó házirend beállításához. 
  
A DLP sok különböző nyelvhez tartalmaz használatra kész házirendsablonokat. Például Ausztrália pénzügyi adatok, Kanada személyes adatok törvény, az Egyesült Államok pénzügyi adatok, és így tovább. Tekintse meg, [milyen a DLP házirendsablonok](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) a teljes listához. Az összes ilyen sablon a PII példához hasonlóan engedélyezhető. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>E-mail megőrzés beállítása az Exchange Online archiválással

 Az **Exchange Online archiválási** licencfunkciói segítenek fenntartani a megfelelést és a szabályozó szabványokat az eDiscovery e-mail tartalmának megőrzésével. Ez is segít csökken-a kockázat ha van egy polgári per, és szolgáltat egy út-hoz visszaszerez adat után egy biztonság megszegés amikor vagy szükség-hoz visszaszerez töröl cikk. Peres eljárás miatti tartás használatával megőrizheti az összes felhasználó tartalmát, vagy az adatmegőrzési szabályok segítségével testreszabhatja a megőrizni kívánt tartalmat.
  
**Peres eljárás miatti tartás:** Megőrizheti az összes postaláda tartalmát, beleértve a törölt elemeket is, ha a felhasználó teljes postaládáját peres eljárás miatti tartásba helyezzük. 
    
Ha peres eljárás miatti tartásba szeretne helyezni egy postafiókot, az admin központban:
    
1. -Ban bal NAV, megy **használók** \> **aktivál használók**.
    
2. Jelölje ki azt a felhasználót, akinek a postaládáját peres eljárás miatti tartásba szeretné helyezni. A felhasználói ablaktáblán bontsa ki a **levelezési beállítások**, majd a **További beállítások**mellett az **Exchange-Tulajdonságok szerkesztése parancsot**.
    
3. A felhasználó postaládájának lapján válassza a bal oldali NAV * * postafiók jellemzőit, majd válassza a link **engedélyezése** **peres eljárás miatt tartás**alatt.
    
4. A peres **eljárások** visszatartási párbeszédpaneljén megadhatja a peres eljárás miatti tartás időtartamát a **peres eljárások tartam** mezőben. Hagyja üresen a mezőt, ha egy végtelen visszatartott helyet szeretne. Megjegyzéseket is felvehet, és közvetlenül a postaláda tulajdonosát egy olyan webhelyre irányhatja, amelyet esetleg meg kell magyarázni a peres eljárás miatti tartásba. \>**Save**.
    
**Visszatartás:** Engedélyezheti a testreszabott adatmegőrzési szabályokat, például egy adott idő megtartása érdekében, vagy a megőrzési időszak végén véglegesen törölheti a tartalmat. További információ [az adatmegőrzési szabályok áttekintése](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423)című témakörben található.

## <a name="set-up-sensitivity-labels"></a>A érzékenységi címkék beállítása

Érzékenység címkék jönnek Azure Information Protection (AIP) terv 1, és segít osztályozni, és opcionálisan védi a dokumentumok és e-maileket alkalmazásával címkéket. A címkék automatikusan alkalmazhatók, ha a rendszergazdák szabályokat és feltételeket határoznak meg, manuálisan, felhasználók szerint, vagy olyan kombinációban, ahol a felhasználók ajánlásokat kapnak.

Az érzékenységi címkék beállításához tekintse meg az [érzékenységi címkék létrehozását és kezelését](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) ismertető videót.



### <a name="install-the-azure-information-protection-client-manually"></a>A Azure adatvédelmi ügyfél manuális telepítése

Az AIP ügyfél manuális telepítése:

1. Letölt **AzinfoProtection_UL. exe** - [bólMikroszkóp Letölt Központ](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Ellenőrizheti, hogy a telepítés működött-e, ha megtekinti a Word-dokumentumot, és meggyőződött arról, hogy az **érzékenység** lehetőség elérhető a **Kezdőlap** lapon.
<br/>![Védelem lap legördülő lista Word-dokumentumban.](media/word-sensitivity.png)

További információt [az ügyfél telepítése](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3)című témakörben talál.

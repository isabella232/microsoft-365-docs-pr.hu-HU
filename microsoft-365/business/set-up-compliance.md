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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
description: Állítsa be az Office 365 fejlett Fenyegetésvédelmet, és őrizzék meg a bizalmas adatokat.
ms.openlocfilehash: 8144bcebe8a0cdf28a5e092f592362922ccbdd48
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288745"
---
# <a name="set-up-compliance-features"></a>Megfelelőségi funkciók beállítása

A Microsoft 365 üzleti szolgáltatásai védik az adatokat és az eszközöket, és segítenek megőrizni az Ön és ügyfelei kényes információit.

## <a name="set-up-dlp-features"></a>DLP-szolgáltatások beállítása

Lásd a [DLP-házirend létrehozása sablonból](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) példát a személyes azonosításra alkalmas adatok (PII) elleni védelemre vonatkozó házirend beállításához. 
  
A DLP sok különböző nyelvhez tartalmaz használatra kész házirendsablonokat. Például, Ausztrália pénzügyi adatok, Kanada személyes adatok törvény, az Egyesült Államok pénzügyi adatok, stb. Tekintse meg, [milyen a DLP házirendsablonok](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) a teljes listához. Az összes ilyen sablon a PII példához hasonlóan engedélyezhető. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>E-mail megőrzés beállítása az Exchange Online archiválással

 Az **Exchange Online archiválási** licencfunkciói segítenek fenntartani a megfelelést és a szabályozó szabványokat az eDiscovery e-mail tartalmának megőrzésével. Ez is segít csökkenteni a kockázatot a perben, és biztosítja a módját, hogy visszaszerez adat után a biztonság megsértése, vagy ha kell visszaállítani törölt elemeket. Peres eljárás miatti tartás használatával megőrizheti az összes felhasználó tartalmát, vagy az adatmegőrzési szabályok segítségével testreszabhatja a megőrizni kívánt tartalmat.
  
**Peres eljárás miatti tartás:** Megőrizheti az összes postaláda tartalmát, beleértve a törölt elemeket is, ha a felhasználó teljes postaládáját peres eljárás miatti tartásba helyezzük. 
    
Ha peres eljárás miatti tartásba szeretne helyezni egy postafiókot, az admin központban:
    
1. -Ban bal NAV, megy **használók** \> **aktivál használók**.
    
2. Válassza ki azt a felhasználót, akinek a postaládáját peres eljárás miatti tartásba szeretné helyezni, és a felhasználó ablaktáblában bontsa ki a **levelezési beállításokat** , majd a **További beállítások** mellett válassza az **Exchange-Tulajdonságok szerkesztése parancsot**.
    
3. A felhasználó postaládájának lapján válassza a bal oldali NAV * * postafiók jellemzőit, majd válassza a link **engedélyezése** **peres eljárás miatt tartás**alatt.
    
4. A peres **eljárások** tartása párbeszédablakban megadhatja a peres eljárás miatti tartás időtartamát a **peres tartás időtartama** mezőben, ha egy végtelen tartást kíván elhelyezni, hagyja üresen a mezőt. Azt is hozzá megjegyzéseket, és közvetlenül a levéldoboz tulajdonos egy honlapot, lehet, hogy többet kell magyaráznia a peres eljárás \> tart **megment**.
    
**Visszatartás:** Engedélyezheti a testreszabott adatmegőrzési szabályokat, például egy adott idő megtartása érdekében, vagy a megőrzési időszak végén véglegesen törölheti a tartalmat. További információ [az adatmegőrzési szabályok áttekintése](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423)című témakörben található.

## <a name="set-up-azure-information-protection-features"></a>Az azúrkék információvédelmi funkciók beállítása

Azúrkék információ védelem (AIP) segít ön osztályoz és tetszés szerinti, megvéd-a okiratok és elektronikus levél, mellett alkalmaz felirat. A címkék automatikusan alkalmazhatók, ha a rendszergazdák szabályokat és feltételeket határoznak meg, manuálisan, felhasználók szerint, vagy olyan kombinációban, ahol a felhasználók ajánlásokat kapnak.

Az Outlook az interneten akkor lehet alkalmazni, a következő beépített címkék és korlátozások az Ön e-maileket:
  
- **Nem továbbíthatja**: a címzettek elolvashatják az üzenetet, de nem továbbíthatja, nyomtathatja vagy másolhatja a tartalmat
    
- **Titkosítás**: a teljes üzenet titkosítva van. A címzetteknek igazolnia kell személyazonosságukat a titkosított tartalom elérése előtt, és nem tudják eltávolítani a titkosítást.
    
- **Bizalmas**: a szervezet alkalmazottai számára teljes körű engedélyeket ad az e-mail tartalmakhoz és mellékletekhez, a szervezeten kívüli személyeknek azonban nem. Az adatok tulajdonosai bármely ponton nyomon követhetjük és visszavonhatják a tartalmat.
    
- **Nagyon bizalmas**: Ez a korlátozás rendkívül bizalmas adatokra is alkalmazható, így az alkalmazottak megtekinthetik, szerkeszthetik és válaszolhatják az adatokat, de nem továbbíthatók, nyomtathatók vagy másolhatók. Az adatok tulajdonosai bármely ponton nyomon követhetjük és visszavonhatják a tartalmat.

### <a name="make-sure-azure-information-protection-is-activated"></a>Győződjön meg arról, hogy a Azure információvédelem aktiválva van

Annak ellenőrzése, hogy az AIP aktiválva van-e:

1. Jelentkezz be az [Azure portálra](https://portal.azure.com/).

2. Kiválaszt **minden szolgáltatás** és begépel *Azure információ védelem* -ban **kutatás doboz**.

3. Egyszer a eredmények bemutatás, kettyenés a Elkezd mellett **Azure információ védelem** -hoz csinál ez egy kedvenc és könnyű-hoz talál később.

4. Jelölje be az **Azure** \> **adatvédelmi védelem aktiválása** választógombot, és győződjön meg arról, hogy az állapot aktivált állapotú-e. 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a>Az Azure adatvédelmi házirend és az alapértelmezett címkék megtekintése 

A meglévő címkék megtekintéséhez és módosításához:

1. Az Azure információs védelem irányítópultján válassza a **besorolások** \> **címkéit**. <br/>![Az Azure információvédelem szabványos címkéi.](media/AIPLabels.png)

2. Választhat címkét, hogy megtekinthesse lehetőségek, meg tudod változtatni a megjelenítendő név, színek, stb
 
3. Lásd: [módosítás és új Címkék létrehozása](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) , ha saját magunk szeretnénk létrehozni. 

### <a name="install-the-azure-information-protection-client-manually"></a>A Azure adatvédelmi ügyfél manuális telepítése

Az AIP ügyfél manuális telepítése:

1. Letölt **Azinfoprotection. exe** - [bólMikroszkóp Letölt Központ](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Ellenőrizheti, hogy a telepítés működött-e, ha megtekinti a Word-dokumentumot, és meggyőződött arról, hogy a **védelem** lehetőség elérhető a **Kezdőlap** lapon. <br/>![Védelem lap legördülő lista Word-dokumentumban.](media/Word_Protect.png)

További információért [telepítse az ügyfélprogramot](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).

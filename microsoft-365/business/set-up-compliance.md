---
title: A Microsoft 365 Business veszélyforrások elleni védelmének növelése
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
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
description: Megfelelőségi funkciók beállítása az adatvesztés és a címkeérzékeny adatok elkerülése érdekében.
ms.openlocfilehash: d569ff8d84faf82881035f0ed54e5d175605776f
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/15/2020
ms.locfileid: "42064705"
---
# <a name="set-up-compliance-features"></a>Megfelelőségi funkciók beállítása

A Microsoft 365 Business olyan funkciókkal rendelkezik, amelyek védik az adatokat és az eszközöket, és segítenek megvédeni az Ön és ügyfelei bizalmas adatait.

## <a name="set-up-dlp-features"></a>A DLP szolgáltatásainak beállítása

Lásd: [DLP-házirend létrehozása sablonból](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) című témakörben talál példát arról, hogyan állíthat be házirendet a személyazonosításra alkalmas adatok (PII) elleni védelem érdekében. 
  
A DLP számos használatra kész házirendsablont hoz számos különböző területi beállításhoz. Például, Ausztrália Pénzügyi Adatok, Kanada személyes adatokról szóló törvény, amerikai pénzügyi adatok, és így tovább. Tekintse meg, hogy [mit tartalmaznak a DLP-házirendsablonok](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) a teljes listához. Ezek a sablonok a SZEMÉLYazonosításra alkalmas sablon példához hasonlóan engedélyezhetők. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>A levelezés megőrzésének beállítása az Exchange Online archiválással

 **Az Exchange Online Archiválási** licencszolgáltatásai segítenek fenntartani a megfelelőségi és szabályozási szabványokat azáltal, hogy megőrzik az e-mail-tartalmakat az elektronikus adatfeltáráshoz. Ez is segít csökkenteni a kockázatot, ha van egy pert, és biztosítja a módját, hogy visszaszerezze az adatokat, miután a biztonsági rést, vagy ha meg kell, hogy visszaszerezze törölt elemeket. A peres eljárás miatti tartás segítségével megőrizheti a felhasználó összes tartalmát, vagy adatmegőrzési szabályzatokkal testreszabhatja, hogy mit szeretne megőrizni.
  
**Peres eljárás tartás:** A postaláda összes tartalmát, beleértve a törölt elemeket is, úgy őrizheti meg, hogy a felhasználó teljes postaládáját peres eljárás miatti tartásba helyezi. 
    
Postaláda peres eljárás miatti tartásba helyezése a Felügyeleti központban:
    
1. A bal oldali navigációs **** \> sávon nyissa meg az **Aktív felhasználók felhasználók lehetőséget.**
    
2. Válassza ki azt a felhasználót, akinek a postaládáját peres eljárás miatti tartásba kívánja helyezni. A felhasználói ablaktáblán bontsa ki a **Posta beállítások**csomópontot, és a **További beállítások**csoportban válassza az **Exchange tulajdonságainak szerkesztése**lehetőséget.
    
3. A felhasználó postaládájában válassza a bal oldali navigációs sáv ** postaláda-szolgáltatásai ** lehetőséget, majd a **Peres eljárás várakoztatás**a **hivatkozást.**
    
4. A **peres eljárás miatti tartás** párbeszédpanelen megadhatja a peres eljárás megtartásának időtartamát a **Peres eljárás megtartása időtartam** mezőben. Hagyja üresen a mezőt, ha végtelen tartást szeretne tenni. Jegyzeteket is hozzáadhat, és a postaláda tulajdonosát olyan webhelyre irányíthatja, amelyet esetleg el kell magyaráznia a peres eljárás miatti tartásról. \>**Mentés.**
    
**Megőrzés:** Engedélyezheti a testreszabott adatmegőrzési házirendeket, például egy adott ideig, vagy a tartalom végleges törléséhez a megőrzési időszak végén. További információ: [Adatmegőrzési házirendek áttekintése](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423)című témakörben olvashat.

## <a name="set-up-sensitivity-labels"></a>Érzékenységi címkék beállítása

Az érzékenységi címkék az Azure Information Protection (AIP) 1-es csomaggal rendelkeznek, és a címkék alkalmazásával segítenek a dokumentumok és e-mailek osztályozásában és tetszési igényében. A címkéket automatikusan alkalmazhatják azok a rendszergazdák, akik szabályokat és feltételeket határoznak meg, manuálisan a felhasználók által, vagy olyan kombináció használatával, amelyben a felhasználók ajánlásokat kapnak.

Az Érzékenységi címkék beállításához tekintse meg [az érzékenységi címkék](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) létrehozásához és kezeléséhez készült videót.



### <a name="install-the-azure-information-protection-client-manually"></a>Az Azure Information Protection ügyfél manuális telepítése

Az AIP-ügyfél manuális telepítése:

1. Töltse le **AzinfoProtection_UL.exe letöltését** a [Microsoft letöltőközpontjából.](https://www.microsoft.com/download/details.aspx?id=53018)
 
2. A Word-dokumentumok megtekintésével és annak biztosításával ellenőrizheti, hogy a telepítés működött-e, és meggyőződhet arról, hogy az **Érzékenység** beállítás elérhető a **Kezdőlap** lapon.
<br/>![A Védelem lap legördülő menüje egy Word-dokumentumban](../media/word-sensitivity.png)

További információt az Ügyfél telepítése című témakörben [talál.](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3)

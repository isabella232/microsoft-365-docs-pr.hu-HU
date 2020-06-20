---
title: A Microsoft 365 Business Premium fenyegetéselleni védelmének növelése
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Megfelelőségi funkciók at állíthat be az adatvesztés megelőzése és az ügyfelek bizalmas adatainak biztonsága érdekében.
ms.openlocfilehash: 18886ff3a0ba5e99e63c70ef083d7a69c75bac91
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44785832"
---
# <a name="set-up-compliance-features"></a>Megfelelőségi funkciók beállítása

A Microsoft 365 Business Premium olyan funkciókkal rendelkezik, amelyek védik az adatokat és az eszközöket, és segítenek biztonságban tartani ügyfeleit.

## <a name="set-up-dlp-features"></a>DLP-szolgáltatások beállítása

Lásd: [DLP-házirend létrehozása sablonból](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) egy példa, hogyan kell beállítani egy szabályzatot a személyazonosításra alkalmas adatok (PII) elleni védelem. 
  
A DLP számos használatra kész házirendsablont használ számos különböző területi beállításhoz. Például: Australia Financial Data, Canada Personal Information Act, Us Financial Data és így tovább. A teljes lista a [DLP-házirendsablonok gyűjteményének](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) megtekintéséről. Ezek a sablonok a példaként ii sablonhoz hasonlóan engedélyezhetők. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>E-mailek megőrzésének beállítása az Exchange Online archiválásával

 **Az Exchange Online archiválási** licencfunkciók segítenek fenntartani a megfelelőséget és a szabályozási szabványokat azáltal, hogy megőrzik az e-mailek tartalmát az elektronikus adatfeltáráshoz. Ez is segít csökkenteni a kockázatot, ha van egy pert, és lehetővé teszi, hogy visszaszerezze az adatokat, miután a biztonság megsértése, vagy ha vissza kell állítani a törölt elemeket. A peres eljárás miatti tartással megőrizheti a felhasználó teljes tartalmát, vagy adatmegőrzési házirendekkel testreszabhatja, hogy mit szeretne megőrizni.
  
**Peres eljárás miatti tartás:** Az összes postaládatartalmat megőrizheti, beleértve a törölt elemeket is, ha a felhasználó teljes postaládáját peres eljárás miatti tartásba helyezi. 
    
Ha egy postaládát peres eljárás miatti tartásba szeretne helyezni, a Felügyeleti központban:
    
1. A bal oldali navigációs sávon nyissa meg a **Felhasználók** \> **aktív felhasználók lehetőséget.**
    
2. Jelöljön ki egy olyan felhasználót, akinek a postaládáját peres eljárás miatti tartásba kívánja helyezni. A felhasználói ablaktáblán bontsa ki a **Posta beállításai csomópontot,** és a **További beállítások csoportban**válassza az **Exchange-tulajdonságok szerkesztése lehetőséget.**
    
3. A felhasználó postaládalapján válassza a bal oldali navigációs eszköz ** postaláda-szolgáltatásait ,* majd a Peres eljárás miatti tartás **csoportban** válassza az **Engedélyezés**hivatkozást.
    
4. A **peres eljárás miatti tartás** párbeszédpanelen megadhatja a peres eljárás várakoztatási időtartamát a **Peres eljárás várakoztatásidőtartama** mezőben. Hagyja üresen a mezőt, ha végtelen tartást szeretne elhelyezni. Megjegyzéseket is hozzáadhat, és a postaláda tulajdonosát egy olyan webhelyre irányíthatja, amelyről előfordulhat, hogy többet kell megmagyaráznia a peres eljárás miatti tartásról. \>**Mentés.**
    
**Megőrzés:** Engedélyezheti például a testreszabott adatmegőrzési házirendeket, hogy adott ideig megőrizzék vagy véglegesen töröljék a tartalmat az adatmegőrzési időszak végén. További információ: [Az adatmegőrzési szabályok áttekintése.](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

## <a name="set-up-sensitivity-labels"></a>Érzékenységi címkék beállítása

Az érzékenységi címkék az Azure Information Protection (AIP) 1- es csomaggal rendelkeznek, és címkék alkalmazásával segítenek a dokumentumok és e-mailek besorolásában és szükség esetén védelmében. A címkéket automatikusan alkalmazhatják azok a rendszergazdák, akik szabályokat és feltételeket határoznak meg, manuálisan a felhasználók által, vagy olyan kombináció használatával, ahol a felhasználók javaslatokat kapnak.

Érzékenységi címkék beállításához tekintse [meg az érzékenységi címkék létrehozása és kezelése](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) videót.



### <a name="install-the-azure-information-protection-client-manually"></a>Az Azure Information Protection ügyfél manuális telepítése

Az AIP-ügyfél manuális telepítése:

1. Töltse le **AzinfoProtection_UL.exe** a [Microsoft letöltőközpontjából.](https://www.microsoft.com/download/details.aspx?id=53018)
 
2. Ellenőrizheti, hogy a telepítés működött-e, ha megtekint egy Word-dokumentumot, és meggyőződik arról, hogy az **Érzékenység** lehetőség elérhető a **Kezdőlap** lapon.
<br/>![A Védelem lap legördülő menüje Egy Word-dokumentumban](../media/word-sensitivity.png)

További információt [az Ügyfél telepítése című](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3)témakörben talál.

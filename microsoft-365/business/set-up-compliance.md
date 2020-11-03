---
title: A fenyegetések elleni védelem növelése a Microsoft 365 vállalati prémium verzióban
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
description: Beállíthatja a megfelelőségi funkciókat az adatvesztés elkerülése érdekében, és segítséget nyújt az ügyfelek bizalmas adatainak biztonságának megőrzésében.
ms.openlocfilehash: 2c95ad3f36df28af2c68cd11192bcfe92dfe29e3
ms.sourcegitcommit: e56894917d2aae05705c3b9447388d10e2156183
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48841173"
---
# <a name="set-up-compliance-features"></a>A megfelelőségi funkciók beállítása

A Microsoft 365 vállalati prémium verzió az adatok és az eszközök védelméhez tartalmaz funkciókat, és segítséget nyújt az ügyfelek bizalmas adatainak biztonságának megőrzésében.

## <a name="set-up-dlp-features"></a>DLP-szolgáltatások beállítása

Lásd: [DLP-házirend létrehozása sablonból](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) , például arról, hogy miként állíthat be házirendet a személyes adatvesztés elleni védekezéshez. 
  
A DLP számos különböző nyelvhez használható, használatra kész házirend-sablonokat tartalmaz. Például Ausztrália pénzügyi adatok, kanadai személyes adatok, Amerikai pénzügyi adatok stb. Ebből a cikkből megtudhatja, hogy [milyen DLP-házirend-sablonok](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) találhatók a teljes lista számára. Az összes ilyen sablonhoz hasonlóan engedélyezhetők a szakmai sablon példája is. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>E-mail-adatmegőrzés beállítása az Exchange Online archiválási szolgáltatásával

 Az **Exchange Online archiválási** licencelési funkciói a megfelelőségi és szabályozási szabványokat a eDiscovery e-mail-tartalmainak megőrzésével segítik. Az is segít csökkenteni a kockázatokat, ha van egy pert, és lehetővé teszi az adathelyreállítást egy biztonsági rést követően, vagy ha a törölt elemek helyreállítására van szükség. A perköltség megőrzésével megőrizheti az összes felhasználó tartalmát, illetve adatmegőrzési házirendeket alkalmazva testre szabhatja a megőrizni kívánt tartalmat.
  
Jogellenes **tartás:** A törölt elemeket tartalmazó összes postaláda-tartalmat megőrizheti, ha a felhasználó teljes postaládáját a peres eljárási mentességre helyezi. 
    
Ha egy postaládát pert-mentességre szeretne helyezni, a felügyeleti központban:
    
1. A bal oldali navigációs sávon **lépjen az** \> **aktív** felhasználók elemre.
    
2. Jelölje ki azt a felhasználót, akinek a postaládáját pert-mentességre szeretné helyezni. A felhasználó ablaktáblában bontsa ki a **posta beállításai** lapot, majd a **További beállítások** mellett válassza az **Exchange-Tulajdonságok szerkesztése** lehetőséget.
    
3. A felhasználó postaládája lapján válassza a * * postaláda-funkciók * * elemet a bal oldali navigációs sávon, majd válassza az **enable (Engedélyezés** ) hivatkozást a **peres eljárási mentesség** csoportban.
    
4. A pert **-mentesség párbeszédpanelen** megadhatja a jogellenes tartás időtartamát a **jogvitákban** . Hagyja üresen a mezőt, ha végtelen mentességet szeretne elhelyezni. Jegyzeteket is adhat hozzá, és a postaláda tulajdonosát egy webhelyre irányíthatja, amelyet érdemes megmagyaráznia a peres eljárás megtartásáról. \>**Mentés gombot**.
    
**Adatmegőrzés:** Engedélyezheti a testre szabott adatmegőrzési házirendeket, például egy adott idő megőrzését vagy a tartalom végleges törlését az adatmegőrzési időszak végén. További információt [az adatmegőrzési házirendek áttekintése](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)című témakörben talál.

## <a name="set-up-sensitivity-labels"></a>A tartalmi címkék beállítása

A tartalmi címkék az Azure Information Protection ("az" 1-es csomag) 1 csomaggal rendelkeznek, és segítséget nyújtanak a dokumentumok és e-mailek osztályozásához, a címkék alkalmazásával. A címkék automatikusan alkalmazhatók olyan rendszergazdák számára, akik szabályok és feltételek meghatározását végzik manuálisan a felhasználók, illetve a felhasználók által megadott javaslatok kombinációjának használatával.

Az érzékenységi címkék beállításához tekintse meg a [tartalmi Címkék létrehozása és kezelése](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) című videót.



### <a name="install-the-azure-information-protection-client-manually"></a>Az Azure Information Protection Client manuális telepítése

Az ügyfélszolgálati ügyfél kézi telepítése:

1. Töltse le **AzinfoProtection_UL.exe** a [Microsoft letöltőközpontból](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Ellenőrizheti, hogy a telepítés a Word-dokumentum megtekintésével is működött-e, és gondoskodjon arról, hogy az **érzékenység** beállítás elérhető legyen a **Kezdőlap** lapon.
<br/>![A védelem lap egy Word-dokumentumban](../media/word-sensitivity.png)

További információt [az ügyfélalkalmazás telepítése](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3)című témakörben talál.

---
title: Veszélyforrások elleni védelem növelése a Microsoft 365 Vállalati prémium verzióban
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
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Megfelelőségi funkciókat állíthat be az adatvesztés megelőzése és az ügyfelek bizalmas adatainak biztonságossá tartása érdekében.
ms.openlocfilehash: c0accc37d3dcda9ba75813f01a98a3233c5a8369
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579954"
---
# <a name="set-up-compliance-features"></a>Megfelelőségi szolgáltatások beállítása

A Microsoft 365 Vállalati prémium verzió olyan szolgáltatásokat tartalmaz, amelyek védik az adatait és az eszközeit, és segítenek Önnek biztonságban tartani ügyfelei és bizalmas információit.

## <a name="set-up-dlp-features"></a>DLP-szolgáltatások beállítása

A [személyes adatok elvesztésével](../compliance/create-a-dlp-policy-from-a-template.md) szembeni védelem beállítása érdekében a DLP-házirend létrehozása sablonból 
  
A DLP számos használatra kész házirendsablont tartalmaz, amelyek számos különböző területi szabályhoz használhatók. Ilyen például az ausztráliai pénzügyi adatokra, a Kanadai személyes adatokra vonatkozó törvény, az Amerikai Egyesült Államok pénzügyi adatai stb. Lásd: Mit tartalmaznak a [DLP-házirendsablonok](../compliance/what-the-dlp-policy-templates-include.md) a teljes listához. Ezek a sablonok a pii-sablon példához hasonlóan engedélyezhetők. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>A levelezés megőrzésének beállítása az Exchange Online archiválásával

 **Az Exchange Online archiválási** licenc szolgáltatásai a megfelelőségi és szabályozási szabványok megőrzésével segítik a levelezési tartalmak megőrzését a elektronikus adatfeltárás érdekében. A biztonsági visszaélés vagy a törölt elemek helyreállítása után is segít a kockázat csökkentésében, és lehetőséget nyújt az adatok helyreállítására is. A jogi visszatartás segítségével megőrizheti egy felhasználó összes tartalmát, vagy adatmegőrzési házirendek használatával testre szabhatja a megőrizni kívánt tartalmakat.
  
**Jogi hold:** A postaláda teljes tartalmát megőrizheti, beleértve a törölt elemeket is, ha a felhasználó teljes postaládáját jogi jogi eljárásban tartja meg. 
    
Egy postaláda jogi úton való tartásba való behelyének helyének megnyitásához a Felügyeleti központban:
    
1. A bal oldali navigációs sávon menjen a **Users** Active users (Felhasználók \> **aktív felhasználók) csoportra.**
    
2. Jelöljön ki egy felhasználót, akinek a postaládáját jogi úton szeretné eltenni. A felhasználópanelen bontsa ki a **Levelezési** beállítások ot, és a **További** beállítások mellett válassza az **Exchange-tulajdonságok szerkesztése lehetőséget.**
    
3. A felhasználó postaládalapján válassza a ** postaláda-szolgáltatások  ** lehetőséget a bal oldali navigációs sávon, majd válassza a Hivatkozás engedélyezése lehetőséget a Jogi **tartás csoportban.**
    
4. A jogi **tartás párbeszédpanelen** a jogi tartás időtartamát a Jogi tartás időtartama mezőben **adhatja** meg. Ha végtelen holdhelyet szeretne, hagyja üresen a mezőt. Jegyzeteket is adhat hozzá, és a postaláda-tulajdonost egy webhelyre irányíthatja, amelyről bővebben el kell magyaráznia a jogi holdról. \>**Mentés gombra.**
    
**Adatmegőrzés:** Engedélyezheti a testre szabott adatmegőrzési házirendeket, például adott ideig megőrizheti őket, vagy véglegesen törölheti a tartalmakat az adatmegőrzési időszak végén. További információt Az adatmegőrzési házirendek [áttekintése témakörben talál.](../compliance/retention.md)

## <a name="set-up-sensitivity-labels"></a>Bizalmasság-címkék beállítása

A bizalmasság-címkéket az Azure Information Protection (AIP) 1. csomagja tartalmaz, és címkék alkalmazásával segítik a dokumentumok és e-mailek osztályozását és szükség esetén védelmét. A címkéket a rendszergazdák automatikusan, szabályokat és feltételeket definiálva, felhasználók által manuálisan, illetve olyan kombinációk használatával alkalmazhatók, amelyekben a felhasználók javaslatokat kapnak.

Bizalmasság-címkék beállításához tekintse meg a [bizalmasság-címkék](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) létrehozása és kezelése videót.



### <a name="install-the-azure-information-protection-client-manually"></a>Az Azure Information Protection-ügyfél manuális telepítése

Az AIP-ügyfélprogram manuális telepítése:

1. Töltse **AzinfoProtection_UL.exe** a [Microsoft letöltőközpontból.](https://www.microsoft.com/download/details.aspx?id=53018)
 
2. A telepítés ellenőrzéséhez megtekinthet egy Word-dokumentumot,  és ellenőrizheti, hogy a Bizalmasság lehetőség elérhető-e a **Kezdőlap** lapon.
<br/>![A Védelem lap legördülő menüje egy Word-dokumentumban.](../media/word-sensitivity.png)

További információ: [Az ügyfél telepítése.](/azure/information-protection/infoprotect-tutorial-step3)
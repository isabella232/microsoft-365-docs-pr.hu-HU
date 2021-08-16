---
title: Veszélyforrások elleni védelem növelése Microsoft 365 Vállalati prémium verzió
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
ms.openlocfilehash: ae5e5727db1f372c40aa4468329021525b6dfc8c5ebbf34705184e461df069e5
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53881857"
---
# <a name="set-up-compliance-features"></a>Megfelelőségi szolgáltatások beállítása

A Microsoft 365 Vállalati prémium verzió az adatai és az eszközei védelmére, valamint az ügyfelek bizalmas adatainak védelmére vonatkozó funkciókat tartalmaz.

## <a name="set-up-dlp-features"></a>DLP-szolgáltatások beállítása

A [személyes adatok elvesztésével](../compliance/create-a-dlp-policy-from-a-template.md) szembeni védelem beállítása érdekében a DLP-házirend létrehozása sablonból 
  
A DLP számos használatra kész házirendsablont tartalmaz, amelyek számos különböző területi szabályhoz használhatók. Ilyen például az ausztráliai pénzügyi adatokra, a Kanadai személyes adatokra vonatkozó törvény, az Amerikai Egyesült Államok pénzügyi adatai stb. Lásd: Mit tartalmaznak a [DLP-házirendsablonok](../compliance/what-the-dlp-policy-templates-include.md) a teljes listához. Ezek a sablonok a pii-sablon példához hasonlóan engedélyezhetők. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>A levelezés megőrzésének beállítása Exchange Online Archiválás

 **Exchange Online Archiválás** a licencelési funkciók a megfelelőségi és szabályozási szabványok megőrzésével segítik a levelezési tartalmak megőrzését a elektronikus adatok észlelése érdekében. A biztonsági visszaélés vagy a törölt elemek helyreállítása után is segít a kockázat csökkentésében, és lehetőséget nyújt az adatok helyreállítására is. A jogi visszatartás segítségével megőrizheti egy felhasználó összes tartalmát, vagy adatmegőrzési házirendek használatával testre szabhatja a megőrizni kívánt tartalmakat.
  
**Jogi hold:** A postaláda teljes tartalmát megőrizheti, beleértve a törölt elemeket is, ha a felhasználó teljes postaládáját jogi jogi eljárásban tartja meg. 
    
Egy postaláda jogi úton való tartásba való behelyének helyének megnyitásához a Felügyeleti központban:
    
1. A bal oldali navigációs sávon menjen a **Users** Active users (Felhasználók \> **aktív felhasználók) csoportra.**
    
2. Jelöljön ki egy felhasználót, akinek a postaládáját jogi úton szeretné eltenni. A felhasználópanelen bontsa ki a **Levelezési** beállítások ot, és a További beállítások mellett **válassza** a Szerkesztés **Exchange gombra.**
    
3. A felhasználó postaládalapján válassza a ** postaláda-szolgáltatások  ** lehetőséget a bal oldali navigációs sávon, majd válassza a Hivatkozás engedélyezése lehetőséget a Jogi **tartás csoportban.**
    
4. A jogi **tartás párbeszédpanelen** a jogi tartás időtartamát a Jogi tartás időtartama mezőben **adhatja** meg. Ha végtelen holdhelyet szeretne, hagyja üresen a mezőt. Jegyzeteket is adhat hozzá, és a postaláda-tulajdonost egy webhelyre irányíthatja, amelyről bővebben el kell magyaráznia a jogi holdról. \>**Mentés gombra.**
    
**Adatmegőrzés:** Engedélyezheti a testre szabott adatmegőrzési házirendeket, például adott ideig megőrizheti őket, vagy véglegesen törölheti a tartalmakat az adatmegőrzési időszak végén. További információt Az adatmegőrzési házirendek [áttekintése témakörben talál.](../compliance/retention.md)

## <a name="set-up-sensitivity-labels"></a>Bizalmasság-címkék beállítása

A bizalmasság-címkéket az Azure Information Protection (AIP) 1. csomagja tartalmaz, és címkék alkalmazásával segítik a dokumentumok és e-mailek osztályozását és szükség esetén védelmét. A címkéket a rendszergazdák automatikusan, szabályokat és feltételeket definiálva, felhasználók által manuálisan, illetve olyan kombinációk használatával alkalmazhatók, amelyekben a felhasználók javaslatokat kapnak.

Bizalmasság-címkék beállításához tekintse meg a [bizalmasság-címkék](../business-video/create-sensitivity-labels.md) létrehozása és kezelése videót.



### <a name="install-the-azure-information-protection-client-manually"></a>Az Azure Information Protection-ügyfél manuális telepítése

Az AIP-ügyfélprogram manuális telepítése:

1. Töltse **AzinfoProtection_UL.exe** a [Microsoft letöltőközpontból.](https://www.microsoft.com/download/details.aspx?id=53018)
 
2. A telepítés ellenőrzéséhez megtekinthet egy Word-dokumentumot,  és ellenőrizheti, hogy a Bizalmasság lehetőség elérhető-e a **Kezdőlap** lapon.
<br/>![A Védelem lap legördülő menüje egy Word-dokumentumban.](../media/word-sensitivity.png)

További információ: [Az ügyfél telepítése.](/azure/information-protection/infoprotect-tutorial-step3)
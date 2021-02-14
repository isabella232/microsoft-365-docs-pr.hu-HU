---
title: Felkészülés az Office-ügyfél központi telepítésére a Microsoft 365 Vállalati verzióban
f1.keywords:
- CSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 10/31/2017
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Megtudhatja, hogy miként telepítheti automatikusan a 32 bites Office-appokat Windows 10 rendszerű számítógépekre, és hogyan tarthatja őket naprakészen.
ms.openlocfilehash: 2de492914edbde2afe593aac290c4a634b801443
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44470947"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a>Felkészülés az Office-ügyfél központi telepítésére a Microsoft 365 Vállalati verzióban

Ez a cikk a Microsoft 365 Vállalati prémium verzióra vonatkozik.

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Felkészülés az Office-appok ügyfélszámítógépekre történő automatikus telepítésére

A Microsoft 365 Vállalati prémium verzióval automatikusan telepítheti a 32 bites Office-appokat Windows 10 rendszerű számítógépekre, és a frissítésekkel kordában tarthatja őket.
  
Az automatikus telepítés akkor működik a legjobban, ha a végfelhasználó számítógépe a Windows 10 Business rendszert használja, és:
  
- Nincsenek telepített asztali Office-appjai (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access és OneDrive).
    
    vagy
    
- Telepítve van egy Office Kattintásra verzió.
    
Ha ki szeretné deríteni, hogy az Office Office Kattintásra verziójával rendelkezik-e, egy tetszőleges Office-appban válassza a **Fájl** \> **Fiók** (az Outlookban **Office-fiók**) lehetőséget). Ha az Alábbi ábrán látható **módon** látja az Office-frissítéseket, akkor a telepítés az Office Kattintásra használatával történt. 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Kik számára előnyös ez a funkció?**
  
Annak a végfelhasználónak, akinek a PC-jén:
  
- **Rendelkezik**  Windows 10 Vállalati verziós felhasználói licenccel, aktív Microsoft 365 Vállalati verziós licenccel, a Windows 10 alkotói frissítéssel, és csatlakozik az Azure Active Directoryhoz. 
    
- **Nincs 64** bites Office-appja (például: Word, Excel, PowerPoint). Ha 64 bites Office-appokra van szükség, akkor ez a funkció nem megfelelő, mert az Office 2016 Kattintásra 64 bites verzióját a Microsoft 365 Vállalati verzió felügyeleti konzolján nem lehet eltenni. 
    
- **Nem található meg** egy Windows Installer (MSI) technológiával telepített különálló 2016-os app sem (például Visio vagy Project). A Microsoft 365 Vállalati verzió frissíti az Office-t az Office 2016 Office Kattintásra verziójára, és nem működik az Office 2016 MSI különálló appokkal. 
    
Az alábbi táblázatban látható, hogy a kezdő állapotuktól függően a végfelhasználóknak/rendszergazdáknak milyen műveletet kell követniük ahhoz, hogy az Office 365 Vállalati verzió felügyeleti konzolján az Office Kattintásra 32 bites verziója sikeres legyen.
  
|**Az Office telepítésének kezdő állapota**|**A Microsoft 365 Vállalati verzió telepítése előtt szükséges teendők az Office telepítése előtt**|**Záró állapot**|
|:-----|:-----|:-----|
|Nincs telepítve Office programcsomag  <br/> |Nincs  <br/> |Az Office 2016 32 bites telepítése az Office Kattintásra használatával  <br/> |
|Az Office Kattintásra technológiával telepített Office 32 bites verziója (2016-os vagy korábbi verzió), különálló appok nélkül  <br/> |Nincs  <br/> |Frissítve az Office 2016 legújabb 32 bites, Office Kattintásra verziójára, szükség szerint **\*** <br/> |
|Az Office Kattintásra 32 bites verziója és az Office Kattintásra 32 bites vagy 64 bites különálló Office-appok (például Visio, Project)  <br/> |Egyikre sem.  <br/> |A különálló appokat ez nem érinti. A programcsomag frissül az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára  <br/> |
|Az Office Kattintásra technológiával telepített Office 32 bites verziója és bármely 32 vagy 64 bites (a 2016-os verzió kivételével), MSI technológiával telepített különálló Office-app  <br/> |Nincs  <br/> |A különálló appokat ez nem érinti. A programcsomag frissül az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára  <br/> ||||
|Az Office Kattintásra technológiával telepített Office bármely meglévő, 64 bites verziója  <br/> |Távolítsa el a 64 bites Office-appokat, ha nem gond, hogy lecserélje őket a 32 bites Office-appokkal  <br/> |Ha eltávolítja a 64 bites Office-appokat, az Office Kattintásra technológiával telepített Office 2016 32 bites verziója települ  <br/> |
|Az Office 2016 meglévő, MSI technológiával telepített példánya különálló appokkal vagy anélkül  <br/> |Az MSI technológiával telepített Office 2016 eltávolítása  <br/> |Telepítve van az Office Kattintásra technológiával telepített Office 2016 32 bites verziója. A különálló appokat nem érinti semmilyen változás.  <br/> |
|Az Office 2013 és/vagy különálló Office-appok meglévő, MSI technológiával telepített példánya  <br/> |Nincs  <br/> |Az Office Kattintásra technológiával telepített Office 2016 32 bites verziója, amely együtt létezik a korábbról meglévő, MSI technológiával telepített Office-példánnyal (és különálló appokkal)  <br/> |
||||
   
 **(\*) Megjegyzés:** Egy ismert hiba miatt nem történik meg az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára való frissítés. A javítás folyamatban van. 
  

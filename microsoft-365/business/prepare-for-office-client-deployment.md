---
title: Felkészülés Office-ügyfél központi telepítésére a Microsoft 365 Vállalati verzióban
f1.keywords:
- CSH
ms.author: efrene
author: efrene
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
description: Megtudhatja, hogy miként telepítheti automatikusan a 32 bites Office-appokat Windows 10-es számítógépekre, és hogyan tarthatja őket naprakészen.
ms.openlocfilehash: 843be426d817da1173769b3b66dc4c054179f0fd
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/14/2021
ms.locfileid: "52924227"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a>Felkészülés Office-ügyfél központi telepítésére a Microsoft 365 Vállalati verzióban

Ez a cikk a Microsoft 365 Vállalati prémium verzióra vonatkozik.

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Felkészülés az Office-appok ügyfélszámítógépekre történő automatikus telepítésére

A Microsoft 365 Vállalati prémium verzióval automatikusan telepítheti a 32 bites Office-appokat Windows 10-es számítógépekre, és folyamatosan frissülhet a frissítésekkel.
  
Az automatikus telepítés akkor működik a legjobban, ha a végfelhasználó számítógépe a Windows 10 Business rendszert használja, és:
  
- Nincsenek telepített asztali Office-appjai (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access és OneDrive).
    
    vagy
    
- Telepítve van egy Office Kattintásra verzió.
    
Ha ki szeretné deríteni, hogy az Office Office Kattintásra verziójával rendelkezik-e, egy tetszőleges Office-appban válassza a **Fájl** \> **Fiók** (az Outlookban **Office-fiók**) lehetőséget). Ha az **Office-frissítések az** alábbi ábrán látható módon jelennek meg, akkor a telepítés az Office Kattintásra használatával történt. 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Kik számára előnyös ez a funkció?**
  
Annak a végfelhasználónak, akinek a PC-jén:
  
- **Windows**  10 Business felhasználói licenccel, aktív Microsoft 365 Vállalati verziós licenccel és a Windows 10 alkotói frissítéssel rendelkezik, és csatlakozik az Azure Active Directoryhoz. 
    
- **Nincs 64** bites Office-appja (például: Word, Excel, PowerPoint). Ha 64 bites Office-appokra van szükség, akkor ez a funkció nem jó hely, mert az Office 2016 64 bites, Office Kattintásra verziójának a Microsoft 365 Vállalati verzió felügyeleti konzolról való kiváltása nem támogatott. 
    
- **Nem található meg** egy Windows Installer (MSI) technológiával telepített különálló 2016-os app sem (például Visio vagy Project). A Microsoft 365 vállalati verzió az Office-t az Office 2016 Office Kattintásra verziójára frissíti, és nem működik együtt az MSI különálló Office 2016-appokkal. 
    
Az alábbi táblázatban látható, hogy a felhasználóknak/rendszergazdáknak milyen műveletet kell követniük a kezdő állapotuktól függően ahhoz, hogy az Office 365 Vállalati verzió felügyeleti konzolján az Office 32 bites, Office Kattintásra típusú verzióját futtatják.<br/>


|Az Office telepítésének kezdő állapota|A Microsoft 365 Vállalati verzió telepítése előtt szükséges teendők|Záró állapot|
|:-----|:-----|:-----|
|Nincs telepítve Office programcsomag  <br/> |Nincs  <br/> |Az Office 2016 32 bites telepítése az Office Kattintásra használatával  <br/> |
|Az Office Kattintásra technológiával telepített Office 32 bites verziója (2016-os vagy korábbi verzió), különálló appok nélkül  <br/> |Nincs  <br/> |Frissítve az Office 2016 legújabb 32 bites, Office Kattintásra verziójára, szükség szerint **\*** <br/> |
|Az Office Kattintásra szolgáltatás meglévő, 32 bites verziója és 32 bites vagy 64 bites különálló Office-appok (például Visio, Project)  <br/> |Egyikre sem.  <br/> |A különálló appok nem érintettek. A programcsomag frissül az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára  <br/> |
|Az Office Kattintásra technológiával telepített Office 32 bites verziója és bármely 32 vagy 64 bites (a 2016-os verzió kivételével), MSI technológiával telepített különálló Office-app  <br/> |Nincs  <br/> |A különálló appok nem érintettek. A programcsomag frissül az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára  <br/> |
|Az Office Kattintásra technológiával telepített Office bármely meglévő, 64 bites verziója  <br/> |Távolítsa el a 64 bites Office-appokat, ha nem gond, hogy lecserélje őket a 32 bites Office-appokkal  <br/> |Ha eltávolítja a 64 bites Office-appokat, az Office Kattintásra technológiával telepített Office 2016 32 bites verziója települ  <br/> |
|Az Office 2016 meglévő, MSI technológiával telepített példánya különálló appokkal vagy anélkül  <br/> |Az MSI technológiával telepített Office 2016 eltávolítása  <br/> |Telepítve van az Office Kattintásra technológiával telepített Office 2016 32 bites verziója. A különálló appokat nem érinti semmilyen változás.  <br/> |
|Az Office 2013 és/vagy különálló Office-appok meglévő, MSI technológiával telepített példánya  <br/> |Nincs  <br/> |Az Office Kattintásra technológiával telepített Office 2016 32 bites verziója, amely együtt létezik a korábbról meglévő, MSI technológiával telepített Office-példánnyal (és különálló appokkal)  <br/> |
||||
   
 **(\*) Megjegyzés:** Egy ismert hiba miatt nem történik meg az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára való frissítés. Már folyamatban van a javítás. 
  

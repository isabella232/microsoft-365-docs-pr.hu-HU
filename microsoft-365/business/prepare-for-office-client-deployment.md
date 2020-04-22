---
title: Felkészülés a Microsoft 365 vállalati verzió statisztulásának Office-ügyféltelepítésére
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
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Megtudhatja, hogy miként telepítheti automatikusan a 32 bites Office-alkalmazásokat Windows 10 rendszerű számítógépekre, és hogyan őrizheti meg azokat.
ms.openlocfilehash: b5f01bc9bb10765929f3c6bdd5908e8b48a51a11
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/21/2020
ms.locfileid: "43633099"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a>Felkészülés a Microsoft 365 vállalati verzió statisztulásának Office-ügyféltelepítésére

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Felkészülés az Office-appok ügyfélszámítógépekre történő automatikus telepítésére

A Microsoft 365 vállalati verzióval automatikusan telepítheti a 32 bites Office-alkalmazásokat Windows 10 rendszerű számítógépekre, és naprakészen tarthatja őket a frissítésekkel kapcsolatban.
  
Az automatikus telepítés akkor működik a legjobban, ha a végfelhasználó számítógépe Windows 10 Business rendszeren van, és:
  
- Nincsenek telepített asztali Office-appjai (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access és OneDrive).
    
    vagy
    
- Telepítve van egy Office Kattintásra verzió.
    
Ha ki szeretné deríteni, hogy az Office Office Kattintásra verziójával rendelkezik-e, egy tetszőleges Office-appban válassza a **Fájl** \> **Fiók** (az Outlookban **Office-fiók**) lehetőséget). Ha az **Office-frissítések** az alábbi ábrán látható módon jelenik meg, akkor a telepítés az Office-hoz kattintással történt. 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Ki élvezi ezt a funkciót?**
  
Annak a végfelhasználónak, akinek a PC-jén:
  
- **Windows** 10 Business felhasználói licenccel, aktív Microsoft 365 vállalati licenccel, Windows 10 Alkotók frissítésével rendelkezik, és csatlakozik az Azure Active Directoryhoz. 
    
- **Nem rendelkezik** 64 bites Office-alkalmazásokkal (például Word, Excel, PowerPoint). Ha 64 bites Office-alkalmazásokra van szükség, akkor ez a funkció nem megfelelő, mert nem támogatja az Office 64 bites Office Kattintásra verziójának elindítását a Microsoft 365 vállalati verziós felügyeleti konzolról. 
    
- **Nem található meg** egy Windows Installer (MSI) technológiával telepített különálló 2016-os app sem (például Visio vagy Project). A Microsoft 365 vállalati verzió frissíti az Office-t az Office 2016 Office 2016 Kattintásra verziója szolgáltatásra, és ez nem működik az Office 2016 MSI önálló alkalmazásaival. 
    
Az alábbi táblázat bemutatja, hogy a végfelhasználóknak/rendszergazdáknak a kezdeti állapotuktól függően milyen műveletet kell végrehajtaniuk ahhoz, hogy a Microsoft 365 vállalati verziós felügyeleti konzolon az Office-telepítés sikeres, Kattintásra alkalmazásra készült verziója meglegyen.
  
|**Az Office telepítésének kezdő állapota**|**Végrehajtandó művelet a Microsoft 365 vállalati verzió Office-telepítése előtt**|**Záró állapot**|
|:-----|:-----|:-----|
|Nincs telepítve Office programcsomag  <br/> |Egyikre sem.  <br/> |Az Office 2016 32 bites telepítése az Office Kattintásra alkalmazással történik  <br/> |
|Az Office Kattintásra technológiával telepített Office 32 bites verziója (2016-os vagy korábbi verzió), különálló appok nélkül  <br/> |Egyikre sem.  <br/> |Frissítve az Office 2016 legújabb 32 bites, Office Kattintásra verziójára, szükség szerint **\*** <br/> |
|Az Office meglévő Kattintásra 32 bites verziója és az Office Kattintásra 32 bites vagy 64 bites önálló Office-alkalmazások (például Visio, Project)  <br/> |Egyikre sem.  <br/> |Az önálló alkalmazásokat ez nem érinti. A programcsomag frissül az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára  <br/> |
|Az Office Kattintásra technológiával telepített Office 32 bites verziója és bármely 32 vagy 64 bites (a 2016-os verzió kivételével), MSI technológiával telepített különálló Office-app  <br/> |Egyikre sem.  <br/> |Az önálló alkalmazásokat ez nem érinti. A programcsomag frissül az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára  <br/> ||||
|Az Office Kattintásra technológiával telepített Office bármely meglévő, 64 bites verziója  <br/> |A 64 bites Office-alkalmazások eltávolítása, ha nem baj, ha 32 bites Office-appokkal helyettesíti őket  <br/> |Ha eltávolítja a 64 bites Office-appokat, az Office Kattintásra technológiával telepített Office 2016 32 bites verziója települ  <br/> |
|Az Office 2016 meglévő, MSI technológiával telepített példánya különálló appokkal vagy anélkül  <br/> |Az MSI technológiával telepített Office 2016 eltávolítása  <br/> |Telepítve van az Office Kattintásra technológiával telepített Office 2016 32 bites verziója. A különálló appokat nem érinti semmilyen változás.  <br/> |
|Az Office 2013 és/vagy különálló Office-appok meglévő, MSI technológiával telepített példánya  <br/> |Nincs  <br/> |Az Office Kattintásra technológiával telepített Office 2016 32 bites verziója, amely együtt létezik a korábbról meglévő, MSI technológiával telepített Office-példánnyal (és különálló appokkal)  <br/> |
||||
   
 **(\*) Megjegyzés:** Egy ismert hiba miatt nem történik meg az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára való frissítés. A javítás folyamatban van. 
  

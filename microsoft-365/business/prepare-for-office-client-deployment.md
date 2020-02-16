---
title: Felkészülés Office-ügyfél központi telepítésére a Microsoft 365 Business segítségével
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
description: Megtudhatja, hogy miként telepítheti automatikusan a 32 bites Office-alkalmazásokat Windows 10-es számítógépekre, és hogyan tarthatja őket naprakészen.
ms.openlocfilehash: 0f8cd7df49ad627b190fad6737ec95a6d64d99d0
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/15/2020
ms.locfileid: "42065106"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a>Felkészülés Office-ügyfél központi telepítésére a Microsoft 365 Business segítségével

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Felkészülés az Office-appok ügyfélszámítógépekre történő automatikus telepítésére

A Microsoft 365 Vállalati verzió segítségével automatikusan telepítheti a 32 bites Office-alkalmazásokat Windows 10-es számítógépekre, és naprakészen tarthatja őket a frissítésekkel.
  
Az automatikus telepítés akkor működik a legjobban, ha a végfelhasználó számítógépe Windows 10 Business rendszeren van, és:
  
- Nincsenek telepített asztali Office-appjai (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access és OneDrive).
    
    vagy
    
- Telepítve van egy Office Kattintásra verzió.
    
Ha ki szeretné deríteni, hogy az Office Office Kattintásra verziójával rendelkezik-e, egy tetszőleges Office-appban válassza a **Fájl** \> **Fiók** (az Outlookban **Office-fiók**) lehetőséget). Ha az **Office-frissítések** az alábbi ábrán látható módon jelenik meg, akkor a telepítés a Kattintásra szolgáltatás sal történt. 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Kinek származik előnye ennek a funkciónak a birtoklásából?**
  
Annak a végfelhasználónak, akinek a PC-jén:
  
- **Megtalálható** egy Windows 10 Business verzióhoz való felhasználói licenc, egy aktív Microsoft 365 Business-licenc és a Windows 10 alkotói frissítés, illetve akinek a PC-je csatlakoztatva van az Azure Active Directoryhoz. 
    
- **Nincs** 64 bites Office-alkalmazás (például Word, Excel, PowerPoint). Ha 64 bites Office-alkalmazásokra van szükség, akkor ez a funkció nem megfelelő, mert nem támogatja az Office 64 bites, kattintásra futó verziójának aktiválását a Microsoft 365 Vállalati verzió felügyeleti konzoljáról. 
    
- **Nem található meg** egy Windows Installer (MSI) technológiával telepített különálló 2016-os app sem (például Visio vagy Project). A Microsoft 365 Vállalati verzió az Office-t az Office 2016 Office Kattintásra verziójára frissíti, és ez nem működik az Office 2016-os MSI önálló alkalmazásokkal. 
    
Az alábbi táblázat bemutatja, hogy a végfelhasználóknak/rendszergazdáknak milyen lépéseket kell tenniük a kezdeti állapotuktól függően ahhoz, hogy az Office központi telepítésének sikeres 32 bites Office-telepítést a Microsoft 365 Vállalati verzió felügyeleti konzoljáról történő futtatásához.
  
|**Az Office telepítésének kezdő állapota**|**Az Office Microsoft 365 Business-szel való telepítése előtt szükséges művelet**|**Záró állapot**|
|:-----|:-----|:-----|
|Nincs telepítve Office programcsomag  <br/> |Egyikre sem.  <br/> |Az Office 2016 32 bites telepítése kattintásra  <br/> |
|Az Office Kattintásra technológiával telepített Office 32 bites verziója (2016-os vagy korábbi verzió), különálló appok nélkül  <br/> |Egyikre sem.  <br/> |Frissítve az Office 2016 legújabb 32 bites, Office Kattintásra verziójára, szükség szerint **\*** <br/> |
|Az Office és a Kattintásra 32 bites vagy a 64 bites önálló Office-alkalmazások (például Visio, Project) meglévő, Kattintásra 32 bites verziója  <br/> |Egyikre sem.  <br/> |Az önálló alkalmazásokat ez nem érinti. A programcsomag frissül az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára  <br/> |
|Az Office Kattintásra technológiával telepített Office 32 bites verziója és bármely 32 vagy 64 bites (a 2016-os verzió kivételével), MSI technológiával telepített különálló Office-app  <br/> |Egyikre sem.  <br/> |Az önálló alkalmazásokat ez nem érinti. A programcsomag frissül az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára  <br/> ||||
|Az Office Kattintásra technológiával telepített Office bármely meglévő, 64 bites verziója  <br/> |Távolítsa el a 64 bites Office-alkalmazásokat, ha nem baj, ha 32 bites Office-appokra cseréli őket  <br/> |Ha eltávolítja a 64 bites Office-appokat, az Office Kattintásra technológiával telepített Office 2016 32 bites verziója települ  <br/> |
|Az Office 2016 meglévő, MSI technológiával telepített példánya különálló appokkal vagy anélkül  <br/> |Az MSI technológiával telepített Office 2016 eltávolítása  <br/> |Telepítve van az Office Kattintásra technológiával telepített Office 2016 32 bites verziója. A különálló appokat nem érinti semmilyen változás.  <br/> |
|Az Office 2013 és/vagy különálló Office-appok meglévő, MSI technológiával telepített példánya  <br/> |Nincs  <br/> |Az Office Kattintásra technológiával telepített Office 2016 32 bites verziója, amely együtt létezik a korábbról meglévő, MSI technológiával telepített Office-példánnyal (és különálló appokkal)  <br/> |
||||
   
 **(\*) Megjegyzés:** Egy ismert hiba miatt nem történik meg az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára való frissítés. A javítás folyamatban van. 
  

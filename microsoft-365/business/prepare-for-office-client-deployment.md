---
title: Felkészülés Office-ügyfél központi telepítésére a Microsoft 365 Business segítségével
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 10/31/2017
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Automatikusan a 32 bites Office-alkalmazások telepítése Windows 10 számítógépeken és őrizzük frissített útmutató.
ms.openlocfilehash: c8e93746b89925d6b6a928a474fe5736e2834987
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32286651"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a>Felkészülés Office-ügyfél központi telepítésére a Microsoft 365 Business segítségével

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Felkészülés az Office-appok ügyfélszámítógépekre történő automatikus telepítésére

A Microsoft 365 Business használatával automatikusan telepítheti az Office-appok 32 bites verzióját a Windows 10-es számítógépekre, és frissítésekkel naprakészen tarthatja őket.
  
Ez akkor működik a legjobban, ha a végfelhasználó számítógépén Windows 10 Business fut, és:
  
- Nincsenek telepített asztali Office-appjai (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access és OneDrive).
    
    vagy
    
- Telepítve van egy Office Kattintásra verzió.
    
Ha ki szeretné deríteni, hogy az Office Office Kattintásra verziójával rendelkezik-e, egy tetszőleges Office-appban válassza a **Fájl** \> **Fiók** (az Outlookban **Office-fiók**) lehetőséget). Ha ekkor megjelennek az Office-frissítések az alábbi ábrán látható módon, akkor a telepített példány Office Kattintásra verziójú. 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Kinek származik előnye a funkcióból?**
  
Annak a végfelhasználónak, akinek a PC-jén:
  
- **Megtalálható** egy Windows 10 Business verzióhoz való felhasználói licenc, egy aktív Microsoft 365 Business-licenc és a Windows 10 alkotói frissítés, illetve akinek a PC-je csatlakoztatva van az Azure Active Directoryhoz. 
    
- **Nem található meg** az Office-appok 64 bites verziója (például: Word, Excel, Powerpoint). Ha az Office-appok 64 bites verzióját kell használnia, akkor ez a funkció nem jó választás, mivel az Office 2016 64 bites, Office Kattintásra verziójának elindítása a Microsoft 365 Business felügyeleti konzoljából nem támogatott. 
    
- **Nem található meg** egy Windows Installer (MSI) technológiával telepített különálló 2016-os app sem (például Visio vagy Project). A Microsoft 365 Business az Office-t az Office 2016 Office Kattintásra verziójára frissíti, amely nem működik együtt az MSI telepítésű különálló Office 2016-appokkal. 
    
Az alábbi táblázat azt részletezi, hogy a kezdő állapotuktól függően a végfelhasználóknak/rendszergazdáknak milyen műveleteket kell végrehajtaniuk a Microsoft 365 Business felügyeleti konzoljában ahhoz, hogy megfelelően működjön az Office 32 bites, Office Kattintásra verziója.
  
|**Az Office telepítésének kezdő állapota**|**Az Office Microsoft 365 Business-szel való telepítése előtt szükséges művelet**|**Záró állapot**|
|:-----|:-----|:-----|
|Nincs telepítve Office programcsomag  <br/> |Nincs  <br/> |Az Office Kattintásra technológiával telepített Office 2016 32 bites verziója  <br/> |
|Az Office Kattintásra technológiával telepített Office 32 bites verziója (2016-os vagy korábbi verzió), különálló appok nélkül  <br/> |Nincs  <br/> |Frissítve az Office 2016 legújabb 32 bites, Office Kattintásra verziójára, szükség szerint **\*** <br/> |
|Az Office Kattintásra technológiával telepített Office 32 bites verziója és Office Kattintásra technológiával telepített 32 vagy 64 bites különálló Office-appok (például Visio, Project)  <br/> |Nincs  <br/> |A különálló appok nem érintettek. A programcsomag frissül az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára  <br/> |
|Az Office Kattintásra technológiával telepített Office 32 bites verziója és bármely 32 vagy 64 bites (a 2016-os verzió kivételével), MSI technológiával telepített különálló Office-app  <br/> |Nincs  <br/> |A különálló appok nem érintettek. A programcsomag frissül az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára  <br/> ||||
|Az Office Kattintásra technológiával telepített Office bármely meglévő, 64 bites verziója  <br/> |Az Office-appok 64 bites verziójának eltávolítása, ha az lecserélhető az Office-appok 32 bites verziójára  <br/> |Ha eltávolítja a 64 bites Office-appokat, az Office Kattintásra technológiával telepített Office 2016 32 bites verziója települ  <br/> |
|Az Office 2016 meglévő, MSI technológiával telepített példánya különálló appokkal vagy anélkül  <br/> |Az MSI technológiával telepített Office 2016 eltávolítása  <br/> |Telepítve van az Office Kattintásra technológiával telepített Office 2016 32 bites verziója. A különálló appokat nem érinti semmilyen változás.  <br/> |
|Az Office 2013 és/vagy különálló Office-appok meglévő, MSI technológiával telepített példánya  <br/> |Nincs  <br/> |Az Office Kattintásra technológiával telepített Office 2016 32 bites verziója, amely együtt létezik a korábbról meglévő, MSI technológiával telepített Office-példánnyal (és különálló appokkal)  <br/> |
||||
   
 **(\*) Megjegyzés:** Egy ismert hiba miatt nem történik meg az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára való frissítés. A javítás folyamatban van. 
  



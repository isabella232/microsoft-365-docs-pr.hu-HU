---
title: Felkészülés Office-ügyfél központi telepítésére a Microsoft 365 Business segítségével
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
description: Útmutató a 32 bites Office-alkalmazások automatikus telepítéséhez Windows 10 számítógépre, és a frissítés naprakészen tartása.
ms.openlocfilehash: 09857ddeb28e953da07979045a65f6b91925aeaf
ms.sourcegitcommit: 2c2248b03f7753d64490f2f7e56ec644a235b65a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/15/2019
ms.locfileid: "38640769"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a>Felkészülés Office-ügyfél központi telepítésére a Microsoft 365 Business segítségével

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Felkészülés az Office-appok ügyfélszámítógépekre történő automatikus telepítésére

Tudod használ Mikroszkóp 365 teendő-hoz gépiesen felszerel a 32-darab Hivatal apps-ra Windows 10 számítógépek és eltartás őket időszerű-val korszerűsít.
  
Önműködő bevezetés szerkezet legjobb ha a végfelhasználó ' számítógép van-ra Windows 10 teendő és:
  
- Nincsenek telepített asztali Office-appjai (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access és OneDrive).
    
    vagy
    
- Telepítve van egy Office Kattintásra verzió.
    
Ha ki szeretné deríteni, hogy az Office Office Kattintásra verziójával rendelkezik-e, egy tetszőleges Office-appban válassza a **Fájl** \> **Fiók** (az Outlookban **Office-fiók**) lehetőséget). Ha az alábbi ábrán látható **Office-frissítések** jelennek meg, a telepítés a kattintásra paranccsal történt. 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Kinek előnyös ez a funkció**
  
Annak a végfelhasználónak, akinek a PC-jén:
  
- **Megtalálható** egy Windows 10 Business verzióhoz való felhasználói licenc, egy aktív Microsoft 365 Business-licenc és a Windows 10 alkotói frissítés, illetve akinek a PC-je csatlakoztatva van az Azure Active Directoryhoz. 
    
- **Nem ' volna** 64-darab Hivatal apps (példa: szó, kitűnik, PowerPoint). Ha a 64 bites Office alkalmazások szükségesek, akkor ez a funkció nem egy jó illeszkedést, mert nem támogatja a kiváltó 64-bites 2016 az Office Kattintásra futtatása a Microsoft 365 Business admin konzoljáról. 
    
- **Nem található meg** egy Windows Installer (MSI) technológiával telepített különálló 2016-os app sem (például Visio vagy Project). Mikroszkóp 365 teendő felfelé tartók hivatal-hoz kettyenés--hoz-fuss változat-ból Hivatal 2016 és amit nem ' dolgozik-val Hivatal 2016 MSI standalone apps. 
    
A következő táblázat bemutatja, hogy a végfelhasználók/rendszergazdák milyen lépéseket tettek az első állapotától függően ahhoz, hogy a Microsoft 365 Business admin konzolon sikeresen 32 bites Click-to-Run verziójú Office-telepítést lehessen futtatni.
  
|**Az Office telepítésének kezdő állapota**|**Az Office Microsoft 365 Business-szel való telepítése előtt szükséges művelet**|**Záró állapot**|
|:-----|:-----|:-----|
|Nincs telepítve Office programcsomag  <br/> |Egyikre sem.  <br/> |Hivatal 2016 32-darab van beiktatott mellett használ kettyenés--hoz-fuss  <br/> |
|Az Office Kattintásra technológiával telepített Office 32 bites verziója (2016-os vagy korábbi verzió), különálló appok nélkül  <br/> |Egyikre sem.  <br/> |Frissítve az Office 2016 legújabb 32 bites, Office Kattintásra verziójára, szükség szerint **\*** <br/> |
|Létező kettyenés--hoz-fuss 32-darab változat-ból Hivatal és kettyenés--hoz-fuss 32-darab vagy 64-darab standalone Hivatal apps (például, látomás, tervez)  <br/> |Egyikre sem.  <br/> |Az önálló alkalmazások nem érintettek. A programcsomag frissül az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára  <br/> |
|Az Office Kattintásra technológiával telepített Office 32 bites verziója és bármely 32 vagy 64 bites (a 2016-os verzió kivételével), MSI technológiával telepített különálló Office-app  <br/> |Egyikre sem.  <br/> |Az önálló alkalmazások nem érintettek. A programcsomag frissül az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára  <br/> ||||
|Az Office Kattintásra technológiával telepített Office bármely meglévő, 64 bites verziója  <br/> |Uninstall a 64-darab Hivatal apps, ha-a ' rendben van helyettesíteni őket-val 32-darab Hivatal apps  <br/> |Ha eltávolítja a 64 bites Office-appokat, az Office Kattintásra technológiával telepített Office 2016 32 bites verziója települ  <br/> |
|Az Office 2016 meglévő, MSI technológiával telepített példánya különálló appokkal vagy anélkül  <br/> |Az MSI technológiával telepített Office 2016 eltávolítása  <br/> |Telepítve van az Office Kattintásra technológiával telepített Office 2016 32 bites verziója. A különálló appokat nem érinti semmilyen változás.  <br/> |
|Az Office 2013 és/vagy különálló Office-appok meglévő, MSI technológiával telepített példánya  <br/> |Nincs  <br/> |Az Office Kattintásra technológiával telepített Office 2016 32 bites verziója, amely együtt létezik a korábbról meglévő, MSI technológiával telepített Office-példánnyal (és különálló appokkal)  <br/> |
||||
   
 **(\*) Megjegyzés:** Egy ismert hiba miatt nem történik meg az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára való frissítés. A javítás folyamatban van. 
  
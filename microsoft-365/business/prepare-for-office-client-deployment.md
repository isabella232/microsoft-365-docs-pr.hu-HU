---
title: Felkészülés az Office központi telepítésére Microsoft 365 vállalati verzióban
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
description: Megtudhatja, hogy miként telepítheti automatikusan a 32 bites Office alkalmazásokat Windows 10 számítógépen, és hogyan frissítheti őket.
ms.openlocfilehash: 134d5f2918e3f28c2025b282b9ae0325b64fe0474ae8123d0637bb43c4730c55
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53803576"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a>Felkészülés az Office központi telepítésére Microsoft 365 vállalati verzióban

Ez a cikk a Microsoft 365 Vállalati prémium verzió.

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Felkészülés az Office-appok ügyfélszámítógépekre történő automatikus telepítésére

A Microsoft 365 Vállalati prémium verzió automatikusan telepítheti a 32 bites Office alkalmazásokat Windows 10 számítógépére, és így folyamatosan frissülhet a frissítésekkel.
  
Az automatikus telepítés akkor működik a legjobban, ha a végfelhasználó számítógépe Windows 10 Business:
  
- Nincsenek telepített asztali Office-appjai (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access és OneDrive).
    
    vagy
    
- Telepítve van egy Office Kattintásra verzió.
    
Ha ki szeretné deríteni, hogy az Office Office Kattintásra verziójával rendelkezik-e, egy tetszőleges Office-appban válassza a **Fájl** \> **Fiók** (az Outlookban **Office-fiók**) lehetőséget). Ha a **Office** alábbi ábrán látható módon látja a frissítéseket, akkor a telepítés az Kattintásra használatával történt. 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Who e funkció előnyei**
  
Annak a végfelhasználónak, akinek a PC-jén:
  
- **Rendelkezik** Windows 10 Business felhasználói licenccel, aktív vállalati Microsoft 365 licenccel, Windows 10 alkotói frissítés, és csatlakozik a Azure Active Directory. 
    
- **Nincs 64** bites Office alkalmazása (például: Word, Excel, PowerPoint). Ha 64 bites Office-appokra van szükség, akkor ez a funkció nem jó illesztés, mert az Office 64 bites, 2016 Kattintásra verziója nem indítható el az Microsoft 365 Vállalati verzió felügyeleti konzolról. 
    
- **Nem található meg** egy Windows Installer (MSI) technológiával telepített különálló 2016-os app sem (például Visio vagy Project). Microsoft 365 vállalati verziós Office az Office 2016 Office Kattintásra verziójára frissít, és nem működik az Office 2016 MSI különálló appokkal. 
    
Az alábbi táblázatban látható, hogy a végfelhasználóknak/rendszergazdáknak milyen műveletet kell követniük a kezdő állapotuktól függően ahhoz, hogy az Office Vállalati verzió felügyeleti konzolján az Microsoft 365 Office 32 bites, Office Kattintásra verzióját futtatják.<br/>


|Az Office telepítésének kezdő állapota|A vállalati verziós Microsoft 365 előtt szükséges Office teendő|Záró állapot|
|:-----|:-----|:-----|
|Nincs telepítve Office programcsomag  <br/> |Nincs  <br/> |Office 2016 32 bites is telepítve van az Kattintásra használatával  <br/> |
|Az Office Kattintásra technológiával telepített Office 32 bites verziója (2016-os vagy korábbi verzió), különálló appok nélkül  <br/> |Nincs  <br/> |Frissítve az Office 2016 legújabb 32 bites, Office Kattintásra verziójára, szükség szerint **\*** <br/> |
|Az Office kattintásra és az Office Kattintásra 32 bites verziójának meglévő, 32 bites vagy 64 bites különálló Office-appok (például Visio, Project)  <br/> |Egyikre sem.  <br/> |A különálló appok nem érintettek. A programcsomag frissül az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára  <br/> |
|Az Office Kattintásra technológiával telepített Office 32 bites verziója és bármely 32 vagy 64 bites (a 2016-os verzió kivételével), MSI technológiával telepített különálló Office-app  <br/> |Nincs  <br/> |A különálló appok nem érintettek. A programcsomag frissül az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára  <br/> |
|Az Office Kattintásra technológiával telepített Office bármely meglévő, 64 bites verziója  <br/> |Távolítsa el a 64 bites Office, ha nem gond, hogy lecseréli őket a 32 bites Office alkalmazásokra  <br/> |Ha eltávolítja a 64 bites Office-appokat, az Office Kattintásra technológiával telepített Office 2016 32 bites verziója települ  <br/> |
|Az Office 2016 meglévő, MSI technológiával telepített példánya különálló appokkal vagy anélkül  <br/> |Az MSI technológiával telepített Office 2016 eltávolítása  <br/> |Telepítve van az Office Kattintásra technológiával telepített Office 2016 32 bites verziója. A különálló appokat nem érinti semmilyen változás.  <br/> |
|Az Office 2013 és/vagy különálló Office-appok meglévő, MSI technológiával telepített példánya  <br/> |Nincs  <br/> |Az Office Kattintásra technológiával telepített Office 2016 32 bites verziója, amely együtt létezik a korábbról meglévő, MSI technológiával telepített Office-példánnyal (és különálló appokkal)  <br/> |
||||
   
 **(\*) Megjegyzés:** Egy ismert hiba miatt nem történik meg az Office Kattintásra technológiával telepített Office 2016 32 bites verziójára való frissítés. Már folyamatban van a javítás. 
  

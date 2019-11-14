---
title: Az AutoPilot-profil beállításai
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- ZTDProfileSettings
- O365E_ZTDProfileSettings
- BCS365_ZTDProfileSettings
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: A robotpilóta-profilok segítségével szabályozhatja, hogyan lesz telepítve a Windows a felhasználói eszközökre. A profilok olyan alapértelmezett és választható beállításokat tartalmaznak, mint a Cortana-telepítés kihagyása.
ms.openlocfilehash: 912a24e3d458986a4bcf7dcf903f80211996aca2
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/14/2019
ms.locfileid: "38321785"
---
# <a name="about-autopilot-profile-settings"></a>Az AutoPilot-profil beállításai

## <a name="autopilot-profile-settings"></a>Az AutoPilot-profil beállításai

A robotpilóta-profilok segítségével szabályozhatja, hogyan legyen telepítve a Windows a felhasználói eszközökön. A profilok a következő beállításokat tartalmazzák.
  
 **Az AutoPilot alapértelmezett (kötelező) funkciói, amelyek beállítása automatikusan megtörténik:**
  
|**Beállítás**|**Leírás**|
|:-----|:-----|
|Ugrál Cortana, OneDrive, és OEM beírás  <br/> |A telepítő nem telepíti a Cortanához és a személyes OneDrive-hoz hasonló fogyasztói appokat. Az eszköz felhasználója ezeket később is telepítheti, amíg a felhasználó helyi rendszergazdaként van az eszközön. Az eredeti gyártó regisztrálása azért marad ki, mert az eszközt a Microsoft 365 Business fogja kezelni.  <br/> |
|Céges bejelentkezési felület  <br/> |Ha a vállalata a [vállalat márkajelzését hozzáadja az Office 365 bejelentkezés laphoz](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), akkor az eszköz felhasználója ezt a tapasztalatot bejelentkezéskor fogja kapni.  <br/> |
|Automatikus regisztrálás mobileszköz-kezelésre a konfigurált Azure Active Directory-fiókokkal  <br/> |A felhasználó azonosság lesz kezelt mellett Azure Aktivál Címtár, és használók akarat jel-ban-hoz Windows és Hivatal 365-val-uk Mikroszkóp 365 teendő megbízólevél.  <br/> |
   
 **Nem kötelező beállítások:**
  
|**Beállítás**|**Leírás**|
|:-----|:-----|
|Adatvédelmi beállítások kihagyása (alapértelmezés szerint ki van kapcsolva)  <br/> |Ha ez a beállítás **Be** van kapcsolva, a felhasználó nem látja az eszköz és a Windows licencszerződését az első bejelentkezés alkalmával.  <br/> |
|Nem léptethető elő a felhasználó a helyi rendszergazdává  <br/> |Ha ez a beállítás **Be** van kapcsolva, a felhasználó nem telepíthet személyes appokat, így például Cortanát sem.<br/> |
   

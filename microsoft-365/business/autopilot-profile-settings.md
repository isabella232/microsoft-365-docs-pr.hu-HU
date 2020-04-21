---
title: Az AutoPilot-profil beállításai
f1.keywords:
- NOCSH
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
description: Az AutoPilot-profilok segítségével szabályozhatja, hogy a Windows hogyan települjön a felhasználói eszközökre. A profilok tartalmazzák az alapértelmezett és választható beállításokat, például a Cortana telepítésének kihagyását.
ms.openlocfilehash: 5c2ec3f4c3e0ebc4ea545d11f819c897f414ad52
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/21/2020
ms.locfileid: "43627414"
---
# <a name="about-autopilot-profile-settings"></a>Az AutoPilot-profil beállításai

## <a name="autopilot-profile-settings"></a>Az AutoPilot-profil beállításai

Az AutoPilot-profilok segítségével szabályozhatja, hogy a Windows hogyan települjön a felhasználói eszközökre. A profilok a következő beállításokat tartalmazzák.
  
 **Az AutoPilot alapértelmezett (kötelező) funkciói, amelyek beállítása automatikusan megtörténik:**
  
|**Beállítás**|**Leírás**|
|:-----|:-----|
|A Cortana, a OneDrive és az OEM-regisztráció kihagyása  <br/> |A telepítő nem telepíti a Cortanához és a személyes OneDrive-hoz hasonló fogyasztói appokat. Az eszköz felhasználó telepítheti ezeket később, amíg a felhasználó egy helyi rendszergazda az eszközön. Az eredeti gyártóregisztráció kimarad, mert az eszközt a Microsoft 365 Business Premium fogja kezelni.  <br/> |
|Céges bejelentkezési felület  <br/> |Ha a vállalat rendelkezik [a Vállalati márkajelzés hozzáadása a Microsoft 365 bejelentkezési lapjára,](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a)az eszköz felhasználója ezt az élményt kapja a bejelentkezéskor.  <br/> |
|Automatikus regisztrálás mobileszköz-kezelésre a konfigurált Azure Active Directory-fiókokkal  <br/> |A felhasználói identitást az Azure Active Directory kezeli, és a felhasználók a Microsoft 365 Üzleti prémium szintű hitelesítő adataikkal jelentkeznek be a Windows ba és a Microsoft 365-be.  <br/> |
   
 **Nem kötelező beállítások:**
  
|**Beállítás**|**Leírás**|
|:-----|:-----|
|Adatvédelmi beállítások kihagyása (alapértelmezés szerint ki van kapcsolva)  <br/> |Ha ez a beállítás **Be** van kapcsolva, a felhasználó nem látja az eszköz és a Windows licencszerződését az első bejelentkezés alkalmával.  <br/> |
|Nem léptethető elő a felhasználó a helyi rendszergazdává  <br/> |Ha ez a beállítás **Be** van kapcsolva, a felhasználó nem telepíthet személyes appokat, így például Cortanát sem.<br/> |
   

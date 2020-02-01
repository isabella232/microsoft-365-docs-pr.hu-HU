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
description: Az AutoPilot-profilok segítségével szabályozhatja, hogy a Windows hogyan települjön be a felhasználói eszközökre. A profilok alapértelmezett és választható beállításokat tartalmaznak, például kihagyja a Cortana telepítését.
ms.openlocfilehash: 1cc8a3171bbc4a1e5cb531b9364c7791586fc339
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593333"
---
# <a name="about-autopilot-profile-settings"></a>Az AutoPilot-profil beállításai

## <a name="autopilot-profile-settings"></a>Az AutoPilot-profil beállításai

Az AutoPilot-profilok segítségével szabályozhatja, hogy a Windows hogyan települjön a felhasználói eszközökre. A profilok a következő beállításokat tartalmazzák.
  
 **Az AutoPilot alapértelmezett (kötelező) funkciói, amelyek beállítása automatikusan megtörténik:**
  
|**Beállítás**|**Leírás**|
|:-----|:-----|
|Cortana, OneDrive és OEM regisztráció kihagyása  <br/> |A telepítő nem telepíti a Cortanához és a személyes OneDrive-hoz hasonló fogyasztói appokat. Az eszköz felhasználója később telepítheti ezeket, amennyiben a felhasználó helyi rendszergazda az eszközön. Az eredeti gyártó regisztrálása azért marad ki, mert az eszközt a Microsoft 365 Business fogja kezelni.  <br/> |
|Céges bejelentkezési felület  <br/> |Ha a vállalat [rendelkezik a Cég márkajelzésének hozzáadása az Office 365 Bejelentkezési lapján,](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a)az eszköz felhasználója ezt a felhasználói élményt kapja a bejelentkezéskor.  <br/> |
|Automatikus regisztrálás mobileszköz-kezelésre a konfigurált Azure Active Directory-fiókokkal  <br/> |A felhasználói identitást az Azure Active Directory kezeli, és a felhasználók a Microsoft 365 Vállalati verzió hitelesítő adataival jelentkeznek be a Windows és az Office 365 rendszerbe.  <br/> |
   
 **Nem kötelező beállítások:**
  
|**Beállítás**|**Leírás**|
|:-----|:-----|
|Adatvédelmi beállítások kihagyása (alapértelmezés szerint ki van kapcsolva)  <br/> |Ha ez a beállítás **Be** van kapcsolva, a felhasználó nem látja az eszköz és a Windows licencszerződését az első bejelentkezés alkalmával.  <br/> |
|Nem léptethető elő a felhasználó a helyi rendszergazdává  <br/> |Ha ez a beállítás **Be** van kapcsolva, a felhasználó nem telepíthet személyes appokat, így például Cortanát sem.<br/> |
   

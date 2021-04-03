---
title: Az AutoPilot-profil beállításai
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: Az AutoPilot-profilok segítségével szabályozhatja, hogy miként telepíthető a Windows a felhasználói eszközökre. A profilok alapértelmezett és választható beállításokat tartalmaznak, például Cortana telepítésének kihagyása.
ms.openlocfilehash: 86f8718131f0a0b93e18e65e39e02e7d65aded1a
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578507"
---
# <a name="about-autopilot-profile-settings"></a>Az AutoPilot-profil beállításai

## <a name="autopilot-profile-settings"></a>Az AutoPilot-profil beállításai

Az AutoPilot-profilokkal szabályozhatja, hogy a Windows hogyan telepíthető a felhasználói eszközökre. A profilok a következő beállításokat tartalmazzák.
  
 **Az AutoPilot alapértelmezett (kötelező) funkciói, amelyek beállítása automatikusan megtörténik:**
  
|**Beállítás**|**Leírás**|
|:-----|:-----|
|Cortana, a OneDrive és az OEM-regisztráció kihagyása  <br/> |A telepítő nem telepíti a Cortanához és a személyes OneDrive-hoz hasonló fogyasztói appokat. Az eszköz felhasználója később telepítheti ezeket, ha a felhasználó helyi rendszergazda az eszközön. Az eredeti gyártó regisztrálása azért nem lesz berakva, mert az eszközt a Microsoft 365 Business Premium fogja kezelni.  <br/> |
|Céges bejelentkezési felület  <br/> |Ha cége rendelkezik a Céges arculat hozzáadása a [Microsoft 365](../admin/setup/customize-sign-in-page.md)Bejelentkezési laphoz, az eszköz felhasználója ezt a felhasználói élményt fogja tapasztalni a bejelentkezés során.  <br/> |
|Automatikus regisztrálás mobileszköz-kezelésre a konfigurált Azure Active Directory-fiókokkal  <br/> |A felhasználói identitást az Azure Active Directory kezeli, a felhasználók pedig a Microsoft 365 Vállalati prémium verziós hitelesítő adataik segítségével fognak bejelentkezni a Windowsba és a Microsoft 365-be.  <br/> |
   
 **Nem kötelező beállítások:**
  
|**Beállítás**|**Leírás**|
|:-----|:-----|
|Adatvédelmi beállítások kihagyása (alapértelmezés szerint ki van kapcsolva)  <br/> |Ha ez a beállítás **Be** van kapcsolva, a felhasználó nem látja az eszköz és a Windows licencszerződését az első bejelentkezés alkalmával.  <br/> |
|Nem léptethető elő a felhasználó a helyi rendszergazdává  <br/> |Ha ez a beállítás **Be** van kapcsolva, a felhasználó nem telepíthet személyes appokat, így például Cortanát sem.<br/> |

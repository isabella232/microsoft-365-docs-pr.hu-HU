---
title: Az AutoPilot-profil beállításai
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: overview
f1_keywords:
- ZTDProfileSettings
- O365E_ZTDProfileSettings
- BCS365_ZTDProfileSettings
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: Automata profilok segítségével szabályozhatja, hogyan kap a Windows telepítése a felhasználói eszközök. A profilok alapértelmezett tartalmaznak, és egyéb beállítások, például Cortana telepítésének kihagyása.
ms.openlocfilehash: 5440286f1363780c87ab60514584c4addfeea0b2
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982245"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="5089b-104">Az AutoPilot-profil beállításai</span><span class="sxs-lookup"><span data-stu-id="5089b-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="5089b-105">Az AutoPilot-profil beállításai</span><span class="sxs-lookup"><span data-stu-id="5089b-105">AutoPilot profile settings</span></span>

<span data-ttu-id="5089b-p102">Az AutoPilot-profilok segítségével szabályozhatja a Windows felhasználói eszközökre való telepítését. A profilok a következő beállításokat tartalmazzák.</span><span class="sxs-lookup"><span data-stu-id="5089b-p102">You can control how Windows gets installed on user devices by using the AutoPilot profiles. The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="5089b-108">**Az AutoPilot alapértelmezett (kötelező) funkciói, amelyek beállítása automatikusan megtörténik:**</span><span class="sxs-lookup"><span data-stu-id="5089b-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="5089b-109">**Beállítás**</span><span class="sxs-lookup"><span data-stu-id="5089b-109">**Setting**</span></span>|<span data-ttu-id="5089b-110">**Leírás**</span><span class="sxs-lookup"><span data-stu-id="5089b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5089b-111">A Cortana, a OneDrive és az OEM-regisztráció kihagyása</span><span class="sxs-lookup"><span data-stu-id="5089b-111">Skip Cortana, OneDrive and OEM registration</span></span>  <br/> |<span data-ttu-id="5089b-p103">A telepítő nem telepíti a Cortanához és a személyes OneDrive-hoz hasonló fogyasztói appokat. Az eszköz felhasználója később telepítheti őket, ha helyi rendszergazda az eszközön. Az eredeti gyártó regisztrálása azért marad ki, mert az eszközt a Microsoft 365 Business fogja kezelni.</span><span class="sxs-lookup"><span data-stu-id="5089b-p103">Skips the installation of consumer apps like Cortana and personal OneDrive. The device user can install these later as long as he or she is a local admin on the device. The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="5089b-115">Céges bejelentkezési felület</span><span class="sxs-lookup"><span data-stu-id="5089b-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="5089b-116">Ha a vállalat rendelkezik az [Office 365 bejelentkezési lapra védjegyezés hozzáadása a vállalat](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), az eszköz felhasználói tapasztalatok kap történő bejelentkezés során.</span><span class="sxs-lookup"><span data-stu-id="5089b-116">If your company has a [Add your company branding to Office 365 Sign In page](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="5089b-117">Automatikus regisztrálás mobileszköz-kezelésre a konfigurált Azure Active Directory-fiókokkal</span><span class="sxs-lookup"><span data-stu-id="5089b-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="5089b-118">A felhasználó identitását az Azure Active Directory fogja kezelni, és a felhasználók a Microsoft 365 Business-beli hitelesítő adataikkal fognak bejelentkezni a Windowsba és az Office 365-be.</span><span class="sxs-lookup"><span data-stu-id="5089b-118">The user identity will be managed by Azure Active directory, and the users will sign into Windows and Office 365 with their Microsoft 365 Business credentials.</span></span>  <br/> |
   
 <span data-ttu-id="5089b-119">**Nem kötelező beállítások:**</span><span class="sxs-lookup"><span data-stu-id="5089b-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="5089b-120">**Beállítás**</span><span class="sxs-lookup"><span data-stu-id="5089b-120">**Setting**</span></span>|<span data-ttu-id="5089b-121">**Leírás**</span><span class="sxs-lookup"><span data-stu-id="5089b-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5089b-122">Adatvédelmi beállítások kihagyása (alapértelmezés szerint ki van kapcsolva)</span><span class="sxs-lookup"><span data-stu-id="5089b-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="5089b-123">Ha ez a beállítás **Be** van kapcsolva, a felhasználó nem látja az eszköz és a Windows licencszerződését az első bejelentkezés alkalmával.</span><span class="sxs-lookup"><span data-stu-id="5089b-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="5089b-124">Nem léptethető elő a felhasználó a helyi rendszergazdává</span><span class="sxs-lookup"><span data-stu-id="5089b-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="5089b-125">Ha ez a beállítás **Be** van kapcsolva, a felhasználó nem telepíthet személyes appokat, így például Cortanát sem.</span><span class="sxs-lookup"><span data-stu-id="5089b-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span>  <br/> |
   

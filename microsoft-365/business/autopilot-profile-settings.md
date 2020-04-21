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
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="828ce-104">Az AutoPilot-profil beállításai</span><span class="sxs-lookup"><span data-stu-id="828ce-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="828ce-105">Az AutoPilot-profil beállításai</span><span class="sxs-lookup"><span data-stu-id="828ce-105">AutoPilot profile settings</span></span>

<span data-ttu-id="828ce-106">Az AutoPilot-profilok segítségével szabályozhatja, hogy a Windows hogyan települjön a felhasználói eszközökre.</span><span class="sxs-lookup"><span data-stu-id="828ce-106">You can use AutoPilot profiles to control how Windows is installed on user devices.</span></span> <span data-ttu-id="828ce-107">A profilok a következő beállításokat tartalmazzák.</span><span class="sxs-lookup"><span data-stu-id="828ce-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="828ce-108">**Az AutoPilot alapértelmezett (kötelező) funkciói, amelyek beállítása automatikusan megtörténik:**</span><span class="sxs-lookup"><span data-stu-id="828ce-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="828ce-109">**Beállítás**</span><span class="sxs-lookup"><span data-stu-id="828ce-109">**Setting**</span></span>|<span data-ttu-id="828ce-110">**Leírás**</span><span class="sxs-lookup"><span data-stu-id="828ce-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="828ce-111">A Cortana, a OneDrive és az OEM-regisztráció kihagyása</span><span class="sxs-lookup"><span data-stu-id="828ce-111">Skip Cortana, OneDrive, and OEM registration</span></span>  <br/> |<span data-ttu-id="828ce-112">A telepítő nem telepíti a Cortanához és a személyes OneDrive-hoz hasonló fogyasztói appokat.</span><span class="sxs-lookup"><span data-stu-id="828ce-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="828ce-113">Az eszköz felhasználó telepítheti ezeket később, amíg a felhasználó egy helyi rendszergazda az eszközön.</span><span class="sxs-lookup"><span data-stu-id="828ce-113">The device user can install these later as long as the user is a local admin on the device.</span></span> <span data-ttu-id="828ce-114">Az eredeti gyártóregisztráció kimarad, mert az eszközt a Microsoft 365 Business Premium fogja kezelni.</span><span class="sxs-lookup"><span data-stu-id="828ce-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="828ce-115">Céges bejelentkezési felület</span><span class="sxs-lookup"><span data-stu-id="828ce-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="828ce-116">Ha a vállalat rendelkezik [a Vállalati márkajelzés hozzáadása a Microsoft 365 bejelentkezési lapjára,](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a)az eszköz felhasználója ezt az élményt kapja a bejelentkezéskor.</span><span class="sxs-lookup"><span data-stu-id="828ce-116">If your company has a [Add your company branding to Microsoft 365 Sign In page](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="828ce-117">Automatikus regisztrálás mobileszköz-kezelésre a konfigurált Azure Active Directory-fiókokkal</span><span class="sxs-lookup"><span data-stu-id="828ce-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="828ce-118">A felhasználói identitást az Azure Active Directory kezeli, és a felhasználók a Microsoft 365 Üzleti prémium szintű hitelesítő adataikkal jelentkeznek be a Windows ba és a Microsoft 365-be.</span><span class="sxs-lookup"><span data-stu-id="828ce-118">The user identity will be managed by Azure Active Directory, and users will sign in to Windows and Microsoft 365 with their Microsoft 365 Business Premium credentials.</span></span>  <br/> |
   
 <span data-ttu-id="828ce-119">**Nem kötelező beállítások:**</span><span class="sxs-lookup"><span data-stu-id="828ce-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="828ce-120">**Beállítás**</span><span class="sxs-lookup"><span data-stu-id="828ce-120">**Setting**</span></span>|<span data-ttu-id="828ce-121">**Leírás**</span><span class="sxs-lookup"><span data-stu-id="828ce-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="828ce-122">Adatvédelmi beállítások kihagyása (alapértelmezés szerint ki van kapcsolva)</span><span class="sxs-lookup"><span data-stu-id="828ce-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="828ce-123">Ha ez a beállítás **Be** van kapcsolva, a felhasználó nem látja az eszköz és a Windows licencszerződését az első bejelentkezés alkalmával.</span><span class="sxs-lookup"><span data-stu-id="828ce-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="828ce-124">Nem léptethető elő a felhasználó a helyi rendszergazdává</span><span class="sxs-lookup"><span data-stu-id="828ce-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="828ce-125">Ha ez a beállítás **Be** van kapcsolva, a felhasználó nem telepíthet személyes appokat, így például Cortanát sem.</span><span class="sxs-lookup"><span data-stu-id="828ce-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span><br/> |
   

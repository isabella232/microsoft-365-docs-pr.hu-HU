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
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="543ae-104">Az AutoPilot-profil beállításai</span><span class="sxs-lookup"><span data-stu-id="543ae-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="543ae-105">Az AutoPilot-profil beállításai</span><span class="sxs-lookup"><span data-stu-id="543ae-105">AutoPilot profile settings</span></span>

<span data-ttu-id="543ae-106">A robotpilóta-profilok segítségével szabályozhatja, hogyan legyen telepítve a Windows a felhasználói eszközökön.</span><span class="sxs-lookup"><span data-stu-id="543ae-106">You can use AutoPilot profiles to control how Windows is installed on user devices.</span></span> <span data-ttu-id="543ae-107">A profilok a következő beállításokat tartalmazzák.</span><span class="sxs-lookup"><span data-stu-id="543ae-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="543ae-108">**Az AutoPilot alapértelmezett (kötelező) funkciói, amelyek beállítása automatikusan megtörténik:**</span><span class="sxs-lookup"><span data-stu-id="543ae-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="543ae-109">**Beállítás**</span><span class="sxs-lookup"><span data-stu-id="543ae-109">**Setting**</span></span>|<span data-ttu-id="543ae-110">**Leírás**</span><span class="sxs-lookup"><span data-stu-id="543ae-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="543ae-111">Ugrál Cortana, OneDrive, és OEM beírás</span><span class="sxs-lookup"><span data-stu-id="543ae-111">Skip Cortana, OneDrive, and OEM registration</span></span>  <br/> |<span data-ttu-id="543ae-112">A telepítő nem telepíti a Cortanához és a személyes OneDrive-hoz hasonló fogyasztói appokat.</span><span class="sxs-lookup"><span data-stu-id="543ae-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="543ae-113">Az eszköz felhasználója ezeket később is telepítheti, amíg a felhasználó helyi rendszergazdaként van az eszközön.</span><span class="sxs-lookup"><span data-stu-id="543ae-113">The device user can install these later as long as the user is a local admin on the device.</span></span> <span data-ttu-id="543ae-114">Az eredeti gyártó regisztrálása azért marad ki, mert az eszközt a Microsoft 365 Business fogja kezelni.</span><span class="sxs-lookup"><span data-stu-id="543ae-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="543ae-115">Céges bejelentkezési felület</span><span class="sxs-lookup"><span data-stu-id="543ae-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="543ae-116">Ha a vállalata a [vállalat márkajelzését hozzáadja az Office 365 bejelentkezés laphoz](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), akkor az eszköz felhasználója ezt a tapasztalatot bejelentkezéskor fogja kapni.</span><span class="sxs-lookup"><span data-stu-id="543ae-116">If your company has a [Add your company branding to Office 365 Sign In page](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="543ae-117">Automatikus regisztrálás mobileszköz-kezelésre a konfigurált Azure Active Directory-fiókokkal</span><span class="sxs-lookup"><span data-stu-id="543ae-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="543ae-118">A felhasználó azonosság lesz kezelt mellett Azure Aktivál Címtár, és használók akarat jel-ban-hoz Windows és Hivatal 365-val-uk Mikroszkóp 365 teendő megbízólevél.</span><span class="sxs-lookup"><span data-stu-id="543ae-118">The user identity will be managed by Azure Active Directory, and users will sign in to Windows and Office 365 with their Microsoft 365 Business credentials.</span></span>  <br/> |
   
 <span data-ttu-id="543ae-119">**Nem kötelező beállítások:**</span><span class="sxs-lookup"><span data-stu-id="543ae-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="543ae-120">**Beállítás**</span><span class="sxs-lookup"><span data-stu-id="543ae-120">**Setting**</span></span>|<span data-ttu-id="543ae-121">**Leírás**</span><span class="sxs-lookup"><span data-stu-id="543ae-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="543ae-122">Adatvédelmi beállítások kihagyása (alapértelmezés szerint ki van kapcsolva)</span><span class="sxs-lookup"><span data-stu-id="543ae-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="543ae-123">Ha ez a beállítás **Be** van kapcsolva, a felhasználó nem látja az eszköz és a Windows licencszerződését az első bejelentkezés alkalmával.</span><span class="sxs-lookup"><span data-stu-id="543ae-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="543ae-124">Nem léptethető elő a felhasználó a helyi rendszergazdává</span><span class="sxs-lookup"><span data-stu-id="543ae-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="543ae-125">Ha ez a beállítás **Be** van kapcsolva, a felhasználó nem telepíthet személyes appokat, így például Cortanát sem.</span><span class="sxs-lookup"><span data-stu-id="543ae-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span><br/> |
   

---
title: Feltételes hozzáférési házirendek beállítása a Microsoft 365-kampányokhoz
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
description: Megtudhatja, hogy miként állíthat be feltételes hozzáférési szabályzatokat a Microsoft 365-kampányokhoz, hogy jelentős további biztonságot nyújtjon.
ms.openlocfilehash: 58ee760877ee2fd7e53ef9463242657ab66a2b6e
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44470647"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="811fc-103">Feltételes hozzáférési házirendek beállítása</span><span class="sxs-lookup"><span data-stu-id="811fc-103">Set up conditional access policies</span></span>

<span data-ttu-id="811fc-104">Ez a cikk a Microsoft 365 Business Premium szolgáltatásra vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="811fc-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="811fc-105">[A feltételes hozzáférési](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) házirendek jelentős további biztonságot adnak.</span><span class="sxs-lookup"><span data-stu-id="811fc-105">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substantial additional security.</span></span> <span data-ttu-id="811fc-106">A Microsoft olyan alapszintű feltételes hozzáférési házirendeket biztosít, amelyek minden ügyfél számára ajánlottak.</span><span class="sxs-lookup"><span data-stu-id="811fc-106">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="811fc-107">Az alapházirendek olyan előre definiált házirendek, amelyek segítenek megvédeni a szervezeteket számos gyakori támadásellen.</span><span class="sxs-lookup"><span data-stu-id="811fc-107">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="811fc-108">Ezek a gyakori támadások közé tartozhat a jelszóspray, a visszajátszás és az adathalászat.</span><span class="sxs-lookup"><span data-stu-id="811fc-108">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="811fc-109">Ezek a házirendek megkövetelik a rendszergazdáktól és a felhasználóktól, hogy bizonyos feltételek teljesülése esetén adjanak meg egy második hitelesítési formát (úgynevezett többtényezős hitelesítést vagy Többtényezős hitelesítést).</span><span class="sxs-lookup"><span data-stu-id="811fc-109">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="811fc-110">Ha például egy felhasználó egy másik országból jelentkezik be, a bejelentkezés kockázatosnak minősülhet, és a felhasználónak egy további hitelesítési formát kell megadnia.</span><span class="sxs-lookup"><span data-stu-id="811fc-110">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="811fc-111">Az alappolitikák jelenleg a következők:</span><span class="sxs-lookup"><span data-stu-id="811fc-111">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="811fc-112">**Többkori faszükségtelével kell elévülve a rendszergazdákszámára** &ndash; Többtényezős hitelesítést igényel a legtöbb kiemelt rendszergazdai szerepkörhöz, beleértve a globális rendszergazdai szerepköröket is.</span><span class="sxs-lookup"><span data-stu-id="811fc-112">**Require MFA for admins** &ndash; Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="811fc-113">**Végfelhasználói védelem** &ndash; Többtényezős hitelesítést igényel a felhasználók csak akkor, ha a bejelentkezés kockázatos.</span><span class="sxs-lookup"><span data-stu-id="811fc-113">**End user protection** &ndash; Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="811fc-114">**Örökölt hitelesítés blokkolása** &ndash; A régebbi ügyfélalkalmazások és néhány új alkalmazás nem használ újabb, biztonságosabb hitelesítési protokollokat.</span><span class="sxs-lookup"><span data-stu-id="811fc-114">**Block legacy authentication** &ndash; Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="811fc-115">Ezek a régebbi alkalmazások megkerülhetik a feltételes hozzáférési szabályzatokat, és jogosulatlanul hozzáférhetnek a környezethez.</span><span class="sxs-lookup"><span data-stu-id="811fc-115">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="811fc-116">Ez a házirend blokkolja a hozzáférést az ügyfelek, amelyek nem támogatják a feltételes hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="811fc-116">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="811fc-117">**Többéves kor–szolgáltatás kezeléshez szükséges többfa** &ndash; Többtényezős hitelesítést igényel a felügyeleti eszközökhöz való hozzáféréshez, beleértve az Azure Portalt (ahol konfigurálja az alapházirendeket).</span><span class="sxs-lookup"><span data-stu-id="811fc-117">**Require MFA for Service Management** &ndash; Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="811fc-118">A Microsoft azt javasolja, hogy engedélyezze az összes ilyen alapházirendet.</span><span class="sxs-lookup"><span data-stu-id="811fc-118">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="811fc-119">Miután ezek a szabályzatok engedélyezve vannak, a rendszergazdák és a felhasználók kérni fogja, hogy regisztráljon az Azure multii-factor hitelesítés.</span><span class="sxs-lookup"><span data-stu-id="811fc-119">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="811fc-120">Ezekről a házirendekről a [Mik az alapházirendek?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)</span><span class="sxs-lookup"><span data-stu-id="811fc-120">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="811fc-121">Alaptervházirendek beállítása</span><span class="sxs-lookup"><span data-stu-id="811fc-121">Set up baseline policies</span></span>

1. <span data-ttu-id="811fc-122">Nyissa meg az [Azure Portalt,](https://portal.azure.com)és keresse meg az **Azure Active Directory** feltételes \> **hozzáférését.**</span><span class="sxs-lookup"><span data-stu-id="811fc-122">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="811fc-123">Az alapházirendek az oldalon vannak felsorolva.</span><span class="sxs-lookup"><span data-stu-id="811fc-123">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="811fc-124">![A feltételes hozzáférés alapházirendjeit felsoroló lap.](../media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="811fc-124">![Page that lists baseline policies for conditional access.](../media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="811fc-125">Az egyes házirendekhez tartozó alábbi konkrét utasításokat olvassa el:</span><span class="sxs-lookup"><span data-stu-id="811fc-125">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="811fc-126">Többkori faszükségtelével kell elévülve a rendszergazdákszámára</span><span class="sxs-lookup"><span data-stu-id="811fc-126">Require MFA for admins</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="811fc-127">Többkori faszükséglés megkövetelése a felhasználók számára</span><span class="sxs-lookup"><span data-stu-id="811fc-127">Require MFA for users</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="811fc-128">Örökölt hitelesítés blokkolása</span><span class="sxs-lookup"><span data-stu-id="811fc-128">Block legacy authentication</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="811fc-129">Többéves kortól megkövetelhető a szolgáltatáskezeléshez</span><span class="sxs-lookup"><span data-stu-id="811fc-129">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="811fc-130">Számos további szabályzatot állíthat be, például jóváhagyott ügyfélalkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="811fc-130">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="811fc-131">További információt a [Feltételes hozzáférés dokumentációjában talál.](https://docs.microsoft.com/azure/active-directory/conditional-access/)</span><span class="sxs-lookup"><span data-stu-id="811fc-131">For more information, see the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>

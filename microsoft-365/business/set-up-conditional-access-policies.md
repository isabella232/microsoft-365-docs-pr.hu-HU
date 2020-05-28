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
ms.openlocfilehash: d7c9cfee2ef00e4ebe231a28ccca185c10f53c6b
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403018"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="8e43c-103">Feltételes hozzáférési házirendek beállítása</span><span class="sxs-lookup"><span data-stu-id="8e43c-103">Set up conditional access policies</span></span>

<span data-ttu-id="8e43c-104">[A feltételes hozzáférési](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) házirendek jelentős további biztonságot adnak.</span><span class="sxs-lookup"><span data-stu-id="8e43c-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substantial additional security.</span></span> <span data-ttu-id="8e43c-105">A Microsoft olyan alapszintű feltételes hozzáférési házirendeket biztosít, amelyek minden ügyfél számára ajánlottak.</span><span class="sxs-lookup"><span data-stu-id="8e43c-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="8e43c-106">Az alapházirendek olyan előre definiált házirendek, amelyek segítenek megvédeni a szervezeteket számos gyakori támadásellen.</span><span class="sxs-lookup"><span data-stu-id="8e43c-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="8e43c-107">Ezek a gyakori támadások közé tartozhat a jelszóspray, a visszajátszás és az adathalászat.</span><span class="sxs-lookup"><span data-stu-id="8e43c-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="8e43c-108">Ezek a házirendek megkövetelik a rendszergazdáktól és a felhasználóktól, hogy bizonyos feltételek teljesülése esetén adjanak meg egy második hitelesítési formát (úgynevezett többtényezős hitelesítést vagy Többtényezős hitelesítést).</span><span class="sxs-lookup"><span data-stu-id="8e43c-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="8e43c-109">Ha például egy felhasználó egy másik országból jelentkezik be, a bejelentkezés kockázatosnak minősülhet, és a felhasználónak egy további hitelesítési formát kell megadnia.</span><span class="sxs-lookup"><span data-stu-id="8e43c-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="8e43c-110">Az alappolitikák jelenleg a következők:</span><span class="sxs-lookup"><span data-stu-id="8e43c-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="8e43c-111">**Többkori faszükségtelével kell elévülve a rendszergazdákszámára** &ndash; Többtényezős hitelesítést igényel a legtöbb kiemelt rendszergazdai szerepkörhöz, beleértve a globális rendszergazdai szerepköröket is.</span><span class="sxs-lookup"><span data-stu-id="8e43c-111">**Require MFA for admins** &ndash; Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="8e43c-112">**Végfelhasználói védelem** &ndash; Többtényezős hitelesítést igényel a felhasználók csak akkor, ha a bejelentkezés kockázatos.</span><span class="sxs-lookup"><span data-stu-id="8e43c-112">**End user protection** &ndash; Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="8e43c-113">**Örökölt hitelesítés blokkolása** &ndash; A régebbi ügyfélalkalmazások és néhány új alkalmazás nem használ újabb, biztonságosabb hitelesítési protokollokat.</span><span class="sxs-lookup"><span data-stu-id="8e43c-113">**Block legacy authentication** &ndash; Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="8e43c-114">Ezek a régebbi alkalmazások megkerülhetik a feltételes hozzáférési szabályzatokat, és jogosulatlanul hozzáférhetnek a környezethez.</span><span class="sxs-lookup"><span data-stu-id="8e43c-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="8e43c-115">Ez a házirend blokkolja a hozzáférést az ügyfelek, amelyek nem támogatják a feltételes hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="8e43c-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="8e43c-116">**Többéves kor–szolgáltatás kezeléshez szükséges többfa** &ndash; Többtényezős hitelesítést igényel a felügyeleti eszközökhöz való hozzáféréshez, beleértve az Azure Portalt (ahol konfigurálja az alapházirendeket).</span><span class="sxs-lookup"><span data-stu-id="8e43c-116">**Require MFA for Service Management** &ndash; Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="8e43c-117">A Microsoft azt javasolja, hogy engedélyezze az összes ilyen alapházirendet.</span><span class="sxs-lookup"><span data-stu-id="8e43c-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="8e43c-118">Miután ezek a szabályzatok engedélyezve vannak, a rendszergazdák és a felhasználók kérni fogja, hogy regisztráljon az Azure multii-factor hitelesítés.</span><span class="sxs-lookup"><span data-stu-id="8e43c-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="8e43c-119">Ezekről a házirendekről a [Mik az alapházirendek?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)</span><span class="sxs-lookup"><span data-stu-id="8e43c-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="8e43c-120">Alaptervházirendek beállítása</span><span class="sxs-lookup"><span data-stu-id="8e43c-120">Set up baseline policies</span></span>

1. <span data-ttu-id="8e43c-121">Nyissa meg az [Azure Portalt,](https://portal.azure.com)és keresse meg az **Azure Active Directory** feltételes \> **hozzáférését.**</span><span class="sxs-lookup"><span data-stu-id="8e43c-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="8e43c-122">Az alapházirendek az oldalon vannak felsorolva.</span><span class="sxs-lookup"><span data-stu-id="8e43c-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="8e43c-123">![A feltételes hozzáférés alapházirendjeit felsoroló lap.](../media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="8e43c-123">![Page that lists baseline policies for conditional access.](../media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="8e43c-124">Az egyes házirendekhez tartozó alábbi konkrét utasításokat olvassa el:</span><span class="sxs-lookup"><span data-stu-id="8e43c-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="8e43c-125">Többkori faszükségtelével kell elévülve a rendszergazdákszámára</span><span class="sxs-lookup"><span data-stu-id="8e43c-125">Require MFA for admins</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="8e43c-126">Többkori faszükséglés megkövetelése a felhasználók számára</span><span class="sxs-lookup"><span data-stu-id="8e43c-126">Require MFA for users</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="8e43c-127">Örökölt hitelesítés blokkolása</span><span class="sxs-lookup"><span data-stu-id="8e43c-127">Block legacy authentication</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="8e43c-128">Többéves kortól megkövetelhető a szolgáltatáskezeléshez</span><span class="sxs-lookup"><span data-stu-id="8e43c-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="8e43c-129">Számos további szabályzatot állíthat be, például jóváhagyott ügyfélalkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="8e43c-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="8e43c-130">További információt a [Feltételes hozzáférés dokumentációjában talál.](https://docs.microsoft.com/azure/active-directory/conditional-access/)</span><span class="sxs-lookup"><span data-stu-id="8e43c-130">For more information, see the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>

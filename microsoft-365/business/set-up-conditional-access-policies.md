---
title: Feltételes hozzáférési házirendek beállítása a Microsoft 365 kampányhoz
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
search.appverid:
- BCS160
- MET150
- MOE150
description: Útmutató a Microsoft 365 kampányok feltételes hozzáférési házirendjeinek beállításához.
ms.openlocfilehash: 3772aa0d505ef54a0587423e890ede519d571e0c
ms.sourcegitcommit: 70e920f76526f47fc849df615de4569e0ac2f4be
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/07/2019
ms.locfileid: "38031395"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="58631-103">Feltételes hozzáférési házirendek beállítása</span><span class="sxs-lookup"><span data-stu-id="58631-103">Set up conditional access policies</span></span>

<span data-ttu-id="58631-104">A [feltételes hozzáférésű](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) házirendek további biztonságot is hozzáadnak.</span><span class="sxs-lookup"><span data-stu-id="58631-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substancial additional security.</span></span> <span data-ttu-id="58631-105">A Microsoft az összes ügyfelnél ajánlott alaptervi feltételes hozzáférési házirendeket biztosít.</span><span class="sxs-lookup"><span data-stu-id="58631-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="58631-106">Az alapirányelvek olyan előre definiált házirendek, amelyek segítenek megvédeni a szervezeteket a sok gyakori támadástól.</span><span class="sxs-lookup"><span data-stu-id="58631-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="58631-107">Ezek a gyakori támadások lehetnek jelszó spray, visszajátszás, és az adathalászat.</span><span class="sxs-lookup"><span data-stu-id="58631-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="58631-108">Ezek a házirendek megkövetelik a rendszergazdákról és a felhasználóktól, hogy egy második hitelesítési formát (többtényezős hitelesítést vagy MFA) adjon meg, ha bizonyos feltételek teljesülnek.</span><span class="sxs-lookup"><span data-stu-id="58631-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="58631-109">Ha például egy felhasználó egy másik országból jelentkezik be, a bejelentkezés kockázatosnak tekinthető, és a felhasználónak meg kell adnia egy további hitelesítési formát.</span><span class="sxs-lookup"><span data-stu-id="58631-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="58631-110">Jelenleg az alábbi alapirányelvek tartalmazzák a következőket:</span><span class="sxs-lookup"><span data-stu-id="58631-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="58631-111">**Megkövetel MFA részére admins** — megkövetel multi--tényező hitelesítés részére a leg--bb kiváltságos ügyintéző szerepek, beleértve világ-ügyintéző.</span><span class="sxs-lookup"><span data-stu-id="58631-111">**Require MFA for admins** — Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="58631-112">**Végfelhasználói védelem** – csak akkor igényel többtényezős hitelesítést a felhasználóknak, ha a bejelentkezés kockázatos.</span><span class="sxs-lookup"><span data-stu-id="58631-112">**End user protection** — Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="58631-113">**Örökölt hitelesítés blokkolása** — a régebbi ügyfélalkalmazások és néhány új alkalmazás nem használ újabb, biztonságosabb hitelesítési protokollokat.</span><span class="sxs-lookup"><span data-stu-id="58631-113">**Block legacy authentication** — Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="58631-114">Ezek a régebbi alkalmazások megkerülhetik a feltételes hozzáférési házirendeket, és jogosulatlan hozzáférést nyerhetnek a környezetéhez.</span><span class="sxs-lookup"><span data-stu-id="58631-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="58631-115">Ez a házirend blokkolja a feltételes hozzáférést nem támogató ügyfélszámítógépekről való hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="58631-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="58631-116">**Szükséges az MFA szolgáltatás kezelése** – ehhez többtényezős hitelesítésre van szükség a kezelőeszközök számára, beleértve az Azure portált is (ahol az alaptervi házirendeket konfigurálja).</span><span class="sxs-lookup"><span data-stu-id="58631-116">**Require MFA for Service Management** — Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="58631-117">A Microsoft az alábbi alapházirendek használatát javasolja.</span><span class="sxs-lookup"><span data-stu-id="58631-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="58631-118">Miután ezek a házirendek engedélyezve vannak, a rendszer megkérdezi az adminisztrátorokat és a felhasználókat, hogy regisztrálják-e az Azure Multii-Factor hitelesítést.</span><span class="sxs-lookup"><span data-stu-id="58631-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="58631-119">További információt ezekről a házirendekkel kapcsolatban: [Mik az alaptervi szabályzatok](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span><span class="sxs-lookup"><span data-stu-id="58631-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="58631-120">Alaptervi házirendek beállítása</span><span class="sxs-lookup"><span data-stu-id="58631-120">Set up baseline policies</span></span>

1. <span data-ttu-id="58631-121">Látogasson el az [Azure portálra](https://portal.azure.com), majd keresse meg az **Azure Active Directory** \> **feltételes elérését**.</span><span class="sxs-lookup"><span data-stu-id="58631-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="58631-122">Az alapházirendek az oldalon vannak felsorolva.</span><span class="sxs-lookup"><span data-stu-id="58631-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="58631-123">![A feltételes hozzáférésű alaptervi házirendeket tartalmazó lap.](media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="58631-123">![Page that lists baseline policies for conditional access.](media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="58631-124">Az egyes házirendek esetében tekintse meg a következő konkrét utasításokat:</span><span class="sxs-lookup"><span data-stu-id="58631-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="58631-125">MFA megkövetelése az adminoknak</span><span class="sxs-lookup"><span data-stu-id="58631-125">Require MFA for admins</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="58631-126">A felhasználók számára az MFA megkövetelése</span><span class="sxs-lookup"><span data-stu-id="58631-126">Require MFA for users</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="58631-127">Örökölt hitelesítés blokkolása</span><span class="sxs-lookup"><span data-stu-id="58631-127">Block legacy authentication</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="58631-128">Az MFA megkövetelése a Szervizkezelés számára</span><span class="sxs-lookup"><span data-stu-id="58631-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="58631-129">Számos további házirend is beállítható, például a jóváhagyott ügyfélalkalmazások megkövetelése.</span><span class="sxs-lookup"><span data-stu-id="58631-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="58631-130">További információt a [feltételes hozzáférésű dokumentációban](https://docs.microsoft.com/azure/active-directory/conditional-access/) talál.</span><span class="sxs-lookup"><span data-stu-id="58631-130">See the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/) for more information.</span></span>
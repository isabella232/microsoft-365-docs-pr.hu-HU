---
title: Microsoft 365 kampányok feltételes hozzáférési házirendek beállítása
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
search.appverid:
- BCS160
- MET150
- MOE150
description: Útmutató a Microsoft 365 kampányok feltételes hozzáférési házirendek beállítása.
ms.openlocfilehash: 7d8e1f16019d151478aae57b1593b0e0758e5b19
ms.sourcegitcommit: 7e46db0b35c188ee6a7b40ab3eb2d76ff6c101c5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/19/2019
ms.locfileid: "35086349"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="8d53e-103">Feltételes hozzáférési házirendek beállítása</span><span class="sxs-lookup"><span data-stu-id="8d53e-103">Set up conditional access policies</span></span>

<span data-ttu-id="8d53e-104">[Feltételes hozzáférési](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) házirendek hozzá további biztonsági substancial.</span><span class="sxs-lookup"><span data-stu-id="8d53e-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substancial additional security.</span></span> <span data-ttu-id="8d53e-105">A Microsoft baseline feltételes hozzáférési házirendek ajánlott biztosít az összes vevőre.</span><span class="sxs-lookup"><span data-stu-id="8d53e-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="8d53e-106">Eredeti házirendek olyan előre definiált házirendeket, amelyek a szervezetek sok közös támadások elleni védelme.</span><span class="sxs-lookup"><span data-stu-id="8d53e-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="8d53e-107">E közös támadások lehetnek jelszó spray, ismétlés és az adathalászat.</span><span class="sxs-lookup"><span data-stu-id="8d53e-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="8d53e-108">Ezek a házirendek szükséges rendszergazdák és a felhasználók egy második űrlap (úgynevezett többtényezős hitelesítést, vagy MFA) hitelesítés megadása esetén bizonyos feltételek teljesülése esetén.</span><span class="sxs-lookup"><span data-stu-id="8d53e-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="8d53e-109">Például ha egy felhasználó egy másik ország bejelentkezés során, bejelentkezési fontolóra lehet venni a kockázatos, és a felhasználónak meg kell adnia egy további formája.</span><span class="sxs-lookup"><span data-stu-id="8d53e-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="8d53e-110">Jelenleg eredeti házirendek a következők:</span><span class="sxs-lookup"><span data-stu-id="8d53e-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="8d53e-111">**A rendszergazdák számára szükséges MFA** – leginkább kiemelt rendszergazdai szerepkörhöz, beleértve a globális rendszergazdai többtényezős hitelesítést igényel.</span><span class="sxs-lookup"><span data-stu-id="8d53e-111">**Require MFA for admins** — Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="8d53e-112">**Végfelhasználó védelem** – felhasználók többtényezős hitelesítést igényel, csak ha a jel a kockázatos.</span><span class="sxs-lookup"><span data-stu-id="8d53e-112">**End user protection** — Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="8d53e-113">**Régebbi hitelesítés blokk** – régebbi ügyfélalkalmazások és néhány új alkalmazás újabb, biztonságosabb, hitelesítési protokollok nem használ.</span><span class="sxs-lookup"><span data-stu-id="8d53e-113">**Block legacy authentication** — Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="8d53e-114">A régebbi alkalmazások átugorhatjuk a feltételes hozzáférési házirendek, és a környezet jogosulatlan hozzáférést szerezhet.</span><span class="sxs-lookup"><span data-stu-id="8d53e-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="8d53e-115">A házirend blokkolja, amelyek nem támogatják a feltételes hozzáférésű ügyfelek hozzáférése.</span><span class="sxs-lookup"><span data-stu-id="8d53e-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="8d53e-116">**Szolgáltatáskezelési szükséges MFA** – eszközök, beleértve (amennyiben Ön eredeti házirendek konfigurálása) Azure portal eléréséhez többtényezős hitelesítést igényel.</span><span class="sxs-lookup"><span data-stu-id="8d53e-116">**Require MFA for Service Management** — Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="8d53e-117">A Microsoft javasolja, hogy az összes eredeti házirendek lehetővé teszik.</span><span class="sxs-lookup"><span data-stu-id="8d53e-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="8d53e-118">Után a házirend engedélyezve van, a rendszergazdák és a felhasználók regisztrálni Azure Multii-tényező hitelesítés kéri.</span><span class="sxs-lookup"><span data-stu-id="8d53e-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="8d53e-119">További információt ezekről az irányelvekről lásd: [Mik az eredeti házirendek](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span><span class="sxs-lookup"><span data-stu-id="8d53e-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="8d53e-120">Eredeti házirendek beállítása</span><span class="sxs-lookup"><span data-stu-id="8d53e-120">Set up baseline policies</span></span>

1. <span data-ttu-id="8d53e-121">[Borzas portal](https://portal.azure.com)lépjen, és keresse meg **Az Active Directory Azure** \> **a feltételes hozzáférésű**.</span><span class="sxs-lookup"><span data-stu-id="8d53e-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="8d53e-122">Az eredeti házirendek jelennek meg az oldalon.</span><span class="sxs-lookup"><span data-stu-id="8d53e-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="8d53e-123">![A feltételes hozzáférésű eredeti szabályzatok listája lap.](media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="8d53e-123">![Page that lists baseline policies for conditional access.](media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="8d53e-124">Olvassa el az alábbi konkrét utasításokat minden:</span><span class="sxs-lookup"><span data-stu-id="8d53e-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="8d53e-125">MFA igényelnek a rendszergazdák számára</span><span class="sxs-lookup"><span data-stu-id="8d53e-125">Require MFA for admins</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="8d53e-126">A felhasználók Reequire MFA</span><span class="sxs-lookup"><span data-stu-id="8d53e-126">Reequire MFA for users</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="8d53e-127">Régebbi hitelesítés letiltása</span><span class="sxs-lookup"><span data-stu-id="8d53e-127">Block legacy authentication</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="8d53e-128">Szükséges az MFA-kezelő</span><span class="sxs-lookup"><span data-stu-id="8d53e-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="8d53e-129">Beállíthatja például a jóváhagyott ügyfélalkalmazások igénylő számos további házirendeket.</span><span class="sxs-lookup"><span data-stu-id="8d53e-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="8d53e-130">További információt a [Feltételes hozzáférést biztosító dokumentációjában](https://docs.microsoft.com/azure/active-directory/conditional-access/) talál.</span><span class="sxs-lookup"><span data-stu-id="8d53e-130">See the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/) for more information.</span></span>
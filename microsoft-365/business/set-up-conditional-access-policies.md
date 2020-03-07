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
search.appverid:
- BCS160
- MET150
- MOE150
description: Megtudhatja, hogy miként állíthat be feltételes hozzáférési házirendeket a Microsoft 365-kampányokhoz, hogy további jelentős biztonságot nyújthassanak.
ms.openlocfilehash: eda65e335df2a7c2c443d7095f7b35b5c1cf27e4
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/07/2020
ms.locfileid: "42561220"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="35284-103">Feltételes hozzáférési házirendek beállítása</span><span class="sxs-lookup"><span data-stu-id="35284-103">Set up conditional access policies</span></span>

<span data-ttu-id="35284-104">[A feltételes hozzáférési](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) házirendek jelentős további biztonságot adnak hozzá.</span><span class="sxs-lookup"><span data-stu-id="35284-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substantial additional security.</span></span> <span data-ttu-id="35284-105">A Microsoft az összes ügyfél számára ajánlott alapkonfigurációs feltételes hozzáférési házirendek egy sorát biztosítja.</span><span class="sxs-lookup"><span data-stu-id="35284-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="35284-106">Az alapházirendek olyan előre definiált házirendek, amelyek segítenek megvédeni a szervezeteket számos gyakori támadással szemben.</span><span class="sxs-lookup"><span data-stu-id="35284-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="35284-107">Ezek a gyakori támadások közé tartozhat a jelszóspray, a visszajátszás és az adathalászat.</span><span class="sxs-lookup"><span data-stu-id="35284-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="35284-108">Ezek a házirendek megkövetelik a rendszergazdáktól és a felhasználóktól, hogy bizonyos feltételek teljesülése esetén adjanak meg egy második hitelesítési formát (más néven többtényezős hitelesítést vagy MFA-t).</span><span class="sxs-lookup"><span data-stu-id="35284-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="35284-109">Ha például egy felhasználó egy másik országból jelentkezik be, a bejelentkezés kockázatosnak tekinthető, és a felhasználónak egy további hitelesítési formát kell megadnia.</span><span class="sxs-lookup"><span data-stu-id="35284-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="35284-110">Jelenleg az alapházirendek a következőket tartalmazzák:</span><span class="sxs-lookup"><span data-stu-id="35284-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="35284-111">**A rendszergazdák többtényezős hitelesítésének megkövetelése többtényezős** &ndash; hitelesítést igényel a legtöbb kiemelt rendszergazdai szerepkörhöz, beleértve a globális rendszergazdát is.</span><span class="sxs-lookup"><span data-stu-id="35284-111">**Require MFA for admins** &ndash; Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="35284-112">**A végfelhasználói védelem** &ndash; csak akkor igényel többtényezős hitelesítést a felhasználók számára, ha a bejelentkezés kockázatos.</span><span class="sxs-lookup"><span data-stu-id="35284-112">**End user protection** &ndash; Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="35284-113">**Letiltás a régebbi hitelesítéssel** &ndash; Régebbi ügyfélalkalmazások és néhány új alkalmazás nem használ újabb, biztonságosabb hitelesítési protokollokat.</span><span class="sxs-lookup"><span data-stu-id="35284-113">**Block legacy authentication** &ndash; Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="35284-114">Ezek a régebbi alkalmazások megkerülhetik a feltételes hozzáférési szabályzatokat, és jogosulatlan ultrásként juthatnak el a környezethez.</span><span class="sxs-lookup"><span data-stu-id="35284-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="35284-115">Ez a házirend blokkolja a feltételes hozzáférést nem támogató ügyfelek hozzáférését.</span><span class="sxs-lookup"><span data-stu-id="35284-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="35284-116">A &ndash; **szolgáltatáskezelés többtényezős hitelesítésének megkövetelése** többtényezős hitelesítést igényel a felügyeleti eszközökhöz való hozzáféréshez, beleértve az Azure Portalt is (ahol az alapházirendeket konfigurálja).</span><span class="sxs-lookup"><span data-stu-id="35284-116">**Require MFA for Service Management** &ndash; Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="35284-117">A Microsoft azt javasolja, hogy engedélyezze az összes alapházirendet.</span><span class="sxs-lookup"><span data-stu-id="35284-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="35284-118">Miután ezek a szabályzatok engedélyezve vannak, a rendszergazdák és a felhasználók kérik, hogy regisztráljon az Azure Multii-Factor hitelesítés.</span><span class="sxs-lookup"><span data-stu-id="35284-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="35284-119">Ezekről a házirendekről további információt [a Mik az alapházirendek?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)</span><span class="sxs-lookup"><span data-stu-id="35284-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="35284-120">Alapházirendek beállítása</span><span class="sxs-lookup"><span data-stu-id="35284-120">Set up baseline policies</span></span>

1. <span data-ttu-id="35284-121">Nyissa meg az [Azure Portalot,](https://portal.azure.com)majd keresse meg az **Azure Active Directory** \> **feltételes hozzáférését.**</span><span class="sxs-lookup"><span data-stu-id="35284-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="35284-122">Az alapházirendek az oldalon jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="35284-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="35284-123">![A feltételes hozzáférés alapházirendjeit tartalmazó lap.](../media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="35284-123">![Page that lists baseline policies for conditional access.](../media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="35284-124">Az egyes házirendekhez tartozó alábbi utasításokat találja:</span><span class="sxs-lookup"><span data-stu-id="35284-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="35284-125">Többoldalz megkövetelése rendszergazdáknak</span><span class="sxs-lookup"><span data-stu-id="35284-125">Require MFA for admins</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="35284-126">Többéves fa megkövetelése a felhasználók számára</span><span class="sxs-lookup"><span data-stu-id="35284-126">Require MFA for users</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="35284-127">Örökölt hitelesítés blokkolása</span><span class="sxs-lookup"><span data-stu-id="35284-127">Block legacy authentication</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="35284-128">Többéves fa megkövetelése a szolgáltatáskezeléshez</span><span class="sxs-lookup"><span data-stu-id="35284-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="35284-129">Számos további szabályzatot is beállíthat, például jóváhagyott ügyfélalkalmazásokat igényel.</span><span class="sxs-lookup"><span data-stu-id="35284-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="35284-130">További információt a [Feltételes hozzáférés dokumentációjában](https://docs.microsoft.com/azure/active-directory/conditional-access/)talál.</span><span class="sxs-lookup"><span data-stu-id="35284-130">For more information, see the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>

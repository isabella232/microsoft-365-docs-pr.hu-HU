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
ms.openlocfilehash: aebdb733c2dd9a05947335ad4f151104d801568e
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38718829"
---
# <a name="set-up-conditional-access-policies"></a>Feltételes hozzáférési házirendek beállítása

A [feltételes hozzáférési](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) házirendek jelentős további biztonságot adhatnak. A Microsoft az összes ügyfelnél ajánlott alaptervi feltételes hozzáférési házirendeket biztosít. Az alapirányelvek olyan előre definiált házirendek, amelyek segítenek megvédeni a szervezeteket a sok gyakori támadástól. Ezek a gyakori támadások lehetnek jelszó spray, visszajátszás, és az adathalászat.

Ezek a házirendek megkövetelik a rendszergazdákról és a felhasználóktól, hogy egy második hitelesítési formát (többtényezős hitelesítést vagy MFA) adjon meg, ha bizonyos feltételek teljesülnek. Ha például egy felhasználó egy másik országból jelentkezik be, a bejelentkezés kockázatosnak tekinthető, és a felhasználónak meg kell adnia egy további hitelesítési formát. 

Jelenleg az alábbi alapirányelvek tartalmazzák a következőket:
- A &ndash; **rendszergazdák számára az MFA megkövetelése** többtényezős hitelesítést igényel a legkiváltságosabb rendszergazdai szerepkörökhöz, beleértve a globális rendszergazdát is.
- A **végfelhasználói védelem** &ndash; csak akkor igényel többtényezős hitelesítést a felhasználóknak, ha a bejelentkezés kockázatos. 
- **Örökölt hitelesítés** &ndash; letiltása régebbi ügyfélalkalmazások és néhány új alkalmazás nem használ újabb, biztonságosabb hitelesítési protokollokat. Ezek a régebbi alkalmazások megkerülhetik a feltételes hozzáférési házirendeket, és jogosulatlan hozzáférést nyerhetnek a környezetéhez. Ez a házirend blokkolja a feltételes hozzáférést nem támogató ügyfélszámítógépekről való hozzáférést. 
- **Megkövetel MFA részére szolgáltatás vezetés** &ndash; megkövetel multi--tényező hitelesítés részére belépés-hoz vezetés szerszámok, beleértve Azure bejárat (hol vagy configure alap politikák). 

A Microsoft az alábbi alapházirendek használatát javasolja. Miután ezek a házirendek engedélyezve vannak, a rendszer megkérdezi az adminisztrátorokat és a felhasználókat, hogy regisztrálják-e az Azure Multii-Factor hitelesítést.

További információt ezekről a házirendekkel kapcsolatban: [Mik az alaptervi szabályzatok](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?


## <a name="set-up-baseline-policies"></a>Alaptervi házirendek beállítása

1. Látogasson el az [Azure portálra](https://portal.azure.com), majd keresse meg az **Azure Active Directory** \> **feltételes elérését**.
    
    Az alapházirendek az oldalon vannak felsorolva. <br/> <br/>
    ![A feltételes hozzáférésű alaptervi házirendeket tartalmazó lap.](media/baslinepolicies.png)
1. Az egyes házirendek esetében tekintse meg a következő konkrét utasításokat:

  - [MFA megkövetelése az adminoknak](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [A felhasználók számára az MFA megkövetelése](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Örökölt hitelesítés blokkolása](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Az MFA megkövetelése a Szervizkezelés számára](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Számos további házirend is beállítható, például a jóváhagyott ügyfélalkalmazások megkövetelése. További információért tekintse meg a [feltételes hozzáférés dokumentációját](https://docs.microsoft.com/azure/active-directory/conditional-access/).

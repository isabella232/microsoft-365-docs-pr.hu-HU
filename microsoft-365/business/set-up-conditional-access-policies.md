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
search.appverid:
- BCS160
- MET150
- MOE150
description: Útmutató a Microsoft 365 kampányok feltételes hozzáférési házirendjeinek beállításához.
ms.openlocfilehash: 614e3a6e13a14114f40ecf87bf936d4165744503
ms.sourcegitcommit: 91ff1d4339f0f043c2b43997d87d84677c79e279
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2019
ms.locfileid: "36982381"
---
# <a name="set-up-conditional-access-policies"></a>Feltételes hozzáférési házirendek beállítása

A [feltételes hozzáférésű](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) házirendek további biztonságot is hozzáadnak. A Microsoft az összes ügyfelnél ajánlott alaptervi feltételes hozzáférési házirendeket biztosít. Az alapirányelvek olyan előre definiált házirendek, amelyek segítenek megvédeni a szervezeteket a sok gyakori támadástól. Ezek a gyakori támadások lehetnek jelszó spray, visszajátszás, és az adathalászat.

Ezek a házirendek megkövetelik a rendszergazdákról és a felhasználóktól, hogy egy második hitelesítési formát (többtényezős hitelesítést vagy MFA) adjon meg, ha bizonyos feltételek teljesülnek. Ha például egy felhasználó egy másik országból jelentkezik be, a bejelentkezés kockázatosnak tekinthető, és a felhasználónak meg kell adnia egy további hitelesítési formát. 

Jelenleg az alábbi alapirányelvek tartalmazzák a következőket:
- A **rendszergazdák számára az MFA megkövetelése** – többtényezős hitelesítést igényel a legkiváltságosabb rendszergazdai szerepkörökhöz, beleértve a globális rendszergazdát is.
- **Végfelhasználói védelem** – csak akkor igényel többtényezős hitelesítést a felhasználóknak, ha a bejelentkezés kockázatos. 
- **Örökölt hitelesítés blokkolása** — a régebbi ügyfélalkalmazások és néhány új alkalmazás nem használ újabb, biztonságosabb hitelesítési protokollokat. Ezek a régebbi alkalmazások megkerülhetik a feltételes hozzáférési házirendeket, és jogosulatlan hozzáférést nyerhetnek a környezetéhez. Ez a házirend blokkolja a feltételes hozzáférést nem támogató ügyfélszámítógépekről való hozzáférést. 
- **Az MFA Szolgáltatáskezelés** futtatásához szükséges – többtényezős hitelesítést igényel a kezelőeszközök eléréséhez, beleértve az Azure portált is (ahol az alaptervi házirendeket konfigurálja). 

A Microsoft az alábbi alapházirendek használatát javasolja. Miután ezek a házirendek engedélyezve vannak, a rendszer megkérdezi az adminisztrátorokat és a felhasználókat, hogy regisztrálják-e az Azure Multii-Factor hitelesítést.

További információt ezekről a házirendekkel kapcsolatban: [Mik az alaptervi szabályzatok](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?


## <a name="set-up-baseline-policies"></a>Alaptervi házirendek beállítása

1. Látogasson el az [Azure portálra](https://portal.azure.com), majd keresse meg az **Azure Active Directory** \> **feltételes elérését**.
    
    Az alapházirendek az oldalon vannak felsorolva. <br/> <br/>
    ![A feltételes hozzáférésű alaptervi házirendeket tartalmazó lap.](media/baslinepolicies.png)
1. Az egyes házirendek esetében tekintse meg a következő konkrét utasításokat:

  - [Az MFA megkövetelése az adminoknak](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [Az MFA megkövetelése a felhasználóknak](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Örökölt hitelesítés blokkolása](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Az MFA Szolgáltatáskezelés megkövetelése](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Számos további házirend is beállítható, például a jóváhagyott ügyfélalkalmazások megkövetelése. További információt a [feltételes hozzáférésű dokumentációban](https://docs.microsoft.com/azure/active-directory/conditional-access/) talál.
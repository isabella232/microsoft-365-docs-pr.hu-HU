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
# <a name="set-up-conditional-access-policies"></a>Feltételes hozzáférési házirendek beállítása

[Feltételes hozzáférési](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) házirendek hozzá további biztonsági substancial. A Microsoft baseline feltételes hozzáférési házirendek ajánlott biztosít az összes vevőre. Eredeti házirendek olyan előre definiált házirendeket, amelyek a szervezetek sok közös támadások elleni védelme. E közös támadások lehetnek jelszó spray, ismétlés és az adathalászat.

Ezek a házirendek szükséges rendszergazdák és a felhasználók egy második űrlap (úgynevezett többtényezős hitelesítést, vagy MFA) hitelesítés megadása esetén bizonyos feltételek teljesülése esetén. Például ha egy felhasználó egy másik ország bejelentkezés során, bejelentkezési fontolóra lehet venni a kockázatos, és a felhasználónak meg kell adnia egy további formája. 

Jelenleg eredeti házirendek a következők:
- **A rendszergazdák számára szükséges MFA** – leginkább kiemelt rendszergazdai szerepkörhöz, beleértve a globális rendszergazdai többtényezős hitelesítést igényel.
- **Végfelhasználó védelem** – felhasználók többtényezős hitelesítést igényel, csak ha a jel a kockázatos. 
- **Régebbi hitelesítés blokk** – régebbi ügyfélalkalmazások és néhány új alkalmazás újabb, biztonságosabb, hitelesítési protokollok nem használ. A régebbi alkalmazások átugorhatjuk a feltételes hozzáférési házirendek, és a környezet jogosulatlan hozzáférést szerezhet. A házirend blokkolja, amelyek nem támogatják a feltételes hozzáférésű ügyfelek hozzáférése. 
- **Szolgáltatáskezelési szükséges MFA** – eszközök, beleértve (amennyiben Ön eredeti házirendek konfigurálása) Azure portal eléréséhez többtényezős hitelesítést igényel. 

A Microsoft javasolja, hogy az összes eredeti házirendek lehetővé teszik. Után a házirend engedélyezve van, a rendszergazdák és a felhasználók regisztrálni Azure Multii-tényező hitelesítés kéri.

További információt ezekről az irányelvekről lásd: [Mik az eredeti házirendek](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?


## <a name="set-up-baseline-policies"></a>Eredeti házirendek beállítása

1. [Borzas portal](https://portal.azure.com)lépjen, és keresse meg **Az Active Directory Azure** \> **a feltételes hozzáférésű**.
    
    Az eredeti házirendek jelennek meg az oldalon. <br/> <br/>
    ![A feltételes hozzáférésű eredeti szabályzatok listája lap.](media/baslinepolicies.png)
1. Olvassa el az alábbi konkrét utasításokat minden:

  - [MFA igényelnek a rendszergazdák számára](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [A felhasználók Reequire MFA](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Régebbi hitelesítés letiltása](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Szükséges az MFA-kezelő](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Beállíthatja például a jóváhagyott ügyfélalkalmazások igénylő számos további házirendeket. További információt a [Feltételes hozzáférést biztosító dokumentációjában](https://docs.microsoft.com/azure/active-directory/conditional-access/) talál.
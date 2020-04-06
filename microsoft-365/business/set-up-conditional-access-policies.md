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
description: Megtudhatja, hogy miként állíthat be feltételes hozzáférési szabályzatokat a Microsoft 365-kampányokhoz, hogy jelentős további biztonságot nyújtjon.
ms.openlocfilehash: 26fadecc69486d7931dac069d8f53061592f397f
ms.sourcegitcommit: e525bcf073a61e1350484719a0c3ceb6ff0d8db1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/06/2020
ms.locfileid: "43153766"
---
# <a name="set-up-conditional-access-policies"></a>Feltételes hozzáférési házirendek beállítása

[A feltételes hozzáférési](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) házirendek jelentős további biztonságot adnak. A Microsoft olyan alapszintű feltételes hozzáférési házirendeket biztosít, amelyek minden ügyfél számára ajánlottak. Az alapházirendek olyan előre definiált házirendek, amelyek segítenek megvédeni a szervezeteket számos gyakori támadásellen. Ezek a gyakori támadások közé tartozhat a jelszóspray, a visszajátszás és az adathalászat.

Ezek a házirendek megkövetelik a rendszergazdáktól és a felhasználóktól, hogy bizonyos feltételek teljesülése esetén adjanak meg egy második hitelesítési formát (úgynevezett többtényezős hitelesítést vagy Többtényezős hitelesítést). Ha például egy felhasználó egy másik országból jelentkezik be, a bejelentkezés kockázatosnak minősülhet, és a felhasználónak egy további hitelesítési formát kell megadnia. 

Az alappolitikák jelenleg a következők:
- **A rendszergazdák többtényezős hitelesítésének megkövetelése Többtényezős** &ndash; hitelesítést igényel a legtöbb kiemelt rendszergazdai szerepkörhöz, beleértve a globális rendszergazdai szerepköröket is.
- **Végfelhasználói védelem** &ndash; Többtényezős hitelesítést igényel a felhasználók számára csak akkor, ha a bejelentkezés kockázatos. 
- **A régebbi ügyfélalkalmazások** &ndash; és néhány új alkalmazás blokkolása régebbi, biztonságosabb hitelesítési protokollokat nem használ. Ezek a régebbi alkalmazások megkerülhetik a feltételes hozzáférés házirendjeit, és jogosulatlanul hozzáférhetnek a környezethez. Ez a házirend blokkolja a hozzáférést az ügyfelek, amelyek nem támogatják a feltételes hozzáférés. 
- **Többtényezős hitelesítés megkövetelése a szolgáltatáskezeléshez** &ndash; többtényezős hitelesítést igényel a felügyeleti eszközökhöz való hozzáféréshez, beleértve az Azure Portalt (ahol konfigurálja az alapházirendeket). 

A Microsoft azt javasolja, hogy engedélyezze az összes ilyen alapházirendet. Miután ezek a szabályzatok engedélyezve vannak, a rendszergazdák és a felhasználók kérni fogja, hogy regisztráljon az Azure multii-factor hitelesítés.

Ezekről a házirendekről a [Mik az alapházirendek?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)


## <a name="set-up-baseline-policies"></a>Alaptervházirendek beállítása

1. Nyissa meg az [Azure Portalt,](https://portal.azure.com)és keresse meg az **Azure Active Directory** \> **feltételes hozzáférését.**
    
    Az alapházirendek az oldalon vannak felsorolva. <br/> <br/>
    ![A feltételes hozzáférés alapházirendjeit felsoroló lap.](../media/baslinepolicies.png)
1. Az egyes házirendekhez tartozó alábbi konkrét utasításokat olvassa el:

  - [Többkori faszükségtelével kell elévülve a rendszergazdákszámára](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [Többkori faszükséglés megkövetelése a felhasználók számára](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Örökölt hitelesítés blokkolása](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Többéves kortól megkövetelhető a szolgáltatáskezeléshez](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Számos további szabályzatot állíthat be, például jóváhagyott ügyfélalkalmazásokat. További információt a [Feltételes hozzáférés dokumentációjában talál.](https://docs.microsoft.com/azure/active-directory/conditional-access/)

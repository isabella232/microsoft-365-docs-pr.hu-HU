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
search.appverid:
- BCS160
- MET150
- MOE150
description: Megtudhatja, hogy miként állíthat be feltételes hozzáférési házirendeket a Microsoft 365-ös kampányokhoz.
ms.openlocfilehash: 335fbd7e771b1595e1846529daed76e5ddd3a8f5
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593385"
---
# <a name="set-up-conditional-access-policies"></a>Feltételes hozzáférési házirendek beállítása

[A feltételes hozzáférési](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) házirendek jelentős további biztonságot adnak hozzá. A Microsoft az összes ügyfél számára ajánlott alapkonfigurációs feltételes hozzáférési házirendek egy sorát biztosítja. Az alapházirendek olyan előre definiált házirendek, amelyek segítenek megvédeni a szervezeteket számos gyakori támadással szemben. Ezek a gyakori támadások közé tartozhat a jelszóspray, a visszajátszás és az adathalászat.

Ezek a házirendek megkövetelik a rendszergazdáktól és a felhasználóktól, hogy bizonyos feltételek teljesülése esetén adjanak meg egy második hitelesítési formát (más néven többtényezős hitelesítést vagy MFA-t). Ha például egy felhasználó egy másik országból jelentkezik be, a bejelentkezés kockázatosnak tekinthető, és a felhasználónak egy további hitelesítési formát kell megadnia. 

Jelenleg az alapházirendek a következőket tartalmazzák:
- **A rendszergazdák többtényezős hitelesítésének megkövetelése többtényezős** &ndash; hitelesítést igényel a legtöbb kiemelt rendszergazdai szerepkörhöz, beleértve a globális rendszergazdát is.
- **A végfelhasználói védelem** &ndash; csak akkor igényel többtényezős hitelesítést a felhasználók számára, ha a bejelentkezés kockázatos. 
- **Letiltás a régebbi hitelesítéssel** &ndash; Régebbi ügyfélalkalmazások és néhány új alkalmazás nem használ újabb, biztonságosabb hitelesítési protokollokat. Ezek a régebbi alkalmazások megkerülhetik a feltételes hozzáférési szabályzatokat, és jogosulatlan ultrásként juthatnak el a környezethez. Ez a házirend blokkolja a feltételes hozzáférést nem támogató ügyfelek hozzáférését. 
- A &ndash; **szolgáltatáskezelés többtényezős hitelesítésének megkövetelése** többtényezős hitelesítést igényel a felügyeleti eszközökhöz való hozzáféréshez, beleértve az Azure Portalt is (ahol az alapházirendeket konfigurálja). 

A Microsoft azt javasolja, hogy engedélyezze az összes alapházirendet. Miután ezek a szabályzatok engedélyezve vannak, a rendszergazdák és a felhasználók kérik, hogy regisztráljon az Azure Multii-Factor hitelesítés.

Ezekről a házirendekről további információt [a Mik az alapházirendek?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)


## <a name="set-up-baseline-policies"></a>Alapházirendek beállítása

1. Nyissa meg az [Azure Portalot,](https://portal.azure.com)majd keresse meg az **Azure Active Directory** \> **feltételes hozzáférését.**
    
    Az alapházirendek az oldalon jelennek meg. <br/> <br/>
    ![A feltételes hozzáférés alapházirendjeit tartalmazó lap.](media/baslinepolicies.png)
1. Az egyes házirendekhez tartozó alábbi utasításokat találja:

  - [Többoldalz megkövetelése rendszergazdáknak](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [Többéves fa megkövetelése a felhasználók számára](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Örökölt hitelesítés blokkolása](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Többéves fa megkövetelése a szolgáltatáskezeléshez](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Számos további szabályzatot is beállíthat, például jóváhagyott ügyfélalkalmazásokat igényel. További információt a [Feltételes hozzáférés dokumentációjában](https://docs.microsoft.com/azure/active-directory/conditional-access/)talál.

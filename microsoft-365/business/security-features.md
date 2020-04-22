---
title: A Microsoft 365 Business Premium biztonsági és megfelelőségi funkciói
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-security-compliance
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Ismerje meg a Microsoft 365 Business Premium biztonsági funkcióit, amelyek segítenek megvédeni a pc-ken, telefonokon és táblagépeken lévő adatokat.
ms.openlocfilehash: 35eb0ac1dce216ccc557fc629ddb5d2df50e7134
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/21/2020
ms.locfileid: "43635144"
---
# <a name="microsoft-365-business-premium-security-and-compliance-features"></a>A Microsoft 365 Business Premium biztonsági és megfelelőségi funkciói

A Microsoft 365 Business Premium egyszerűsített biztonsági funkciókat kínál a pc-ken, telefonokon és táblagépeken tárolt adatok védelme érdekében.
    
## <a name="microsoft-365-admin-center-security-features"></a>A Microsoft 365 Felügyeleti központ biztonsági szolgáltatásai

[![A megjelenő címke figyelmeztet a felügyeleti központ változásaira, további részleteket itt talál: aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

A Microsoft 365 Business Premium számos biztonsági szolgáltatását kezelheti a felügyeleti központban, amely egyszerűsített módon be- és kikapcsolhatja ezeket a funkciókat. A felügyeleti központban a következőket teheti:
  
- [Alkalmazáskezelési beállítások megadása Android vagy iOS rendszerű eszközökhöz](app-protection-settings-for-android-and-ios.md) . 
    
    Ezek a beállítások magukban foglalják a fájlok törlését egy inaktív eszközről egy meghatározott időszak után, a munkafájlok titkosítását, a PIN-kód beállításának megkövetelését, és így tovább.
    
- [Alkalmazásvédelmi beállítások megadása Windows 10-es eszközökhöz.](protection-settings-for-windows-10-devices.md) 
    
    Ezek a beállítások mind a vállalat tulajdonában lévő, mind a személyes tulajdonú eszközökvállalati adataira alkalmazhatók.
    
- [A Windows 10-es eszközök eszközvédelmi beállításainak megadása.](protection-settings-for-windows-10-pcs.md) 
    
    Engedélyezheti a [BitLocker](https://go.microsoft.com/fwlink/p/?linkid=871405) titkosítást az adatok védelmére, ha egy eszköz elveszik vagy ellopják, és lehetővé teszi, hogy a [Windows Exploit Guard](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) speciális védelmet nyújtson a zsarolóprogramok ellen. 
    
- [Céges adatok eltávolítása az eszközökről](remove-company-data.md)
    
    Távolról törölheti a vállalati adatokat, ha egy eszköz elveszett, ellopták, vagy egy alkalmazott elhagyja a vállalatot.
    
- [Állítsa vissza a Windows 10-es eszközöket a gyári beállításokra.](reset-devices-to-factory-settings.md) 
    
    Minden olyan Windows 10-es eszközt visszaállíthat, amelyre eszközvédelmi beállítások vonatkoznak.
    
## <a name="additional-security-features"></a>További biztonsági funkciókról 

A Microsoft 365 Business Premium speciális szolgáltatásai segítenek megvédeni vállalkozását a kiberfenyegetésekkel szemben, és védelmezni a bizalmas adatokat.
  
- **[Office 365 komplex veszélyforrások elleni védelem](https://support.office.com/article/e100fe7c-f2a1-4b7d-9e08-622330b83653)**
    
    A komplex veszélyforrások elleni védelem (ADVANCED Threat Protection, ATP) segít megvédeni vállalkozását a kifinomult adathalászatés zsarolóprogramok támadásaitól, amelyek célja az alkalmazottak vagy az ügyfelek adatainak veszélyeztetése. A szolgáltatások a következők:
    
  - Kifinomult mellékletszkennelés és AI-alapú elemzés a veszélyes üzenetek észlelésére és elvetésére.
    
  - Az e-mailben található hivatkozások automatikus ellenőrzése annak felmérése érdekében, hogy azok adathalászati rendszer részét képezik-e. Ez biztonságban tartja a nem biztonságos webhelyek elérését.

- **[Az Intune teljes képességei az Azure Portalon](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Az Azure Portalin az Intune felügyeleti központjának elérésével további biztonsági funkciókat állíthat be, például a MacOS-eszközök, az iPhone és az Android-eszközök felügyeletét, valamint a Windows speciális eszközfelügyeletét, amelyek nem érhetők el a Microsoft 365 felügyeleti központon keresztül.
- **Ugyanaz [a feltételes hozzáférés,](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) mint az Azure AD Premium P1 csomag**


    A feltételes hozzáférés segítségével megvédheti a szervezetet a bejelentkezési kockázattól, a váratlan hálózatról vagy területi beállításból érkező hozzáférési kísérletektől, a kockázatos eszköztípusok hozzáférési kísérleteitől és így tovább. A feltételes hozzáférési házirendek az első hitelesítés befejezése után lépnek érvénybe, és az első hitelesítési esemény jeleit használja annak meghatározására, hogy a megkísérelt hozzáférést jóvá kell-e hagyni, meg kell-e tagadni, vagy több bizonyítékra (például egy második azonosítási űrlapra) van szükség.

    A feltételes hozzáférési szolgáltatások a következők:

    - Hozzáférés felhasználónév, csoport és szerepkör alapján
    - Hozzáférés [alkalmazás alapján](https://docs.microsoft.com/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Hozzáférés a hely alapján;](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration)  csak megbízható IP-tartományokból vagy meghatározott országokból engedélyezhet hozzáférést 
    - Többéves kortól megkövetelhető a hozzáféréshez
    - Örökölt [hitelesítést](https://docs.microsoft.com/azure/active-directory/conditional-access/block-legacy-authentication) használó alkalmazások hoz való hozzáférés letiltása
    - Alkalmazások megkövetelése az [Intune-alkalmazásvédelem](https://docs.microsoft.com/azure/active-directory/conditional-access/app-protection-based-conditional-access) használatához
    - Egyéni hitelesítés, például az MFA külső szolgáltatókkal, például DUO-val.
   
    Egyéb jellemzők:
    - [Önkiszolgáló jelszó-visszaállítás](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-customization) a hibrid Azure AD-hez
    
## <a name="compliance-features"></a>Megfelelőségi funkciók

A Microsoft 365 Business Premium előfizetés olyan funkciókat tartalmaz, amelyek segítenek a megfelelőségi és szabályozási szabványok fenntartásában.

- **[Adatveszteség-megelőzési házirendek](https://support.office.com/article/1966b2a7-d1e2-4d92-ab61-42efbb137f5e)** (DLP) áttekintése. 
    
    Beállíthatja a DLP-t, hogy automatikusan észlelje a bizalmas adatokat, például hitelkártyaszámokat, társadalombiztosítási számokat és így tovább, hogy megakadályozza a vállalaton kívüli véletlen megosztásukat.
    
- **[Exchange Online Archiválás](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Az Exchange Online archiválási licenc lehetővé teszi az üzenetek egyszerű archiválását folyamatos adatmentéssel. A felhasználó összes e-mailjeit tárolja, beleértve a törölt elemeket is, abban az esetben, ha később szükség lenne rájuk a felfedezéshez vagy a helyreállításhoz. Emellett különböző adatmegőrzési szabályzatok segítségével megőrizheti az e-mail adatokat a peres ügyekben, az elektronikus adatfeltáráshoz vagy a megfelelőségi követelmények teljesítéséhez.
    
- **[Érzékenységi címkék](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)**

   A Microsoft 365 Business Premium az [Azure Information Protection Plan 1](https://go.microsoft.com/fwlink/p/?linkid=871407)összes funkcióját tartalmazza. Ezzel a tervvel **olyan érzékenységi címkéket** hozhat létre, amelyek lehetővé teszik a bizalmas adatokhoz való hozzáférést az e-mailekben és dokumentumokban, olyan vezérlőkkel, mint a "Ne továbbítsa" és a "Ne másolja" vezérlőkkel. A bizalmas információkat "Bizalmas"-ként is osztályozhatja, és megadhatja, hogy a minősített információk hogyan oszthatók meg a vállalkozáson kívül és azon belül. A nagyvállalati szintű titkosítás könnyen alkalmazható az e-mailekre és a dokumentumokra, hogy adatait bizalmasan tartsa. Az Azure Information Protection ügyfélbővítményt is telepítheti az Office-alkalmazásokhoz. További információ: [Azure Information Protection unified labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history). Az érzékenységi címkékhez telepítse a **AzInfoProtection_UL.exe**.

Ezeket a funkciókat &amp; a Biztonsági megfelelőségi központban és az Intune felügyeleti központban kezelheti. Idővel az egyszerűsített vezérlők a Microsoft 365 felügyeleti központba kerülnek.
  
    
## <a name="faq"></a>GYIK

 ### <a name="are-these-security-features-available-in-all-markets"></a>Ezek a biztonsági funkciók minden piacon elérhetők?
  
Igen, ezek a funkciók minden olyan piacon elérhetők, ahol a Microsoft 365 Business Premium szolgáltatást értékesítik.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Hogyan találhatom meg &amp; a Biztonsági megfelelőségi központot?
  
1. [Jelentkezzen be a Microsoft 365 Business Premium szolgáltatásba](https://portal.microsoft.com/) rendszergazdai hitelesítő adataival. 
    
2. A bal oldali navigációs sávon keresse meg a **Felügyeleti központokat, és bontsa** ki azt. 
    
    ![A Microsoft 365 Felügyeleti központ bal oldali navigációs sávjában válassza a Felügyeleti központok lehetőséget.](../media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Válassza a **Biztonsági &amp; ** megfelelőség &amp; lehetőséget a Biztonsági megfelelőségi központ megugrásához.

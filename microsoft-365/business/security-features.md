---
title: Mikroszkóp 365 teendő biztonság és engedékenység jellegét meghatározza
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
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Ismerje meg a Microsoft 365 Business biztonsági szolgáltatásait.
ms.openlocfilehash: 98eb0c2015ed6088b2d5e8621c8e72a5b63f2a17
ms.sourcegitcommit: 58a7bd70a4bcf52530baf5f82507fd5dc4455fd9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/03/2019
ms.locfileid: "39668848"
---
# <a name="microsoft-365-business-security-and-compliance-features"></a>Mikroszkóp 365 teendő biztonság és engedékenység jellegét meghatározza

Mikroszkóp 365 teendő felajánl Simplified biztonság jellegét meghatározza-hoz segít oltalmaz-a adat-ra PCs, telefon, és tabletta.
    
## <a name="microsoft-365-business-admin-center-security-features"></a>Microsoft 365 Business Admin Center biztonsági szolgáltatások

[![A megjelenő címke figyelmeztet a felügyeleti központ változásaira, további részleteket itt talál: aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

A Microsoft 365 üzleti biztonsági szolgáltatásainak nagy részét az admin központban kezelheti, így a szolgáltatások be-és kikapcsolhatók. Az admin központban a következőkre van szüksége:
  
- [Készlet alkalmazás vezetés elintézés részére Android vagy iOS berendezés](app-protection-settings-for-android-and-ios.md) . 
    
    Ezek közé tartozik például a fájlok törlése egy inaktív eszközről egy meghatározott időszak után, a munka fájljainak titkosítása, hogy a felhasználók PIN-kódot hozzanak létre stb.
    
- [A Windows 10 eszköz alkalmazásvédelmi beállításainak megadása](protection-settings-for-windows-10-devices.md) . 
    
    Ezek a beállítások vállalati vagy személyes tulajdonú eszközökön is alkalmazhatók vállalati adatokra.
    
- [Állítsa be a Windows 10 eszköz eszközvédelmi beállításait](protection-settings-for-windows-10-pcs.md) . 
    
    A [BitLocker](https://go.microsoft.com/fwlink/p/?linkid=871405) titkosítással engedélyezheti az adatok védelmét az eszköz elvesztése vagy ellopása esetén, és engedélyezheti, hogy a [Windows Exploit Guard](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) speciális védelmet nyújtson a ransomware ellen. 
    
- [Céges adatok eltávolítása az eszközökről](remove-company-data.md)
    
    A vállalati adatok távolról is megtörölhetők, ha az eszköz elvész, ellopják, vagy ha az alkalmazott elhagyja a vállalatot.
    
- [Orrgazdaság Windows 10 berendezés-hoz-uk gyár elintézés](reset-devices-to-factory-settings.md) . 
    
    Minden olyan Windows 10 eszközt alaphelyzetbe lehet állítani, amelyekhez az eszközvédelmi beállítások vonatkoznak.
    
## <a name="additional-security-features"></a>További biztonsági funkciókról 

A Microsoft 365 Business továbbfejlesztett szolgáltatásai segítenek megvédeni vállalkozástól az internetes fenyegetésektől és a bizalmas információk védelmérig.
  
- **[Az Office 365 fejlett fenyegetettség elleni védelem](https://support.office.com/article/e100fe7c-f2a1-4b7d-9e08-622330b83653)**
    
    Haladó fenyeget védelem (ATP) segít őr-a teendő ellen kifinomult phishing és ransomware támadás szándékos-hoz kiegyezés alkalmazott vagy ügyfél információ. Jellegét meghatározza tartalmaz:
    
  - Kifinomult egybefűzés fürkésző és AI-energiát termelő analízis-hoz kinyomoz és eldob veszélyes üzenet.
    
  - Önműködő ellenőriz-ból láncszemek-ban elektronikus levél-hoz felbecsáll ha ők ' része egy phishing terv. Ez emléktárgy Ön biztos-ból bejutó nem biztonságos websites.

- **[A Intune teljes képességei az Azure portálon](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Az Intune admin központ eléréséhez az Azure portálon további biztonsági szolgáltatásokat állíthat be, például a MacOS eszközök, iPhone és Android eszközök kezelését, valamint a Windows speciális eszközkezelőit, amelyek nem érhetők el a Microsoft 365 üzleti admin központ.
- **Ugyanez a [feltételes hozzáférés](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) azúrkék ad P1 terv**


    A feltételes elérés segítségével megvédheti szervezetét a bejelentkezési kockázatból, a váratlan hálózatból vagy területi beállításból származó hozzáférési kísérletektől, a kockázatos eszköztípusok elérésének kísérletétől stb. A feltételes hozzáférési házirendek érvényesítése az első hitelesítés befejezése után történik, és az első hitelesítési esemény jeleit használja annak megállapításához, hogy a megkísérelt hozzáférést jóvá kell-e hagyja, meg kell tagadni, vagy ha több bizonyítékot (például egy második azonosítási formát) szükséges.

    A tartalmazott feltételes hozzáférési funkciók:

    - Hozzáférés felhasználónévvel, csoporttal és szerepkörre alapozva
    - Hozzáférés [egy alkalmazás alapján](https://docs.microsoft.com/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Hozzáférés a hely alapján](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration);  csak megbízható IP-tartományoktól vagy adott országokból engedélyeznek hozzáférést 
    - Hozzáférés megkövetelése az MFA-hoz
    - Az [örökölt hitelesítést](https://docs.microsoft.com/azure/active-directory/conditional-access/block-legacy-authentication) használó alkalmazásokhoz való hozzáférés blokkolása
    - Alkalmazások használata a TP [Intune app védelem](https://docs.microsoft.com/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Egyéni hitelesítés, mint például a MFA, külső szolgáltatók, például a DUO.
   
    Egyéb jellemzők:
    - [Önkiszolgáló jelszóvisszaállító](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-customization) a hibrid Azure ad szolgáltatásra
    
## <a name="compliance-features"></a>Megfelelőségi jellemzők

A Microsoft 365 üzleti előfizetés olyan szolgáltatásokat tartalmaz, amelyek segítenek fenntartani a megfelelést és a szabályozási szabványokat.

- **[Az adatvesztés-megelőzési politikák áttekintése](https://support.office.com/article/1966b2a7-d1e2-4d92-ab61-42efbb137f5e)** (DLP). 
    
    Beállíthatja, hogy a DLP automatikusan észlelje a bizalmas adatokat, például a hitelkártyaszámokat, a társadalombiztosítási számokat, és így tovább, hogy megakadályozza a vállalaton kívülre történő véletlen megosztását.
    
- **[Exchange Online Archiválás](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Az Exchange Online archiválási licenc lehetővé teszi az üzenetek egyszerű archiválását folyamatos adatmentéssel. Tárolja az összes felhasználó e-maileket, beleértve a törölt elemek, abban az esetben, ha ők szükség később felfedezés vagy helyreállítás. Emellett különböző adatmegőrzési szabályokat is használhat az e-mail adatok megőrzésére a peres eljárások esetében, az eDiscovery vagy a megfelelőségi követelmények betartása érdekében.
    
- **[Érzékenységi címkék](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)**

   Mikroszkóp 365 teendő beleértve minden a jellegét meghatározza-ból [Azure információ védelem tervez 1](https://go.microsoft.com/fwlink/p/?linkid=871407). Ezzel tervez, tudod teremt **érzékenység felirat** ami lehetővé teszi ön-hoz irányít belépés-hoz érzékeny információ-ban elektronikus levél és okiratok,-val vezérlőberendezés szeret "nem továbbít" és "nem másol" A kényes információkat "bizalmas"-ként is besorolhatja, és meghatározhatja, hogy a minősített információk hogyan oszthatók el a vállalkozországon kívül és belül. Enterprise-Grade titkosítás könnyen alkalmazható az e-mail és dokumentumok tartani az adatokat magán. Telepítheti a Azure informatikai ügyfélbővítményt az Office alkalmazásokhoz is. További információ: [Azure információvédelem egységes címkézési ügyfél](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history). A érzékenységi címkék esetében telepítse az **AzInfoProtection_UL. exe fájlt**.

Ezeket a szolgáltatásokat a biztonsági &amp; megfelelőség központ és az Intune felügyeleti központ segítségével kezelheti. Idővel az egyszerűsített vezérlők bekerülnek a Microsoft 365 Business admin központba.
  
    
## <a name="faq"></a>GYIK

 ### <a name="are-these-security-features-available-in-all-markets"></a>Ezek a biztonsági funkciók minden piacon elérhetők?
  
Igen, ezek a szolgáltatások minden olyan piacon elérhetők, ahol a Microsoft 365 Business-ot értékesítik.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Hogyan találom meg a biztonsági &amp; megfelelés központját?
  
1. [Jelentkezzen be a Microsoft 365 Business](https://portal.microsoft.com/) segítségével rendszergazdai hitelesítő adataival. 
    
2. -Ban bal NAV, elhelyez **Admin középpontok** és kiterjed ez. 
    
    ![-Ban bal NAV-ban Mikroszkóp 365 admin központ, választ admin középpontok.](media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. A biztonsági megfelelőség központ elemre történő ugrás &amp; esetén válassza a ** &amp; biztonság megfelelőséget** .

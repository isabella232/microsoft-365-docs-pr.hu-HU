---
title: A Microsoft 365 Vállalati prémium verzió biztonsági és megfelelőségi funkciói
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Ismerje meg a Microsoft 365 Vállalati prémium verzió biztonsági funkcióit, amelyek segítenek a PC-n, telefonon és táblagépen található adatok védelmében.
ms.openlocfilehash: f04a998c74128edac306167617e073c412fce2ea
ms.sourcegitcommit: dcb97fbfdae52960ae62b6faa707a05358193ed5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51198411"
---
# <a name="microsoft-365-business-premium-security-and-compliance-features"></a>A Microsoft 365 Vállalati prémium verzió biztonsági és megfelelőségi funkciói

A Microsoft 365 Vállalati prémium verzió egyszerűsített biztonsági funkciókat kínál, hogy védjük az adatait PC-n, telefonon és táblagépen.
    
## <a name="microsoft-365-admin-center-security-features"></a>A Microsoft 365 Felügyeleti központ biztonsági funkciói

A Felügyeleti központban kezelheti a Microsoft 365 Vállalati prémium verzió számos biztonsági funkcióját, így egyszerűbben kapcsolhatja be és ki ezeket a szolgáltatásokat. A Felügyeleti központban az alábbi lehetőségek közül választhat:
  
- [Alkalmazáskezelési beállítások megadása Android- vagy iOS-eszközökhöz.](app-protection-settings-for-android-and-ios.md) 
    
    Ezek közé a beállítások közé tartozik a fájlok inaktív eszközről való törlése adott időszak után, a munkahelyi fájlok titkosítása, a PIN-kód beállításának előírása stb.
    
- [Alkalmazásvédelmi beállítások megadása Windows 10-es eszközökhöz.](protection-settings-for-windows-10-devices.md) 
    
    Ezeket a beállításokat céges vagy személyes tulajdonú eszközökön egyaránt alkalmazni lehet.
    
- [Eszközvédelmi beállítások megadása Windows 10-es eszközökhöz.](protection-settings-for-windows-10-pcs.md) 
    
    A [BitLocker-titkosítás engedélyezésével](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions) megvédheti az adatokat abban az esetben, ha ellopják vagy ellopják az eszközt, és lehetővé teheti, hogy a [Windows biztonsági](/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) résőr speciális védelmet nyújtson a zsarolóvírusok ellen. 
    
- [Céges adatok eltávolítása az eszközökről](remove-company-data.md)
    
    Távolról is törölhet céges adatokat, ha egy eszköz elveszett, ellopták, vagy ha egy alkalmazott elhagyja a vállalatot.
    
- [Állítsa vissza a Windows 10-es eszközöket a gyári beállításaikra.](reset-devices-to-factory-settings.md) 
    
    Minden olyan Windows 10-es eszközt alaphelyzetbe állíthat, amelyekre eszközvédelmi beállítások vannak alkalmazva.
    
## <a name="additional-security-features"></a>További biztonsági funkciókról 

A Microsoft 365 Vállalati prémium verzió speciális funkciói segítenek megvédeni vállalkozását a kibertámadásokkal szemben, és megóvni a bizalmas információkat.
  
- **[Microsoft Defender az Office 365-hez](../security/office-365-security/defender-for-office-365.md)**
    
    Az Office 365-höz készült Microsoft Defender védelmet nyújt vállalkozása számára a kifinomult adathalászati és zsarolóvírus-támadások ellen, amelyek az alkalmazotti és ügyféladatok veszélyeztető kísérletére vannak tervezve. A funkciók közé tartoznak az alábbiak:
    
  - Kifinomult mellékletvizsgálat és AI-alapú elemzés a veszélyes üzenetek észleléséhez és elvetéhez.
    
  - Az e-mailekben található hivatkozások automatikus ellenőrzése annak felmérése érdekében, hogy azok részei-e az adathalászati sémának. Ez megakadályozza, hogy hozzáférjen a nem biztonságos webhelyekhez.

- **[Az Intune teljes funkciói az Azure Portalon](/mem/intune/fundamentals/what-is-intune)**
    
    Ha az Intune felügyeleti központot használja az Azure Portalon, további biztonsági funkciókat állíthat be, például a MacOS-eszközök, az iPhone és az Android-eszközök kezelését, valamint a Microsoft 365 Felügyeleti központon keresztül nem elérhető speciális windowsos eszközkezelést.
- **Az [](/azure/active-directory/conditional-access/overview) Azure AD Premium P1 csomag feltételes hozzáférésének megegyezik**


    A feltételes hozzáféréssel megvédheti szervezetét a bejelentkezési kockázatoktól, a váratlan hálózatoktól vagy területi beállításoktól származó hozzáférési kísérletektől, a veszélyes eszköztípusoktól származó hozzáférési kísérletektől stb. A feltételes hozzáférési házirendek az első hitelesítés befejezése után érvényesülnek, és az első hitelesítési esemény szignálja alapján határozzák meg, hogy a hozzáférést jóvá kell-e hagyni, megtagadni vagy további bizonyítékra van szükség (például egy másik azonosításra).

    A feltételes hozzáférés a következő funkciókat tartalmazza:

    - Access felhasználónév, csoport és szerepkör alapján
    - Access [alkalmazás alapján](/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Hozzáférés hely alapján;](/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration)  csak megbízható IP-tartományokból vagy adott országokból engedélyezi a hozzáférést 
    - Több hitelesítés szükséges a hozzáféréshez
    - A régi típusú hitelesítést használt appok [elérésének blokkolása](/azure/active-directory/conditional-access/block-legacy-authentication)
    - Az Intune appvédelmi szolgáltatás [használatának megkövetelheti az appokat](/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Egyéni hitelesítés, például több hitelesítés külső szolgáltatókkal, például DUO.
   
    Egyéb funkciók:
    - [Önkiszolgáló jelszó-visszaállítás](/azure/active-directory/authentication/concept-sspr-customization) hibrid Azure AD-hez
    
## <a name="compliance-features"></a>Megfelelőségi funkciók

Microsoft 365 Vállalati prémium verziós előfizetése olyan szolgáltatásokat tartalmaz, amelyek segítenek a megfelelőségi és szabályozási szabványok fenntartásában.

- **[Adatveszteség-megelőzési házirendek](../compliance/data-loss-prevention-policies.md)** (DLP) – áttekintés. 
    
    A DLP beállításával automatikusan észlelheti a bizalmas adatokat, például a hitelkártyaszámokat, a társadalombiztosítási számokat stb. annak érdekében, hogy megakadályozza a vállalaton kívüli véletlen megosztást.
    
- **[Exchange Online Archiválás](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Az Exchange Online archiválási licence lehetővé teszi az üzenetek egyszerű archiválását folyamatos adatmentés használatával. A felhasználó összes e-mailjeit tárolja, beleértve a törölt elemeket is, arra az esetre, ha később szükség lenne rájuk a feltárás vagy a visszaállítás érdekében. Emellett különböző adatmegőrzési házirendek használatával megőrizheti az e-mail-adatokat jogi visszatartások, elektronikus adatfeladatokat vagy megfelelőségi követelmények teljesítéséhez.
    
- **[Érzékenységi címkék](../compliance/sensitivity-labels.md)**

   A Microsoft 365 Business Premium az [Azure Information Protection 1. csomag összes funkcióját tartalmazza.](https://go.microsoft.com/fwlink/p/?linkid=871407) Ezzel a csomaggal  bizalmas címkéket hozhat létre, amelyek lehetővé teszik az e-mailekben és dokumentumokban található bizalmas információkhoz való hozzáférést a "Nincs továbbítás" és a "Nincs másolás" vezérlőkkel. A bizalmas adatokat "Bizalmas" kategóriába is sorolhatja, és megadhatja, hogy a bizalmas információkat hogyan lehet megosztani a vállalaton belül és kívül. A nagyvállalati szintű titkosítás egyszerűen alkalmazható az e-mailekre és a dokumentumokra, hogy adatai privátak maradnak. Az Office-appok Azure Information Protection ügyfélprogram bővítményét is telepítheti. További információ: [Az Azure Information Protection egyesített címkézési ügyfélalkalmazása.](/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history) Bizalmasság-címkékhez telepítse a **AzInfoProtection_UL.exe.**

Ezeket a funkciókat a Biztonsági megfelelőségi központban és az &amp; Intune Felügyeleti központban kezelheti. Idővel az egyszerűsített vezérlők bekerülnek a Microsoft 365 Felügyeleti központba.
  
    
## <a name="faq"></a>GYIK

 ### <a name="are-these-security-features-available-in-all-markets"></a>Minden piacon elérhetők ezek a biztonsági funkciók?
  
Igen, ezek a funkciók minden olyan piacon elérhetők, ahol a Microsoft 365 Business Premiumt értékesítik.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Hogyan találhatom meg a Biztonsági &amp; megfelelőségi központot?
  
1. [Jelentkezzen be a Microsoft 365 Vállalati prémium verzióba](https://portal.microsoft.com/) a rendszergazdai hitelesítő adataival. 
    
2. A bal oldali navigációs sávon keresse meg a **Felügyeleti központokat,** és bontsa ki. 
    
    ![A Microsoft 365 Felügyeleti központ bal oldali navigációs sávjában válassza a Felügyeleti központok lehetőséget.](../media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Válassza **a Biztonsági megfelelőség &amp; lehetőséget** a Biztonsági megfelelőségi &amp; központba való ugráshoz.

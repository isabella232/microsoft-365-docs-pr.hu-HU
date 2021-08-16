---
title: Microsoft 365 Vállalati prémium verzió biztonsági és megfelelőségi funkciók
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
description: Ismerje meg a számítógéphez, telefonhoz és táblagéphez Microsoft 365 Vállalati prémium verzió biztonsági funkciókat.
ms.openlocfilehash: 50b74ed18d641e8de38db3284c3ef3abf319825f4f7dbe02b6575f6c0fbc6f85
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53887573"
---
# <a name="microsoft-365-business-premium-security-and-compliance-features"></a>Microsoft 365 Vállalati prémium verzió biztonsági és megfelelőségi funkciók

Microsoft 365 Vállalati prémium verzió rendszer egyszerűsített biztonsági funkciókat biztosít, amelyek segítenek a PC-n, telefonon és táblagépen található adatok védelmében.
    
## <a name="microsoft-365-admin-center-security-features"></a>Microsoft 365 Felügyeleti központ biztonsági funkciók

A Felügyeleti központ számos biztonsági Microsoft 365 Vállalati prémium verzió funkcióját kezelheti, így egyszerűbben kapcsolhatja be és ki ezeket a funkciókat. A Felügyeleti központban az alábbi lehetőségek közül választhat:
  
- [Alkalmazáskezelési beállítások megadása Android- vagy iOS-eszközökhöz.](app-protection-settings-for-android-and-ios.md) 
    
    Ezek közé a beállítások közé tartozik a fájlok inaktív eszközről való törlése adott időszak után, a munkahelyi fájlok titkosítása, a PIN-kód beállításának előírása stb.
    
- [Alkalmazásvédelmi beállítások megadása Windows 10 eszközökhöz.](protection-settings-for-windows-10-devices.md) 
    
    Ezeket a beállításokat céges vagy személyes tulajdonú eszközökön egyaránt alkalmazni lehet.
    
- [Eszközvédelmi beállítások megadása Windows 10 eszközökhöz.](protection-settings-for-windows-10-pcs.md) 
    
    A [BitLocker-titkosítás engedélyezésével](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions) megvédheti az adatokat abban az esetben, ha ellopnak vagy ellopnak egy eszközt, és lehetővé teheti, hogy a [Windows Biztonsági](/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) rés kiaknázása elleni védelem a zsarolóvírusok ellen nyújtson speciális védelmet. 
    
- [Céges adatok eltávolítása az eszközökről](remove-company-data.md)
    
    Távolról is törölhet céges adatokat, ha egy eszköz elveszett, ellopták, vagy ha egy alkalmazott elhagyja a vállalatot.
    
- [Állítsa Windows 10 eszköz gyári beállításait.](reset-devices-to-factory-settings.md) 
    
    Az összes olyan Windows 10 alaphelyzetbe állíthatja, amelyekre eszközvédelmi beállítások vannak alkalmazva.
    
## <a name="additional-security-features"></a>További biztonsági funkciókról 

A számítógépes Microsoft 365 Vállalati prémium verzió speciális funkciói segítenek megvédeni vállalkozását a kibertámadásokkal szemben, és megóvni a bizalmas információkat.
  
- **[Microsoft Defender Office 365](../security/office-365-security/defender-for-office-365.md)**
    
    A Microsoft Defender Office 365 védelmet nyújt vállalkozása számára a kifinomult adathalászati és zsarolóvírus-támadások ellen, amelyek az alkalmazotti és ügyféladatok veszélyeztető kísérletére vannak tervezve. A funkciók közé tartoznak az alábbiak:
    
  - Kifinomult mellékletvizsgálat és AI-alapú elemzés a veszélyes üzenetek észleléséhez és elvetéhez.
    
  - Az e-mailekben található hivatkozások automatikus ellenőrzése annak felmérése érdekében, hogy azok részei-e az adathalászati sémának. Ez megakadályozza, hogy hozzáférjen a nem biztonságos webhelyekhez.

- **[Az Intune teljes funkciói az Azure Portalon](/mem/intune/fundamentals/what-is-intune)**
    
    Ha az Intune felügyeleti központot használja az Azure Portalon, további biztonsági funkciókat állíthat be, például a MacOS-eszközök, az iPhone és az Android-eszközök kezelését, valamint az Windows speciális eszközkezelési funkcióit, amelyek nem érhetők el a Microsoft 365 Felügyeleti központ-ban.
- **A [feltételes hozzáférés ugyanaz,](/azure/active-directory/conditional-access/overview) mint Prémium P1 szintű Azure AD terv**


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

Az Microsoft 365 Vállalati prémium verzió előfizetése olyan szolgáltatásokat tartalmaz, amelyek segítenek a megfelelőségi és szabályozási szabványok fenntartásában.

- **[További információ az adatveszteség-megelőzésről](../compliance/dlp-learn-about-dlp.md))** (DLP). 
    
    A DLP beállításával automatikusan észlelheti a bizalmas adatokat, például a hitelkártyaszámokat, a társadalombiztosítási számokat stb. annak érdekében, hogy megakadályozza a vállalaton kívüli véletlen megosztást.
    
- **[Exchange Online Archiválás](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Exchange Online Archiválás lehetővé teszi az üzenetek egyszerű archiválását folyamatos adatmentés használatával. A felhasználó összes e-mailjeit tárolja, beleértve a törölt elemeket is, arra az esetre, ha később szükség lenne rájuk a feltárás vagy a visszaállítás érdekében. Emellett különböző adatmegőrzési házirendek használatával megőrizheti az e-mail-adatokat jogi visszatartások, elektronikus adatfeladatokat vagy megfelelőségi követelmények teljesítéséhez.
    
- **[Érzékenységi címkék](../compliance/sensitivity-labels.md)**

   Microsoft 365 Vállalati prémium verzió Azure [Information Protection 1. csomag összes funkcióját tartalmazza.](https://go.microsoft.com/fwlink/p/?linkid=871407) Ezzel a csomaggal  bizalmas címkéket hozhat létre, amelyek lehetővé teszik az e-mailekben és dokumentumokban található bizalmas információkhoz való hozzáférést a "Nincs továbbítás" és a "Nincs másolás" vezérlőkkel. A bizalmas adatokat "Bizalmas" kategóriába is sorolhatja, és megadhatja, hogy a bizalmas információkat hogyan lehet megosztani a vállalaton belül és kívül. A nagyvállalati szintű titkosítás egyszerűen alkalmazható az e-mailekre és a dokumentumokra, hogy adatai privátak maradnak. Telepítheti az Azure Information Protection client bővítményt Office alkalmazásokhoz. További információ: [Az Azure Information Protection egyesített címkézési ügyfélalkalmazása.](/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history) Bizalmasság-címkékhez telepítse a **AzInfoProtection_UL.exe.**

Ezeket a funkciókat a Biztonsági megfelelőségi központban és az &amp; Intune Felügyeleti központban kezelheti. Idővel az egyszerűsített vezérlők bekerülnek a Microsoft 365 Felügyeleti központ.
  
    
## <a name="faq"></a>GYIK

 ### <a name="are-these-security-features-available-in-all-markets"></a>Minden piacon elérhetők ezek a biztonsági funkciók?
  
Igen, ezek a funkciók minden olyan piacon elérhetők, ahol a Microsoft 365 Vállalati prémium verzió értékesítik.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Hogyan találhatom meg a Biztonsági &amp; megfelelőségi központot?
  
1. [Jelentkezzen be a Microsoft 365 Vállalati prémium verzió](https://portal.microsoft.com/) a rendszergazdai hitelesítő adataival. 
    
2. A bal oldali navigációs sávon keresse meg a **Felügyeleti központokat,** és bontsa ki. 
    
    ![A bal oldali navigációs sávon válassza Microsoft 365 Felügyeleti központ Felügyeleti központok lehetőséget.](../media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Válassza **a Biztonsági megfelelőség &amp; lehetőséget** a Biztonsági megfelelőségi &amp; központba való ugráshoz.

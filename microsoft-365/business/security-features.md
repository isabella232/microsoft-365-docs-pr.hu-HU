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
ms.openlocfilehash: b7fdd3d7fa25c23ee49ae82aa037588d8fba61a1
ms.sourcegitcommit: 83a40facd66e14343ad3ab72591cab9c41ce6ac0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49840389"
---
# <a name="microsoft-365-business-premium-security-and-compliance-features"></a>A Microsoft 365 Vállalati prémium verzió biztonsági és megfelelőségi funkciói

A Microsoft 365 Vállalati prémium verzió egyszerűsített biztonsági funkciókat kínál, amelyek segítenek a PC-n, telefonon és táblagépen található adatok védelmében.
    
## <a name="microsoft-365-admin-center-security-features"></a>A Microsoft 365 Felügyeleti központ biztonsági funkciói

A Felügyeleti központban kezelheti a Microsoft 365 Vállalati prémium verzió számos biztonsági funkcióját, így egyszerűbben kapcsolhatja be és ki ezeket a funkciókat. A Felügyeleti központban az alábbi lehetőségek közül választhat:
  
- [Alkalmazáskezelési beállítások megadása Android- vagy iOS-eszközökön.](app-protection-settings-for-android-and-ios.md) 
    
    Ezek közé a beállítások közé tartozik például, hogy adott időszak után töröljön fájlokat egy inaktív eszközről, titkosítsa a munkahelyi fájlokat, megkövetelje a felhasználóknak a PIN-kód beállítását stb.
    
- [Alkalmazásvédelmi beállítások megadása Windows 10-es eszközökhöz.](protection-settings-for-windows-10-devices.md) 
    
    Ezek a beállítások a céges vagy a személyes tulajdonú eszközökön egyaránt alkalmazhatók a céges adatokra.
    
- [Eszközvédelmi beállítások megadása Windows 10-es eszközökhöz.](protection-settings-for-windows-10-pcs.md) 
    
    A [BitLocker-titkosítás engedélyezésével](https://go.microsoft.com/fwlink/p/?linkid=871405) megvédheti az adatokat az eszközök ellopása vagy ellopása esetén, és lehetővé teheti, hogy a [Windows Biztonsági](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) résőr speciális védelmet nyújtson a zsarolóvírusok ellen. 
    
- [Céges adatok eltávolítása az eszközökről](remove-company-data.md)
    
    Távolról is törölhet céges adatokat, ha egy eszköz elveszett, ellopták, vagy ha egy alkalmazott elhagyja a vállalatát.
    
- [Állítsa vissza a Windows 10-es eszközöket gyári beállításaikra.](reset-devices-to-factory-settings.md) 
    
    Alaphelyzetbe állíthatja azokat a Windows 10-es eszközöket, amelyekre eszközvédelmi beállítások vannak alkalmazva.
    
## <a name="additional-security-features"></a>További biztonsági funkciókról 

A Microsoft 365 Vállalati prémium verzió speciális funkciói segítenek megvédeni vállalkozását a kibertámadásokkal szemben, és megóvni a bizalmas információkat.
  
- **[Microsoft Defender az Office 365-hez](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)**
    
    Az Office 365-höz készült Microsoft Defender védelmet nyújt vállalkozása számára a kifinomult adathalászati és zsarolóvírus-támadások ellen, amelyek célja az alkalmazotti vagy ügyféladatok veszélyeztető támadása. A funkciók közé tartoznak az alábbiak:
    
  - Kifinomult mellékletvizsgálat és AI-alapú elemzés a veszélyes üzenetek észleléséhez és elvetéséhez.
    
  - Az e-mailekben található hivatkozások automatikus ellenőrzése annak felmérésére, hogy azok adathalászati sémának részei-e. Ez megakadályozza, hogy hozzáférjen a nem biztonságos webhelyekhez.

- **[Az Intune teljes képességei az Azure Portalon](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Ha az Intune Felügyeleti központot használja az Azure Portalon, további biztonsági funkciókat állíthat be, például a MacOS-eszközök, az iPhone és az Android-eszközök kezelését, valamint a Speciális eszközkezelést a Windowshoz, amelyek nem érhetők el a Microsoft 365 Felügyeleti központban.
- **Ugyanaz [a feltételes hozzáférés,](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) mint az Azure AD Premium P1 csomag**


    A feltételes hozzáféréssel megvédheti szervezetét a bejelentkezési kockázatoktól, a nem várt hálózati vagy területi beállításoktól származó hozzáférési kísérletektől, a kockázatos eszköztípusoktól származó hozzáférési kísérletektől stb. A feltételes hozzáférési házirendek az első hitelesítés befejezése után lesznek kényszerítve, és az első hitelesítési esemény szignálja alapján határozzák meg, hogy a megkísérelt hozzáférést jóvá kell-e hagyni, megtagadni kell-e, vagy további igazolásra van-e szükség (például egy másik azonosításra).

    A feltételes hozzáférés a következő funkciókat tartalmazza:

    - Access felhasználónév, csoport és szerepkör alapján
    - Access [alkalmazás alapján](https://docs.microsoft.com/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Hozzáférés hely alapján;](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration)  csak megbízható IP-tartományokból vagy adott országokból való hozzáférés engedélyezése 
    - Több hitelesítés szükséges a hozzáféréshez
    - A régi hitelesítést felhasználó alkalmazások [elérésének blokkolása](https://docs.microsoft.com/azure/active-directory/conditional-access/block-legacy-authentication)
    - Az Intune appvédelmi szolgáltatás [használatának megkövetele az alkalmazások számára](https://docs.microsoft.com/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Egyéni hitelesítés, például több hitelesítés külső szolgáltatókkal( például DUO).
   
    Egyéb funkciók:
    - [Önkiszolgáló jelszó-visszaállítás](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-customization) a hibrid Azure AD-hez
    
## <a name="compliance-features"></a>Megfelelőségi funkciók

Microsoft 365 Vállalati prémium verziós előfizetése olyan funkciókat tartalmaz, amelyek segítenek a megfelelőségi és szabályozási szabványok fenntartásában.

- **[Az adatveszteség-megelőzési házirendek](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies)** (DLP) áttekintése. 
    
    Beállíthatja, hogy a DLP automatikusan észlelje a bizalmas adatokat, például a hitelkártyaszámokat, a társadalombiztosítási számokat stb. annak érdekében, hogy megakadályozza a vállalaton kívüli véletlen megosztást.
    
- **[Exchange Online Archiválás](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Az Exchange Online archiválási licence lehetővé teszi az üzenetek egyszerű archiválását folyamatos adatmentés használatával. Tárolja a felhasználó összes e-mail-üzenetét, beleértve a törölt elemeket is, arra az esetre, ha később szüksége lenne rájuk a feltárás vagy a visszaállítás érdekében. Emellett különböző adatmegőrzési házirendek használatával megőrizheti az e-mail-adatokat jogi visszatartások, elektronikus adatfeladatokat vagy megfelelőségi követelmények teljesítéséhez.
    
- **[Érzékenységi címkék](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)**

   A Microsoft 365 Vállalati prémium verzió az [Azure Information Protection 1. csomag összes funkcióját tartalmazza.](https://go.microsoft.com/fwlink/p/?linkid=871407) Ezzel a csomaggal  bizalmas címkéket hozhat létre, amelyek lehetővé teszik a bizalmas információkhoz való hozzáférést az e-mailekben és a dokumentumokban, a "Nem továbbítható" és a "Nincs másolás" vezérlőkkel. A bizalmas adatokat "Bizalmasként" is osztályozhatja, és megadhatja, hogy a bizalmas információkat miként lehet megosztani a vállalaton belül és kívül. A nagyvállalati szintű titkosítás egyszerűen alkalmazható az e-mailekre és a dokumentumokra, hogy adatai privátak maradnak. Az Office-appok Azure Information Protection-ügyfél bővítményét is telepítheti. További információt az [Azure Information Protection egyesített címkézési ügyfélalkalmazásában található.](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history) Bizalmasság-címkékhez telepítse a **AzInfoProtection_UL.exe.**

Ezeket a funkciókat a Biztonsági megfelelőségi központban és az &amp; Intune Felügyeleti központban kezelheti. Idővel az egyszerűsített vezérlők felkerülnek a Microsoft 365 Felügyeleti központba.
  
    
## <a name="faq"></a>GYIK

 ### <a name="are-these-security-features-available-in-all-markets"></a>Minden piacon elérhetők ezek a biztonsági funkciók?
  
Igen, ezek a funkciók minden olyan piacon elérhetők, ahol a Microsoft 365 Vállalati prémium verzió vásárolható meg.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Hogyan találhatom meg a Biztonsági &amp; megfelelőségi központot?
  
1. Jelentkezzen be a [Microsoft 365 Vállalati prémium](https://portal.microsoft.com/) verzióba a rendszergazdai hitelesítő adataival. 
    
2. A bal oldali navigációs sávon keresse meg a **Felügyeleti központokat,** és bontsa ki. 
    
    ![A Microsoft 365 Felügyeleti központ bal oldali navigációs sávjában válassza a Felügyeleti központok lehetőséget.](../media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Válassza **a Biztonsági megfelelőség &amp; lehetőséget** a Biztonsági megfelelőségi &amp; központba való ugráshoz.

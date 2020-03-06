---
title: A Microsoft 365 vállalati biztonsági és megfelelőségi szolgáltatásai
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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Ismerje meg a Microsoft 365 Business biztonsági szolgáltatásait, amelyek segítenek megvédeni az adatokat pc-ken, telefonokon és táblagépeken.
ms.openlocfilehash: eb92131cc937875615342b2b0d39c78d51a8a99f
ms.sourcegitcommit: 26e4d5091583765257b7533b5156daa373cd19fe
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/06/2020
ms.locfileid: "42550037"
---
# <a name="microsoft-365-business-security-and-compliance-features"></a>A Microsoft 365 vállalati biztonsági és megfelelőségi szolgáltatásai

A Microsoft 365 Business egyszerűsített biztonsági funkciókat kínál a pc-ken, telefonokon és táblagépeken tárolt adatok védelme érdekében.
    
## <a name="microsoft-365-business-admin-center-security-features"></a>A Microsoft 365 Vállalati verzió felügyeleti központ biztonsági szolgáltatásai

[![A megjelenő címke figyelmeztet a felügyeleti központ változásaira, további részleteket itt talál: aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

A Microsoft 365 Vállalati verzió számos biztonsági szolgáltatását kezelheti a felügyeleti központban, így egyszerűsített módon kapcsolhatja be vagy ki ezeket a szolgáltatásokat. A felügyeleti központban a következőket teheti:
  
- [Android vagy iOS-eszközök alkalmazáskezelési beállításainak megadása.](app-protection-settings-for-android-and-ios.md) 
    
    Ezek a beállítások magukban foglalják a fájlok törlését egy inaktív eszközről egy meghatározott időszak után, a munkahelyi fájlok titkosítása, a felhasználók PIN-kódjának beállítása és így tovább.
    
- [Állítsa be a Windows 10-es eszközök alkalmazásvédelmi beállításait.](protection-settings-for-windows-10-devices.md) 
    
    Ezek a beállítások a vállalati vagy a személyes tulajdonú eszközök vállalati adataira is alkalmazhatók.
    
- [Állítsa be a Windows 10-es eszközök eszközvédelmi beállításait.](protection-settings-for-windows-10-pcs.md) 
    
    Engedélyezheti a [BitLocker](https://go.microsoft.com/fwlink/p/?linkid=871405) titkosítást az adatok védelméhez abban az esetben, ha egy eszköz elveszne vagy ellopna, és lehetővé teheti a [Windows Exploit Guard](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) számára, hogy speciális védelmet nyújtson a zsarolóprogramok ellen. 
    
- [Céges adatok eltávolítása az eszközökről](remove-company-data.md)
    
    Távolról törölheti a vállalati adatokat, ha egy eszköz elveszett, ellopták, vagy egy alkalmazott elhagyja a vállalatot.
    
- Állítsa vissza a [Windows 10-es eszközöket a gyári beállításokra](reset-devices-to-factory-settings.md) . 
    
    Visszaállíthatja azokat a Windows 10-es eszközöket, amelyekre eszközvédelmi beállítások vonatkoznak.
    
## <a name="additional-security-features"></a>További biztonsági funkciókról 

A Microsoft 365 Business speciális funkciói segítenek megvédeni vállalkozását a kiberfenyegetésekkel szemben, és megvédheti a bizalmas információkat.
  
- **[Az Office 365 speciális veszélyforrások elleni védelme](https://support.office.com/article/e100fe7c-f2a1-4b7d-9e08-622330b83653)**
    
    Az Advanced Threat Protection (ATP) segít megvédeni vállalkozását a kifinomult adathalász és zsarolóprogramok támadásaitól, amelyek célja az alkalmazottak vagy az ügyfelek adatainak veszélyeztetése. A funkciók a következők:
    
  - Kifinomult mellékletszkennelés és AI-alapú elemzés a veszélyes üzenetek észleléséhez és elvetéséhez.
    
  - Az e-mailben lévő hivatkozások automatikus ellenőrzése annak megállapítására, hogy adathalász rendszer részei-e. Ez megakadályozza, hogy biztonságban hozzáférjen a nem biztonságos webhelyekhez.

- **[Az Intune teljes körű funkciói az Azure Portalon](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Az Intune Felügyeleti központ azure-portálon való elérése lehetővé teszi további biztonsági funkciók, például a MacOS-eszközök, az iPhone és az Android rendszerű eszközök felügyeletét, valamint a Windows speciális eszközfelügyeletét, amelyek nem érhetők el a Microsofton keresztül 365 Üzleti felügyeleti központ.
- **Ugyanaz a [feltételes hozzáférés,](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) mint az Azure AD P1-csomag**


    A feltételes hozzáférés segít megvédeni a szervezetet a bejelentkezési kockázattól, a váratlan hálózatvagy területi beállításhozzáférési kísérletek, a kockázatos eszköztípusok hozzáférési kísérletei től, és így tovább. A feltételes hozzáférési házirendek az első hitelesítés befejezése után lépnek érvénybe, és az első hitelesítési esemény jeleit használja annak meghatározására, hogy a megkísérelt hozzáférést jóvá kell-e hagyni, meg kell-e tagadni, vagy ha több bizonyíték (például az azonosítás második formája) szükséges.

    A feltételes hozzáférési funkciók a következők:

    - Hozzáférés felhasználónév, csoport és szerepkör alapján
    - Hozzáférés [alkalmazás alapján](https://docs.microsoft.com/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Hozzáférés a hely alapján](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration);  csak megbízható IP-tartományokból vagy adott országokból engedélyezhet hozzáférést 
    - Többéves fa megkövetelése a hozzáféréshez
    - Az [örökölt hitelesítést](https://docs.microsoft.com/azure/active-directory/conditional-access/block-legacy-authentication) használó alkalmazásokhoz való hozzáférés letiltása
    - Alkalmazások megkövetelése tp használata [Intune-alkalmazásvédelem](https://docs.microsoft.com/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Egyéni hitelesítés, például mfa külső szolgáltatókkal, például DUO.
   
    Egyéb funkciók:
    - [Önkiszolgáló jelszó-visszaállítás](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-customization) a hibrid Azure AD-hez
    
## <a name="compliance-features"></a>Megfelelőségi funkciók

A Microsoft 365 Business-előfizetés olyan funkciókat tartalmaz, amelyek segítenek a megfelelőségi és szabályozási szabványok fenntartásában.

- **[Adatveszteség-megelőzési szabályzatok](https://support.office.com/article/1966b2a7-d1e2-4d92-ab61-42efbb137f5e)** (DLP) áttekintése. 
    
    Beállíthatja a DLP-t, hogy automatikusan észlelje a bizalmas adatokat, például a hitelkártyaszámokat, a társadalombiztosítási számokat és így tovább, hogy megakadályozza a vállalaton kívüli véletlen megosztásukat.
    
- **[Exchange Online Archiválás](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Az Exchange Online archiválási licenc lehetővé teszi az üzenetek egyszerű archiválását folyamatos adatmentéssel. Tárolja a felhasználó összes e-mailjeit, beleértve a törölt elemeket is, arra az esetre, ha később szükség lenne rájuk a felderítéshez vagy a helyreállításhoz. Emellett különböző adatmegőrzési házirendek segítségével őrizheti meg az e-mail adatokat peres ügyekben, elektronikus adatfeltárás, vagy a megfelelőségi követelmények teljesítéséhez.
    
- **[Érzékenységi címkék](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)**

   A Microsoft 365 Business tartalmazza az Azure Information Protection Plan 1 összes [funkcióját.](https://go.microsoft.com/fwlink/p/?linkid=871407) Ezzel a csomaggal **olyan érzékenységi címkéket** hozhat létre, amelyek lehetővé teszik az e-mailekben és dokumentumokban található bizalmas információkhoz való hozzáférés szabályozását, olyan vezérlőkkel, mint a "Ne továbbítson" és a "Ne másolja" vezérlőket. A bizalmas információkat "Bizalmas" kategóriába is sorolhatja, és megadhatja, hogy a minősített adatok hogyan oszthatók meg a vállalkozáson kívül és azon belül. A nagyvállalati szintű titkosítás könnyen alkalmazható az e-mailekre és dokumentumokra, hogy adatait bizalmasan őrizze. Telepítheti az Azure Information Protection ügyfél bővítményt az Office-alkalmazásokhoz is. További információt az [Azure Information Protection egyesített címkézési ügyfele](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history)című témakörben talál. Érzékenységi címkék esetén telepítse a **AzInfoProtection_UL.exe**.

Ezeket a szolgáltatásokat a &amp; Biztonsági megfelelőségi központban és az Intune Felügyeleti központban kezelheti. Idővel az egyszerűsített vezérlők hozzáadódnak a Microsoft 365 Vállalati felügyeleti központhoz.
  
    
## <a name="faq"></a>GYIK

 ### <a name="are-these-security-features-available-in-all-markets"></a>Ezek a biztonsági funkciók minden piacon elérhetők?
  
Igen, ezek a funkciók minden olyan piacon elérhetők, ahol a Microsoft 365 Business-t értékesítik.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Hogyan találhatom meg &amp; a Biztonsági megfelelőségi központot?
  
1. [Jelentkezzen be a Microsoft 365 Business be](https://portal.microsoft.com/) a rendszergazdai hitelesítő adatok használatával. 
    
2. A bal oldali navigációs sávon keresse meg a **Felügyeleti központokat,** és bontsa ki. 
    
    ![A Microsoft 365 Felügyeleti központ bal oldali navigációs sávjában válassza a Felügyeleti központok lehetőséget.](../media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Válassza ** &amp; a Biztonsági** megfelelőség &amp; lehetőséget a Biztonsági megfelelőségi központhoz való ugráshoz.

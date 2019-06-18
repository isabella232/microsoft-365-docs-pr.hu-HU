---
title: Microsoft 365 üzleti biztonsági és megfelelési szolgáltatások
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
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: 'További tudnivalók: Microsoft 365 üzleti biztonsági szolgáltatásairól.'
ms.openlocfilehash: bd61ad3bf1b34635a7b80f1c9ccf63fa98d31915
ms.sourcegitcommit: 274af83139ad7da3aa33366c3323d533d95c7db4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/17/2019
ms.locfileid: "35017522"
---
# <a name="microsoft-365-business-security-and-compliance-features"></a>Microsoft 365 üzleti biztonsági és megfelelési szolgáltatások

Microsoft 365 üzleti kínál egyszerűsített biztonsági szolgáltatásai segítségével a védintézkedések az adatokat a személyi számítógépek, telefonok és tabletta.
    
## <a name="microsoft-365-business-admin-center-security-features"></a>Microsoft Business-365 felügyeleti központ biztonsági szolgáltatások

![Mutató transzparens https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

A felügyeleti központ, amely lehetőséget nyújt a egyszerűsített, ezek a szolgáltatások be- és kikapcsolása a Microsoft 365 üzleti biztonsági szolgáltatások számos kezelheti. A felügyeleti központ a következőket teheti:
  
  
- [Alkalmazás beállítása Android vagy iOS eszközök](app-protection-settings-for-android-and-ios.md) . 
    
    Ezek a beállítások tartalmazzák a fájlok törlése az inaktív eszközök egy bizonyos időtartam után, a munka fájlok titkosítása, igénylő felhasználók állítsa be a PIN-kód, stb.
    
- [Alkalmazás védelmének beállítása Windows 10 eszközök](protection-settings-for-windows-10-devices.md) . 
    
    Ezek a beállítások mind a társaság tulajdonában lévő vállalati adatok, vagy személyesen a tulajdonában lévő eszközök alkalmazhatók.
    
- [Eszköz védelem beállítása Windows 10 eszközök](protection-settings-for-windows-10-pcs.md) . 
    
    Abban az esetben, ha az eszköz elvész vagy ellopják az adatok védelme érdekében a [BitLocker-alapú](https://go.microsoft.com/fwlink/p/?linkid=871405) titkosítás engedélyezéséhez, és ransomware speciális szerte [Windows kihasználására Guard](https://go.microsoft.com/fwlink/p/?linkid=871404) engedélyezése. 
    
- [Céges adatok eltávolítása az eszközökről](remove-company-data.md)
    
    Vállalati adatok távoli törlés, ha az eszköz elvész, ellopják, vagy a munkavállaló kilép a vállalat.
    
- [A gyári beállítások visszaállítása Windows 10 eszközök](reset-devices-to-factory-settings.md) . 
    
    Visszaállíthatja a hozzájuk rendelt eszköz védelmi beállításokkal rendelkező Windows 10 eszközöket.
    
## <a name="additional-security-features"></a>További biztonsági funkciókról 

Microsoft 365 üzleti továbbfejlesztett szolgáltatások segítségével a vállalat számítógépes fenyegetésektől védelme és bizalmas információk védelme érhetők el.
  
- **[Office 365 speciális veszély védelmi](https://support.office.com/article/e100fe7c-f2a1-4b7d-9e08-622330b83653)**
    
    Speciális veszély védelmi (ATP) védelmét segíti az üzleti kifinomult adathalászat és veszélyeztetheti az alkalmazott vagy a vevő adatai ransomware támadások ellen. Szolgáltatások a következők:
    
  - Kifinomult mellékletet ellenőrzési és vizsgálati AI táplált észleli és veszélyes üzenetek.
    
  - Automatikus ellenőrzésének hivatkozások e-mailben, hogy ha egy adathalász rendszer részét képezik. Ez tartja meg a biztonságos, nem biztonságos webhelyek hozzáférjenek.

- **[Intune teljes képességeit a Azure portálon](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Az Azure portálon felügyeleti központ segítségével állítsa be a kiegészítő biztonsági jellemzők, mint a kezelés MacOS eszközök, iPhone és Android-eszköz speciális Eszközkezelés Windows, valamint a Intune elérése, amelyek nem érhetők el Microsoft Üzleti 365 felügyeleti központ.
- **Megegyező [Feltételes hozzáférést](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/overview) AD a P1 Azure terv**

    Feltételes hozzáférésű segít megvédeni a szervezet a bejelentkezési kockázat, hozzáférési kísérletek nem várt hálózati vagy területi, hozzáférések kockázatos eszköztípusok képernyő, és így tovább. Házirendek akkor lépnek érvénybe, miután az első hitelesítés befejeződött, és az első eseménytől hitelesítési jelek segítségével határozza meg, ha a kísérlet hozzáférés jóvá kell hagyni, a feltételes hozzáférésű megtagadja, vagy további bizonyítékot (például a második űrlap azonosító) f szükséges.

    A feltételes hozzáférésű szolgáltatásai a következők:

    - A felhasználónév, a csoport és a szerepkör alapú hozzáférés
    - Hozzáférés [az app alapján](https://docs.microsoft.com/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Hozzáférési hely alapján](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration);  csak a megbízható IP-tartományokat vagy az adott országok hozzáférés engedélyezése 
    - MFA igényelnek hozzáférést
    - [Régi típusú hitelesítést](https://docs.microsoft.com/azure/active-directory/conditional-access/block-legacy-authentication) használó alkalmazások elérésének blokkolása
    - Szükséges apps tp használata [Intune app védelem](https://docs.microsoft.com/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Harmadik fél szolgáltatók, például DUO MFA például egyéni hitelesítést.
   
    Egyéb jellemzők:
    - Hibrid Azure AD [az önkiszolgáló jelszó alaphelyzetbe állítása](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-customization)
    
## <a name="compliance-features"></a>E szolgáltatások

A Microsoft-365 előfizetés tartalmaz üzleti szolgáltatások megmaradjanak a megfelelőségi és szabályozási előírások, amelyek segítenek.

- **[Adatok elvesztésének megelőzésére irányuló politikák áttekintése](https://support.office.com/article/1966b2a7-d1e2-4d92-ab61-42efbb137f5e)** (DLP). 
    
    DLP automatikusan felismeri a bizalmas adatok, például hitelkártyaszámok, társadalombiztosítási számok, stb, hogy megakadályozzák a véletlen állíthatja a vállalaton kívüli megosztása.
    
- **[Exchange Online Archiválás](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Exchange Online archiválás licenc lehetővé teszi a folyamatos biztonsági mentés egyszerűen archiválhatók. Tárolja az összes felhasználó e-mailek, beleértve a törölt elemek, abban az esetben, ha azok később szükség van feltárása és helyreállítása. Ezenkívül használhatja különböző adatmegőrzési per tartás, elektronikus adatok feltárása, az e-mail adatok megőrzése érdekében, vagy a megfelelőségi követelmények teljesítésére.
    
- **[Borzas információk védelméről](https://go.microsoft.com/fwlink/p/?linkid=871406)**
    
    "Információ védelem meghatározásában, hogy az e-mailek és dokumentumok bizalmas információkhoz való hozzáférés vezérlőkkel, mint nem előre", "Lemásolni tilos." "Bizalmas" érzékeny információk besorolásához és adja meg, hogyan minősített információ megosztható kívül és belül üzleti is. Vállalati minőségű titkosítási is könnyen alkalmazása az e-mailek és dokumentumok tartani az adatokat. 365 üzleti Microsoft [Azure információ védelmi terv 1](https://go.microsoft.com/fwlink/p/?linkid=871407)összes szolgáltatását tartalmazza. Az Azure információvédelem ügyfél beépülő modul Office alkalmazásokhoz is telepíthet. További részletekért [Azure információvédelem ügyfél rendszergazdai útmutatójában](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide)talál.

Ezek a biztonsági szolgáltatások segítségével kezelheti &amp; Megfelelési központba és az Intune admin center. Idővel a Microsoft 365 üzleti felügyeleti központ bekerül az egyszerűsített szabályozza.
  
    
## <a name="faq"></a>GYIK

 ### <a name="are-these-security-features-available-in-all-markets"></a>Érhetők el ezek a szolgáltatások valamennyi piacon?
  
Igen, ezek a szolgáltatások érhetők el minden területen, ahol Microsoft 365 üzleti értékesítik.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Hogyan találja meg a biztonsági &amp; Megfelelési központba?
  
1. [Jelentkezzen be a Microsoft 365 Business](https://portal.microsoft.com/) a rendszergazdai hitelesítő adatok használatával. 
    
2. Keresse meg az **Admin-centers** és bontsa ki a bal oldali navigációs sáv. 
    
    ![Válassza ki a bal oldali navigációs sáv a Microsoft 365 felügyeleti központban, Admin-centers.](media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Válassza a **biztonsági &amp; való** go to biztonsági &amp; Megfelelési központba.
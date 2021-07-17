---
title: Az Microsoft Defender víruskereső által észlelt Microsoft Defender víruskereső
f1.keywords: CSH
ms.author: sharik
author: SKjerland
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- Adm_O365
- Adm_TOC
ms.custom: AdminSurgePortfolio
search.appverid: MET150
description: Megtudhatja Microsoft Defender víruskereső hogyan védi Windows eszközét a szoftver veszélyforrásoktól, például vírusoktól, kártevőktől és kémprogramoktól.
ms.openlocfilehash: 7c5d000e2a8c30e17d1f890cef69fe88beed75bb
ms.sourcegitcommit: dcb97fbfdae52960ae62b6faa707a05358193ed5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/25/2021
ms.locfileid: "53465418"
---
# <a name="threats-detected-by-microsoft-defender-antivirus"></a>Az Microsoft Defender víruskereső által észlelt Microsoft Defender víruskereső

Microsoft Defender víruskereső megvédi Windows eszközeit a szoftver veszélyforrásoktól, például vírusoktól, kártevőktől és kémprogramoktól.

- A vírusok általában úgy terjednek, hogy az eszközén vagy a hálózatán lévő más fájlokhoz csatolják a kódjukat, és a fertőzött programok helytelenül működnek.
- A kártevők kártékony fájlokat, alkalmazásokat és kódokat tartalmaznak, amelyek kárt okozhatnak, és megzavarhatják az eszközök normál használatát. Emellett a kártevők jogosulatlan hozzáférést engedélyeznek, rendszer-erőforrásokat használhatnak, jelszavakat és fiókadatokat ellopnak, bezárhatják a számítógépéről, zsarolóvírust kérhetnek stb.
- A kémprogramok adatokat gyűjtenek, például webböngésző tevékenységet, és elküldik az adatokat a távoli kiszolgálókra.
 
A veszélyforrások elleni védelem érdekében Microsoft Defender víruskereső módszerek közül. Ezek közé a módszerek közé tartozik a felhőalapú védelem, a valós idejű védelem és a dedikált védelmi frissítések.

- A felhőalapú védelem segít az új és felmerülő veszélyforrások azonnali észlelésében és letiltásában.
- Az folyamatos vizsgálat fájl- és folyamatviselkedés-figyelést és más technikákat (más néven valós idejű *védelmet) használ.*
- A dedikált védelmi frissítések gépi tanuláson, emberi és automatizált big-data-elemzésen, valamint a veszélyforrások elleni részletes ellenállási kutatáson alapulnak. 

A kártevőkről és a kártevőkről Microsoft Defender víruskereső az alábbi cikkekben olvashat: 

- [A kártevők & veszélyforrások ismertetése](/windows/security/threat-protection/intelligence/understanding-malware)
- [Hogyan azonosítja a Microsoft a kártevőket és a potenciálisan nemkívánatos alkalmazásokat?](/windows/security/threat-protection/intelligence/criteria)
- [A következő generációs védelem a Windows 10](/windows/security/threat-protection/microsoft-defender-antivirus/microsoft-defender-antivirus-in-windows-10)

## <a name="what-happens-when-a-non-microsoft-antivirus-solution-is-used"></a>Mi történik nem Microsoft által használt víruskereső megoldás használata esetén? 

Microsoft Defender víruskereső operációs rendszer része, és engedélyezett az olyan eszközökön, amelyeken fut Windows 10. Ha azonban nem Microsoft víruskereső megoldást használ, és nem a [Microsoft Defendert](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-advanced-threat-protection)használja végpontként, akkor az Microsoft Defender víruskereső automatikusan letiltott üzemmódba lép.  

Ha letiltott módban van, a felhasználók és az ügyfelek továbbra is Microsoft Defender víruskereső az ütemezett vagy igény szerinti kereséseket a veszélyforrások azonosítására; A Microsoft Defender víruskereső azonban:

- használható alapértelmezett víruskereső alkalmazásként.
- aktívan vizsgálja meg a fájlokat a veszélyforrások után.
- remediate, or resolve, threats.

Ha eltávolítja a nem Microsoft által telepített víruskereső Microsoft Defender víruskereső, a rendszer automatikusan aktív üzemmódba vált, hogy megvédje Windows eszközöket a veszélyforrásoktól.

> [!TIP]
> - Ha használja a Microsoft 365, fontolja meg a Microsoft Defender víruskereső használata elsődleges víruskereső megoldásként. Az integráció nagyobb védelmet nyújthat. Együtt [még jobb: Microsoft Defender víruskereső és Office 365.](/windows/security/threat-protection/microsoft-defender-antivirus/office-365-microsoft-defender-antivirus)
> - Ügyeljen arra, hogy a Microsoft Defender víruskereső akkor is naprakész legyen, ha nem Microsoft víruskereső megoldást használ.

## <a name="what-to-expect-when-threats-are-detected"></a>Mi történik a veszélyforrások észlelésekor?

Ha a veszélyforrások észlelését Microsoft Defender víruskereső, a következő történik:

- A felhasználók [értesítést kapnak a Windows.](https://support.microsoft.com/windows/8942c744-6198-fe56-4639-34320cf9444e) 
- Az észlelések listája a Windows biztonság [a](/windows/security/threat-protection/windows-defender-security-center/windows-defender-security-center) Védelmi előzmények lapon található **alkalmazással.**  
- Ha már biztosította [Windows 10-eszközeit,](secure-win-10-pcs.md) és regisztrálta őket az [Intune-ban,](/mem/intune/enrollment/windows-enrollment-methods)és szervezete 800 vagy kevesebb eszközt regisztrált be, a  veszélyforrások észlelését és összefüggéseit a <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">Microsoft 365 Felügyeleti központ</a> veszélyforrások  és víruskeresők lapján láthatja, amelyeket a **kezdőlap Microsoft Defender víruskereső-kártyáján** (vagy a navigációs panelen az Állapot veszélyforrások & víruskereső lehetőséget választva) férhet   >  hozzá.

    Ha szervezetében több mint 800 eszköz regisztrálva van az Intune-ban, a rendszer a [Microsoft Endpoint Manager](/mem/endpoint-manager-overview) veszélyforrások észlelését és összefüggéseit fogja megtekinteni a Veszélyforrások és víruskereső lap **helyett.**
 
    > [!NOTE]
    > A **Microsoft Defender víruskereső** és **a** veszélyforrások és víruskeresők lap fázisokként van elérhető, így előfordulhat, hogy nem lesz azonnal hozzáférése hozzájuk.

A legtöbb esetben a felhasználóknak nincs semmilyen további teendőjuk. Amint kártékony fájlt vagy programot észlel az eszközön, az Microsoft Defender víruskereső letiltja, és megakadályozza a futtatását. Emellett az újonnan észlelt veszélyforrások bekerülnek a víruskereső és a kártevőirtó motorba, így más eszközök és felhasználók is védettek.  

Ha egy felhasználónak el kell fogadnia egy műveletet, például jóvá kell hagyatni egy kártékony fájl eltávolítását, azt a kapott értesítésben látni fogja. A felhasználó nevében Microsoft Defender víruskereső műveletekről, illetve a felhasználóknak esetleg szükséges műveletekről a Védelmi előzmények [csoportban olvashat bővebben.](https://support.microsoft.com/office/f1e5fd95-09b4-46d1-b8c7-1059a1e09708) Ha meg szeretne tudni arról, hogy miként kezelheti a veszélyforrások észlelését it-rendszergazdaként, olvassa el az Észlelt veszélyforrások áttekintése és [a teendők áttekintése című témakört.](review-threats-take-action.md)

A különböző veszélyforrásokról a <a href="https://www.microsoft.com/wdsi/threats" target="_blank"></a>Microsoft biztonsági intelligencia webhelyét felkeresve, ahol elvégezheti az alábbi műveleteket: 

- Megtekintheti a legfontosabb veszélyforrásokra vonatkozó aktuális információkat.
- Az adott régiót fenyegető legújabb veszélyforrások megtekintése.
- Egy adott veszélyforrás részleteiért keresse az encyclopedia veszélyforrást.

## <a name="related-content"></a>Kapcsolódó tartalom

[Eszközök Windows 10](secure-windows-10-devices.md) (cikk)\
[A Microsoft Defender víruskereső](/windows/security/threat-protection/microsoft-defender-antivirus/evaluate-microsoft-defender-antivirus) (cikk)\
A valós idejű és a felhőalapú víruskeresők elleni védelem [bekapcsolásának mikéntjéhez](/mem/intune/user-help/turn-on-defender-windows#turn-on-real-time-and-cloud-delivered-protection) (cikk)\
[Hogyan kapcsolhatja be és használhatja Microsoft Defender víruskereső a Windows biztonság alkalmazásból](/windows/security/threat-protection/microsoft-defender-antivirus/microsoft-defender-security-center-antivirus) (cikk)\
[Hogyan kapcsolhatja be a Microsoft Defender víruskereső csoportházirend használatával](/mem/intune/user-help/turn-on-defender-windows#turn-on-windows-defender) (cikk)\
[A víruskereső definíciójának frissítése](/mem/intune/user-help/turn-on-defender-windows#update-your-antivirus-definitions) (cikk)\
Kártevők és nem kártevők elküldése a [Microsoftnak elemzésre](/microsoft-365/security/office-365-security/submitting-malware-and-non-malware-to-microsoft-for-analysis) (cikk)

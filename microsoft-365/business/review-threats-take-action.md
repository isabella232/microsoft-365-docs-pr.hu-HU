---
title: Észlelt veszélyforrások áttekintése és a teendők
f1.keywords: NOCSH
ms.author: sharik
author: SKjerland
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- Adm_O365
- Adm_TOC
ms.custom: AdminSurgePortfolio
search.appverid: MET150
description: Ebből a cikkből megtudhatja, hogy miként kezelheti a felhasználók által Microsoft Defender víruskereső az Windows 10 eszközein.
ms.openlocfilehash: 15e99fb75e4a3ac1af842ca7d0b900e02cbc6bd4
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "53465414"
---
# <a name="review-detected-threats-and-take-action"></a>Észlelt veszélyforrások áttekintése és a teendők

A kártékony fájlok vagy szoftverek észlelését Microsoft Defender víruskereső letiltja, és meggátolja a futtatását. Ha pedig be van kapcsolva a felhőalapú védelem, az újonnan észlelt veszélyforrások bekerülnek a víruskereső és a kártevőirtó motorba, így más eszközök és felhasználók is védettek.

Microsoft Defender víruskereső a következő típusú veszélyforrások észlelésére és azokkal szembeni védelemre:

- Vírusokkal, kártevőkvel és webes fenyegetésekkel kapcsolatos eszközök
- Adathalászati kísérletek
- Adatlopási kísérletek

Rendszergazdaként megtekintheti a veszélyforrások észlelésére vonatkozó információkat [](/mem/intune/enrollment/device-enrollment) az Windows 10 Intune-ban regisztrált összes Microsoft 365 Felügyeleti központ. Összegző információkat fog látni, például:

- How many devices need antivirus protection
- Hány eszköz nem felel meg a biztonsági házirendnek?
- Jelenleg hány veszélyforrások vannak aktívak, csökkenthetők vagy oldódnak meg

A veszélyforrások észlelésére és az eszközökre vonatkozó információk megtekintéséhez több lehetőség közül választhat:

- Az **Aktív eszközök** lap a <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">Microsoft 365 Felügyeleti központ.</a> Lásd a jelen cikk A [veszélyforrások észlelésének kezelése](#manage-threat-detections-on-the-active-devices-page) az Aktív eszközök lapon.
- Az **Aktív veszélyforrások** lap a <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">Microsoft 365 Felügyeleti központ.</a> Lásd a jelen cikk A [veszélyforrások](#manage-threat-detections-on-the-active-threats-page) észlelésének kezelése az Aktív veszélyforrások lapon.
- A **víruskereső** lap a <a href="https://go.microsoft.com/fwlink/p/?linkid=2150463" target="_blank">Microsoft Endpoint Manager.</a> Lásd: [Veszélyforrások észlelésének kezelése Microsoft Endpoint Manager](#manage-threat-detections-in-microsoft-endpoint-manager) cikkben.

További információt a Következő által [észlelt veszélyforrások Microsoft Defender víruskereső.](threats-detected-defender-av.md)

## <a name="manage-threat-detections-on-the-active-devices-page"></a>Veszélyforrások észlelésének kezelése az **Aktív eszközök lapon**

Az alábbi eljárás azokra az ügyfelekre vonatkozik, akik Microsoft 365 Vállalati prémium verzió.

1. A bejelentkezéshez Microsoft 365 Felügyeleti központ <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> a bejelentkezéshez.

2. A navigációs lapon válassza az **Eszközök** aktív  >  **eszközök lehetőséget.** Megjelenik az aktív eszközök listája és részletei, például a védelmi állapot, a víruskereső (AV) védelmi állapota és az észlelt aktív veszélyforrások száma.

3. Jelöljön ki egy eszközt, ha további részleteket is meg tud tekinteni az eszközről, és tekintse meg az elérhető műveleteket. Megnyílik egy javaslatokkal és a rendelkezésre álló műveletekkel, például **Frissítési** **házirend,** Víruskereső **frissítése,** Gyors vizsgálat futtatása, **Teljes** vizsgálat futtatása stb.

## <a name="manage-threat-detections-on-the-active-threats-page"></a>Veszélyforrások észlelésének kezelése az **Aktív veszélyforrások lapon**

Az alábbi eljárás azokra az ügyfelekre vonatkozik, akik Microsoft 365 Vállalati prémium verzió. [Windows 10 az eszközöket biztonságosnak kell lennie,](./secure-win-10-pcs.md) és regisztrálni [kell őket az Intune-ban.](/mem/intune/enrollment/windows-enrollment-methods)

> [!NOTE]
> A **Microsoft Defender víruskereső** és az **Aktív** veszélyforrások lapot fázisokként juk ki, így előfordulhat, hogy Nem lesz azonnal hozzáférése hozzájuk.

1. A bejelentkezéshez Microsoft 365 Felügyeleti központ <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> a bejelentkezéshez.

2. A **Microsoft Defender víruskereső** válassza az **Aktív veszélyforrások megtekintése lehetőséget.** (Másik lehetőségként a navigációs ablakban válassza az Állapot **lehetőséget**  >  **Víruskereső & veszélyforrások.)**

3. Az Aktív **veszélyforrások lapon** jelöljön ki egy észlelt fenyegetést további információért. Megnyílik egy úszó panel, amelyen részleteket talál a fenyegetésről, beleértve az érintett eszközöket is.

4. Az úszó panelen válasszon ki egy eszközt az elérhető műveletek megtekintéséhez, például **Frissítési házirend** **,** Víruskereső frissítése, **Gyors** vizsgálat futtatása stb.

## <a name="actions-you-can-take"></a>Műveletek

Amikor részleteket lát adott veszélyforrásokról vagy eszközökről, javaslatokat és egy vagy több, Ön által esetleg elérhető műveletet fog látni. Az alábbi táblázat a lehetséges műveleteket ismerteti.<br><br>

| Művelet | Leírás |
|--|--|
| Védelem beállítása | Be kell állítani a veszélyforrás-védelmi házirendeket. A hivatkozásra kattintva a házirend konfigurációjának lapjára mehetsz.<br><br>Segítségre van szüksége? Lásd: [Eszközbiztonság kezelése végpontbiztonsági házirendekkel a Microsoft Intune.](/mem/intune/protect/endpoint-security-policy) |
| Frissítési házirend | Frissíteni vagy konfigurálni kell a víruskeresőt és a valós idejű védelmi házirendeket. A hivatkozást választva a házirend konfigurációjának lapjára mehetsz.<br><br>Segítségre van szüksége? Lásd: [Eszközbiztonság kezelése végpontbiztonsági házirendekkel a Microsoft Intune.](/mem/intune/protect/endpoint-security-policy) |
| Gyors vizsgálat futtatása | Gyors víruskereső vizsgálatot kezd az eszközön, és a leggyakoribb helyekre összpontosít, ahol a kártevők regisztrálva lehetnek, például a beállításkulcsok és az Windows mappák. |
| Teljes vizsgálat futtatása | Teljes víruskereső vizsgálatot kezd az eszközön, és a leggyakoribb helyekre összpontosít, ahol a kártevők regisztrálva lehetnek, beleértve az eszközön található összes fájlt és mappát is. A találatokat a [Microsoft Endpoint Manager.](/mem/intune/fundamentals/tutorial-walkthrough-endpoint-manager) |
| Víruskereső frissítése | Az eszköznek biztonsági [intelligencia-frissítéseket](https://go.microsoft.com/fwlink/?linkid=2149926) kell kapnia a víruskereső és a kártevővédelem használatához. |
| Eszköz újraindítása | Egy Windows 10 újraindítását kényszeríti öt percen belül.<br><br>**FONTOS:** Az eszköz tulajdonosa vagy a felhasználó nem kap automatikusan értesítést az újraindításról, és elveszítheti a nem mentett munkát. |

## <a name="manage-threat-detections-in-microsoft-endpoint-manager"></a>Veszélyforrások észlelésének kezelése a Microsoft Endpoint Manager

A veszélyforrások Microsoft Endpoint Manager a kezeléséhez. Windows 10 [intune-ban](/mem/intune/enrollment/windows-enrollment-methods) (a szolgáltatás része) kell regisztrálnia az Microsoft Endpoint Manager.

1. Jelentkezzen be Microsoft Endpoint Manager Felügyeleti <a href="https://go.microsoft.com/fwlink/p/?linkid=2150463" target="_blank">https://endpoint.microsoft.com</a> központba.

2. A navigációs ablakban válassza a Végpont **biztonsága lehetőséget.**

3. A **Kezelés alatt válassza** a Víruskereső **lehetőséget.** Számos fület fog látni , például az Összegzés **,** **Windows 10 a** nem jónak talált végpontokat és Windows 10 **kártevőket.**

4. Tekintse át az információkat a rendelkezésre álló lapokon, és a szükséges lépéseket.

Tegyük fel például, hogy az eszközök a Windows 10 **kártevőt észleltek lapon.** Amikor kijelöl egy eszközt, rendelkezésére állnak bizonyos műveletek, például **Újraindítás,** Gyors **vizsgálat,** **Teljes** **vizsgálat,** Szinkronizálás vagy **Aláírások frissítése.** Válasszon egy műveletet az eszközhöz.

Az alábbi táblázatban azokat a műveleteket láthatja, amelyek a Microsoft Endpoint Manager.<br><br>

| Művelet | Leírás |
|--|--|
| Újraindítás | Egy Windows 10 újraindítását kényszeríti öt percen belül.<br><br>**FONTOS:** Az eszköz tulajdonosa vagy a felhasználó nem kap automatikusan értesítést az újraindításról, és elveszítheti a nem mentett munkát. |
| Gyors vizsgálat | Gyors víruskereső vizsgálatot kezd az eszközön, és a leggyakoribb helyekre összpontosít, ahol a kártevők regisztrálva lehetnek, például a beállításkulcsok és az Windows mappák. A találatokat a [Microsoft Endpoint Manager.](/mem/intune/fundamentals/tutorial-walkthrough-endpoint-manager) |
| Teljes vizsgálat | Teljes víruskereső vizsgálatot kezd az eszközön, és a leggyakoribb helyekre összpontosít, ahol a kártevők regisztrálva lehetnek, beleértve az eszközön található összes fájlt és mappát is. A találatokat a [Microsoft Endpoint Manager.](/mem/intune/fundamentals/tutorial-walkthrough-endpoint-manager) |
| Szinkronizálás | Az Intune-nal való bejelentkezéshez eszköz szükséges (a bejelentkezés Microsoft Endpoint Manager). Amikor az eszköz adatokat ad be, az eszköz megkapja az eszközhöz rendelt függőben lévő műveleteket vagy házirendeket. |
| Aláírások frissítése | Az eszköznek biztonsági [intelligencia-frissítéseket](https://go.microsoft.com/fwlink/?linkid=2149926) kell kapnia a víruskereső és a kártevővédelem használatához. |

> [!TIP]
> További információ: Eszközök [távoli műveleteke.](/mem/intune/protect/endpoint-security-manage-devices#remote-actions-for-devices)

## <a name="how-to-submit-a-file-for-malware-analysis"></a>Fájl elküldése kártevőelemzéshez

Ha olyan fájlja van, amelyről úgy gondolja, hogy elmulasztott vagy hibásan lett kártevőként osztályozva, elküldheti a fájlt a Microsoftnak kártevőelemzésre. A felhasználók és a rendszergazdák elküldhetik a fájlokat elemzésre. Keresse fel [https://www.microsoft.com/wdsi/filesubmission](https://www.microsoft.com/wdsi/filesubmission) a webhelyet.
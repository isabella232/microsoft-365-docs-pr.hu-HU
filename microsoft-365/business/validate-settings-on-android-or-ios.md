---
title: Alkalmazásvédelmi beállítások érvényesítése Android vagy iOS eszközökön
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: f3433b6b-02f7-447f-9d62-306bf03638b0
description: Learn how to validate the Microsoft 365 Business app protection settings in your Android or iOS devices.
ms.openlocfilehash: 19a7ce48e8df5c80964a250b0bc087591a0530c1
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "37287875"
---
# <a name="validate-app-protection-settings-on-android-or-ios-devices"></a>Alkalmazásvédelmi beállítások érvényesítése Android vagy iOS eszközökön

Követ a oktatás-ban tabs-hoz érvényesít app védelem elintézés-ra Android vagy iOS berendezés.
  
## <a name="androidtab"></a>[Android](#tab/)
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a>Az appkezelési beállítások működésének ellenőrzése a felhasználói eszközökön

Miután [konfigurálta az Android-eszközök beállításait](app-protection-settings-for-android-and-ios.md) az appok védelmére, az alábbi lépésekkel ellenőrizheti, hogy működnek-e a kiválasztott beállítások. 
  
Elsőként győződjön meg arról, hogy a házirend arra az appra vonatkozik, amelyben az ellenőrzését végezni készül.
  
1. A Microsoft 365 Business [felügyeleti központjában](https://portal.office.com) válassza a **Házirendek** \> **Házirend szerkesztése** lehetőséget.
    
2. Válassza az **Alkalmazás-házirend Android-eszközökhöz** lehetőséget a telepítéskor létrehozott beállításokhoz, illetve egy másik Ön által létrehozott házirendet, és ellenőrizze, hogy az kényszerítve van-e, például az Outlookhoz. 
    
    ![Shows all the apps for which this policy protects files.](media/b3be3ddd-f683-4073-8d7a-9c639a636a2c.png)
  
### <a name="validate-require-a-pin-or-a-fingerprint-to-access-office-apps"></a>A „PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez" beállítás ellenőrzése

A **Házirend szerkesztése** ablaktáblában válassza a **Szerkesztés** elemet az **Office-dokumentumok elérésének szabályozása** elem mellett, bontsa ki az **Office-fájlok felhasználói mobileszközökön történő elérésének felügyelete** csomópontot, és győződjön meg arról, hogy a **PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez** beállítás értéke **Be**.
  
![Make sure that the Require a PIN or fingerprint to acces Office apps is set to On.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. A felhasználó Android-eszközén nyissa meg az Outlookot, és jelentkezzen be a felhasználó Microsoft 365 Businesshez használt hitelesítő adataival.
    
2. A rendszer PIN-kód megadására vagy ujjlenyomat használatára is kérni fogja.
    
    ![Enter a PIN on your Android device to access Office apps.](media/9e8ecfee-8122-4a3a-8918-eece80344310.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a>A „PIN-kód alaphelyzetbe állítása ennyi sikertelen kísérlet után" beállítás ellenőrzése

A **Házirend szerkesztése** ablaktáblában válassza a **Szerkesztés** elemet az **Office-dokumentumok elérésének szabályozása** elem mellett, bontsa ki az **Office-fájlok felhasználói mobileszközökön történő elérésének felügyelete** csomópontot, és győződjön meg arról, hogy a **PIN-kód alaphelyzetbe állítása ennyi sikertelen kísérlet után** beállítás értéke egy szám - alapértelmezés szerint 5. 
  
1. A felhasználó Android-eszközén nyissa meg az Outlookot, és jelentkezzen be a felhasználó Microsoft 365 Businesshez használt hitelesítő adataival.
    
2. Írjon be egy helytelen PIN-kódot a házirendben megadott alkalommal. Megjelenik egy üzenet a **Több PIN-kódot már nem adhat meg** szöveggel, amelyen alaphelyzetbe állíthatja a PIN-kódot. 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fca6fcb4-bb5c-477f-af5e-5dc937e8b835.png)
  
3. Válassza a **PIN-kód visszaállítása** elemet. Ekkor a rendszer arra kéri, hogy jelentkezzen be a felhasználó Microsoft 365 Businesshez használt hitelesítő adataival, majd állítson be egy új PIN-kódot.
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a>„A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió" beállítás ellenőrzése

A **Házirend szerkesztése** ablaktáblában válassza a **Szerkesztés** elemet az **Elveszett vagy ellopott eszközök elleni védelem** elem mellett, bontsa ki a **Munkahelyi fájlok védelme az eszköz elvesztése vagy ellopása esetén** csomópontot, és győződjön meg arról, hogy **A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió** beállítás értéke **Be**.
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. A felhasználó Android-eszközén nyissa meg az Outlookot, jelentkezzen be a felhasználó Microsoft 365 Businesshez használt hitelesítő adataival, és szükség esetén adja meg a PIN-kódot.
    
2. Nyisson meg egy mellékletet tartalmazó e-mailt, és koppintson a lefelé mutató nyíl ikonra a melléklet adatai mellett.
    
    ![Tap the down arrow next to an attachment to try to save it.](media/b22573bb-91ce-455f-84fa-8feb2846b117.png)
  
    A képernyő alján megjelenik **A fájl nem menthető az eszközre** felirat. 
    
    ![Warning text that indicates cannot save a file locally to an Android.](media/52ca3f3d-7ed0-4a52-9621-4872da6ea9c5.png)
  
    > [!NOTE]
    > A OneDrive Vállalati verzióba való mentés jelenleg nem engedélyezett az Android rendszerben, így csak annyi látható, hogy a helyi mentés le van tiltva. 
  
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a>„A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után" beállítás ellenőrzése

A **Házirend szerkesztése** ablaktáblában válassza a **Szerkesztés** elemet az **Office-dokumentumok elérésének szabályozása** elem mellett, bontsa ki az **Office-fájlok felhasználói mobileszközökön történő elérésének felügyelete** csomópontot, és győződjön meg arról, hogy **A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után** beállítás értéke egy szám - alapértelmezés szerint 30 perc. 
  
1. A felhasználó Android-eszközén nyissa meg az Outlookot, jelentkezzen be a felhasználó Microsoft 365 Businesshez használt hitelesítő adataival, és szükség esetén adja meg a PIN-kódot.
    
2. Ekkor megjelenik az Outlook Beérkezett üzenetek mappája. Hagyja az Android-eszközt üresjáratban legalább 30 percig (vagy más időtartamig, az a lényeg, hogy hosszabb legyen a házirendben meghatározottnál). Az eszköz valószínűleg elsötétül.
    
3. Nyissa meg újra az Outlookot az Android-eszközön.
    
4. A rendszer arra fogja kérni, hogy adja meg a PIN-kódot az Outlook ismételt eléréséhez.
    
### <a name="validate-protect-work-files-with-encryption"></a>A „Munkahelyi fájlok védelme titkosítással" beállítás ellenőrzése

A **Házirend szerkesztése** ablaktáblában válassza a **Szerkesztés** elemet az **Elveszett vagy ellopott eszközök elleni védelem** elem mellett, bontsa ki a **Munkahelyi fájlok védelme az eszköz elvesztése vagy ellopása esetén** csomópontot, és győződjön meg arról, hogy a **Munkahelyi fájlok védelme titkosítással** beállítás értéke **Be**, **A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió** beállításé pedig **Ki**.
  
1. A felhasználó Android-eszközén nyissa meg az Outlookot, jelentkezzen be a felhasználó Microsoft 365 Businesshez használt hitelesítő adataival, és szükség esetén adja meg a PIN-kódot.
    
2. Nyisson meg egy olyan e-mailt, amely tartalmaz néhány képfájlt mellékletként.
    
3. Koppintson a lefelé mutató nyílra a melléklet adatai mellett a mentéséhez.
    
    ![Tap the down arrow to save the figure file to the Android device.](media/08a9e21e-4022-45d5-acff-59cface651e7.png)
  
4. Ekkor a rendszer arra kérheti, hogy engedélyezze a hozzáférést az Outlooknak a fényképekhez, médiatartalmakhoz és más fájlokhoz. Koppintson az **Engedélyezés** gombra.
    
5. A képernyő alján válassza a **Mentés helye: Eszköz** lehetőséget, majd nyissa meg a **Galéria** appot. 
    
6. A listában látható lehet egy (vagy - ha több, képfájlt tartalmazó mellékletet mentett - több) titkosított fájl. Egy szürke négyzetként jelenhet meg a Képek listában, amelyben középen egy fehér felkiáltójel látható egy fehér körön belül.
    
    ![An encrypted image file in the Gallery app.](media/25936414-bd7e-421d-824e-6e59b877722d.png)
  
## <a name="iostab"></a>[Ios](#tab/)
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a>Az appkezelési beállítások működésének ellenőrzése a felhasználói eszközökön

Miután [konfigurálta az iOS-eszközök beállításait](app-protection-settings-for-android-and-ios.md) az appok védelmére, az alábbi lépésekkel ellenőrizheti, hogy működnek-e a kiválasztott beállítások. 
  
Elsőként győződjön meg arról, hogy a házirend arra az appra vonatkozik, amelyben az ellenőrzését végezni készül.
  
1. A Microsoft 365 Business [felügyeleti központjában](https://portal.office.com) válassza a **Házirendek** \> **Házirend szerkesztése** lehetőséget.
    
2. Válassza az **Alkalmazás-házirend iOS-eszközökhöz** lehetőséget a telepítéskor létrehozott beállításokhoz, illetve egy másik Ön által létrehozott házirendet, és ellenőrizze, hogy az kényszerítve van-e, például az Outlookhoz. 
    
    ![Shows all the apps for which this policy protects files.](media/842441b8-e7b1-4b86-9edd-d94d1f77b6f4.png)
  
### <a name="validate-require-a-pin-to-access-office-apps"></a>A „PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez" beállítás ellenőrzése

A **Házirend szerkesztése** ablaktáblában válassza a **Szerkesztés** elemet az **Office-dokumentumok elérésének szabályozása** elem mellett, bontsa ki az **Office-fájlok felhasználói mobileszközökön történő elérésének felügyelete** csomópontot, és győződjön meg arról, hogy a **PIN-kód vagy ujjlenyomat megkövetelése az Office-appok eléréséhez** beállítás értéke **Be**.
  
![Make sure that the Require a PIN or fingerprint to acces Office apps is set to On.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. A felhasználó iOS-eszközén nyissa meg az Outlookot, és jelentkezzen be a felhasználó Microsoft 365 Businesshez használt hitelesítő adataival.
    
2. A rendszer PIN-kód megadására vagy ujjlenyomat használatára is kérni fogja.
    
    ![Enter a PIN on your IOS device to access Office apps.](media/06fc5cf3-9f19-4090-b23c-14bb59805b7a.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a>A „PIN-kód alaphelyzetbe állítása ennyi sikertelen kísérlet után" beállítás ellenőrzése

A **Házirend szerkesztése** ablaktáblában válassza a **Szerkesztés** elemet az **Office-dokumentumok elérésének szabályozása** elem mellett, bontsa ki az **Office-fájlok felhasználói mobileszközökön történő elérésének felügyelete** csomópontot, és győződjön meg arról, hogy a **PIN-kód alaphelyzetbe állítása ennyi sikertelen kísérlet után** beállítás értéke egy szám - alapértelmezés szerint 5. 
  
1. A felhasználó iOS-eszközén nyissa meg az Outlookot, és jelentkezzen be a felhasználó Microsoft 365 Businesshez használt hitelesítő adataival.
    
2. Írjon be egy helytelen PIN-kódot a házirendben megadott alkalommal. Megjelenik egy üzenet a **Több PIN-kódot már nem adhat meg** szöveggel, amelyen alaphelyzetbe állíthatja a PIN-kódot. 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fab5c089-a4a5-4e8d-8c95-b8eed1dfa262.png)
  
3. Válassza az **OK** gombot. Ekkor a rendszer arra kéri, hogy jelentkezzen be a felhasználó Microsoft 365 Businesshez használt hitelesítő adataival, majd állítson be egy új PIN-kódot.
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a>„A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió" beállítás ellenőrzése

A **Házirend szerkesztése** ablaktáblában válassza a **Szerkesztés** elemet az **Elveszett vagy ellopott eszközök elleni védelem** elem mellett, bontsa ki a **Munkahelyi fájlok védelme az eszköz elvesztése vagy ellopása esetén** csomópontot, és győződjön meg arról, hogy **A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió** beállítás értéke **Be**.
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. A felhasználó iOS-eszközén nyissa meg az Outlookot, jelentkezzen be a felhasználó Microsoft 365 Businesshez használt hitelesítő adataival, és szükség esetén adja meg a PIN-kódot.
    
2. Nyisson meg egy mellékletet tartalmazó e-mailt, nyissa meg a mellékletet, és válassza a **Mentés** elemet a képernyő alján. 
    
    ![Tap the Save option after you open an attachment to try to save it.](media/b419b070-1530-4f14-86a8-8d89933a2b25.png)
  
3. Elvileg csak a OneDrive Vállalati verzió beállítás látható. Ha nem így van, koppintson a **Fiók hozzáadása** elemre, és válassza a **OneDrive Vállalati verzió** lehetőséget a **Tárhelyfiók hozzáadása** képernyőn. Amikor szükséges, adja meg a végfelhasználó Microsoft 365 Businesshez használt adatait a bejelentkezéshez. 
    
    Koppintson a **Mentés** elemre, és válassza a **OneDrive Vállalati verzió** lehetőséget.
    
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a>„A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után" beállítás ellenőrzése

A **Házirend szerkesztése** ablaktáblában válassza a **Szerkesztés** elemet az **Office-dokumentumok elérésének szabályozása** elem mellett, bontsa ki az **Office-fájlok felhasználói mobileszközökön történő elérésének felügyelete** csomópontot, és győződjön meg arról, hogy **A felhasználónak ismét be kell jelentkeznie az Office-appok ennyi ideig tartó üresjárata után** beállítás értéke egy szám - alapértelmezés szerint 30 perc. 
  
1. A felhasználó iOS-eszközén nyissa meg az Outlookot, jelentkezzen be a felhasználó Microsoft 365 Businesshez használt hitelesítő adataival, és szükség esetén adja meg a PIN-kódot.
    
2. Ekkor megjelenik az Outlook Beérkezett üzenetek mappája. Hagyja az iOS-eszközt érintetlenül legalább 30 percig (vagy más időtartamig, az a lényeg, hogy hosszabb legyen a házirendben meghatározottnál). Az eszköz valószínűleg elsötétül.
    
3. Nyissa meg újra az Outlookot az iOS-eszközön.
    
4. A rendszer arra fogja kérni, hogy adja meg a PIN-kódot az Outlook ismételt eléréséhez.
    
### <a name="validate-protect-work-files-with-encryption"></a>A „Munkahelyi fájlok védelme titkosítással" beállítás ellenőrzése

A **Házirend szerkesztése** ablaktáblában válassza a **Szerkesztés** elemet az **Elveszett vagy ellopott eszközök elleni védelem** elem mellett, bontsa ki a **Munkahelyi fájlok védelme az eszköz elvesztése vagy ellopása esetén** csomópontot, és győződjön meg arról, hogy a **Munkahelyi fájlok védelme titkosítással** beállítás értéke **Be**, **A felhasználók kényszerítése arra, hogy az összes munkahelyi fájljukat ide mentsék: OneDrive Vállalati verzió** beállításé pedig **Ki**.
  
1. A felhasználó iOS-eszközén nyissa meg az Outlookot, jelentkezzen be a felhasználó Microsoft 365 Businesshez használt hitelesítő adataival, és szükség esetén adja meg a PIN-kódot.
    
2. Nyisson meg egy olyan e-mailt, amely tartalmaz néhány képfájlt mellékletként.
    
3. Koppintson a mellékletre, majd alatta a **Mentés** elemre. 
    
4. Nyissa meg a **Fotók** appot a kezdőképernyőről. Ekkor egy (vagy - ha több, képfájlt tartalmazó mellékletet mentett - több) mentett, ám titkosított fényképet kell látnia. 
    
---


---
title: Alkalmazásvédelmi beállítások megadása Windows 10-es eszközökhöz
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
f1_keywords:
- Win10AppPolicy
- O365E_Win10AppPolicy
- BCS365_Win10AppPolicy
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Útmutató az app adatkezelési házirend létrehozása és munka fájlok Windows 10 eszközök védelme.
ms.openlocfilehash: f649454417dceae05255df6b37760af99c0b8d4f
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660374"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="19d87-103">Alkalmazásvédelmi beállítások megadása Windows 10-es eszközökhöz</span><span class="sxs-lookup"><span data-stu-id="19d87-103">Set application protection settings for Windows 10 devices</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="19d87-104">Appkezelési házirend létrehozása Windows 10-es eszközhöz</span><span class="sxs-lookup"><span data-stu-id="19d87-104">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="19d87-105">Ha a felhasználók munkahelyi feladatokra is használják saját Windows 10-es eszközeiket, az azokon tárolt munkahelyi adatok is védhetők.</span><span class="sxs-lookup"><span data-stu-id="19d87-105">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="19d87-106">Ugrás az admin center <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span><span class="sxs-lookup"><span data-stu-id="19d87-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="19d87-107">A bal oldali navigációs sáv, válassza az **eszközök** \> **politika** \> **hozzáadása**.</span><span class="sxs-lookup"><span data-stu-id="19d87-107">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>

3. <span data-ttu-id="19d87-108">A **Házirend felvétele** ablaktáblában adja meg a házirend egyedi nevét.</span><span class="sxs-lookup"><span data-stu-id="19d87-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="19d87-109">A **Házirend típusa** beállításnál válassza az **Alkalmazáskezelés Windows 10-es eszközökhöz** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="19d87-109">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
    
5. <span data-ttu-id="19d87-110">**Eszköz típusa**csoportban válasszon a **személyes** vagy a **Vállalat birtokában**.</span><span class="sxs-lookup"><span data-stu-id="19d87-110">Under **Device type**, choose either **Personal** or **Company Owned**.</span></span>
    
6. <span data-ttu-id="19d87-111">A **Munkahelyi fájlok titkosítása** lehetőség automatikusan be van kapcsolva.</span><span class="sxs-lookup"><span data-stu-id="19d87-111">The **Encrypt work files** is turned on automatically.</span></span> 
    
7. <span data-ttu-id="19d87-112">Ha nem szeretné, hogy a felhasználók a saját számítógépükre mentsék a munkahelyi fájlokat, állítsa **A felhasználók nem másolhatnak céges adatokat saját fájljaikba, a munkahelyi fájlokat pedig csak a OneDrive Vállalati verzióba menthetik** beállítást **Be** értékre.</span><span class="sxs-lookup"><span data-stu-id="19d87-112">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
    
9. <span data-ttu-id="19d87-113">Bontsa ki a **Windowsos eszközökön lévő adatok helyreállítása** beállítást, és ajánlott, hogy azt állítsa **Be** értékre.</span><span class="sxs-lookup"><span data-stu-id="19d87-113">Expand **Recover data on Windows devices** and it is recommended that you turn it **On**.</span></span>
    
    <span data-ttu-id="19d87-p101">Ahhoz, hogy megkereshesse az adat-helyreállítási megbízott tanúsítványának helyét, először létre kell hoznia egyet. Pontos utasításokat [A titkosított fájlrendszer (EFS) adat-helyreállítási megbízottja (DRA) tanúsítványának létrehozása és ellenőrzése](https://go.microsoft.com/fwlink/p/?linkid=853700) című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="19d87-p101">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one. For instructions see, [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](https://go.microsoft.com/fwlink/p/?linkid=853700).</span></span>
    
    <span data-ttu-id="19d87-p102">A munkahelyi fájlok alapértelmezés szerint egy az eszközön tárolt és a felhasználó profiljához társított titkos kulccsal vannak titkosítva. Csak a felhasználó tudja megnyitni és visszafejteni a fájlt. Így tehát, ha valaki elveszít egy eszközt, vagy törölnek egy felhasználót, egy szükséges fájl titkosított állapotban ragadhat. A kizárólag rendszergazda által használható adat-helyreállítási megbízott (DRA) tanúsítvánnyal visszafejthető a fájl.</span><span class="sxs-lookup"><span data-stu-id="19d87-p102">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile. Only the user can open and decrypt the file. However, if a device is lost or a user is removed, a file can be stuck in an encrypted state. The Data Recovery Agent (DRA) certificate can be used by an admin to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="19d87-p103">Bontsa ki a **További hálózati és felhőbeli helyek védelme** beállítást, ha szeretne további tartományokat vagy SharePoint Online-helyeket felvenni a felsorolt appokban lévő fájlok védelmének biztosítása érdekében. Ha bármelyik mezőben egynél több elemet kell megadnia, pontosvesszővel (;) válassza el őket egymástól.</span><span class="sxs-lookup"><span data-stu-id="19d87-p103">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps will be protected. If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span>
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="19d87-p104">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span><span class="sxs-lookup"><span data-stu-id="19d87-p104">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
12. <span data-ttu-id="19d87-126">Végül válassza a **Hozzáadás** lehetőséget a házirend mentéséhez és eszközökhöz való hozzárendeléséhez.</span><span class="sxs-lookup"><span data-stu-id="19d87-126">Finally, choose **Add** to save the policy, and assign it to devices.</span></span> 
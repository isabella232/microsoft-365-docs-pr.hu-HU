---
title: Alkalmazásvédelmi beállítások szerkesztése vagy beállítása Windows 10-es eszközökön
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
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
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Megtudhatja, hogy miként hozhat létre és szerkeszthet alkalmazáskezelési házirendeket, és hogyan védheti meg a munkahelyi fájlokat a felhasználók személyes Windows 10-es eszközein.
ms.openlocfilehash: f85a59649e43c141b62091337b842a490d411833
ms.sourcegitcommit: abf63669daf12993ad3353e4b578f41c8910b20f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/27/2020
ms.locfileid: "47289199"
---
# <a name="set-or-edit-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="7a60a-103">Alkalmazásvédelmi beállítások megadása és szerkesztése Windows 10-es eszközökön</span><span class="sxs-lookup"><span data-stu-id="7a60a-103">Set or edit application protection settings for Windows 10 devices</span></span>

<span data-ttu-id="7a60a-104">Ez a cikk a Microsoft 365 Vállalati prémium verzióra vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="7a60a-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="edit-an-app-management-policy-for-windows-10"></a><span data-ttu-id="7a60a-105">Alkalmazáskezelési házirend szerkesztése Windows 10-ben</span><span class="sxs-lookup"><span data-stu-id="7a60a-105">Edit an app management policy for Windows 10</span></span>

1. <span data-ttu-id="7a60a-106">A felügyeleti központ megnyitásához: <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="7a60a-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>     
2. <span data-ttu-id="7a60a-107">A bal oldali navigációs sávon válassza az **Eszköz-házirendek** \> **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="7a60a-107">On the left nav, choose **Devices** \> **Policies** .</span></span>
1. <span data-ttu-id="7a60a-108">Válasszon ki egy meglévő Windows-alkalmazás-házirendet, majd **szerkessze.**</span><span class="sxs-lookup"><span data-stu-id="7a60a-108">Choose an existing Windows app policy and then **Edit**.</span></span>
1. <span data-ttu-id="7a60a-109">Válassza **a Módosítani** kívánt beállítás melletti Szerkesztés gombot, majd a Mentés **gombot.**</span><span class="sxs-lookup"><span data-stu-id="7a60a-109">Choose **Edit** next to a setting you want to change and then **Save**.</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="7a60a-110">Appkezelési házirend létrehozása Windows 10-es eszközhöz</span><span class="sxs-lookup"><span data-stu-id="7a60a-110">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="7a60a-111">Ha a felhasználók munkahelyi feladatokra is használják saját Windows 10-es eszközeiket, az azokon tárolt munkahelyi adatok is védhetők.</span><span class="sxs-lookup"><span data-stu-id="7a60a-111">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="7a60a-112">A felügyeleti központ megnyitásához: <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="7a60a-112">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
2. <span data-ttu-id="7a60a-113">A bal oldali navigációs sávon válassza az **Eszköz-házirendek** \> **hozzáadása** \> **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="7a60a-113">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
3. <span data-ttu-id="7a60a-114">A **Házirend felvétele** ablaktáblában adja meg a házirend egyedi nevét.</span><span class="sxs-lookup"><span data-stu-id="7a60a-114">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
4. <span data-ttu-id="7a60a-115">A **Házirend típusa** beállításnál válassza az **Alkalmazáskezelés Windows 10-es eszközökhöz** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="7a60a-115">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
5. <span data-ttu-id="7a60a-116">Az **Eszköz típusa alatt válassza** a Személyes **vagy** a **Vállalati tulajdonú lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="7a60a-116">Under **Device type**, choose either **Personal** or **Company Owned**.</span></span>
6. <span data-ttu-id="7a60a-117">A **Munkahelyi fájlok titkosítása** lehetőség automatikusan be van kapcsolva.</span><span class="sxs-lookup"><span data-stu-id="7a60a-117">The **Encrypt work files** is turned on automatically.</span></span> 
7. <span data-ttu-id="7a60a-118">Ha nem szeretné, hogy a felhasználók a saját számítógépükre mentsék a munkahelyi fájlokat, állítsa **A felhasználók nem másolhatnak céges adatokat saját fájljaikba, a munkahelyi fájlokat pedig csak a OneDrive Vállalati verzióba menthetik** beállítást **Be** értékre.</span><span class="sxs-lookup"><span data-stu-id="7a60a-118">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
9. <span data-ttu-id="7a60a-119">**Bontsa ki az Adatok helyreállítása adatokat Windows-eszközökön.**</span><span class="sxs-lookup"><span data-stu-id="7a60a-119">Expand **Recover data on Windows devices**.</span></span> <span data-ttu-id="7a60a-120">Azt javasoljuk, hogy kapcsolja **be.**</span><span class="sxs-lookup"><span data-stu-id="7a60a-120">We recommend that you turn it **On**.</span></span>
    <span data-ttu-id="7a60a-121">Ahhoz, hogy megkereshesse az adat-helyreállítási megbízott tanúsítványának helyét, először létre kell hoznia egyet.</span><span class="sxs-lookup"><span data-stu-id="7a60a-121">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one.</span></span> <span data-ttu-id="7a60a-122">Az utasításokért olvassa el a Titkosított fájlrendszer (EFS) adat-helyreállítási [megbízottja (DRA)](https://go.microsoft.com/fwlink/p/?linkid=853700)tanúsítvány létrehozása és ellenőrzése.</span><span class="sxs-lookup"><span data-stu-id="7a60a-122">For instructions, see [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](https://go.microsoft.com/fwlink/p/?linkid=853700).</span></span>
    
    <span data-ttu-id="7a60a-123">A munkahelyi fájlok alapértelmezés szerint egy az eszközön tárolt és a felhasználó profiljához társított titkos kulccsal vannak titkosítva.</span><span class="sxs-lookup"><span data-stu-id="7a60a-123">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile.</span></span> <span data-ttu-id="7a60a-124">Csak a felhasználó tudja megnyitni és visszafejteni a fájlt.</span><span class="sxs-lookup"><span data-stu-id="7a60a-124">Only the user can open and decrypt the file.</span></span> <span data-ttu-id="7a60a-125">Így tehát, ha valaki elveszít egy eszközt, vagy törölnek egy felhasználót, egy szükséges fájl titkosított állapotban ragadhat.</span><span class="sxs-lookup"><span data-stu-id="7a60a-125">However, if a device is lost or a user is removed, a file can be stuck in an encrypted state.</span></span> <span data-ttu-id="7a60a-126">A rendszergazda az adat-helyreállítási megbízott tanúsítványával visszafejtheti a fájlt.</span><span class="sxs-lookup"><span data-stu-id="7a60a-126">An admin can use the Data Recovery Agent (DRA) certificate to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="7a60a-128">Bontsa ki a További hálózati és **felhőbeli** helyek védelme lehetőséget, ha további tartományokat vagy SharePoint Online-helyeket szeretne felvenni, hogy a felsorolt appokban lévő fájlok védettek-e.</span><span class="sxs-lookup"><span data-stu-id="7a60a-128">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps are protected.</span></span> <span data-ttu-id="7a60a-129">Ha bármelyik mezőben egynél több elemet kell megadnia, pontosvesszővel (;) válassza el őket egymástól.</span><span class="sxs-lookup"><span data-stu-id="7a60a-129">If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span>
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="7a60a-p104">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span><span class="sxs-lookup"><span data-stu-id="7a60a-p104">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
12. <span data-ttu-id="7a60a-133">Végül válassza a **Hozzáadás** lehetőséget a házirend mentéséhez és eszközökhöz való hozzárendeléséhez.</span><span class="sxs-lookup"><span data-stu-id="7a60a-133">Finally, choose **Add** to save the policy, and assign it to devices.</span></span> 

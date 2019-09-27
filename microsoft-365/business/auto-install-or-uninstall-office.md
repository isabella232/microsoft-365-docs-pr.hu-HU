---
title: Az Office automatikus telepítése vagy eltávolítása Windows 10-es eszközökön
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: cbc6bfe5-565a-4fb8-95f0-b06e7b74ac46
description: 'Telepítse vagy távolítsa el az Office a Windows 10 eszközök a Microsoft 365 Business Admin Center. '
ms.openlocfilehash: d82ab8292211d1adacba732922bf693dd2157ad6
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "37287535"
---
# <a name="automatically-install-or-uninstall-office-on-windows-10-devices"></a><span data-ttu-id="17c68-103">Az Office automatikus telepítése vagy eltávolítása Windows 10-es eszközökön</span><span class="sxs-lookup"><span data-stu-id="17c68-103">Automatically install or uninstall Office on Windows 10 devices</span></span>

<span data-ttu-id="17c68-104">[![Label, hogy tudd, az admin központ változik, és találsz további részleteket a aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="17c68-104">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="17c68-105">Gyorsan és egyszerűen telepítheti az Office-t Windows 10-es PC-kre a Microsoft 365 Business felügyeleti központjából.</span><span class="sxs-lookup"><span data-stu-id="17c68-105">You can quickly and easily install Office to Windows 10 PCs from the Microsoft 365 Business admin center.</span></span>
  
<span data-ttu-id="17c68-106">Ha meg szeretné érteni, hogy ez hogyan működik a korábban telepített Office-appokkal, olvassa el a [Felkészülés az Office-ügyfél telepítésére](prepare-for-office-client-deployment.md) című témakört.</span><span class="sxs-lookup"><span data-stu-id="17c68-106">To understand how this works with previously installed Office apps, read [Prepare for Office client installation](prepare-for-office-client-deployment.md) before you get started.</span></span> 
  
## <a name="manage-office-deployments"></a><span data-ttu-id="17c68-107">Az Office üzembe helyezésének kezelése</span><span class="sxs-lookup"><span data-stu-id="17c68-107">Manage Office deployments</span></span>

1. <span data-ttu-id="17c68-108">Jelentkezzen be a [felügyeleti központba](https://aka.ms/bcsportal) globális rendszergazdai hitelesítő adatokkal.</span><span class="sxs-lookup"><span data-stu-id="17c68-108">Sign in to the [admin center](https://aka.ms/bcsportal) with global admin credentials.</span></span> 
    
2. <span data-ttu-id="17c68-109">Az **Eszközök** kártyán válassza **Az Office üzembe helyezésének kezelése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="17c68-109">On the **Devices** card, choose **Manage Office Deployment**.</span></span>
      <span data-ttu-id="17c68-110">Ha nem látható az **eszközműveletek** karton, akkor az Admin Center **Kezdőlap** lapján kattintson a **Hozzáadás** (+) gombra, ha fel szeretné adni az adminisztrátori otthont.</span><span class="sxs-lookup"><span data-stu-id="17c68-110">If you do not see the **Device actions** card, in the admin center **Home** page, click **Add** (+) to add it to your admin home.</span></span>
    
    ![Screenshot of the Devices card in the admin center](media/9982e784-dbf9-4a76-a159-bb3e2e5aa23f.png)
  
3. <span data-ttu-id="17c68-112">A megnyíló **Az Office üzembe helyezésének kezelése** ablaktáblában válassza a **Csoport hozzáadása** elemet, majd jelölje ki a használni kívánt csoportokat.</span><span class="sxs-lookup"><span data-stu-id="17c68-112">On the **Manage Office deployment** pane that opens, choose **Add a group**, then select the groups you want use.</span></span>
    
4. <span data-ttu-id="17c68-113">Miután felvette a használni kívánt csoportot vagy csoportokat, válassza az **Üzembe helyezési művelet** legördülő listában **Az Office mihamarabbi telepítése** vagy **Az Office eltávolítása** elemet.</span><span class="sxs-lookup"><span data-stu-id="17c68-113">After you have added the group or groups you want to use, from the **Deployment Action** drop-down, select either **Install Office as soon as possible** or **Uninstall Office**.</span></span>
    
    ![In the Manage Office deployment pane, choose either Install Office as soon as possible, or Uninstall Office.](media/00f24a61-1848-40c0-b037-78d726c7d757.png)
  
5. <span data-ttu-id="17c68-115">Choose **Next** \> review the settings and then choose **Confirm**.</span><span class="sxs-lookup"><span data-stu-id="17c68-115">Choose **Next** \> review the settings and then choose **Confirm**.</span></span>
    
<span data-ttu-id="17c68-116">A 32 bites Office telepítése vagy újratelepítése automatikusan megtörténik az Ön által használt csoport vagy csoportok által megadott felhasználók eszközein.</span><span class="sxs-lookup"><span data-stu-id="17c68-116">A 32-bit Office will be automatically installed, or uninstalled in the devices owned by users specified by the group or groups you used.</span></span>
  
<span data-ttu-id="17c68-117">Ennek ellenőrzéséhez nyissa meg a Feladatkezelőt egy olyan számítógépen, amely ki lett jelölve egy Office-telepítéshez, és keresse meg a Microsoft Office Kattintásra folyamatot.</span><span class="sxs-lookup"><span data-stu-id="17c68-117">To verify you can open the Task Manager on a computer that was selected for an Office install and look for Microsoft Office Click-to-Run process.</span></span>
  



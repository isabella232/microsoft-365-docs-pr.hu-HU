---
title: Az eszközökön lévő adatok védelmének előfeltételei a Microsoft 365 vállalati verzióval
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
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
ms.assetid: 7770e280-3a6c-436f-a157-b008a2744f51
description: Ismerje meg a szervezet microsoft 365 vállalati verzióval történő beállításának és a munkahelyi adatok védelmének követelményeit a felhasználók eszközein.
ms.openlocfilehash: 1bfa2b2d2ceba68d39da9c65560e67a6602e6cfa
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44470967"
---
# <a name="prerequisites-for-protecting-data-on-devices-with-microsoft-365-for-business"></a><span data-ttu-id="f5a10-103">Az eszközökön lévő adatok védelmének előfeltételei a Microsoft 365 vállalati verzióval</span><span class="sxs-lookup"><span data-stu-id="f5a10-103">Prerequisites for protecting data on devices with Microsoft 365 for business</span></span>

<span data-ttu-id="f5a10-104">Ez a cikk a Microsoft 365 Business Premium szolgáltatásra vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="f5a10-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="f5a10-105">A szervezet Microsoft 365 vállalati verzióval való beállításának első lépése annak biztosítása, hogy megfeleljen az előfeltételeknek.</span><span class="sxs-lookup"><span data-stu-id="f5a10-105">The first step in setting up your organization with Microsoft 365 for business is to make sure you can meet the prerequisites.</span></span>
  
## <a name="requirements-for-setting-up-your-organization-with-microsoft-365-for-business"></a><span data-ttu-id="f5a10-106">A szervezet microsoft 365 vállalati verzióval való beállításának követelményei</span><span class="sxs-lookup"><span data-stu-id="f5a10-106">Requirements for setting up your organization with Microsoft 365 for business</span></span>

- <span data-ttu-id="f5a10-107">A windowsos eszközöknek Windows 7 Professional, Windows 8 Pro vagy Windows 8.1 Pro operációs rendszert kell futtatniuk.</span><span class="sxs-lookup"><span data-stu-id="f5a10-107">Windows devices must be running Windows 7 Professional, Windows 8 Pro, or Windows 8.1 Pro.</span></span>
    
    [<span data-ttu-id="f5a10-108">Windows-eszközök frissítése a Windows Pro alkotói frissítésére</span><span class="sxs-lookup"><span data-stu-id="f5a10-108">Upgrade Windows devices to Windows Pro Creators Update</span></span>](upgrade-to-windows-pro-creators-update.md)
    
    <span data-ttu-id="f5a10-109">Ha A Windows 10 Home, akkor meg kell **vásárolnia a** Windows 10 Pro.</span><span class="sxs-lookup"><span data-stu-id="f5a10-109">If you're running Windows 10 Home, then you must **purchase** Windows  10 Pro.</span></span> <span data-ttu-id="f5a10-110">További útmutatásért lásd [a Windows 10 Home frissítése Windows 10 Pro rendszerre.](https://support.office.com/article/0aee10c1-4d34-43ee-a325-579c6c2df90e?ui=en-US&rs=en-US&ad=US)</span><span class="sxs-lookup"><span data-stu-id="f5a10-110">See [upgrade Windows 10 Home to Windows 10 Pro](https://support.office.com/article/0aee10c1-4d34-43ee-a325-579c6c2df90e?ui=en-US&rs=en-US&ad=US) for instructions.</span></span> 
    
- <span data-ttu-id="f5a10-111">Távolítsa el az eszközöket a mobil felügyeleti megoldásokból (Mobile Iron, AirWatch és így tovább).</span><span class="sxs-lookup"><span data-stu-id="f5a10-111">Remove devices from mobile management solutions (Mobile Iron, AirWatch, and so on).</span></span> <span data-ttu-id="f5a10-112">A microsoft 365 vállalati verziómobilkezeléséhez regisztrálhatja a szervezet összes tagja számára.</span><span class="sxs-lookup"><span data-stu-id="f5a10-112">You'll enroll all the people in your organization in Microsoft 365 for business mobile management.</span></span>
    
- <span data-ttu-id="f5a10-113">Apple iOS 8.0 vagy újabb verzió</span><span class="sxs-lookup"><span data-stu-id="f5a10-113">Apple iOS 8.0 and later.</span></span>
    
    <span data-ttu-id="f5a10-114">Google Android 4.0 vagy újabb verzió (beleértve a Samsung KNOX Standard 4.0-t, illetve az újabb verziókat).</span><span class="sxs-lookup"><span data-stu-id="f5a10-114">Google Android 4.0 and later (including Samsung KNOX Standard 4.0 and higher).</span></span> <span data-ttu-id="f5a10-115">További információt az Intune által támogatott eszközök című [témakörben talál.](https://go.microsoft.com/fwlink/p/?linkid=852307)</span><span class="sxs-lookup"><span data-stu-id="f5a10-115">For more information, see [Intune supported devices](https://go.microsoft.com/fwlink/p/?linkid=852307).</span></span>
    
- <span data-ttu-id="f5a10-116">Ha már rendelkezik meglévő Office-alkalmazásokkal a felhasználói számítógépeken, olvassa el [az Office-ügyféltelepítésre való felkészülést,](prepare-for-office-client-deployment.md) hogy megértse azokat a lépéseket, amelyeket meg kell tennie ahhoz, hogy beállíthassa a Microsoft 365 vállalati verziót az Office 2016 felhasználói számítógépekre történő telepítéséhez.</span><span class="sxs-lookup"><span data-stu-id="f5a10-116">If you have existing Office applications on user computers, read [prepare for Office client installation](prepare-for-office-client-deployment.md) to understand steps you might need to take before you can set up Microsoft 365 for business to install Office 2016 on user computers.</span></span> 

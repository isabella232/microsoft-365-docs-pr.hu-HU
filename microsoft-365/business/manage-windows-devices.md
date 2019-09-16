---
title: A tartományhoz csatlakoztatott Windows 10-es eszközök kezelésének engedélyezése a Microsoft 365 Vállalati verzió számára
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
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Útmutató a Microsoft 365 a helyi AD-hez csatlakozott Windows 10-eszközök védelmének engedélyezéséhez.
ms.openlocfilehash: 5cce4bc53f118560e31ad7e6048e4efcb49d662e
ms.sourcegitcommit: c0f769244d05ad019ea2307c38d5543d7b1e5afd
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992229"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="afac5-103">A tartományhoz csatlakoztatott Windows 10-es eszközök kezelésének engedélyezése a Microsoft 365 Vállalati verzió számára</span><span class="sxs-lookup"><span data-stu-id="afac5-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="afac5-104">Ha a szervezet helyi Windows Server Active Directoryt használ, beállíthatja a Microsoft 365 Business rendszert, hogy védje a Windows 10 eszközeit, miközben továbbra is fenntartja az intézményi erőforrásokhoz való hozzáférést, amelyekhez szükség van lokális hitelesítésre.</span><span class="sxs-lookup"><span data-stu-id="afac5-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="afac5-105">Ezt úgy állíthatja be, hogy először a Azure Active Directoryval szinkronizálja az Active Directory címtárat, majd regisztrálja a Windows 10 eszközöket az azúrkék HIRDETÉSRE, és a Microsoft 365 Business mobileszköz-kezelést végez.</span><span class="sxs-lookup"><span data-stu-id="afac5-105">You can set this up by first synchronizing your Active Directory with Azure Active Directory, followed by registering the Windows 10 devices with Azure AD and enrolling them for mobile device management by Microsoft 365 Business.</span></span>
<span data-ttu-id="afac5-106">A következő videó részletesen ismerteti, hogy hogyan lehet ezt beállítani a leggyakoribb forgatókönyvhöz.</span><span class="sxs-lookup"><span data-stu-id="afac5-106">The following video details the steps for how to set this up for the most common scenario.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="afac5-107">A Microsoft 365 Business által kezelhető, tartományhoz csatlakoztatott eszközök beállítása</span><span class="sxs-lookup"><span data-stu-id="afac5-107">Set up domain-joined devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="afac5-108">Ahhoz, hogy a szervezet tartományhoz csatlakoztatott eszközeit úgy állítsa be, hogy a helyszíni Active Directory címtáron kívül az Azure Active Directory által nyújtott szolgáltatások előnyeit is élvezheti, a **hibrid Azure beépített eszközöket**is implementálja.</span><span class="sxs-lookup"><span data-stu-id="afac5-108">To set up your organization's domain-joined devices to benefit from the capabilities provided by Azure Active Directory in addition to on-premises Active Directory, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="afac5-109">Ezek olyan eszközök, amelyek mind a helyi Active Directory címtárba, mind a Azure Active Directoryba csatlakoztak.</span><span class="sxs-lookup"><span data-stu-id="afac5-109">These are devices that are joined both to your on-premises Active Directory and your Azure Active Directory.</span></span> <span data-ttu-id="afac5-110">A Hybrid Azure egyesített eszközök a Microsoft 365 Business által védhetők és kezelhetők.</span><span class="sxs-lookup"><span data-stu-id="afac5-110">Hybrid Azure AD joined devices can be protected and managed by Microsoft 365 Business.</span></span> 
  
<span data-ttu-id="afac5-111">Hajtsa végre az alábbi lépéseket a Microsoft 365 Business által a Hybrid Azure AD által egyesített és kezelt Windows 10-eszközök elérhetővé tétele érdekében.</span><span class="sxs-lookup"><span data-stu-id="afac5-111">Complete the steps below to make your Windows 10 devices Hybrid Azure AD joined and managed by Microsoft 365 Business.</span></span>
  
1. <span data-ttu-id="afac5-112">A felhasználók, csoportok és kapcsolattartók helyi Active Directoryból Azure Active Directoryba történő szinkronizálásához futtassa a címtár-szinkronizálás varázslót és az Azure Active Directory csatlakozási szolgáltatást az [Office 365 címtár-szinkronizálás beállítása](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)című témakörben leírtak szerint.</span><span class="sxs-lookup"><span data-stu-id="afac5-112">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure Active Directory Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
    > [!NOTE]
    > <span data-ttu-id="afac5-113">A lép van pontosan ugyanaz részére Mikroszkóp 365 teendő.</span><span class="sxs-lookup"><span data-stu-id="afac5-113">The steps are exactly the same for Microsoft 365 Business.</span></span> 
  
2. <span data-ttu-id="afac5-114">A 3. lépés elvégzése előtt ahhoz, hogy a Windows 10 eszközök Hybrid Azure AD csatlakozhatók legyenek, a következő előfeltételeknek kell eleget tennie:</span><span class="sxs-lookup"><span data-stu-id="afac5-114">Before you complete step 3 to enable Windows 10 devices to be Hybrid Azure AD joined, you need to make sure that you meet the following prerequisites:</span></span>

   - <span data-ttu-id="afac5-115">A legújabb verziójú Azure AD Connect-et futtatja.</span><span class="sxs-lookup"><span data-stu-id="afac5-115">You are running the latest version of Azure AD connect.</span></span>

   - <span data-ttu-id="afac5-116">Azúrkék AD összeköt birtokol szinkronizál minden a számítógép tárgy-ból berendezés ön akar-hoz lenni hibrid Azure AD összekapcsolt.</span><span class="sxs-lookup"><span data-stu-id="afac5-116">Azure AD connect has synchronized all the computer objects of the devices you want to be hybrid Azure AD joined.</span></span> <span data-ttu-id="afac5-117">Ha a számítógép-objektumok meghatározott szervezeti egységekhez tartoznak, akkor győződjön meg arról, hogy ezek a szervezeti egységek szinkronizálásra vannak beállítva a Azure AD Connect-ben is.</span><span class="sxs-lookup"><span data-stu-id="afac5-117">If the computer objects belong to specific organizational units (OU), then make sure these OUs are set for synchronization in Azure AD connect as well.</span></span>
    
3. <span data-ttu-id="afac5-118">Regisztrálja a meglévő, tartományhoz csatlakoztatott Windows 10-eszközöket a hibrid Azure AD-hez, és igényelje azokat az Intune (Microsoft 365 Business) mobil eszközkezelésére:</span><span class="sxs-lookup"><span data-stu-id="afac5-118">Register existing domain-joined Windows 10 devices to be hybrid Azure AD Joined and enroll them for mobile device management by Intune (Microsoft 365 Business):</span></span>
    
4. <span data-ttu-id="afac5-119">Kövesse lépésről lépésre, [Hogyan állítsuk be a hibrid Azure Active Directory egyesített eszközeit](https://go.microsoft.com/fwlink/p/?linkid=872870).</span><span class="sxs-lookup"><span data-stu-id="afac5-119">Follow the step by step instructions in [How to configure hybrid Azure Active Directory joined devices](https://go.microsoft.com/fwlink/p/?linkid=872870).</span></span> <span data-ttu-id="afac5-120">Ez lehetővé teszi az intézményi Active Directory-nak a Windows 10 számítógépekhez való szinkronizálását, és készen áll a felhőre.</span><span class="sxs-lookup"><span data-stu-id="afac5-120">This will enable the synchronization of your on-premises Active Directory joined Windows 10 computers and make them cloud ready.</span></span>
    
5. <span data-ttu-id="afac5-121">A Windows 10 eszköz mobil eszközkezelés céljából történő igényléséhez tekintse meg a [Windows 10 eszköznek az Intune szolgáltatással történő igénylésével](https://go.microsoft.com/fwlink/p/?linkid=872871) kapcsolatos utasításokat a csoportházirend segítségével.</span><span class="sxs-lookup"><span data-stu-id="afac5-121">In order to enroll a Windows 10 device for mobile device management, see [Enroll a Windows 10 device with Intune by using a Group Policy](https://go.microsoft.com/fwlink/p/?linkid=872871) for instructions.</span></span> <span data-ttu-id="afac5-122">A csoportházirendet beállíthatja helyi számítógépszinten vagy tömeges műveleteknél, ezt a csoportházirend-beállítást létrehozhatja a tartományvezérlő-kiszolgálón is.</span><span class="sxs-lookup"><span data-stu-id="afac5-122">You can set the Group Policy at a local computer level or for bulk operations, you can create this group policy setting on your domain controller server.</span></span>
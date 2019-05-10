---
title: A tartományhoz csatlakoztatott Windows 10-es eszközök kezelésének engedélyezése a Microsoft 365 Vállalati verzió számára
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
description: Útmutató a Microsoft 365 védelmének engedélyezése helyi AD Windows 10 eszközök csatlakozott.
ms.openlocfilehash: 661e5bf8205a661eb4382b4bdd8fcf3a54ecc12f
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660309"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="c247a-103">A tartományhoz csatlakoztatott Windows 10-es eszközök kezelésének engedélyezése a Microsoft 365 Vállalati verzió számára</span><span class="sxs-lookup"><span data-stu-id="c247a-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="c247a-104">Ha a szervezet használja a Windows Server Active Directory helyszíni, állíthat be Microsoft 365 üzleti védelme érdekében a Windows 10 eszközök továbbra is fenntartva helyi hitelesítést igénylő helyszíni erőforrásokhoz való hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="c247a-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="c247a-105">Beállíthatja a által első szinkronizálása az Active Directory Azure Active Directory regisztrálja a Windows 10 eszközök Azure AD, majd azokat igénylése Microsoft 365 üzleti mobil eszköz kezelésére.</span><span class="sxs-lookup"><span data-stu-id="c247a-105">You can set this up by first synchronizing your Active Directory with Azure Active Directory, followed by registering the Windows 10 devices with Azure AD and enrolling them for mobile device management by Microsoft 365 Business.</span></span>
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="c247a-106">Microsoft 365 üzleti által kezelt tartományhoz csatlakoztatott eszközök beállítása</span><span class="sxs-lookup"><span data-stu-id="c247a-106">Set up domain-joined devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="c247a-107">Tartományhoz csatlakoztatott eszközök a szervezet beállítása a Azure Active Directory mellett helyszíni Active Directory nyújtotta lehetőségeket élvezhessék, megvalósítható **hibrid Azure AD eszközöket csatlakozott**.</span><span class="sxs-lookup"><span data-stu-id="c247a-107">To set up your organization's domain-joined devices to benefit from the capabilities provided by Azure Active Directory in addition to on-premises Active Directory, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="c247a-108">Ezek olyan eszközök, amelyek mind a helyszíni Active Directory és az Azure Active Directory tartományhoz.</span><span class="sxs-lookup"><span data-stu-id="c247a-108">These are devices that are joined both to your on-premises Active Directory and your Azure Active Directory.</span></span> <span data-ttu-id="c247a-109">Hibrid csatlakozott Azure AD eszközöket védett, és kezeli a Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="c247a-109">Hybrid Azure AD joined devices can be protected and managed by Microsoft 365 Business.</span></span> 
  
<span data-ttu-id="c247a-110">Hajtsa végre az alábbi lépéseket a Windows 10 eszközök hibrid Azure AD a tartományhoz, és kezeli a Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="c247a-110">Complete the steps below to make your Windows 10 devices Hybrid Azure AD joined and managed by Microsoft 365 Business.</span></span>
  
1. <span data-ttu-id="c247a-111">A felhasználók, csoportok és a helyi Active Directory ügyfelek Active Directory Azure szinkronizálásához futtassa a címtár-szinkronizálás varázsló és Azure Active Directory csatlakozás az [Office 365 címtár-szinkronizálás beállítása](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="c247a-111">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure Active Directory Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
    > [!NOTE]
    > <span data-ttu-id="c247a-112">A lépések azonosak, pontosan 365 üzleti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c247a-112">The steps are exactly the same for Microsoft 365 Business.</span></span> 
  
2. <span data-ttu-id="c247a-113">3. lépést ahhoz, hogy Windows 10 eszközök hibrid Azure AD a tartományhoz kell, meg kell győződjön meg arról, hogy teljesülnek a következő előfeltételek:</span><span class="sxs-lookup"><span data-stu-id="c247a-113">Before you complete step 3 to enable Windows 10 devices to be Hybrid Azure AD joined, you need to make sure that you meet the following prerequisites:</span></span>

   - <span data-ttu-id="c247a-114">Borzas AD a legújabb verzióját futtatja csatlakozni.</span><span class="sxs-lookup"><span data-stu-id="c247a-114">You are running the latest version of Azure AD connect.</span></span>

   - <span data-ttu-id="c247a-115">Borzas AD csatlakozás van szinkronizálva legyen hibrid Azure AD csatlakozott az eszközök számítógép-objektumok.</span><span class="sxs-lookup"><span data-stu-id="c247a-115">Azure AD connect has synchronized all the computer objects of the devices you want to be hybrid Azure AD joined.</span></span> <span data-ttu-id="c247a-116">Ha a számítógép-objektumok adott szervezeti egység (OU) tartozó, majd állítsuk a szervezeti egységek az Azure Active Directory szinkronizálási kapcsolatot, valamint.</span><span class="sxs-lookup"><span data-stu-id="c247a-116">If the computer objects belong to specific organizational units (OU), then make sure these OUs are set for synchronization in Azure AD connect as well.</span></span>
    
3. <span data-ttu-id="c247a-117">Meglévő tartományhoz tartozó Windows 10 eszközök Azure AD Joined hibrid és Intune (Microsoft 365 Business) mobil eszköz kezelésére őket igényelni regisztrálása:</span><span class="sxs-lookup"><span data-stu-id="c247a-117">Register existing domain-joined Windows 10 devices to be hybrid Azure AD Joined and enroll them for mobile device management by Intune (Microsoft 365 Business):</span></span>
    
4. <span data-ttu-id="c247a-118">[Hibrid Azure Active Directory tartományhoz eszközök konfigurálása](https://go.microsoft.com/fwlink/p/?linkid=872870)lépésről lépésre kövesse.</span><span class="sxs-lookup"><span data-stu-id="c247a-118">Follow the step by step instructions in [How to configure hybrid Azure Active Directory joined devices](https://go.microsoft.com/fwlink/p/?linkid=872870).</span></span> <span data-ttu-id="c247a-119">Ez lehetővé teszi a helyi Active Directory szinkronizálása Windows 10 számítógépek tartományhoz, és azokat a felhő kész.</span><span class="sxs-lookup"><span data-stu-id="c247a-119">This will enable the synchronization of your on-premises Active Directory joined Windows 10 computers and make them cloud ready.</span></span>
    
5. <span data-ttu-id="c247a-120">Annak érdekében, hogy egy mobil eszköz kezelése Windows 10 eszköz igényléséhez utasításokat [igényelni egy Intune a csoportházirend segítségével Windows 10 eszközt](https://go.microsoft.com/fwlink/p/?linkid=872871) talál.</span><span class="sxs-lookup"><span data-stu-id="c247a-120">In order to enroll a Windows 10 device for mobile device management, see [Enroll a Windows 10 device with Intune by using a Group Policy](https://go.microsoft.com/fwlink/p/?linkid=872871) for instructions.</span></span> <span data-ttu-id="c247a-121">Beállíthatja a csoportházirend egy olyan helyi számítógép szinten, vagy a tömeges műveletek esetében a tartomány vezérlő-kiszolgálón hozhat létre a csoportházirend-beállítás.</span><span class="sxs-lookup"><span data-stu-id="c247a-121">You can set the Group Policy at a local computer level or for bulk operations, you can create this group policy setting on your domain controller server.</span></span>
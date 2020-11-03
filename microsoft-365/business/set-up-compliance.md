---
title: A fenyegetések elleni védelem növelése a Microsoft 365 vállalati prémium verzióban
f1.keywords:
- NOCSH
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
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Beállíthatja a megfelelőségi funkciókat az adatvesztés elkerülése érdekében, és segítséget nyújt az ügyfelek bizalmas adatainak biztonságának megőrzésében.
ms.openlocfilehash: 2c95ad3f36df28af2c68cd11192bcfe92dfe29e3
ms.sourcegitcommit: e56894917d2aae05705c3b9447388d10e2156183
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48841173"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="74850-103">A megfelelőségi funkciók beállítása</span><span class="sxs-lookup"><span data-stu-id="74850-103">Set up compliance features</span></span>

<span data-ttu-id="74850-104">A Microsoft 365 vállalati prémium verzió az adatok és az eszközök védelméhez tartalmaz funkciókat, és segítséget nyújt az ügyfelek bizalmas adatainak biztonságának megőrzésében.</span><span class="sxs-lookup"><span data-stu-id="74850-104">Your Microsoft 365 Business Premium comes with features to protect your data and devices, and help you keep your and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="74850-105">DLP-szolgáltatások beállítása</span><span class="sxs-lookup"><span data-stu-id="74850-105">Set up DLP features</span></span>

<span data-ttu-id="74850-106">Lásd: [DLP-házirend létrehozása sablonból](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) , például arról, hogy miként állíthat be házirendet a személyes adatvesztés elleni védekezéshez.</span><span class="sxs-lookup"><span data-stu-id="74850-106">See [Create a DLP policy from a template](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) for an example on how to set up a policy to protect against protect loss of personal data.</span></span> 
  
<span data-ttu-id="74850-107">A DLP számos különböző nyelvhez használható, használatra kész házirend-sablonokat tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="74850-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="74850-108">Például Ausztrália pénzügyi adatok, kanadai személyes adatok, Amerikai pénzügyi adatok stb.</span><span class="sxs-lookup"><span data-stu-id="74850-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="74850-109">Ebből a cikkből megtudhatja, hogy [milyen DLP-házirend-sablonok](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) találhatók a teljes lista számára.</span><span class="sxs-lookup"><span data-stu-id="74850-109">See [What the DLP policy templates include](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) for a full list.</span></span> <span data-ttu-id="74850-110">Az összes ilyen sablonhoz hasonlóan engedélyezhetők a szakmai sablon példája is.</span><span class="sxs-lookup"><span data-stu-id="74850-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="74850-111">E-mail-adatmegőrzés beállítása az Exchange Online archiválási szolgáltatásával</span><span class="sxs-lookup"><span data-stu-id="74850-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="74850-112">Az **Exchange Online archiválási** licencelési funkciói a megfelelőségi és szabályozási szabványokat a eDiscovery e-mail-tartalmainak megőrzésével segítik.</span><span class="sxs-lookup"><span data-stu-id="74850-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="74850-113">Az is segít csökkenteni a kockázatokat, ha van egy pert, és lehetővé teszi az adathelyreállítást egy biztonsági rést követően, vagy ha a törölt elemek helyreállítására van szükség.</span><span class="sxs-lookup"><span data-stu-id="74850-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="74850-114">A perköltség megőrzésével megőrizheti az összes felhasználó tartalmát, illetve adatmegőrzési házirendeket alkalmazva testre szabhatja a megőrizni kívánt tartalmat.</span><span class="sxs-lookup"><span data-stu-id="74850-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="74850-115">Jogellenes **tartás:** A törölt elemeket tartalmazó összes postaláda-tartalmat megőrizheti, ha a felhasználó teljes postaládáját a peres eljárási mentességre helyezi.</span><span class="sxs-lookup"><span data-stu-id="74850-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="74850-116">Ha egy postaládát pert-mentességre szeretne helyezni, a felügyeleti központban:</span><span class="sxs-lookup"><span data-stu-id="74850-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="74850-117">A bal oldali navigációs sávon **lépjen az** \> **aktív** felhasználók elemre.</span><span class="sxs-lookup"><span data-stu-id="74850-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="74850-118">Jelölje ki azt a felhasználót, akinek a postaládáját pert-mentességre szeretné helyezni.</span><span class="sxs-lookup"><span data-stu-id="74850-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="74850-119">A felhasználó ablaktáblában bontsa ki a **posta beállításai** lapot, majd a **További beállítások** mellett válassza az **Exchange-Tulajdonságok szerkesztése** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="74850-119">In the user pane, expand **Mail settings** , and next to **More settings** , choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="74850-120">A felhasználó postaládája lapján válassza a \* \* postaláda-funkciók \* \* elemet a bal oldali navigációs sávon, majd válassza az **enable (Engedélyezés** ) hivatkozást a **peres eljárási mentesség** csoportban.</span><span class="sxs-lookup"><span data-stu-id="74850-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="74850-121">A pert **-mentesség párbeszédpanelen** megadhatja a jogellenes tartás időtartamát a **jogvitákban** .</span><span class="sxs-lookup"><span data-stu-id="74850-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="74850-122">Hagyja üresen a mezőt, ha végtelen mentességet szeretne elhelyezni.</span><span class="sxs-lookup"><span data-stu-id="74850-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="74850-123">Jegyzeteket is adhat hozzá, és a postaláda tulajdonosát egy webhelyre irányíthatja, amelyet érdemes megmagyaráznia a peres eljárás megtartásáról.</span><span class="sxs-lookup"><span data-stu-id="74850-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="74850-124">\>**Mentés gombot**.</span><span class="sxs-lookup"><span data-stu-id="74850-124">\> **Save**.</span></span>
    
<span data-ttu-id="74850-125">**Adatmegőrzés:** Engedélyezheti a testre szabott adatmegőrzési házirendeket, például egy adott idő megőrzését vagy a tartalom végleges törlését az adatmegőrzési időszak végén.</span><span class="sxs-lookup"><span data-stu-id="74850-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="74850-126">További információt [az adatmegőrzési házirendek áttekintése](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="74850-126">To learn more, see [Overview of retention policies](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="74850-127">A tartalmi címkék beállítása</span><span class="sxs-lookup"><span data-stu-id="74850-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="74850-128">A tartalmi címkék az Azure Information Protection ("az" 1-es csomag) 1 csomaggal rendelkeznek, és segítséget nyújtanak a dokumentumok és e-mailek osztályozásához, a címkék alkalmazásával.</span><span class="sxs-lookup"><span data-stu-id="74850-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="74850-129">A címkék automatikusan alkalmazhatók olyan rendszergazdák számára, akik szabályok és feltételek meghatározását végzik manuálisan a felhasználók, illetve a felhasználók által megadott javaslatok kombinációjának használatával.</span><span class="sxs-lookup"><span data-stu-id="74850-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="74850-130">Az érzékenységi címkék beállításához tekintse meg a [tartalmi Címkék létrehozása és kezelése](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) című videót.</span><span class="sxs-lookup"><span data-stu-id="74850-130">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="74850-131">Az Azure Information Protection Client manuális telepítése</span><span class="sxs-lookup"><span data-stu-id="74850-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="74850-132">Az ügyfélszolgálati ügyfél kézi telepítése:</span><span class="sxs-lookup"><span data-stu-id="74850-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="74850-133">Töltse le **AzinfoProtection_UL.exe** a [Microsoft letöltőközpontból](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="74850-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="74850-134">Ellenőrizheti, hogy a telepítés a Word-dokumentum megtekintésével is működött-e, és gondoskodjon arról, hogy az **érzékenység** beállítás elérhető legyen a **Kezdőlap** lapon.</span><span class="sxs-lookup"><span data-stu-id="74850-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="74850-135">![A védelem lap egy Word-dokumentumban](../media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="74850-135">![Protection tab drop-down in a Word document.](../media/word-sensitivity.png)</span></span>

<span data-ttu-id="74850-136">További információt [az ügyfélalkalmazás telepítése](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="74850-136">For more information, see [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>

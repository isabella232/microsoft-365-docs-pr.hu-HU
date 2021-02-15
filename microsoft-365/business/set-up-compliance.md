---
title: Veszélyforrások elleni védelem növelése a Microsoft 365 Vállalati prémium verzióban
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
description: Megfelelőségi funkciókat állíthat be az adatvesztés megelőzése érdekében, és biztosíthatja az Ön és ügyfelei bizalmas adatainak biztonságát.
ms.openlocfilehash: 2c95ad3f36df28af2c68cd11192bcfe92dfe29e3
ms.sourcegitcommit: e56894917d2aae05705c3b9447388d10e2156183
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48841173"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="45cc4-103">Megfelelőségi szolgáltatások beállítása</span><span class="sxs-lookup"><span data-stu-id="45cc4-103">Set up compliance features</span></span>

<span data-ttu-id="45cc4-104">A Microsoft 365 Vállalati prémium verzió olyan szolgáltatásokat tartalmaz, amelyek megvédik az adatait és az eszközeit, és segítenek Önnek biztonságban tartani ügyfelei és bizalmas információit.</span><span class="sxs-lookup"><span data-stu-id="45cc4-104">Your Microsoft 365 Business Premium comes with features to protect your data and devices, and help you keep your and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="45cc4-105">DLP-szolgáltatások beállítása</span><span class="sxs-lookup"><span data-stu-id="45cc4-105">Set up DLP features</span></span>

<span data-ttu-id="45cc4-106">Lásd: [DLP-házirend](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) létrehozása sablonból, például arról, hogy miként állíthat be olyan házirendet, amely védelmet nyújt a személyes adatok elvesztésével szemben.</span><span class="sxs-lookup"><span data-stu-id="45cc4-106">See [Create a DLP policy from a template](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) for an example on how to set up a policy to protect against protect loss of personal data.</span></span> 
  
<span data-ttu-id="45cc4-107">A DLP számos használatra kész házirendsablont tartalmaz, amelyek számos különböző területi szabályhoz használhatók.</span><span class="sxs-lookup"><span data-stu-id="45cc4-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="45cc4-108">Ilyen például az Ausztráliai pénzügyi adatokra, a Kanadai személyes adatokra vonatkozó törvény, az Amerikai Egyesült Államok pénzügyi adatai stb.</span><span class="sxs-lookup"><span data-stu-id="45cc4-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="45cc4-109">A [teljes lista DLP-házirendsablonjai.](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include)</span><span class="sxs-lookup"><span data-stu-id="45cc4-109">See [What the DLP policy templates include](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) for a full list.</span></span> <span data-ttu-id="45cc4-110">Ezek a sablonok a pii sablon példához hasonlóan engedélyezhetők.</span><span class="sxs-lookup"><span data-stu-id="45cc4-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="45cc4-111">A levelezés megőrzésének beállítása az Exchange Online archiválásával</span><span class="sxs-lookup"><span data-stu-id="45cc4-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="45cc4-112">**Az Exchange Online archiválási** licencelési funkciói a levelezési tartalmak elektronikus adatfeltáráshoz való megőrzésével segítik a megfelelőségi és szabályozási szabványok megőrzését.</span><span class="sxs-lookup"><span data-stu-id="45cc4-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="45cc4-113">Az is segít csökkenteni a kockázatot, ha fennáll a peres eljárás, és lehetővé teszi az adatok helyreállítását biztonsági visszaélés vagy a törölt elemek helyreállítása után.</span><span class="sxs-lookup"><span data-stu-id="45cc4-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="45cc4-114">Jogi visszatartás használatával megőrizheti egy felhasználó összes tartalmát, vagy adatmegőrzési házirendekkel testre szabhatja a megőrizni kívánt tartalmakat.</span><span class="sxs-lookup"><span data-stu-id="45cc4-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="45cc4-115">**Jogi hold:** A postaláda teljes tartalmát megőrizheti, beleértve a törölt elemeket is, ha a felhasználó teljes postaládáját jogi úton tartja meg.</span><span class="sxs-lookup"><span data-stu-id="45cc4-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="45cc4-116">Egy postaláda jogi úton való felfüggesztése a Felügyeleti központban:</span><span class="sxs-lookup"><span data-stu-id="45cc4-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="45cc4-117">A bal oldali navigációs sávon a **Felhasználók** aktív felhasználók \> **csoportban.**</span><span class="sxs-lookup"><span data-stu-id="45cc4-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="45cc4-118">Jelölje ki azt a felhasználót, akinek a postaládáját jogi úton szeretné tartani.</span><span class="sxs-lookup"><span data-stu-id="45cc4-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="45cc4-119">A felhasználói panelen bontsa ki a **Levelezési** beállításokat, és **a** További beállítások csoportban válassza **az Exchange-tulajdonságok szerkesztése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="45cc4-119">In the user pane, expand **Mail settings**, and next to **More settings**, choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="45cc4-120">A felhasználó postaládalapján válassza a \*\* postaláda-funkciók \*\* lehetőséget a bal oldali navigációs sávon, majd válassza az **Engedélyezés** hivatkozást a Jogi eljárás miatti **tartás alatt.**</span><span class="sxs-lookup"><span data-stu-id="45cc4-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="45cc4-121">A jogi **hold párbeszédpanelen** megadhatja a jogi tartás időtartamát a Jogi tartás **időtartam mezőjében.**</span><span class="sxs-lookup"><span data-stu-id="45cc4-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="45cc4-122">Hagyja üresen a mezőt, ha végtelen holdat szeretne hagyni.</span><span class="sxs-lookup"><span data-stu-id="45cc4-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="45cc4-123">Jegyzeteket is adhat hozzá, és a postaláda-tulajdonost egy webhelyre irányíthatja, amelyről további magyarázatot kell mondania a jogi holdról.</span><span class="sxs-lookup"><span data-stu-id="45cc4-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="45cc4-124">\>**Mentés gombra.**</span><span class="sxs-lookup"><span data-stu-id="45cc4-124">\> **Save**.</span></span>
    
<span data-ttu-id="45cc4-125">**Adatmegőrzés:** Engedélyezheti a testre szabott adatmegőrzési házirendeket, például adott ideig megőrizheti őket, vagy véglegesen törölheti a tartalmakat az adatmegőrzési időszak végén.</span><span class="sxs-lookup"><span data-stu-id="45cc4-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="45cc4-126">További információt az adatmegőrzési házirendek [áttekintése témakörben talál.](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)</span><span class="sxs-lookup"><span data-stu-id="45cc4-126">To learn more, see [Overview of retention policies](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="45cc4-127">Bizalmasság-címkék beállítása</span><span class="sxs-lookup"><span data-stu-id="45cc4-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="45cc4-128">A bizalmasság-címkék az Azure Information Protection (AIP) 1. csomagját tartalmazják, és címkék alkalmazásával segítik a dokumentumok és e-mailek osztályozását és szükség esetén védelmét.</span><span class="sxs-lookup"><span data-stu-id="45cc4-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="45cc4-129">A címkéket automatikusan felhasználhatja a rendszergazdák, akik szabályokat és feltételeket definiálnak, a felhasználók manuálisan vagy egy olyan kombináció használatával, ahol a felhasználók javaslatokat kapnak.</span><span class="sxs-lookup"><span data-stu-id="45cc4-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="45cc4-130">A bizalmasság-címkék beállításához tekintse meg a [bizalmasság-címkék](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) létrehozásáról és kezelésről készült videót.</span><span class="sxs-lookup"><span data-stu-id="45cc4-130">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="45cc4-131">Az Azure Information Protection ügyfél manuális telepítése</span><span class="sxs-lookup"><span data-stu-id="45cc4-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="45cc4-132">Az AIP-ügyfél manuális telepítése:</span><span class="sxs-lookup"><span data-stu-id="45cc4-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="45cc4-133">Töltse **AzinfoProtection_UL.exe** Microsoft [letöltőközpontból.](https://www.microsoft.com/download/details.aspx?id=53018)</span><span class="sxs-lookup"><span data-stu-id="45cc4-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="45cc4-134">Ha ellenőrizni tudja, hogy a telepítés működött-e,  megtekinthet egy Word-dokumentumot, és meggyőződhet arról, hogy a Bizalmasság beállítás elérhető a **Kezdőlap** lapon.</span><span class="sxs-lookup"><span data-stu-id="45cc4-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="45cc4-135">![A Védelem lap legördülő menüje egy Word-dokumentumban](../media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="45cc4-135">![Protection tab drop-down in a Word document.](../media/word-sensitivity.png)</span></span>

<span data-ttu-id="45cc4-136">További információ: [Az ügyfélprogram telepítése.](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3)</span><span class="sxs-lookup"><span data-stu-id="45cc4-136">For more information, see [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>

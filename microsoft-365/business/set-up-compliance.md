---
title: Veszélyforrások elleni védelem növelése a Microsoft 365 Vállalati prémium verzióban
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
description: Megfelelőségi funkciókat állíthat be az adatvesztés megelőzése és az ügyfelek bizalmas adatainak biztonságossá tartása érdekében.
ms.openlocfilehash: c0accc37d3dcda9ba75813f01a98a3233c5a8369
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579954"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="e9f12-103">Megfelelőségi szolgáltatások beállítása</span><span class="sxs-lookup"><span data-stu-id="e9f12-103">Set up compliance features</span></span>

<span data-ttu-id="e9f12-104">A Microsoft 365 Vállalati prémium verzió olyan szolgáltatásokat tartalmaz, amelyek védik az adatait és az eszközeit, és segítenek Önnek biztonságban tartani ügyfelei és bizalmas információit.</span><span class="sxs-lookup"><span data-stu-id="e9f12-104">Your Microsoft 365 Business Premium comes with features to protect your data and devices, and help you keep your and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="e9f12-105">DLP-szolgáltatások beállítása</span><span class="sxs-lookup"><span data-stu-id="e9f12-105">Set up DLP features</span></span>

<span data-ttu-id="e9f12-106">A [személyes adatok elvesztésével](../compliance/create-a-dlp-policy-from-a-template.md) szembeni védelem beállítása érdekében a DLP-házirend létrehozása sablonból</span><span class="sxs-lookup"><span data-stu-id="e9f12-106">See [Create a DLP policy from a template](../compliance/create-a-dlp-policy-from-a-template.md) for an example on how to set up a policy to protect against protect loss of personal data.</span></span> 
  
<span data-ttu-id="e9f12-107">A DLP számos használatra kész házirendsablont tartalmaz, amelyek számos különböző területi szabályhoz használhatók.</span><span class="sxs-lookup"><span data-stu-id="e9f12-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="e9f12-108">Ilyen például az ausztráliai pénzügyi adatokra, a Kanadai személyes adatokra vonatkozó törvény, az Amerikai Egyesült Államok pénzügyi adatai stb.</span><span class="sxs-lookup"><span data-stu-id="e9f12-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="e9f12-109">Lásd: Mit tartalmaznak a [DLP-házirendsablonok](../compliance/what-the-dlp-policy-templates-include.md) a teljes listához.</span><span class="sxs-lookup"><span data-stu-id="e9f12-109">See [What the DLP policy templates include](../compliance/what-the-dlp-policy-templates-include.md) for a full list.</span></span> <span data-ttu-id="e9f12-110">Ezek a sablonok a pii-sablon példához hasonlóan engedélyezhetők.</span><span class="sxs-lookup"><span data-stu-id="e9f12-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="e9f12-111">A levelezés megőrzésének beállítása az Exchange Online archiválásával</span><span class="sxs-lookup"><span data-stu-id="e9f12-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="e9f12-112">**Az Exchange Online archiválási** licenc szolgáltatásai a megfelelőségi és szabályozási szabványok megőrzésével segítik a levelezési tartalmak megőrzését a elektronikus adatfeltárás érdekében.</span><span class="sxs-lookup"><span data-stu-id="e9f12-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="e9f12-113">A biztonsági visszaélés vagy a törölt elemek helyreállítása után is segít a kockázat csökkentésében, és lehetőséget nyújt az adatok helyreállítására is.</span><span class="sxs-lookup"><span data-stu-id="e9f12-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="e9f12-114">A jogi visszatartás segítségével megőrizheti egy felhasználó összes tartalmát, vagy adatmegőrzési házirendek használatával testre szabhatja a megőrizni kívánt tartalmakat.</span><span class="sxs-lookup"><span data-stu-id="e9f12-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="e9f12-115">**Jogi hold:** A postaláda teljes tartalmát megőrizheti, beleértve a törölt elemeket is, ha a felhasználó teljes postaládáját jogi jogi eljárásban tartja meg.</span><span class="sxs-lookup"><span data-stu-id="e9f12-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="e9f12-116">Egy postaláda jogi úton való tartásba való behelyének helyének megnyitásához a Felügyeleti központban:</span><span class="sxs-lookup"><span data-stu-id="e9f12-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="e9f12-117">A bal oldali navigációs sávon menjen a **Users** Active users (Felhasználók \> **aktív felhasználók) csoportra.**</span><span class="sxs-lookup"><span data-stu-id="e9f12-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="e9f12-118">Jelöljön ki egy felhasználót, akinek a postaládáját jogi úton szeretné eltenni.</span><span class="sxs-lookup"><span data-stu-id="e9f12-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="e9f12-119">A felhasználópanelen bontsa ki a **Levelezési** beállítások ot, és a **További** beállítások mellett válassza az **Exchange-tulajdonságok szerkesztése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="e9f12-119">In the user pane, expand **Mail settings**, and next to **More settings**, choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="e9f12-120">A felhasználó postaládalapján válassza a \*\* postaláda-szolgáltatások  \*\* lehetőséget a bal oldali navigációs sávon, majd válassza a Hivatkozás engedélyezése lehetőséget a Jogi **tartás csoportban.**</span><span class="sxs-lookup"><span data-stu-id="e9f12-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="e9f12-121">A jogi **tartás párbeszédpanelen** a jogi tartás időtartamát a Jogi tartás időtartama mezőben **adhatja** meg.</span><span class="sxs-lookup"><span data-stu-id="e9f12-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="e9f12-122">Ha végtelen holdhelyet szeretne, hagyja üresen a mezőt.</span><span class="sxs-lookup"><span data-stu-id="e9f12-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="e9f12-123">Jegyzeteket is adhat hozzá, és a postaláda-tulajdonost egy webhelyre irányíthatja, amelyről bővebben el kell magyaráznia a jogi holdról.</span><span class="sxs-lookup"><span data-stu-id="e9f12-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="e9f12-124">\>**Mentés gombra.**</span><span class="sxs-lookup"><span data-stu-id="e9f12-124">\> **Save**.</span></span>
    
<span data-ttu-id="e9f12-125">**Adatmegőrzés:** Engedélyezheti a testre szabott adatmegőrzési házirendeket, például adott ideig megőrizheti őket, vagy véglegesen törölheti a tartalmakat az adatmegőrzési időszak végén.</span><span class="sxs-lookup"><span data-stu-id="e9f12-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="e9f12-126">További információt Az adatmegőrzési házirendek [áttekintése témakörben talál.](../compliance/retention.md)</span><span class="sxs-lookup"><span data-stu-id="e9f12-126">To learn more, see [Overview of retention policies](../compliance/retention.md).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="e9f12-127">Bizalmasság-címkék beállítása</span><span class="sxs-lookup"><span data-stu-id="e9f12-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="e9f12-128">A bizalmasság-címkéket az Azure Information Protection (AIP) 1. csomagja tartalmaz, és címkék alkalmazásával segítik a dokumentumok és e-mailek osztályozását és szükség esetén védelmét.</span><span class="sxs-lookup"><span data-stu-id="e9f12-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="e9f12-129">A címkéket a rendszergazdák automatikusan, szabályokat és feltételeket definiálva, felhasználók által manuálisan, illetve olyan kombinációk használatával alkalmazhatók, amelyekben a felhasználók javaslatokat kapnak.</span><span class="sxs-lookup"><span data-stu-id="e9f12-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="e9f12-130">Bizalmasság-címkék beállításához tekintse meg a [bizalmasság-címkék](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) létrehozása és kezelése videót.</span><span class="sxs-lookup"><span data-stu-id="e9f12-130">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="e9f12-131">Az Azure Information Protection-ügyfél manuális telepítése</span><span class="sxs-lookup"><span data-stu-id="e9f12-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="e9f12-132">Az AIP-ügyfélprogram manuális telepítése:</span><span class="sxs-lookup"><span data-stu-id="e9f12-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="e9f12-133">Töltse **AzinfoProtection_UL.exe** a [Microsoft letöltőközpontból.](https://www.microsoft.com/download/details.aspx?id=53018)</span><span class="sxs-lookup"><span data-stu-id="e9f12-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="e9f12-134">A telepítés ellenőrzéséhez megtekinthet egy Word-dokumentumot,  és ellenőrizheti, hogy a Bizalmasság lehetőség elérhető-e a **Kezdőlap** lapon.</span><span class="sxs-lookup"><span data-stu-id="e9f12-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="e9f12-135">![A Védelem lap legördülő menüje egy Word-dokumentumban.](../media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="e9f12-135">![Protection tab drop-down in a Word document.](../media/word-sensitivity.png)</span></span>

<span data-ttu-id="e9f12-136">További információ: [Az ügyfél telepítése.](/azure/information-protection/infoprotect-tutorial-step3)</span><span class="sxs-lookup"><span data-stu-id="e9f12-136">For more information, see [Install the client](/azure/information-protection/infoprotect-tutorial-step3).</span></span>
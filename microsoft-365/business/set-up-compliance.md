---
title: A Microsoft 365 Business Premium fenyegetéselleni védelmének növelése
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
search.appverid:
- BCS160
- MET150
description: Megfelelőségi funkciók at állíthat be az adatvesztés megelőzése és az ügyfelek bizalmas adatainak biztonsága érdekében.
ms.openlocfilehash: e0d853223c7e6f455cba6e68ad173b137992d863
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/21/2020
ms.locfileid: "43635124"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="d4f17-103">Megfelelőségi funkciók beállítása</span><span class="sxs-lookup"><span data-stu-id="d4f17-103">Set up compliance features</span></span>

<span data-ttu-id="d4f17-104">A Microsoft 365 Business Premium olyan funkciókkal rendelkezik, amelyek védik az adatokat és az eszközöket, és segítenek biztonságban tartani ügyfeleit.</span><span class="sxs-lookup"><span data-stu-id="d4f17-104">Your Microsoft 365 Business Premium comes with features to protect your data and devices, and help you keep your and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="d4f17-105">DLP-szolgáltatások beállítása</span><span class="sxs-lookup"><span data-stu-id="d4f17-105">Set up DLP features</span></span>

<span data-ttu-id="d4f17-106">Lásd: [DLP-házirend létrehozása sablonból](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) egy példa, hogyan kell beállítani egy szabályzatot a személyazonosításra alkalmas adatok (PII) elleni védelem.</span><span class="sxs-lookup"><span data-stu-id="d4f17-106">See [Create a DLP policy from a template](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="d4f17-107">A DLP számos használatra kész házirendsablont használ számos különböző területi beállításhoz.</span><span class="sxs-lookup"><span data-stu-id="d4f17-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="d4f17-108">Például: Australia Financial Data, Canada Personal Information Act, Us Financial Data és így tovább.</span><span class="sxs-lookup"><span data-stu-id="d4f17-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="d4f17-109">A teljes lista a [DLP-házirendsablonok gyűjteményének](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) megtekintéséről.</span><span class="sxs-lookup"><span data-stu-id="d4f17-109">See [What the DLP policy templates include](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for a full list.</span></span> <span data-ttu-id="d4f17-110">Ezek a sablonok a példaként ii sablonhoz hasonlóan engedélyezhetők.</span><span class="sxs-lookup"><span data-stu-id="d4f17-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="d4f17-111">E-mailek megőrzésének beállítása az Exchange Online archiválásával</span><span class="sxs-lookup"><span data-stu-id="d4f17-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="d4f17-112">**Az Exchange Online archiválási** licencfunkciók segítenek fenntartani a megfelelőséget és a szabályozási szabványokat azáltal, hogy megőrzik az e-mailek tartalmát az elektronikus adatfeltáráshoz.</span><span class="sxs-lookup"><span data-stu-id="d4f17-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="d4f17-113">Ez is segít csökkenteni a kockázatot, ha van egy pert, és lehetővé teszi, hogy visszaszerezze az adatokat, miután a biztonság megsértése, vagy ha vissza kell állítani a törölt elemeket.</span><span class="sxs-lookup"><span data-stu-id="d4f17-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="d4f17-114">A peres eljárás miatti tartással megőrizheti a felhasználó teljes tartalmát, vagy adatmegőrzési házirendekkel testreszabhatja, hogy mit szeretne megőrizni.</span><span class="sxs-lookup"><span data-stu-id="d4f17-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="d4f17-115">**Peres eljárás miatti tartás:** Az összes postaládatartalmat megőrizheti, beleértve a törölt elemeket is, ha a felhasználó teljes postaládáját peres eljárás miatti tartásba helyezi.</span><span class="sxs-lookup"><span data-stu-id="d4f17-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="d4f17-116">Ha egy postaládát peres eljárás miatti tartásba szeretne helyezni, a Felügyeleti központban:</span><span class="sxs-lookup"><span data-stu-id="d4f17-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="d4f17-117">A bal oldali navigációs sávon nyissa meg a **Felhasználók** \> **aktív felhasználók lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="d4f17-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="d4f17-118">Jelöljön ki egy olyan felhasználót, akinek a postaládáját peres eljárás miatti tartásba kívánja helyezni.</span><span class="sxs-lookup"><span data-stu-id="d4f17-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="d4f17-119">A felhasználói ablaktáblán bontsa ki a **Posta beállításai csomópontot,** és a **További beállítások csoportban**válassza az **Exchange-tulajdonságok szerkesztése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="d4f17-119">In the user pane, expand **Mail settings**, and next to **More settings**, choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="d4f17-120">A felhasználó postaládalapján válassza a bal oldali navigációs eszköz \*\* postaláda-szolgáltatásait ,\* majd a Peres eljárás miatti tartás **csoportban** válassza az **Engedélyezés**hivatkozást.</span><span class="sxs-lookup"><span data-stu-id="d4f17-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="d4f17-121">A **peres eljárás miatti tartás** párbeszédpanelen megadhatja a peres eljárás várakoztatási időtartamát a **Peres eljárás várakoztatásidőtartama** mezőben.</span><span class="sxs-lookup"><span data-stu-id="d4f17-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="d4f17-122">Hagyja üresen a mezőt, ha végtelen tartást szeretne elhelyezni.</span><span class="sxs-lookup"><span data-stu-id="d4f17-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="d4f17-123">Megjegyzéseket is hozzáadhat, és a postaláda tulajdonosát egy olyan webhelyre irányíthatja, amelyről előfordulhat, hogy többet kell megmagyaráznia a peres eljárás miatti tartásról.</span><span class="sxs-lookup"><span data-stu-id="d4f17-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="d4f17-124">\>**Mentés.**</span><span class="sxs-lookup"><span data-stu-id="d4f17-124">\> **Save**.</span></span>
    
<span data-ttu-id="d4f17-125">**Megőrzés:** Engedélyezheti például a testreszabott adatmegőrzési házirendeket, hogy adott ideig megőrizzék vagy véglegesen töröljék a tartalmat az adatmegőrzési időszak végén.</span><span class="sxs-lookup"><span data-stu-id="d4f17-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="d4f17-126">További információ: [Az adatmegőrzési szabályok áttekintése.](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423)</span><span class="sxs-lookup"><span data-stu-id="d4f17-126">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="d4f17-127">Érzékenységi címkék beállítása</span><span class="sxs-lookup"><span data-stu-id="d4f17-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="d4f17-128">Az érzékenységi címkék az Azure Information Protection (AIP) 1- es csomaggal rendelkeznek, és címkék alkalmazásával segítenek a dokumentumok és e-mailek besorolásában és szükség esetén védelmében.</span><span class="sxs-lookup"><span data-stu-id="d4f17-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="d4f17-129">A címkéket automatikusan alkalmazhatják azok a rendszergazdák, akik szabályokat és feltételeket határoznak meg, manuálisan a felhasználók által, vagy olyan kombináció használatával, ahol a felhasználók javaslatokat kapnak.</span><span class="sxs-lookup"><span data-stu-id="d4f17-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="d4f17-130">Érzékenységi címkék beállításához tekintse [meg az érzékenységi címkék létrehozása és kezelése](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) videót.</span><span class="sxs-lookup"><span data-stu-id="d4f17-130">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="d4f17-131">Az Azure Information Protection ügyfél manuális telepítése</span><span class="sxs-lookup"><span data-stu-id="d4f17-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="d4f17-132">Az AIP-ügyfél manuális telepítése:</span><span class="sxs-lookup"><span data-stu-id="d4f17-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="d4f17-133">Töltse le **AzinfoProtection_UL.exe** programot a [Microsoft letöltőközpontjából.](https://www.microsoft.com/download/details.aspx?id=53018)</span><span class="sxs-lookup"><span data-stu-id="d4f17-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="d4f17-134">Ellenőrizheti, hogy a telepítés működött-e, ha megtekint egy Word-dokumentumot, és meggyőződik arról, hogy az **Érzékenység** lehetőség elérhető a **Kezdőlap** lapon.</span><span class="sxs-lookup"><span data-stu-id="d4f17-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="d4f17-135">![A Védelem lap legördülő menüje Egy Word-dokumentumban](../media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="d4f17-135">![Protection tab drop-down in a Word document.](../media/word-sensitivity.png)</span></span>

<span data-ttu-id="d4f17-136">További információt [az Ügyfél telepítése című](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3)témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="d4f17-136">For more information, see [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>

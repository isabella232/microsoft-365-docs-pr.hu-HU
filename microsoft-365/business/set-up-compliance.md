---
title: Növelje a Microsoft 365 Business fenyegetettség elleni védelmét
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
search.appverid:
- BCS160
- MET150
description: A megfelelőségi funkciók beállítása az adatvesztést és a címkeérzékeny adatok megelőzésére.
ms.openlocfilehash: 6fae95e8c5e6d133e3163dbdfd3c09cfede11382
ms.sourcegitcommit: 5d11f516e78ea4a74145e19ba2300f0792c8bac1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38715122"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="23048-103">Megfelelőségi funkciók beállítása</span><span class="sxs-lookup"><span data-stu-id="23048-103">Set up compliance features</span></span>

<span data-ttu-id="23048-104">A Microsoft 365 üzleti szolgáltatásai védik az adatokat és az eszközöket, és segítenek megőrizni az Ön és ügyfelei kényes információit.</span><span class="sxs-lookup"><span data-stu-id="23048-104">Your Microsoft 365 Business comes with features to protect your data and devices, and help you keep yours and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="23048-105">DLP-szolgáltatások beállítása</span><span class="sxs-lookup"><span data-stu-id="23048-105">Set up DLP features</span></span>

<span data-ttu-id="23048-106">Lásd a [DLP-házirend létrehozása sablonból](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) példát a személyes azonosításra alkalmas adatok (PII) elleni védelemre vonatkozó házirend beállításához.</span><span class="sxs-lookup"><span data-stu-id="23048-106">See [Create a DLP policy from a template](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="23048-107">A DLP sok különböző nyelvhez tartalmaz használatra kész házirendsablonokat.</span><span class="sxs-lookup"><span data-stu-id="23048-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="23048-108">Például Ausztrália pénzügyi adatok, Kanada személyes adatok törvény, az Egyesült Államok pénzügyi adatok, és így tovább.</span><span class="sxs-lookup"><span data-stu-id="23048-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="23048-109">Tekintse meg, [milyen a DLP házirendsablonok](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) a teljes listához.</span><span class="sxs-lookup"><span data-stu-id="23048-109">See [What the DLP policy templates include](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for a full list.</span></span> <span data-ttu-id="23048-110">Az összes ilyen sablon a PII példához hasonlóan engedélyezhető.</span><span class="sxs-lookup"><span data-stu-id="23048-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="23048-111">E-mail megőrzés beállítása az Exchange Online archiválással</span><span class="sxs-lookup"><span data-stu-id="23048-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="23048-112">Az **Exchange Online archiválási** licencfunkciói segítenek fenntartani a megfelelést és a szabályozó szabványokat az eDiscovery e-mail tartalmának megőrzésével.</span><span class="sxs-lookup"><span data-stu-id="23048-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="23048-113">Ez is segít csökken-a kockázat ha van egy polgári per, és szolgáltat egy út-hoz visszaszerez adat után egy biztonság megszegés amikor vagy szükség-hoz visszaszerez töröl cikk.</span><span class="sxs-lookup"><span data-stu-id="23048-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="23048-114">Peres eljárás miatti tartás használatával megőrizheti az összes felhasználó tartalmát, vagy az adatmegőrzési szabályok segítségével testreszabhatja a megőrizni kívánt tartalmat.</span><span class="sxs-lookup"><span data-stu-id="23048-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="23048-115">**Peres eljárás miatti tartás:** Megőrizheti az összes postaláda tartalmát, beleértve a törölt elemeket is, ha a felhasználó teljes postaládáját peres eljárás miatti tartásba helyezzük.</span><span class="sxs-lookup"><span data-stu-id="23048-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="23048-116">Ha peres eljárás miatti tartásba szeretne helyezni egy postafiókot, az admin központban:</span><span class="sxs-lookup"><span data-stu-id="23048-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="23048-117">-Ban bal NAV, megy **használók** \> **aktivál használók**.</span><span class="sxs-lookup"><span data-stu-id="23048-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="23048-118">Jelölje ki azt a felhasználót, akinek a postaládáját peres eljárás miatti tartásba szeretné helyezni.</span><span class="sxs-lookup"><span data-stu-id="23048-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="23048-119">A felhasználói ablaktáblán bontsa ki a **levelezési beállítások**, majd a **További beállítások**mellett az **Exchange-Tulajdonságok szerkesztése parancsot**.</span><span class="sxs-lookup"><span data-stu-id="23048-119">In the user pane, expand **Mail settings**, and next to **More settings**, choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="23048-120">A felhasználó postaládájának lapján válassza a bal oldali NAV \* \* postafiók jellemzőit, majd válassza a link **engedélyezése** **peres eljárás miatt tartás**alatt.</span><span class="sxs-lookup"><span data-stu-id="23048-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="23048-121">A peres **eljárások** visszatartási párbeszédpaneljén megadhatja a peres eljárás miatti tartás időtartamát a **peres eljárások tartam** mezőben.</span><span class="sxs-lookup"><span data-stu-id="23048-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="23048-122">Hagyja üresen a mezőt, ha egy végtelen visszatartott helyet szeretne.</span><span class="sxs-lookup"><span data-stu-id="23048-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="23048-123">Megjegyzéseket is felvehet, és közvetlenül a postaláda tulajdonosát egy olyan webhelyre irányhatja, amelyet esetleg meg kell magyarázni a peres eljárás miatti tartásba.</span><span class="sxs-lookup"><span data-stu-id="23048-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="23048-124">\>**Save**.</span><span class="sxs-lookup"><span data-stu-id="23048-124">\> **Save**.</span></span>
    
<span data-ttu-id="23048-125">**Visszatartás:** Engedélyezheti a testreszabott adatmegőrzési szabályokat, például egy adott idő megtartása érdekében, vagy a megőrzési időszak végén véglegesen törölheti a tartalmat.</span><span class="sxs-lookup"><span data-stu-id="23048-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="23048-126">További információ [az adatmegőrzési szabályok áttekintése](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423)című témakörben található.</span><span class="sxs-lookup"><span data-stu-id="23048-126">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="23048-127">A érzékenységi címkék beállítása</span><span class="sxs-lookup"><span data-stu-id="23048-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="23048-128">Érzékenység címkék jönnek Azure Information Protection (AIP) terv 1, és segít osztályozni, és opcionálisan védi a dokumentumok és e-maileket alkalmazásával címkéket.</span><span class="sxs-lookup"><span data-stu-id="23048-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="23048-129">A címkék automatikusan alkalmazhatók, ha a rendszergazdák szabályokat és feltételeket határoznak meg, manuálisan, felhasználók szerint, vagy olyan kombinációban, ahol a felhasználók ajánlásokat kapnak.</span><span class="sxs-lookup"><span data-stu-id="23048-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="23048-130">Az érzékenységi címkék beállításához tekintse meg az [érzékenységi címkék létrehozását és kezelését](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) ismertető videót.</span><span class="sxs-lookup"><span data-stu-id="23048-130">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="23048-131">A Azure adatvédelmi ügyfél manuális telepítése</span><span class="sxs-lookup"><span data-stu-id="23048-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="23048-132">Az AIP ügyfél manuális telepítése:</span><span class="sxs-lookup"><span data-stu-id="23048-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="23048-133">Letölt **AzinfoProtection_UL. exe** - [bólMikroszkóp Letölt Központ](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="23048-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="23048-134">Ellenőrizheti, hogy a telepítés működött-e, ha megtekinti a Word-dokumentumot, és meggyőződött arról, hogy az **érzékenység** lehetőség elérhető a **Kezdőlap** lapon.</span><span class="sxs-lookup"><span data-stu-id="23048-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="23048-135">![Védelem lap legördülő lista Word-dokumentumban.](media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="23048-135">![Protection tab drop-down in a Word document.](media/word-sensitivity.png)</span></span>

<span data-ttu-id="23048-136">További információt [az ügyfél telepítése](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="23048-136">For more information, see [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>

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
ms.openlocfilehash: 5213c55f4a8ce0e223896f1b960847714d6d06cb
ms.sourcegitcommit: 70e920f76526f47fc849df615de4569e0ac2f4be
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/07/2019
ms.locfileid: "38031415"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="5e753-103">Megfelelőségi funkciók beállítása</span><span class="sxs-lookup"><span data-stu-id="5e753-103">Set up compliance features</span></span>

<span data-ttu-id="5e753-104">A Microsoft 365 üzleti szolgáltatásai védik az adatokat és az eszközöket, és segítenek megőrizni az Ön és ügyfelei kényes információit.</span><span class="sxs-lookup"><span data-stu-id="5e753-104">Your Microsoft 365 Business comes with features to protect your data and devices, and help you keep yours and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="5e753-105">DLP-szolgáltatások beállítása</span><span class="sxs-lookup"><span data-stu-id="5e753-105">Set up DLP features</span></span>

<span data-ttu-id="5e753-106">Lásd a [DLP-házirend létrehozása sablonból](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) példát a személyes azonosításra alkalmas adatok (PII) elleni védelemre vonatkozó házirend beállításához.</span><span class="sxs-lookup"><span data-stu-id="5e753-106">See [Create a DLP policy from a template](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="5e753-107">A DLP sok különböző nyelvhez tartalmaz használatra kész házirendsablonokat.</span><span class="sxs-lookup"><span data-stu-id="5e753-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="5e753-108">Például, Ausztrália pénzügyi adatok, Kanada személyes adatok törvény, az Egyesült Államok pénzügyi adatok, stb. Tekintse meg, [milyen a DLP házirendsablonok](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) a teljes listához.</span><span class="sxs-lookup"><span data-stu-id="5e753-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, etc. See [What the DLP policy templates include](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for a full list.</span></span> <span data-ttu-id="5e753-109">Az összes ilyen sablon a PII példához hasonlóan engedélyezhető.</span><span class="sxs-lookup"><span data-stu-id="5e753-109">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="5e753-110">E-mail megőrzés beállítása az Exchange Online archiválással</span><span class="sxs-lookup"><span data-stu-id="5e753-110">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="5e753-111">Az **Exchange Online archiválási** licencfunkciói segítenek fenntartani a megfelelést és a szabályozó szabványokat az eDiscovery e-mail tartalmának megőrzésével.</span><span class="sxs-lookup"><span data-stu-id="5e753-111">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="5e753-112">Ez is segít csökkenteni a kockázatot a perben, és biztosítja a módját, hogy visszaszerez adat után a biztonság megsértése, vagy ha kell visszaállítani törölt elemeket.</span><span class="sxs-lookup"><span data-stu-id="5e753-112">It also helps reduce your risk in the event of a lawsuit and provides a way to recover data after a security breach, or when you need to recover deleted items.</span></span> <span data-ttu-id="5e753-113">Peres eljárás miatti tartás használatával megőrizheti az összes felhasználó tartalmát, vagy az adatmegőrzési szabályok segítségével testreszabhatja a megőrizni kívánt tartalmat.</span><span class="sxs-lookup"><span data-stu-id="5e753-113">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="5e753-114">**Peres eljárás miatti tartás:** Megőrizheti az összes postaláda tartalmát, beleértve a törölt elemeket is, ha a felhasználó teljes postaládáját peres eljárás miatti tartásba helyezzük.</span><span class="sxs-lookup"><span data-stu-id="5e753-114">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="5e753-115">Ha peres eljárás miatti tartásba szeretne helyezni egy postafiókot, az admin központban:</span><span class="sxs-lookup"><span data-stu-id="5e753-115">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="5e753-116">-Ban bal NAV, megy **használók** \> **aktivál használók**.</span><span class="sxs-lookup"><span data-stu-id="5e753-116">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="5e753-117">Válassza ki azt a felhasználót, akinek a postaládáját peres eljárás miatti tartásba szeretné helyezni, és a felhasználó ablaktáblában bontsa ki a **levelezési beállításokat** , majd a **További beállítások** mellett válassza az **Exchange-Tulajdonságok szerkesztése parancsot**.</span><span class="sxs-lookup"><span data-stu-id="5e753-117">Select a user whose mailbox you want to place on litigation hold and in the user pane expand **Mail settings** and next to **More settings** choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="5e753-118">A felhasználó postaládájának lapján válassza a bal oldali NAV \* \* postafiók jellemzőit, majd válassza a link **engedélyezése** **peres eljárás miatt tartás**alatt.</span><span class="sxs-lookup"><span data-stu-id="5e753-118">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="5e753-119">A peres **eljárások** tartása párbeszédablakban megadhatja a peres eljárás miatti tartás időtartamát a **peres tartás időtartama** mezőben, ha egy végtelen tartást kíván elhelyezni, hagyja üresen a mezőt.</span><span class="sxs-lookup"><span data-stu-id="5e753-119">In the **litigation hold** dialog box you can specify the litigation hold duration in the **Litigation hold duration** field, leave field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="5e753-120">Azt is hozzá megjegyzéseket, és közvetlenül a levéldoboz tulajdonos egy honlapot, lehet, hogy többet kell magyaráznia a peres eljárás \> tart **megment**.</span><span class="sxs-lookup"><span data-stu-id="5e753-120">You can also add notes and direct the mail box owner to a website you might have to explain more about the litigation hold \> **Save**.</span></span>
    
<span data-ttu-id="5e753-121">**Visszatartás:** Engedélyezheti a testreszabott adatmegőrzési szabályokat, például egy adott idő megtartása érdekében, vagy a megőrzési időszak végén véglegesen törölheti a tartalmat.</span><span class="sxs-lookup"><span data-stu-id="5e753-121">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="5e753-122">További információ [az adatmegőrzési szabályok áttekintése](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423)című témakörben található.</span><span class="sxs-lookup"><span data-stu-id="5e753-122">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="5e753-123">A érzékenységi címkék beállítása</span><span class="sxs-lookup"><span data-stu-id="5e753-123">Set up Sensitivity labels</span></span>

<span data-ttu-id="5e753-124">Érzékenység címkék jönnek Azure Information Protection (AIP) terv 1, és segít osztályozni, és tetszés szerint, védi a dokumentumok és e-maileket, alkalmazásával címkéket.</span><span class="sxs-lookup"><span data-stu-id="5e753-124">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify and optionally, protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="5e753-125">A címkék automatikusan alkalmazhatók, ha a rendszergazdák szabályokat és feltételeket határoznak meg, manuálisan, felhasználók szerint, vagy olyan kombinációban, ahol a felhasználók ajánlásokat kapnak.</span><span class="sxs-lookup"><span data-stu-id="5e753-125">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="5e753-126">Az érzékenységi címkék beállításához tekintse meg az [érzékenységi címkék létrehozását és kezelését](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) ismertető videót.</span><span class="sxs-lookup"><span data-stu-id="5e753-126">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="5e753-127">A Azure adatvédelmi ügyfél manuális telepítése</span><span class="sxs-lookup"><span data-stu-id="5e753-127">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="5e753-128">Az AIP ügyfél manuális telepítése:</span><span class="sxs-lookup"><span data-stu-id="5e753-128">To manually install the AIP client:</span></span>

1. <span data-ttu-id="5e753-129">Letölt **AzinfoProtection_UL. exe** - [bólMikroszkóp Letölt Központ](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="5e753-129">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="5e753-130">Ellenőrizheti, hogy a telepítés működött-e, ha megtekinti a Word-dokumentumot, és meggyőződött arról, hogy az **érzékenység** lehetőség elérhető a **Kezdőlap** lapon.</span><span class="sxs-lookup"><span data-stu-id="5e753-130">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="5e753-131">![Védelem lap legördülő lista Word-dokumentumban.](media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="5e753-131">![Protection tab drop-down in a Word document.](media/word-sensitivity.png)</span></span>

<span data-ttu-id="5e753-132">További információért [telepítse az ügyfélprogramot](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="5e753-132">For more information see, [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>

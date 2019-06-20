---
title: Fenyegetés növelhető a Microsoft 365 üzleti
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
search.appverid:
- BCS160
- MET150
description: Állítsa be az Office 365 speciális veszély védelmi, és a bizalmas adatok védelme.
ms.openlocfilehash: 53741a7726222bb32329a401953be72257df95cc
ms.sourcegitcommit: 7ac06563c6ff034358e8fd3f9298fc426187ade2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/31/2019
ms.locfileid: "35086342"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="65990-103">E szolgáltatások beállítása</span><span class="sxs-lookup"><span data-stu-id="65990-103">Set up compliance features</span></span>

<span data-ttu-id="65990-104">A Microsoft 365 üzleti adatok és berendezések védelmét, és folyamatosan, Ön és a felhasználók bizalmas adatok biztonságos szolgáltatásokat tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="65990-104">Your Microsoft 365 Business comes with features to protect your data and devices, and help you keep yours and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="65990-105">DLP szolgáltatások beállítása</span><span class="sxs-lookup"><span data-stu-id="65990-105">Set up DLP features</span></span>

<span data-ttu-id="65990-106">[Sablonból DLP házirend létrehozása](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) ellen személyhez köthető adatot Gyűjtenek a házirend beállításával kapcsolatos példát talál.</span><span class="sxs-lookup"><span data-stu-id="65990-106">See [Create a DLP policy from a template](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="65990-107">DLP számos kész használható sablonok számos különböző nyelvhez tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="65990-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="65990-108">Például a pénzügyi adatok Ausztrália, Kanada személyes információ törvény, amerikai pénzügyi adatok, stb. Teljes listájához lásd a [Mi a DLP sablonokat tartalmazza](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) .</span><span class="sxs-lookup"><span data-stu-id="65990-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, etc. See [What the DLP policy templates include](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for a full list.</span></span> <span data-ttu-id="65990-109">Az összes ezeket a sablonokat lehet engedélyezni a Gyűjtenek sablon példára hasonlít.</span><span class="sxs-lookup"><span data-stu-id="65990-109">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="65990-110">E-mail adatmegőrzési az Exchange Online archiválás beállítása</span><span class="sxs-lookup"><span data-stu-id="65990-110">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="65990-111">**Exchange Online archiválás** licencéhez tartozó szolgáltatások fenntartása érdekében megfelelőségi és szabályozási előírások által e-mail megőrzésére szánt elektronikus adatok feltárása.</span><span class="sxs-lookup"><span data-stu-id="65990-111">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="65990-112">Is csökkenthető a kockázat esetén peres és biztosítja az adatbiztonság megsértése után, vagy ha a törölt elemek kell helyreállítani az adatokat.</span><span class="sxs-lookup"><span data-stu-id="65990-112">It also helps reduce your risk in the event of a lawsuit and provides a way to recover data after a security breach, or when you need to recover deleted items.</span></span> <span data-ttu-id="65990-113">Per tartsa használja az összes felhasználói tartalom megőrzése érdekében, vagy testre szeretné megőrizni az adatmegőrzési szabályok segítségével.</span><span class="sxs-lookup"><span data-stu-id="65990-113">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="65990-114">**Per tartás:** Minden postaláda-tartalom helyezi a felhasználó teljes postaláda peres eljárás beleértve törölt elemek tárolására képes megőrizni.</span><span class="sxs-lookup"><span data-stu-id="65990-114">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="65990-115">Helyezze egy postaláda peres eljárás felfüggesztése a felügyeleti központ:</span><span class="sxs-lookup"><span data-stu-id="65990-115">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="65990-116">A bal oldali navigációs sáv, keresse meg **a felhasználók** \> **aktív felhasználók**.</span><span class="sxs-lookup"><span data-stu-id="65990-116">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="65990-117">Jelöljön ki egy felhasználót, akinek el szeretné helyezni a per postaláda tartsa és a felhasználó ablaktáblában bontsa ki a **levelezési beállításokat** , és **További beállítások** mellett válassza a **Tulajdonságok szerkesztése Exchange**.</span><span class="sxs-lookup"><span data-stu-id="65990-117">Select a user whose mailbox you want to place on litigation hold and in the user pane expand **Mail settings** and next to **More settings** choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="65990-118">A felhasználó postaláda lapon válassza ki \*\* postaláda szolgáltatások \*\* kattintson a bal oldali navigációs sáv, és válassza ki a **per tartsa** **engedélyezése** hivatkozásra.</span><span class="sxs-lookup"><span data-stu-id="65990-118">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="65990-119">**Per tartsa** párbeszédpanelen megadhatja, hogy a per tartás időtartama a **per tartás időtartama** mezőben, a mezőt hagyja üresen, ha el szeretné helyezni egy végtelen tartsa.</span><span class="sxs-lookup"><span data-stu-id="65990-119">In the **litigation hold** dialog box you can specify the litigation hold duration in the **Litigation hold duration** field, leave field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="65990-120">Is megjegyzéseket és közvetlen mail lista tulajdonosa egy webhelyre, előfordulhat, hogy tartsa a per bővebben magyarázatot kell \> **mentése**.</span><span class="sxs-lookup"><span data-stu-id="65990-120">You can also add notes and direct the mail box owner to a website you might have to explain more about the litigation hold \> **Save**.</span></span>
    
<span data-ttu-id="65990-121">**Retenciós:** Egyéni adatmegőrzési szabályok, például engedélyezheti egy adott meghatározott ideig megőrizni és tartalom véglegesen törli a birtokon tartási időszak végén.</span><span class="sxs-lookup"><span data-stu-id="65990-121">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="65990-122">További [adatmegőrzési szabályok – áttekintés](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="65990-122">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>

## <a name="set-up-azure-information-protection-features"></a><span data-ttu-id="65990-123">Információvédelem Azure szolgáltatások beállítása</span><span class="sxs-lookup"><span data-stu-id="65990-123">Set up Azure Information Protection features</span></span>

<span data-ttu-id="65990-124">Borzas információk védelme (AIP) segít osztályozására és a dokumentumok és e-mailek, esetleg védelme címkék alkalmazásával.</span><span class="sxs-lookup"><span data-stu-id="65990-124">Azure Information Protection (AIP) helps you classify and optionally, protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="65990-125">Címkék automatikusan alkalmazhatók, a rendszergazdák, akik a szabályokat és feltételeket határozza meg, kézzel felhasználók, vagy együttesének felhasználásával, ahol a felhasználók kapnak ajánlásokat.</span><span class="sxs-lookup"><span data-stu-id="65990-125">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="65990-126">Az Outlook programban a weben alkalmazhatja az e-mailek a következő beépített feliratok és korlátozások:</span><span class="sxs-lookup"><span data-stu-id="65990-126">In Outlook on the web you can apply the following built-in labels and restrictions to your emails:</span></span>
  
- <span data-ttu-id="65990-127">**Nem továbbítandó**: címzettek is olvashassák az üzenetet, de nem továbbíthatják, nyomtatás, másolhatják a tartalmat</span><span class="sxs-lookup"><span data-stu-id="65990-127">**Do Not Forward**: Recipients can read the message, but they can't forward, print, or copy content</span></span>
    
- <span data-ttu-id="65990-128">**Titkosítás**: A teljes üzenet titkosítva van.</span><span class="sxs-lookup"><span data-stu-id="65990-128">**Encrypt**: The entire message is encrypted.</span></span> <span data-ttu-id="65990-129">Címzettek a titkosított tartalom elérése előtt meg kell erősítenie az identitásukat és titkosítása nem távolítható el.</span><span class="sxs-lookup"><span data-stu-id="65990-129">Recipients must confirm their identity before accessing encrypted content and can't remove encryption.</span></span>
    
- <span data-ttu-id="65990-130">**Bizalmas**: a szervezet alkalmazottainak teljes engedélyt ad az e-mail tartalom és mellékletek, de nem a szervezeten kívülieknek.</span><span class="sxs-lookup"><span data-stu-id="65990-130">**Confidential**: Gives the employees in your organization full permissions to the email content and attachments, but not to people outside your organization.</span></span> <span data-ttu-id="65990-131">Adatok tulajdonosai nyomon követheti és tartalmat bármikor visszavonhatja.</span><span class="sxs-lookup"><span data-stu-id="65990-131">Data owners can track and revoke content at any point.</span></span>
    
- <span data-ttu-id="65990-132">**Nagyon bizalmas**: Ez a korlátozás nagyon bizalmas adatok, amely lehetővé teszi az alkalmazottak megtekintése, szerkesztése, és válaszolni, de nem továbbítása, nyomtatása vagy másolja az adatokat lehet alkalmazni.</span><span class="sxs-lookup"><span data-stu-id="65990-132">**Highly Confidential**: This restriction can be applied to highly confidential data, allowing employees to view, edit, and reply, but not forward, print, or copy the data.</span></span> <span data-ttu-id="65990-133">Adatok tulajdonosai nyomon követheti és tartalmat bármikor visszavonhatja.</span><span class="sxs-lookup"><span data-stu-id="65990-133">Data owners can track and revoke content at any point.</span></span>

### <a name="make-sure-azure-information-protection-is-activated"></a><span data-ttu-id="65990-134">Ellenőrizze, hogy aktív Azure információk védelméről</span><span class="sxs-lookup"><span data-stu-id="65990-134">Make sure Azure Information Protection is activated</span></span>

<span data-ttu-id="65990-135">Ellenőrizze, hogy aktiválva van-e az AIP:</span><span class="sxs-lookup"><span data-stu-id="65990-135">To verify that AIP is activated :</span></span>

1. <span data-ttu-id="65990-136">[Borzas portal](https://portal.azure.com/)bejelentkezni.</span><span class="sxs-lookup"><span data-stu-id="65990-136">Sign into [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="65990-137">Jelölje be a **minden szolgáltatás** és típus *Azure információk védelméről* a **Keresés mezőbe**.</span><span class="sxs-lookup"><span data-stu-id="65990-137">Select **All services** and type in *Azure Information Protection* in the **Search Box**.</span></span>

3. <span data-ttu-id="65990-138">Után az eredmények megjelenítéséhez kattintson a következő teszi a kedvenc **Azure információk védelméről** és könnyen megjegyezhető kezdete.</span><span class="sxs-lookup"><span data-stu-id="65990-138">Once the results display, click the start next to **Azure Information Protection** to make it a favorite and easy to find later.</span></span>

4. <span data-ttu-id="65990-139">Válassza ki az **Azure információk védelméről** \> **védelem aktiválás** , és győződjön meg arról, hogy ez a beállítás, aktivált.</span><span class="sxs-lookup"><span data-stu-id="65990-139">Select **Azure Information Protection** \> **Protection activation** and make sure the status is set to activated.</span></span> 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a><span data-ttu-id="65990-140">Az információk védelméről Azure házirendet és az alapértelmezett címkék megjelenítése</span><span class="sxs-lookup"><span data-stu-id="65990-140">View the Azure Information Protection policy and default labels</span></span> 

<span data-ttu-id="65990-141">Megtekintése és módosítása, hogy a meglévő címkék:</span><span class="sxs-lookup"><span data-stu-id="65990-141">To view, and modify, the existing labels:</span></span>

1. <span data-ttu-id="65990-142">Válassza az Azure információvédelem irányítópult **osztályozások** \> **címkék**.</span><span class="sxs-lookup"><span data-stu-id="65990-142">On the Azure Information Protection dashboard, select **Classifications** \> **Labels**.</span></span> <br/><span data-ttu-id="65990-143">![Szabványos címkék Azure információ védelme.](media/AIPLabels.png)</span><span class="sxs-lookup"><span data-stu-id="65990-143">![Standard labels for Azure Information Protection.](media/AIPLabels.png)</span></span>

2. <span data-ttu-id="65990-144">Megadhatja, hogy minden címke beállításainak megtekintéséhez, megváltoztathatja a megjelenítési név, szín, stb.</span><span class="sxs-lookup"><span data-stu-id="65990-144">You can choose any label to view options, you can change the display name, colors, etc.</span></span>
 
3. <span data-ttu-id="65990-145">Lásd: [Módosítás, és hozzon létre új címkéket](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) Ha szeretne létrehozni a saját.</span><span class="sxs-lookup"><span data-stu-id="65990-145">See  [Modify and create new labels](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) if you want to create your own.</span></span> 

### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="65990-146">Az információk védelméről Azure ügyfél telepítése manuálisan</span><span class="sxs-lookup"><span data-stu-id="65990-146">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="65990-147">Az AIP ügyfél manuális telepítéséhez:</span><span class="sxs-lookup"><span data-stu-id="65990-147">To manually install the AIP client:</span></span>

1. <span data-ttu-id="65990-148">**AzInfoProtection.exe** letölthető [a Microsoft letöltőközpontból](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="65990-148">Download **AzInfoProtection.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="65990-149">Ellenőrizheti, hogy a telepítés egy Word dokumentum megtekintése, és ügyelve arra, hogy a **védelem** beállítás érhető el a **Kezdőlap** lap dolgozott.</span><span class="sxs-lookup"><span data-stu-id="65990-149">You can verify that the installation worked by viewing a Word document and making sure that the **Protect** option is available on the **Home** tab.</span></span> <br/><span data-ttu-id="65990-150">![Védelem lapon legördülő Word dokumentumban.](media/Word_Protect.png)</span><span class="sxs-lookup"><span data-stu-id="65990-150">![Protection tab drop-down in a Word document.](media/Word_Protect.png)</span></span>

<span data-ttu-id="65990-151">További tájékoztatás, [az ügyfél telepítése](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="65990-151">For more information see, [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>

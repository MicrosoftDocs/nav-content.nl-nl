---
title: Een boeking ongedaan maken door een tegenboeking te boeken
description: Als u een foutieve boeking in het dagboek hebt gemaakt, kunt u vervolgens de functie Transactie tegenboeken gebruiken om de boeking ongedaan te maken met de juiste audittrail.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reimbursement
ms.date: 08/03/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 2970914c36f892a5610509e9dc4015d0fb159642
ms.contentlocale: nl-nl
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-reverse-postings"></a><span data-ttu-id="19a27-103">Procedure: boekingen tegenboeken</span><span class="sxs-lookup"><span data-stu-id="19a27-103">How to: Reverse Postings</span></span>
<span data-ttu-id="19a27-104">Om een foutieve dagboekpost ongedaan te maken, selecteert en maakt u een tegenboeking (posten die identiek zijn aan de oorspronkelijke post, maar met een tegenovergesteld teken in het bedragveld) met hetzelfde documentnummer en dezelfde boekingsdatum als de originele post.</span><span class="sxs-lookup"><span data-stu-id="19a27-104">To undo an erroneous journal posting, you select the entry and create a reverse entry (entries identical to the original entry but with opposite sign in the amount field) with the same document number and posting date as the original entry.</span></span> <span data-ttu-id="19a27-105">Nadat een post is tegengeboekt, moet u de juiste post maken.</span><span class="sxs-lookup"><span data-stu-id="19a27-105">After reversing an entry, you must make the correct entry.</span></span>

<span data-ttu-id="19a27-106">U kunt alleen posten tegenboeken die zijn geboekt vanaf een algemene dagboekregel.</span><span class="sxs-lookup"><span data-stu-id="19a27-106">You can only reverse entries that are posted from a general journal line.</span></span> <span data-ttu-id="19a27-107">Een post kan slechts één keer worden tegengeboekt.</span><span class="sxs-lookup"><span data-stu-id="19a27-107">An entry can only be reversed once.</span></span>

<span data-ttu-id="19a27-108">Voor meer informatie over het boeken vanuit een dagboek zie [Procedure: Transacties direct naar het grootboek boeken](finance-how-post-transactions-directly.md)</span><span class="sxs-lookup"><span data-stu-id="19a27-108">For more information about posting from a general journal, see [How to: Post Transactions Directly to the General Ledger](finance-how-post-transactions-directly.md).</span></span>

<span data-ttu-id="19a27-109">Als u een onjuist negatief aantal hebt geboekt, dat wil zeggen, als u een inkooporder hebt gemaakt met bijvoorbeeld het verkeerde aantal artikelen en deze order hebt geboekt als ontvangen (maar niet gefactureerd), kunt u de boeking ongedaan maken.</span><span class="sxs-lookup"><span data-stu-id="19a27-109">If you have made an incorrect negative quantity posting, such as a purchase order with the wrong number of items and posted it as received but not invoiced, then you can undo the posting.</span></span>

<span data-ttu-id="19a27-110">Als u een onjuist positief aantal hebt geboekt, dat wil zeggen, als u een inkoopretourorder hebt gemaakt met bijvoorbeeld het verkeerde aantal artikelen en deze order hebt geboekt als verzonden (maar niet gefactureerd), kunt u de boeking ongedaan maken.</span><span class="sxs-lookup"><span data-stu-id="19a27-110">If you have made an incorrect positive quantity posting, such as a purchase return order with the wrong number of items and posted it as shipped but not invoiced, then you can undo the posting.</span></span>   

## <a name="to-reverse-the-journal-posting-of-a-general-ledger-entry"></a><span data-ttu-id="19a27-111">De dagboekboeking van een grootboekpost tegenboeken</span><span class="sxs-lookup"><span data-stu-id="19a27-111">To reverse the journal posting of a general ledger entry</span></span>
<span data-ttu-id="19a27-112">U kunt posten vanuit alle **Posten**-vensters tegenboeken.</span><span class="sxs-lookup"><span data-stu-id="19a27-112">You can reverse entries from all **Ledger Entries** windows.</span></span> <span data-ttu-id="19a27-113">De volgende procedure is gebaseerd op het venster **Grootboekposten**.</span><span class="sxs-lookup"><span data-stu-id="19a27-113">The following procedure is based on the **General Ledger Entries** window.</span></span>
1. <span data-ttu-id="19a27-114">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Grootboekposten** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="19a27-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Entries**, and then choose the related link.</span></span>
2. <span data-ttu-id="19a27-115">Selecteer de post die u wilt tegenboeken en kies vervolgens de actie **Transactie tegenboeken**.</span><span class="sxs-lookup"><span data-stu-id="19a27-115">Select the entry that you want to reverse, and then choose the **Reverse Transaction** action.</span></span> <span data-ttu-id="19a27-116">Het moet afkomstig zijn uit een dagboekboeking.</span><span class="sxs-lookup"><span data-stu-id="19a27-116">Note that is must originate from a journal posting.</span></span>
3. <span data-ttu-id="19a27-117">Selecteer in het venster **Transactieposten tegenboeken** de relevante post en kies de actie **Tegenboeken**.</span><span class="sxs-lookup"><span data-stu-id="19a27-117">In the **Reverse Transaction Entries** window, select the relevant entry, and then choose the **Reverse** action.</span></span>
4. <span data-ttu-id="19a27-118">Kies de knop **Ja** in het bevestigingsbericht.</span><span class="sxs-lookup"><span data-stu-id="19a27-118">Choose the **Yes** button on the confirmation message.</span></span>

## <a name="to-undo-a-quantity-posting-on-a-posted-purchase-receipt"></a><span data-ttu-id="19a27-119">Een aantalsboeking ongedaan maken op een geboekte inkoopontvangst</span><span class="sxs-lookup"><span data-stu-id="19a27-119">To undo a quantity posting on a posted purchase receipt</span></span>  

1.  <span data-ttu-id="19a27-120">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Geboekte inkoopontvangsten** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="19a27-120">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Purchase Receipts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="19a27-121">Open de geboekte ontvangst die u ongedaan wilt maken.</span><span class="sxs-lookup"><span data-stu-id="19a27-121">Open the posted receipt that you want to undo.</span></span>  
3.  <span data-ttu-id="19a27-122">Selecteer de regel(s) die u ongedaan wilt maken.</span><span class="sxs-lookup"><span data-stu-id="19a27-122">Select the line or lines that you want to undo.</span></span>  
4.  <span data-ttu-id="19a27-123">Kies de actie **Ontvangst ongedaan maken**.</span><span class="sxs-lookup"><span data-stu-id="19a27-123">Choose **Undo Receipt** action.</span></span>

    <span data-ttu-id="19a27-124">Er wordt een correctieregel ingevoegd onder de geselecteerde ontvangstregel.</span><span class="sxs-lookup"><span data-stu-id="19a27-124">A corrective line is inserted under the selected receipt line.</span></span>  

    <span data-ttu-id="19a27-125">Als de hoeveelheid in een magazijnontvangst is ontvangen, wordt een correctieregel ingevoegd in de geboekte magazijnontvangst.</span><span class="sxs-lookup"><span data-stu-id="19a27-125">If the quantity was received in a warehouse receipt, then a corrective line is inserted in the posted warehouse receipt.</span></span>  

    <span data-ttu-id="19a27-126">De velden **Ontvangen aantal** en **Niet geboekt aantal** op de bijbehorende inkooporder worden ingesteld op nul.</span><span class="sxs-lookup"><span data-stu-id="19a27-126">The **Quantity Received** and **Qty. Rcd. Not Invoiced** fields on the related purchase order are set to zero.</span></span>

## <a name="to-undo-and-then-redo-a-quantity-posting-on-a-posted-return-shipment"></a><span data-ttu-id="19a27-127">Een aantalboeking ongedaan maken en opnieuw uitvoeren voor een geboekte retourzending</span><span class="sxs-lookup"><span data-stu-id="19a27-127">To undo and then redo a quantity posting on a posted return shipment</span></span>

1.  <span data-ttu-id="19a27-128">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Geboekte inkoopontvangsten** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="19a27-128">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Return Shipments**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="19a27-129">Open de geboekte retourzending die u ongedaan wilt maken.</span><span class="sxs-lookup"><span data-stu-id="19a27-129">Open the posted return shipment that you want to undo.</span></span>
3. <span data-ttu-id="19a27-130">Selecteer de regel(s) die u ongedaan wilt maken.</span><span class="sxs-lookup"><span data-stu-id="19a27-130">Select the line or lines you want to undo.</span></span>  

4.  <span data-ttu-id="19a27-131">Kies de actie **Retourverzending ongedaan maken**.</span><span class="sxs-lookup"><span data-stu-id="19a27-131">Choose the **Undo Return Shipment** action.</span></span>  

    <span data-ttu-id="19a27-132">In het geboekte document wordt een gecorrigeerde regel ingevoegd. Op de retourorder worden de velden **Retouraantal verzonden** en **Retourverzending niet gefact.** ingesteld op nul.</span><span class="sxs-lookup"><span data-stu-id="19a27-132">A corrective line is inserted in the posted document, and the **Return Qty. Shipped** and **Return Shpd. Not Invd.** fields on the return order are set to zero.</span></span>  

    <span data-ttu-id="19a27-133">Ga nu terug naar de inkoopretourorder om opnieuw te boeken.</span><span class="sxs-lookup"><span data-stu-id="19a27-133">Now go back to the purchase return order to redo the posting.</span></span>  

5.  <span data-ttu-id="19a27-134">Let in het venster **Geboekte retourverzending** op het nummer in het **Retourordernr.**</span><span class="sxs-lookup"><span data-stu-id="19a27-134">In the **Posted Return Shipment** window, take a note of the number in the **Return Order No.**</span></span> <span data-ttu-id="19a27-135">veld.</span><span class="sxs-lookup"><span data-stu-id="19a27-135">field.</span></span>  
6.  <span data-ttu-id="19a27-136">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Inkoopretourorders** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="19a27-136">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Return Orders**, and then choose the related link.</span></span>  
7.  <span data-ttu-id="19a27-137">Open de retourorder en kies de actie **Opnieuw openen**.</span><span class="sxs-lookup"><span data-stu-id="19a27-137">Open the return order in question, and then choose the **Reopen** action.</span></span>  
8.  <span data-ttu-id="19a27-138">Corrigeer de post in het veld **Aantal** en boek de inkoopretourorder opnieuw.</span><span class="sxs-lookup"><span data-stu-id="19a27-138">Correct the entry in the **Quantity** field and post the purchase return order again.</span></span>  

## <a name="see-also"></a><span data-ttu-id="19a27-139">Zie ook</span><span class="sxs-lookup"><span data-stu-id="19a27-139">See Also</span></span>
[<span data-ttu-id="19a27-140">Procedure: Transacties direct naar het grootboek boeken</span><span class="sxs-lookup"><span data-stu-id="19a27-140">How to: Post Transactions Directly to the General Ledger</span></span>](finance-how-post-transactions-directly.md)  
[<span data-ttu-id="19a27-141">Werken met diversendagboeken</span><span class="sxs-lookup"><span data-stu-id="19a27-141">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="19a27-142">Financiën</span><span class="sxs-lookup"><span data-stu-id="19a27-142">Finance</span></span>](finance.md)  
<span data-ttu-id="19a27-143">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="19a27-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  


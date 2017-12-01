---
title: Ontvangsten combineren
description: "Als u meer dan één inkoopontvangst tegelijk wilt factureren, kunt u de functie Ontvangsten combineren gebruiken."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/14/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 2e8b2491759ea955104e308eca2750b28e9e466c
ms.contentlocale: nl-nl
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-combine-receipts-on-a-single-invoice"></a><span data-ttu-id="6b776-103">Procedure: Ontvangsten combineren op één factuur</span><span class="sxs-lookup"><span data-stu-id="6b776-103">How to: Combine Receipts on a Single Invoice</span></span>
<span data-ttu-id="6b776-104">Als u meer dan één inkoopontvangst tegelijk wilt factureren, kunt u de functie **Ontvangsten combineren** gebruiken.</span><span class="sxs-lookup"><span data-stu-id="6b776-104">If you want to invoice more than one purchase receipt at a time, you can use the **Combine Receipts** function.</span></span>  

<span data-ttu-id="6b776-105">Een gecombineerde inkoopontvangst kan pas worden gemaakt wanneer meer inkoopontvangsten van dezelfde leverancier in dezelfde valuta zijn geboekt.</span><span class="sxs-lookup"><span data-stu-id="6b776-105">Before you can create a combined purchase receipt, more than one receipt from the same vendor in the same currency must be posted.</span></span> <span data-ttu-id="6b776-106">U moet dus twee of meer inkooporders hebben ingevuld en deze hebben geboekt als ontvangen, maar niet als gefactureerd.</span><span class="sxs-lookup"><span data-stu-id="6b776-106">In other words, you must have filled in two or more purchase orders and posted them as received, but not invoiced.</span></span>  

<span data-ttu-id="6b776-107">Wanneer inkoopontvangsten zijn gecombineerd op een factuur en zijn geboekt, wordt een geboekte inkoopfactuur gemaakt voor de gefactureerde regels.</span><span class="sxs-lookup"><span data-stu-id="6b776-107">When purchase receipts are combined on an invoice and posted, then a posted purchase invoice is created for the invoiced lines.</span></span> <span data-ttu-id="6b776-108">Het veld **Gefactureerd aantal** op de oorspronkelijke inkooporder of het oorspronkelijke inkoopraamcontract wordt bijgewerkt op basis van het gefactureerde aantal.</span><span class="sxs-lookup"><span data-stu-id="6b776-108">The **Quantity Invoiced** field on the originating purchase order, or blanket purchase order, is updated based on the invoiced quantity.</span></span> <span data-ttu-id="6b776-109">Dit oorspronkelijke inkoopdocument wordt echter niet verwijderd, zelfs als dit volledig is ontvangen en gefactureerd en daarom moet u het inkoopdocument zelf verwijderen.</span><span class="sxs-lookup"><span data-stu-id="6b776-109">However, this original purchase document is not deleted, even if it has been fully received and invoiced, and you must therefore delete the purchase document.</span></span>  

## <a name="to-combine-receipts"></a><span data-ttu-id="6b776-110">Ontvangsten combineren</span><span class="sxs-lookup"><span data-stu-id="6b776-110">To combine receipts</span></span>  
1. <span data-ttu-id="6b776-111">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Inkoopfacturen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="6b776-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="6b776-112">Kies de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="6b776-112">Choose the **New** action.</span></span> <span data-ttu-id="6b776-113">Zie voor meer informatie [Procedure: Inkopen vastleggen](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="6b776-113">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>  
3. <span data-ttu-id="6b776-114">Op het sneltabblad **Regels** selecteert u de actie **Ontvangstregels ophalen**.</span><span class="sxs-lookup"><span data-stu-id="6b776-114">On the **Lines** FastTab, choose the **Get Receipt Lines** action.</span></span>  
4. <span data-ttu-id="6b776-115">Selecteer meerdere ontvangstregels die u wilt opnemen in de factuur.</span><span class="sxs-lookup"><span data-stu-id="6b776-115">Select multiple receipt lines that you want to include in the invoice.</span></span>  

    <span data-ttu-id="6b776-116">Als een onjuiste ontvangstregel is geselecteerd of als u opnieuw wilt beginnen, kunt u de regels op de inkoopfactuur gewoon verwijderen en vervolgens de functie **Ontvangstregels ophalen** opnieuw gebruiken.</span><span class="sxs-lookup"><span data-stu-id="6b776-116">If an incorrect receipt line was selected or you want to start over, you can just delete the lines on the purchase invoice and then use the **Get Receipt Lines** function again.</span></span>  
5. <span data-ttu-id="6b776-117">Kies de actie **Boeken** om de factuur te boeken.</span><span class="sxs-lookup"><span data-stu-id="6b776-117">To post the invoice, choose the **Post** action.</span></span>  

## <a name="to-remove-open-purchase-orders-after-combined-receipt-posting"></a><span data-ttu-id="6b776-118">Open inkooporders verwijderen na gecombineerde ontvangstboeking</span><span class="sxs-lookup"><span data-stu-id="6b776-118">To remove open purchase orders after combined receipt posting</span></span>  
1. <span data-ttu-id="6b776-119">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Gefact. inkooporders verwijderen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="6b776-119">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delete Invoiced Purchase Orders**, and select the related link.</span></span>  
2. <span data-ttu-id="6b776-120">Vul indien nodig de velden in.</span><span class="sxs-lookup"><span data-stu-id="6b776-120">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]<span data-ttu-id="6b776-121">.</span><span class="sxs-lookup"><span data-stu-id="6b776-121">.</span></span>
3. <span data-ttu-id="6b776-122">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="6b776-122">Choose the **OK** button.</span></span>  

<span data-ttu-id="6b776-123">U kunt de afzonderlijke orders ook handmatig verwijderen.</span><span class="sxs-lookup"><span data-stu-id="6b776-123">Alternatively, delete the individual orders manually.</span></span>

<span data-ttu-id="6b776-124">Herhaal stap 1 t/m 3 voor alle andere betrokken documenten, zoals inkoopraamcontracten.</span><span class="sxs-lookup"><span data-stu-id="6b776-124">Repeat steps 1 through 3 for any other affected documents, such as blanket purchase orders.</span></span>

## <a name="see-also"></a><span data-ttu-id="6b776-125">Zie ook</span><span class="sxs-lookup"><span data-stu-id="6b776-125">See Also</span></span>  
[<span data-ttu-id="6b776-126">Inkoop</span><span class="sxs-lookup"><span data-stu-id="6b776-126">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="6b776-127">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="6b776-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>


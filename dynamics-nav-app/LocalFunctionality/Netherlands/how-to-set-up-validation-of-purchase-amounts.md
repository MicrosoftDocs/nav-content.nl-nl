---
title: Validatie van inkoopbedragen instellen
description: In [!INCLUDE[navnow](../../includes/navnow_md.md)] kunt u de functie **Totaalbedragen documenten controleren** activeren om het totaalbedrag van inkoopdocumenten te valideren voordat een inkoopfactuur en inkoopcreditnota worden geboekt.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 8f6913388f963cc0852d9f3f6b6090f449a52082
ms.contentlocale: nl-nl
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-set-up-validation-of-purchase-amounts"></a><span data-ttu-id="95f20-103">Procedure: Validatie van inkoopbedragen instellen</span><span class="sxs-lookup"><span data-stu-id="95f20-103">How to: Set Up Validation of Purchase Amounts</span></span>
<span data-ttu-id="95f20-104">In [!INCLUDE[navnow](../../includes/navnow_md.md)] kunt u de functie **Totaalbedragen documenten controleren** activeren om het totaalbedrag van inkoopdocumenten te valideren voordat een inkoopfactuur en inkoopcreditnota worden geboekt.</span><span class="sxs-lookup"><span data-stu-id="95f20-104">In [!INCLUDE[navnow](../../includes/navnow_md.md)], you can activate the **Check Doc. Total Amounts** function to validate the total amount of purchase documents before posting a purchase invoice and purchase credit memo.</span></span> <span data-ttu-id="95f20-105">Standaard wordt het totale inkoopdocumentbedrag gevalideerd wanneer u boekt.</span><span class="sxs-lookup"><span data-stu-id="95f20-105">By default, the purchase document total amount is validated when you post.</span></span> <span data-ttu-id="95f20-106">Het totale bedrag van de ingevoegde inkoopregels moet gelijk zijn aan het bedrag inclusief btw en het btw-bedrag.</span><span class="sxs-lookup"><span data-stu-id="95f20-106">The total amount of the inserted purchase lines must be equal to the amount including VAT and the VAT amount.</span></span> <span data-ttu-id="95f20-107">Als u het inkoopdocumentbedrag automatisch wilt valideren, moet u het documentbedrag inclusief btw en de btw van het documentbedrag in het venster **Inkoopfactuur** of **Inkoopcreditnota** invoeren.</span><span class="sxs-lookup"><span data-stu-id="95f20-107">To validate the purchase document amount automatically, you must enter the document amount including VAT and the document amount VAT on the **Purchase Invoice** or **Purchase Credit Memo** window.</span></span>  

<span data-ttu-id="95f20-108">Als u slechts één inkoopregel of meer verkoopregels met hetzelfde btw-percentage hebt, wordt de juiste documentbedrag-btw automatisch berekend wanneer u de inkoopregels en het documentbedrag inclusief btw invoegt.</span><span class="sxs-lookup"><span data-stu-id="95f20-108">If you have only one purchase line or several purchase lines with the same VAT percentage, the correct document amount VAT is calculated automatically when you insert the purchase lines and the document amount including VAT.</span></span> <span data-ttu-id="95f20-109">Als u verschillende inkoopregels met verschillende btw-percentages hebt, moet de waarde van de documentbedrag-btw handmatig worden gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="95f20-109">If you have several purchase lines with different VAT percentages, the document amount VAT value must be changed manually.</span></span>  

<span data-ttu-id="95f20-110">U kunt ook bepalen wanneer de documenttotaalbedragen en de totaalbedragen van de ingevoegde inkoopregels verschillen.</span><span class="sxs-lookup"><span data-stu-id="95f20-110">You can also locate when the document total amounts and the total amounts of the inserted purchase lines are different.</span></span> <span data-ttu-id="95f20-111">U kunt de optie **Totale op inkoopfactuur/CR-nota weergeven**</span><span class="sxs-lookup"><span data-stu-id="95f20-111">You can activate the **Show Totals on Purch. Inv./CM.**</span></span> <span data-ttu-id="95f20-112">activeren om het volgende weer te geven in de ingevoegde inkoopregels:</span><span class="sxs-lookup"><span data-stu-id="95f20-112">option to view the following in the inserted purchase lines:</span></span>  

- <span data-ttu-id="95f20-113">Totaalbedrag</span><span class="sxs-lookup"><span data-stu-id="95f20-113">Total amount</span></span>  
- <span data-ttu-id="95f20-114">Totaalbasisbedrag</span><span class="sxs-lookup"><span data-stu-id="95f20-114">Total base amount</span></span>  
- <span data-ttu-id="95f20-115">Totaal btw-bedrag</span><span class="sxs-lookup"><span data-stu-id="95f20-115">Total VAT amount</span></span>  
- <span data-ttu-id="95f20-116">Totaalbedrag incl. btw</span><span class="sxs-lookup"><span data-stu-id="95f20-116">Total amount including VAT</span></span>  

<span data-ttu-id="95f20-117">De berekende bedragen worden weergegeven in de inkoopfactuur of de inkoopcreditnota.</span><span class="sxs-lookup"><span data-stu-id="95f20-117">The calculated amounts are displayed in the purchase invoice or purchase credit memo.</span></span> <span data-ttu-id="95f20-118">Standaard wordt dit totaalbedrag niet weergegeven.</span><span class="sxs-lookup"><span data-stu-id="95f20-118">By default, this total amount is not displayed.</span></span>  

<span data-ttu-id="95f20-119">U kunt deze optie alleen inschakelen als de inkoopfactuur of de inkoopcreditnota het volgende heeft:</span><span class="sxs-lookup"><span data-stu-id="95f20-119">You can activate this option only if the purchase invoice or purchase credit memo has:</span></span>  

- <span data-ttu-id="95f20-120">Een minimum van één inkoopregel.</span><span class="sxs-lookup"><span data-stu-id="95f20-120">A minimum of one purchase line.</span></span>  
- <span data-ttu-id="95f20-121">Het aantalveld opgegeven.</span><span class="sxs-lookup"><span data-stu-id="95f20-121">The quantity field specified.</span></span>  

## <a name="to-set-up-validation-of-total-amounts-for-purchase-documents"></a><span data-ttu-id="95f20-122">Validatie van totaalbedragen voor inkoopdocumenten instellen</span><span class="sxs-lookup"><span data-stu-id="95f20-122">To set up validation of total amounts for purchase documents</span></span>  

1.  <span data-ttu-id="95f20-123">Klik op het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Inkoopinstellingen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="95f20-123">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="95f20-124">Vul in het sneltabblad **Algemeen** de velden in, zoals in de volgende tabel is beschreven.</span><span class="sxs-lookup"><span data-stu-id="95f20-124">On the **General** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="95f20-125">Veld</span><span class="sxs-lookup"><span data-stu-id="95f20-125">Field</span></span>|<span data-ttu-id="95f20-126">Description</span><span class="sxs-lookup"><span data-stu-id="95f20-126">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="95f20-127">**Totale op inkoopfactuur/CR-nota weergeven.**</span><span class="sxs-lookup"><span data-stu-id="95f20-127">**Show Totals on Purch. Inv./CM.**</span></span>|<span data-ttu-id="95f20-128">Selecteren om de totalen opnieuw te berekenen van alle inkoopfacturen en creditnota's.</span><span class="sxs-lookup"><span data-stu-id="95f20-128">Select to recalculate the totals on all purchase invoices and credit memos.</span></span> <span data-ttu-id="95f20-129">Dit kan een tijdrovend proces zijn, afhankelijk van het aantal documenten dat moet worden herberekend.</span><span class="sxs-lookup"><span data-stu-id="95f20-129">This can take more time depending on the number of documents that must be recalculated.</span></span>|  
    |<span data-ttu-id="95f20-130">**Totaalbedragen documenten controleren**</span><span class="sxs-lookup"><span data-stu-id="95f20-130">**Check Doc. Total Amounts**</span></span>|<span data-ttu-id="95f20-131">Selecteren om de velden **Documentbedrag incl. btw** en **Btw documentbedrag** in de vensters **Inkoopfactuur** en **Inkoopcreditnota** te wijzigen.</span><span class="sxs-lookup"><span data-stu-id="95f20-131">Select to modify the **Doc. Amount Incl. VAT** and **Doc. Amount VAT** fields on the **Purchase Invoice** and **Purchase Credit Memo** windows.</span></span>|  

3.  <span data-ttu-id="95f20-132">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="95f20-132">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="95f20-133">Zie ook</span><span class="sxs-lookup"><span data-stu-id="95f20-133">See Also</span></span>  
[<span data-ttu-id="95f20-134">Nederlandse lokale functionaliteit</span><span class="sxs-lookup"><span data-stu-id="95f20-134">Netherlands Local Functionality</span></span>](netherlands-local-functionality.md)  
[<span data-ttu-id="95f20-135">Inkopen instellen</span><span class="sxs-lookup"><span data-stu-id="95f20-135">Setting Up Purchases</span></span>](../../sales-how-work-standard-lines.md)


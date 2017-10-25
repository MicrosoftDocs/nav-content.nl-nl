---
title: Validatie van inkoopbedragen instellen
description: In [!INCLUDE[navnow](../../includes/navnow_md.md)] kunt u de functie **Totaalbedragen documenten controleren** activeren om het totaalbedrag van inkoopdocumenten te valideren voordat een inkoopfactuur en inkoopcreditnota worden geboekt. Standaard wordt het totale inkoopdocumentbedrag gevalideerd wanneer u boekt. Het totale bedrag van de ingevoegde inkoopregels moet gelijk zijn aan het bedrag inclusief btw en het btw-bedrag. Als u het inkoopdocumentbedrag automatisch wilt valideren, moet u het documentbedrag inclusief btw en de btw van het documentbedrag in het venster **Inkoopfactuur** of **Inkoopcreditnota** invoeren.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: f8fc638a07e65313a2778779128e4e580404a180
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-validation-of-purchase-amounts"></a><span data-ttu-id="3bef0-106">Procedure: Validatie van inkoopbedragen instellen</span><span class="sxs-lookup"><span data-stu-id="3bef0-106">How to: Set Up Validation of Purchase Amounts</span></span>
<span data-ttu-id="3bef0-107">In [!INCLUDE[navnow](../../includes/navnow_md.md)] kunt u de functie **Totaalbedragen documenten controleren** activeren om het totaalbedrag van inkoopdocumenten te valideren voordat een inkoopfactuur en inkoopcreditnota worden geboekt.</span><span class="sxs-lookup"><span data-stu-id="3bef0-107">In [!INCLUDE[navnow](../../includes/navnow_md.md)], you can activate the **Check Doc. Total Amounts** function to validate the total amount of purchase documents before posting a purchase invoice and purchase credit memo.</span></span> <span data-ttu-id="3bef0-108">Standaard wordt het totale inkoopdocumentbedrag gevalideerd wanneer u boekt.</span><span class="sxs-lookup"><span data-stu-id="3bef0-108">By default, the purchase document total amount is validated when you post.</span></span> <span data-ttu-id="3bef0-109">Het totale bedrag van de ingevoegde inkoopregels moet gelijk zijn aan het bedrag inclusief btw en het btw-bedrag.</span><span class="sxs-lookup"><span data-stu-id="3bef0-109">The total amount of the inserted purchase lines must be equal to the amount including VAT and the VAT amount.</span></span> <span data-ttu-id="3bef0-110">Als u het inkoopdocumentbedrag automatisch wilt valideren, moet u het documentbedrag inclusief btw en de btw van het documentbedrag in het venster **Inkoopfactuur** of **Inkoopcreditnota** invoeren.</span><span class="sxs-lookup"><span data-stu-id="3bef0-110">To validate the purchase document amount automatically, you must enter the document amount including VAT and the document amount VAT on the **Purchase Invoice** or **Purchase Credit Memo** window.</span></span>  
  
 <span data-ttu-id="3bef0-111">Als u slechts één inkoopregel of meer verkoopregels met hetzelfde btw-percentage hebt, wordt de juiste documentbedrag-btw automatisch berekend wanneer u de inkoopregels en het documentbedrag inclusief btw invoegt.</span><span class="sxs-lookup"><span data-stu-id="3bef0-111">If you have only one purchase line or several purchase lines with the same VAT percentage, the correct document amount VAT is calculated automatically when you insert the purchase lines and the document amount including VAT.</span></span> <span data-ttu-id="3bef0-112">Als u verschillende inkoopregels met verschillende btw-percentages hebt, moet de waarde van de documentbedrag-btw handmatig worden gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="3bef0-112">If you have several purchase lines with different VAT percentages, the document amount VAT value must be changed manually.</span></span>  
  
 <span data-ttu-id="3bef0-113">U kunt ook bepalen wanneer de documenttotaalbedragen en de totaalbedragen van de ingevoegde inkoopregels verschillen.</span><span class="sxs-lookup"><span data-stu-id="3bef0-113">You can also locate when the document total amounts and the total amounts of the inserted purchase lines are different.</span></span> <span data-ttu-id="3bef0-114">U kunt de optie **Totale op inkoopfactuur/CR-nota weergeven**</span><span class="sxs-lookup"><span data-stu-id="3bef0-114">You can activate the **Show Totals on Purch. Inv./CM.**</span></span> <span data-ttu-id="3bef0-115">activeren om het volgende weer te geven in de ingevoegde inkoopregels:</span><span class="sxs-lookup"><span data-stu-id="3bef0-115">option to view the following in the inserted purchase lines:</span></span>  
  
-   <span data-ttu-id="3bef0-116">Totaalbedrag</span><span class="sxs-lookup"><span data-stu-id="3bef0-116">Total amount</span></span>  
  
-   <span data-ttu-id="3bef0-117">Totaalbasisbedrag</span><span class="sxs-lookup"><span data-stu-id="3bef0-117">Total base amount</span></span>  
  
-   <span data-ttu-id="3bef0-118">Totaal btw-bedrag</span><span class="sxs-lookup"><span data-stu-id="3bef0-118">Total VAT amount</span></span>  
  
-   <span data-ttu-id="3bef0-119">Totaalbedrag incl. btw</span><span class="sxs-lookup"><span data-stu-id="3bef0-119">Total amount including VAT</span></span>  
  
 <span data-ttu-id="3bef0-120">De berekende bedragen worden weergegeven in de inkoopfactuur of de inkoopcreditnota.</span><span class="sxs-lookup"><span data-stu-id="3bef0-120">The calculated amounts are displayed in the purchase invoice or purchase credit memo.</span></span> <span data-ttu-id="3bef0-121">Standaard wordt dit totaalbedrag niet weergegeven.</span><span class="sxs-lookup"><span data-stu-id="3bef0-121">By default, this total amount is not displayed.</span></span>  
  
 <span data-ttu-id="3bef0-122">U kunt deze optie alleen inschakelen als de inkoopfactuur of de inkoopcreditnota het volgende heeft:</span><span class="sxs-lookup"><span data-stu-id="3bef0-122">You can activate this option only if the purchase invoice or purchase credit memo has:</span></span>  
  
-   <span data-ttu-id="3bef0-123">Een minimum van één inkoopregel.</span><span class="sxs-lookup"><span data-stu-id="3bef0-123">A minimum of one purchase line.</span></span>  
  
-   <span data-ttu-id="3bef0-124">Het aantalveld opgegeven.</span><span class="sxs-lookup"><span data-stu-id="3bef0-124">The quantity field specified.</span></span>  
  
### <a name="to-set-up-validation-of-total-amounts-for-purchase-documents"></a><span data-ttu-id="3bef0-125">Validatie van totaalbedragen voor inkoopdocumenten instellen</span><span class="sxs-lookup"><span data-stu-id="3bef0-125">To set up validation of total amounts for purchase documents</span></span>  
  
1.  <span data-ttu-id="3bef0-126">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Inkoopinstellingen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="3bef0-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="3bef0-127">Vul in het sneltabblad **Algemeen** de velden in, zoals in de volgende tabel is beschreven.</span><span class="sxs-lookup"><span data-stu-id="3bef0-127">On the **General** FastTab, fill in the fields as described in the following table.</span></span>  
  
    |<span data-ttu-id="3bef0-128">Veld</span><span class="sxs-lookup"><span data-stu-id="3bef0-128">Field</span></span>|<span data-ttu-id="3bef0-129">Description</span><span class="sxs-lookup"><span data-stu-id="3bef0-129">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="3bef0-130">**Totale op inkoopfactuur/CR-nota weergeven.**</span><span class="sxs-lookup"><span data-stu-id="3bef0-130">**Show Totals on Purch. Inv./CM.**</span></span>|<span data-ttu-id="3bef0-131">Selecteren om de totalen opnieuw te berekenen van alle inkoopfacturen en creditnota's.</span><span class="sxs-lookup"><span data-stu-id="3bef0-131">Select to recalculate the totals on all purchase invoices and credit memos.</span></span> <span data-ttu-id="3bef0-132">Dit kan een tijdrovend proces zijn, afhankelijk van het aantal documenten dat moet worden herberekend.</span><span class="sxs-lookup"><span data-stu-id="3bef0-132">This can take more time depending on the number of documents that must be recalculated.</span></span>|  
    |<span data-ttu-id="3bef0-133">**Totaalbedragen documenten controleren**</span><span class="sxs-lookup"><span data-stu-id="3bef0-133">**Check Doc. Total Amounts**</span></span>|<span data-ttu-id="3bef0-134">Selecteren om de velden **Documentbedrag incl. btw** en **Btw documentbedrag** in de vensters **Inkoopfactuur** en **Inkoopcreditnota** te wijzigen.</span><span class="sxs-lookup"><span data-stu-id="3bef0-134">Select to modify the **Doc. Amount Incl. VAT** and **Doc. Amount VAT** fields on the **Purchase Invoice** and **Purchase Credit Memo** windows.</span></span>|  
  
3.  <span data-ttu-id="3bef0-135">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="3bef0-135">Choose the **OK** button.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="3bef0-136">Zie ook</span><span class="sxs-lookup"><span data-stu-id="3bef0-136">See Also</span></span>  
 <span data-ttu-id="3bef0-137">Inkoopinstellingen</span><span class="sxs-lookup"><span data-stu-id="3bef0-137">Purchases & Payables Setup</span></span>   
 [<span data-ttu-id="3bef0-138">Nederlandse lokale functionaliteit</span><span class="sxs-lookup"><span data-stu-id="3bef0-138">Netherlands Local Functionality</span></span>](netherlands-local-functionality.md)

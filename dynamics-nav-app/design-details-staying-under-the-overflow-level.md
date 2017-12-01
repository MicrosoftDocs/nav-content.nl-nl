---
title: 'Ontwerpdetails: Onder het overflowniveau blijven'
description: Wanneer Maximum aantal en Vast bestelaantal worden gebruikt, richt het planningssysteem zich alleen op de geplande voorraad in het betreffende tijdsinterval. Dit betekent dat het planningssysteem overbodige voorziening kan voorstellen wanneer negatieve vraag- of positieve voorzieningswijzigingen buiten het betreffende tijdsinterval plaatsvinden.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 40676ee59ed7e0df75796d4633be0013ca73bd21
ms.contentlocale: nl-nl
ms.lasthandoff: 12/01/2017

---
# <a name="design-details-staying-under-the-overflow-level"></a><span data-ttu-id="d1408-104">Ontwerpdetails: Onder het overflowniveau blijven</span><span class="sxs-lookup"><span data-stu-id="d1408-104">Design Details: Staying under the Overflow Level</span></span>
<span data-ttu-id="d1408-105">Wanneer de beleidsopties Maximum aantal en Vast bestelaantal worden gebruikt, richt het planningssysteem zich alleen op de geplande voorraad in het betreffende tijdsinterval.</span><span class="sxs-lookup"><span data-stu-id="d1408-105">When using the Maximum Qty. and Fixed Reorder Qty. policies, the planning system focuses on the projected inventory in the given time-bucket only.</span></span> <span data-ttu-id="d1408-106">Dit betekent dat het planningssysteem overbodige voorziening kan voorstellen wanneer negatieve vraag- of positieve voorzieningswijzigingen buiten het betreffende tijdsinterval plaatsvinden.</span><span class="sxs-lookup"><span data-stu-id="d1408-106">This means that the planning system may suggest superfluous supply when negative demand or positive supply changes occur outside of the given time bucket.</span></span> <span data-ttu-id="d1408-107">Als om deze reden een overbodige voorziening wordt voorgesteld, berekent het planningssysteem tot welk aantal de voorziening moet worden teruggebracht (of verwijderd) om de overbodige voorziening te voorkomen.</span><span class="sxs-lookup"><span data-stu-id="d1408-107">If, for this reason, a superfluous supply is suggested, the planning system calculates which quantity the supply should be decreased to (or deleted) to avoid the superfluous supply.</span></span> <span data-ttu-id="d1408-108">Dit aantal wordt het overflowniveau genoemd.</span><span class="sxs-lookup"><span data-stu-id="d1408-108">This quantity is called the “overflow level.”</span></span> <span data-ttu-id="d1408-109">De overflow wordt gecommuniceerd als een planningsregel met een actie **Aantal wijzigen (afname)** of **Annuleren** en het volgende waarschuwingsbericht:</span><span class="sxs-lookup"><span data-stu-id="d1408-109">The overflow is communicated as a planning line with a **Change Qty. (Decrease)** or **Cancel** action and the following warning message:</span></span>  

<span data-ttu-id="d1408-110">*Let op: De geplande voorraad [xx] is groter dan het overflowniveau [xx] op de Vervaldatum] [xx].*</span><span class="sxs-lookup"><span data-stu-id="d1408-110">*Attention: The projected inventory [xx] is higher than the overflow level [xx] on the Due Date [xx].*</span></span>  

<span data-ttu-id="d1408-111">![Overflowniveau voorraad](media/supplyplanning_2_overflow1_new.png "supplyplanning_2_overflow1_new")</span><span class="sxs-lookup"><span data-stu-id="d1408-111">![Inventory overflow level](media/supplyplanning_2_overflow1_new.png "supplyplanning_2_overflow1_new")</span></span>  

##  <a name="calculating-the-overflow-level"></a><span data-ttu-id="d1408-112">Het overflowniveau berekenen</span><span class="sxs-lookup"><span data-stu-id="d1408-112">Calculating the Overflow Level</span></span>  
<span data-ttu-id="d1408-113">Het overflowniveau wordt op verschillende manieren berekend, afhankelijk van de planningsinstelling.</span><span class="sxs-lookup"><span data-stu-id="d1408-113">The overflow level is calculated in different ways depending on planning setup.</span></span>  

### <a name="maximum-qty-reordering-policy"></a><span data-ttu-id="d1408-114">Bestelbeleid Maximum aantal</span><span class="sxs-lookup"><span data-stu-id="d1408-114">Maximum Qty. reordering policy</span></span>  
<span data-ttu-id="d1408-115">Overflowniveau = Maximale voorraad</span><span class="sxs-lookup"><span data-stu-id="d1408-115">Overflow level = Maximum Inventory</span></span>  

> [!NOTE]  
>  <span data-ttu-id="d1408-116">Als een minimaal orderaantal bestaat, wordt het als volgt toegevoegd: overflowniveau = maximale voorraad + minimaal orderaantal.</span><span class="sxs-lookup"><span data-stu-id="d1408-116">If a minimum order quantity exists, then it will be added as follows: Overflow level = Maximum Inventory + Minimum Order Quantity.</span></span>  

### <a name="fixed-reorder-qty-reordering-policy"></a><span data-ttu-id="d1408-117">Bestelbeleid voor vast bestelaantal</span><span class="sxs-lookup"><span data-stu-id="d1408-117">Fixed Reorder Qty. reordering policy</span></span>  
<span data-ttu-id="d1408-118">Overflowniveau = Bestelaantal + bestelpunt</span><span class="sxs-lookup"><span data-stu-id="d1408-118">Overflow level = Reorder Quantity + Reorder Point</span></span>  

> [!NOTE]  
>  <span data-ttu-id="d1408-119">Als het minimale bestelaantal hoger is dan het bestelpunt, wordt dit als volgt vervangen: overflowniveau = bestelaantal + minimum bestelaantal.</span><span class="sxs-lookup"><span data-stu-id="d1408-119">If the minimum order quantity is higher than the reorder point, then it will replace as follows: Overflow Level = Reorder Quantity + Minimum Order Quantity</span></span>  

### <a name="order-multiple"></a><span data-ttu-id="d1408-120">Vaste lotgrootte</span><span class="sxs-lookup"><span data-stu-id="d1408-120">Order Multiple</span></span>  
<span data-ttu-id="d1408-121">Als een vaste lotgrootte bestaat, wordt het overflowniveau voor zowel het bestelbeleid Maximum aantal als Vast bestelaantal aangepast.</span><span class="sxs-lookup"><span data-stu-id="d1408-121">If an order multiple exists, then it will adjust the overflow level for both Maximum Qty. and Fixed Reorder Qty. reordering policies.</span></span>  

##  <a name="creating-the-planning-line-with-overflow-warning"></a><span data-ttu-id="d1408-122">De planningsregel met overflowwaarschuwing maken</span><span class="sxs-lookup"><span data-stu-id="d1408-122">Creating the Planning Line with Overflow Warning</span></span>  
<span data-ttu-id="d1408-123">Als door een bestaande voorraad de geplande voorziening groter is dan het overflowniveau aan het einde van het tijdsinterval, wordt een planningsregel gemaakt.</span><span class="sxs-lookup"><span data-stu-id="d1408-123">When an existing supply causes the projected inventory to be higher than the overflow level at the end of a time bucket, a planning line is created.</span></span> <span data-ttu-id="d1408-124">Om te waarschuwen voor de mogelijke overbodige voorziening, bevat de planningsregel een waarschuwing, is het veld **Planningsboodschap accepteren** niet geselecteerd en is de planningsboodschap Annuleren of Aantal wijzigen.</span><span class="sxs-lookup"><span data-stu-id="d1408-124">To warn about the potential superfluous supply, the planning line has a warning message, the **Accept Action Message** field is not selected, and the action message is either Cancel or Change Qty.</span></span>  

### <a name="calculating-the-planning-line-quantity"></a><span data-ttu-id="d1408-125">Het planningsregelaantal berekenen</span><span class="sxs-lookup"><span data-stu-id="d1408-125">Calculating the Planning Line Quantity</span></span>  
<span data-ttu-id="d1408-126">Planningsregelaantal = Voorzieningaantal - (Geplande voorraad - Overflowniveau)</span><span class="sxs-lookup"><span data-stu-id="d1408-126">Planning Line Quantity = Current Supply Quantity – (Projected Inventory – Overflow Level)</span></span>  

> [!NOTE]  
>  <span data-ttu-id="d1408-127">Net als alle waarschuwingsregels worden eventuele maximale/minimale orderaantallen of vaste ordergrootte genegeerd.</span><span class="sxs-lookup"><span data-stu-id="d1408-127">As with all warning lines, any maximum/minimum order quantity or order multiple will be ignored.</span></span>  

### <a name="defining-the-action-message-type"></a><span data-ttu-id="d1408-128">De soort planningsboodschap definiëren</span><span class="sxs-lookup"><span data-stu-id="d1408-128">Defining the Action Message Type</span></span>  

-   <span data-ttu-id="d1408-129">Als het planningsregelaantal groter is dan 0, is de planningsboodschap Aantal wijzigen.</span><span class="sxs-lookup"><span data-stu-id="d1408-129">If the planning line quantity is higher than 0, then the action message is Change Qty.</span></span>  
-   <span data-ttu-id="d1408-130">Als het planningsregelaantal gelijk is aan of kleiner is dan 0, is de planningsboodschap Annuleren</span><span class="sxs-lookup"><span data-stu-id="d1408-130">If the planning line quantity is equal to or lower than 0, then the action message is Cancel</span></span>  

### <a name="composing-the-warning-message"></a><span data-ttu-id="d1408-131">Het waarschuwingsbericht opstellen</span><span class="sxs-lookup"><span data-stu-id="d1408-131">Composing the Warning Message</span></span>  
<span data-ttu-id="d1408-132">In het geval van overflow wordt in het venster **Niet-getraceerde planningselementen** een waarschuwing weergegeven met de volgende informatie:</span><span class="sxs-lookup"><span data-stu-id="d1408-132">In case of overflow, the **Untracked Planning Elements** window displays a warning message with the following information:</span></span>  

-   <span data-ttu-id="d1408-133">Het geplande voorraadniveau dat de waarschuwing heeft geactiveerd</span><span class="sxs-lookup"><span data-stu-id="d1408-133">The projected inventory level that triggered the warning</span></span>  
-   <span data-ttu-id="d1408-134">Het berekenende overflowniveau</span><span class="sxs-lookup"><span data-stu-id="d1408-134">The calculated overflow level</span></span>  
-   <span data-ttu-id="d1408-135">De vervaldatum van de voorzieningsgebeurtenis.</span><span class="sxs-lookup"><span data-stu-id="d1408-135">The due date of the supply event.</span></span>  

<span data-ttu-id="d1408-136">Voorbeeld: “De verwachte voorraad 120 is hoger dan het overflowniveau 60 op 28-01-11“</span><span class="sxs-lookup"><span data-stu-id="d1408-136">Example: “The projected inventory 120 is higher than the overflow level 60 on 28-01-11”</span></span>  

## <a name="scenario"></a><span data-ttu-id="d1408-137">Scenario</span><span class="sxs-lookup"><span data-stu-id="d1408-137">Scenario</span></span>  
<span data-ttu-id="d1408-138">In dit scenario verandert een klant een verkooporder van 70 in 40 stuks tussen twee planningen.</span><span class="sxs-lookup"><span data-stu-id="d1408-138">In this scenario, a customer changes a sales order from 70 to 40 pieces between two planning runs.</span></span> <span data-ttu-id="d1408-139">De overflowfunctie wordt geactiveerd om de inkoop te beperken die werd voorgesteld voor het oorspronkelijke verkoopaantal.</span><span class="sxs-lookup"><span data-stu-id="d1408-139">The overflow feature sets in to reduce the purchase that was suggested for the initial sales quantity.</span></span>  

### <a name="item-setup"></a><span data-ttu-id="d1408-140">Artikelinstellingen</span><span class="sxs-lookup"><span data-stu-id="d1408-140">Item setup</span></span>  

|<span data-ttu-id="d1408-141">Bestelbeleid</span><span class="sxs-lookup"><span data-stu-id="d1408-141">Reordering Policy</span></span>|<span data-ttu-id="d1408-142">Maximum aantal</span><span class="sxs-lookup"><span data-stu-id="d1408-142">Maximum Qty.</span></span>|  
|-----------------------|------------------|  
|<span data-ttu-id="d1408-143">Max. bestelaantal</span><span class="sxs-lookup"><span data-stu-id="d1408-143">Maximum Order Quantity</span></span>|<span data-ttu-id="d1408-144">100</span><span class="sxs-lookup"><span data-stu-id="d1408-144">100</span></span>|  
|<span data-ttu-id="d1408-145">Bestelpunt</span><span class="sxs-lookup"><span data-stu-id="d1408-145">Reorder Point</span></span>|<span data-ttu-id="d1408-146">50</span><span class="sxs-lookup"><span data-stu-id="d1408-146">50</span></span>|  
|<span data-ttu-id="d1408-147">Voorraad</span><span class="sxs-lookup"><span data-stu-id="d1408-147">Inventory</span></span>|<span data-ttu-id="d1408-148">80</span><span class="sxs-lookup"><span data-stu-id="d1408-148">80</span></span>|  

### <a name="situation-before-sales-decrease"></a><span data-ttu-id="d1408-149">Situatie voor verkoopafname</span><span class="sxs-lookup"><span data-stu-id="d1408-149">Situation before sales decrease</span></span>  

|<span data-ttu-id="d1408-150">Gebeurtenis</span><span class="sxs-lookup"><span data-stu-id="d1408-150">Event</span></span>|<span data-ttu-id="d1408-151">Aantal wijzigen</span><span class="sxs-lookup"><span data-stu-id="d1408-151">Change Qty.</span></span>|<span data-ttu-id="d1408-152">Geschatte inventaris</span><span class="sxs-lookup"><span data-stu-id="d1408-152">Projected Inventory</span></span>|  
|-----------|-----------------|-------------------------|  
|<span data-ttu-id="d1408-153">Dag één</span><span class="sxs-lookup"><span data-stu-id="d1408-153">Day one</span></span>|<span data-ttu-id="d1408-154">Geen</span><span class="sxs-lookup"><span data-stu-id="d1408-154">None</span></span>|<span data-ttu-id="d1408-155">80</span><span class="sxs-lookup"><span data-stu-id="d1408-155">80</span></span>|  
|<span data-ttu-id="d1408-156">Verkoop</span><span class="sxs-lookup"><span data-stu-id="d1408-156">Sale</span></span>|<span data-ttu-id="d1408-157">-70</span><span class="sxs-lookup"><span data-stu-id="d1408-157">-70</span></span>|<span data-ttu-id="d1408-158">10</span><span class="sxs-lookup"><span data-stu-id="d1408-158">10</span></span>|  
|<span data-ttu-id="d1408-159">Einde van periode</span><span class="sxs-lookup"><span data-stu-id="d1408-159">End of time bucket</span></span>|<span data-ttu-id="d1408-160">Geen</span><span class="sxs-lookup"><span data-stu-id="d1408-160">None</span></span>|<span data-ttu-id="d1408-161">10</span><span class="sxs-lookup"><span data-stu-id="d1408-161">10</span></span>|  
|<span data-ttu-id="d1408-162">Nieuwe inkooporder voorstellen</span><span class="sxs-lookup"><span data-stu-id="d1408-162">Suggest new purchase order</span></span>|<span data-ttu-id="d1408-163">+90</span><span class="sxs-lookup"><span data-stu-id="d1408-163">+90</span></span>|<span data-ttu-id="d1408-164">100</span><span class="sxs-lookup"><span data-stu-id="d1408-164">100</span></span>|  

### <a name="situation-after-sales-decrease"></a><span data-ttu-id="d1408-165">Situatie na verkoopafname</span><span class="sxs-lookup"><span data-stu-id="d1408-165">Situation after sales decrease</span></span>  

|<span data-ttu-id="d1408-166">Wijzigen</span><span class="sxs-lookup"><span data-stu-id="d1408-166">Change</span></span>|<span data-ttu-id="d1408-167">Aantal wijzigen</span><span class="sxs-lookup"><span data-stu-id="d1408-167">Change Qty.</span></span>|<span data-ttu-id="d1408-168">Geschatte inventaris</span><span class="sxs-lookup"><span data-stu-id="d1408-168">Projected Inventory</span></span>|  
|------------|-----------------|-------------------------|  
|<span data-ttu-id="d1408-169">Dag één</span><span class="sxs-lookup"><span data-stu-id="d1408-169">Day one</span></span>|<span data-ttu-id="d1408-170">Geen</span><span class="sxs-lookup"><span data-stu-id="d1408-170">None</span></span>|<span data-ttu-id="d1408-171">80</span><span class="sxs-lookup"><span data-stu-id="d1408-171">80</span></span>|  
|<span data-ttu-id="d1408-172">Verkoop</span><span class="sxs-lookup"><span data-stu-id="d1408-172">Sale</span></span>|<span data-ttu-id="d1408-173">-40</span><span class="sxs-lookup"><span data-stu-id="d1408-173">-40</span></span>|<span data-ttu-id="d1408-174">40</span><span class="sxs-lookup"><span data-stu-id="d1408-174">40</span></span>|  
|<span data-ttu-id="d1408-175">Inkoop</span><span class="sxs-lookup"><span data-stu-id="d1408-175">Purchase</span></span>|<span data-ttu-id="d1408-176">+90</span><span class="sxs-lookup"><span data-stu-id="d1408-176">+90</span></span>|<span data-ttu-id="d1408-177">130</span><span class="sxs-lookup"><span data-stu-id="d1408-177">130</span></span>|  
|<span data-ttu-id="d1408-178">Einde van periode</span><span class="sxs-lookup"><span data-stu-id="d1408-178">End of time bucket</span></span>|<span data-ttu-id="d1408-179">Geen</span><span class="sxs-lookup"><span data-stu-id="d1408-179">None</span></span>|<span data-ttu-id="d1408-180">130</span><span class="sxs-lookup"><span data-stu-id="d1408-180">130</span></span>|  
|<span data-ttu-id="d1408-181">Voorstellen om inkoop te verminderen</span><span class="sxs-lookup"><span data-stu-id="d1408-181">Suggest to decrease purchase</span></span><br /><br /> <span data-ttu-id="d1408-182">van 90 naar 60</span><span class="sxs-lookup"><span data-stu-id="d1408-182">order from 90 to 60</span></span>|<span data-ttu-id="d1408-183">-30</span><span class="sxs-lookup"><span data-stu-id="d1408-183">-30</span></span>|<span data-ttu-id="d1408-184">100</span><span class="sxs-lookup"><span data-stu-id="d1408-184">100</span></span>|  

### <a name="resulting-planning-lines"></a><span data-ttu-id="d1408-185">Resulterende planningsregels</span><span class="sxs-lookup"><span data-stu-id="d1408-185">Resulting Planning Lines</span></span>  
 <span data-ttu-id="d1408-186">Er wordt één planningsregel (waarschuwing) gemaakt om de inkoop met 30 te reduceren, van 90 tot 60, om de geplande voorraad op 100 te houden, op basis van het overflowniveau.</span><span class="sxs-lookup"><span data-stu-id="d1408-186">One planning line (warning) is created to reduce the purchase with 30 from 90 to 60 to keep the projected inventory on 100 according to the overflow level.</span></span>  

<span data-ttu-id="d1408-187">![Plannen op basis van overflowniveau](media/nav_app_supply_planning_2_overflow2.png "nav_app_supply_planning_2_overflow2")</span><span class="sxs-lookup"><span data-stu-id="d1408-187">![Plan according to overflow level](media/nav_app_supply_planning_2_overflow2.png "nav_app_supply_planning_2_overflow2")</span></span>  

> [!NOTE]  
>  <span data-ttu-id="d1408-188">Zonder de overflowfunctie wordt er geen waarschuwing gemaakt als het geplande voorraadniveau boven de maximale voorraad is.</span><span class="sxs-lookup"><span data-stu-id="d1408-188">Without the Overflow feature, no warning is created if the projected inventory level is above maximum inventory.</span></span> <span data-ttu-id="d1408-189">Dit kan een overbodige voorziening van 30 genereren.</span><span class="sxs-lookup"><span data-stu-id="d1408-189">This could cause a superfluous supply of 30.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d1408-190">Zie ook</span><span class="sxs-lookup"><span data-stu-id="d1408-190">See Also</span></span>  
<span data-ttu-id="d1408-191">[Ontwerpdetails: Bestelbeleid](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="d1408-191">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
<span data-ttu-id="d1408-192">[Ontwerpdetails: Planningsparameters](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="d1408-192">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
<span data-ttu-id="d1408-193">[Ontwerpdetails: Bestelbeleid verwerken](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="d1408-193">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
[<span data-ttu-id="d1408-194">Ontwerpdetails: Voorraadplanning</span><span class="sxs-lookup"><span data-stu-id="d1408-194">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)


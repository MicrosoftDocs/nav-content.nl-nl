---
title: 'Aanbevolen procedures instellen: Bestelbeleid'
description: Het veld **Bestelbeleid** op artikelkaarten biedt vier verschillende planningmethodes die de interactie tussen de afzonderlijke planningsparameters aansturen.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b96fc662f741bd705e673f7d17b2467b4e6dc846
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="setup-best-practices-reordering-policies"></a><span data-ttu-id="099ac-103">Aanbevolen procedures instellen: Bestelbeleid</span><span class="sxs-lookup"><span data-stu-id="099ac-103">Setup Best Practices: Reordering Policies</span></span>
<span data-ttu-id="099ac-104">Het veld **Bestelbeleid** op artikelkaarten biedt vier verschillende planningmethodes die de interactie tussen de afzonderlijke planningsparameters aansturen.</span><span class="sxs-lookup"><span data-stu-id="099ac-104">The **Reordering Policy** field on item cards offers four different planning methods that determine how the individual planning parameters interact.</span></span>  

<span data-ttu-id="099ac-105">De aanbevolen procedure voor het selecteren van een bestelbeleid is de ABC-classificatie van het product.</span><span class="sxs-lookup"><span data-stu-id="099ac-105">One best-practice foundation for selecting a reordering policy is the item’s ABC classification.</span></span> <span data-ttu-id="099ac-106">Wanneer u ABC-classificatie voor voorraadbeheer en -planning gebruikt, worden items volgens drie verschillende klassen beheerd, afhankelijk van de waarde en het volume ten opzichte van de totale voorraad.</span><span class="sxs-lookup"><span data-stu-id="099ac-106">When you use ABC classification for inventory control and supply planning, items are managed according to three different classes depending on their value and volume relative to the total stock.</span></span> <span data-ttu-id="099ac-107">De waarde/volume-verhouding van de drie klassen wordt in de volgende tabel weergegeven.</span><span class="sxs-lookup"><span data-stu-id="099ac-107">The value-volume distribution of the three classes is shown in the following table.</span></span>

|<span data-ttu-id="099ac-108">Klasse</span><span class="sxs-lookup"><span data-stu-id="099ac-108">Class</span></span>|<span data-ttu-id="099ac-109">Percentage van de totale omvang in voorraad</span><span class="sxs-lookup"><span data-stu-id="099ac-109">Percent of total stock volume</span></span>|<span data-ttu-id="099ac-110">Percentage van de totale waarde in voorraad</span><span class="sxs-lookup"><span data-stu-id="099ac-110">Percent of total stock value</span></span>|
|-----|-----------------------------|----------------------------|
|<span data-ttu-id="099ac-111">A</span><span class="sxs-lookup"><span data-stu-id="099ac-111">A</span></span>|<span data-ttu-id="099ac-112">10-20</span><span class="sxs-lookup"><span data-stu-id="099ac-112">10-20</span></span>|<span data-ttu-id="099ac-113">50-70</span><span class="sxs-lookup"><span data-stu-id="099ac-113">50-70</span></span>|
|<span data-ttu-id="099ac-114">B</span><span class="sxs-lookup"><span data-stu-id="099ac-114">B</span></span>|<span data-ttu-id="099ac-115">20</span><span class="sxs-lookup"><span data-stu-id="099ac-115">20</span></span>|<span data-ttu-id="099ac-116">20</span><span class="sxs-lookup"><span data-stu-id="099ac-116">20</span></span>|
|<span data-ttu-id="099ac-117">L</span><span class="sxs-lookup"><span data-stu-id="099ac-117">C</span></span>|<span data-ttu-id="099ac-118">60-70</span><span class="sxs-lookup"><span data-stu-id="099ac-118">60-70</span></span>|<span data-ttu-id="099ac-119">10-30</span><span class="sxs-lookup"><span data-stu-id="099ac-119">10-30</span></span>|

<span data-ttu-id="099ac-120">De ABC-classificatie stelt dat inspanningen en geld bespaard kunnen worden door minder controle toe te passen op items met een lage waarde/volume-verhouding dan op items met een hoge waarde/volume-verhouding.</span><span class="sxs-lookup"><span data-stu-id="099ac-120">The ABC classification states that effort and money can be saved by applying looser control to items of low value-volume than to items of high value-volume.</span></span> <span data-ttu-id="099ac-121">De volgende illustratie toont welk bestelbeleid in [!INCLUDE[d365fin](includes/d365fin_md.md)] het geschiktst is voor respectievelijk items van het type A, B of C.</span><span class="sxs-lookup"><span data-stu-id="099ac-121">The following illustration shows which reordering policy in [!INCLUDE[d365fin](includes/d365fin_md.md)] is best suited for A, B, and C items respectively.</span></span>

<span data-ttu-id="099ac-122">![ABC-classificatie](media/abc_classification.png "abc_classification")</span><span class="sxs-lookup"><span data-stu-id="099ac-122">![ABC Classification](media/abc_classification.png "abc_classification")</span></span>

<span data-ttu-id="099ac-123">De volgende tabel bevat de aanbevolen procedures voor het selecteren van de vier beleidsterreinen.</span><span class="sxs-lookup"><span data-stu-id="099ac-123">The following table provides best practices for selecting between the four policies.</span></span>  

|<span data-ttu-id="099ac-124">Insteloptie</span><span class="sxs-lookup"><span data-stu-id="099ac-124">Setup option</span></span>|<span data-ttu-id="099ac-125">Aanbevolen procedure</span><span class="sxs-lookup"><span data-stu-id="099ac-125">Best practice</span></span>|<span data-ttu-id="099ac-126">Opmerking</span><span class="sxs-lookup"><span data-stu-id="099ac-126">Comment</span></span>|  
|------------------|-------------------|-------------|  
|<span data-ttu-id="099ac-127">**Order**</span><span class="sxs-lookup"><span data-stu-id="099ac-127">**Order**</span></span>|<span data-ttu-id="099ac-128">Gebruiken voor A-producten.</span><span class="sxs-lookup"><span data-stu-id="099ac-128">Use for A items.</span></span><br /><br /> <span data-ttu-id="099ac-129">Gebruiken voor op maat gemaakte producten.</span><span class="sxs-lookup"><span data-stu-id="099ac-129">Use for make-to-order items.</span></span><br /><br /> <span data-ttu-id="099ac-130">Gebruik in de productie voor items op het hoogste niveau en voor dure onderdelen en halffabrikaten.</span><span class="sxs-lookup"><span data-stu-id="099ac-130">In manufacturing, use for top-level items and for expensive components and subassemblies.</span></span><br /><br /> <span data-ttu-id="099ac-131">Gebruiken voor artikelen die als doorverzendingen en speciale orders worden aangekocht.</span><span class="sxs-lookup"><span data-stu-id="099ac-131">Use for items that are purchased as drop shipments and special orders.</span></span><br /><br /> <span data-ttu-id="099ac-132">Niet gebruiken als u geen automatische reservering accepteert.</span><span class="sxs-lookup"><span data-stu-id="099ac-132">Do not use if you do not accept automatic reservation.</span></span>|<span data-ttu-id="099ac-133">A-artikelen, zoals lederen banken in een meubelwinkel, zijn dure artikelen met lage en onregelmatige bestelsnelheden waarbij voorraad onaanvaardbaar is of de vereiste kenmerken variëren.</span><span class="sxs-lookup"><span data-stu-id="099ac-133">A items, such as leather couches in a furniture store, are high-value items with low and irregular order velocity where inventory is unacceptable, or the required attributes vary.</span></span> <span data-ttu-id="099ac-134">Het beste bestelbeleid is daarom een beleid dat specifiek voor elke vraag een planning maakt.</span><span class="sxs-lookup"><span data-stu-id="099ac-134">The best reordering policy is therefore one that plans specifically for each demand.</span></span>|  
|<span data-ttu-id="099ac-135">**Lot-for-Lot**</span><span class="sxs-lookup"><span data-stu-id="099ac-135">**Lot-for-Lot**</span></span>|<span data-ttu-id="099ac-136">Gebruiken voor B-producten.</span><span class="sxs-lookup"><span data-stu-id="099ac-136">Use for B items.</span></span><br /><br /> <span data-ttu-id="099ac-137">Gebruiken in de productie voor onderdelen die op meerdere stuklijsten voorkomen.</span><span class="sxs-lookup"><span data-stu-id="099ac-137">In manufacturing, use for components that occur in multiple BOMs.</span></span> <span data-ttu-id="099ac-138">Dit zorgt ervoor dat inkooporders voor dezelfde leverancier worden gecombineerd zodat betere prijzen kunnen worden onderhandeld.</span><span class="sxs-lookup"><span data-stu-id="099ac-138">This ensures that purchase orders are combined for the same vendor, so better prices can be negotiated.</span></span><br /><br /> <span data-ttu-id="099ac-139">Gebruiken als u niet zeker weet welk bestelbeleid u moet selecteren.</span><span class="sxs-lookup"><span data-stu-id="099ac-139">Use if you are not sure about which reordering policy to select.</span></span>|<span data-ttu-id="099ac-140">B-artikelen, zoals eetkamerstoelen, hebben een regelmatige en redelijk hoge bestelsnelheid maar ook hoge opslagkosten.</span><span class="sxs-lookup"><span data-stu-id="099ac-140">B items, such as dining chairs, have a regular and fairly high order velocity, but also high carrying costs.</span></span> <span data-ttu-id="099ac-141">Het beste bestelbeleid voor B-artikelen is daarom een voordelig beleid dat de vraag bij de bestelcyclus bundelt.</span><span class="sxs-lookup"><span data-stu-id="099ac-141">The best reordering policy for B items is therefore one that is economical by bundling demand in the reorder cycle.</span></span><br /><br /> <span data-ttu-id="099ac-142">80 procent van de artikelen kan dit beleid gebruiken.</span><span class="sxs-lookup"><span data-stu-id="099ac-142">80 percent of items can use this policy.</span></span><br /><br /> <span data-ttu-id="099ac-143">Kan worden gebruikt zonder planningparameters.</span><span class="sxs-lookup"><span data-stu-id="099ac-143">Can be used successfully without planning parameters.</span></span>|  
|<span data-ttu-id="099ac-144">**Vast bestelaantal**</span><span class="sxs-lookup"><span data-stu-id="099ac-144">**Fixed Reorder Qty.**</span></span>|<span data-ttu-id="099ac-145">Gebruiken voor C-producten.</span><span class="sxs-lookup"><span data-stu-id="099ac-145">Use for C items.</span></span><br /><br /> <span data-ttu-id="099ac-146">Combineren met bestelpuntparameters.</span><span class="sxs-lookup"><span data-stu-id="099ac-146">Combine with reorder-point parameters.</span></span><br /><br /> <span data-ttu-id="099ac-147">Gebruiken in de productie voor onderdelen van het laagste niveau.</span><span class="sxs-lookup"><span data-stu-id="099ac-147">In manufacturing, use for lowest-level components.</span></span><br /><br /> <span data-ttu-id="099ac-148">Niet gebruiken als het artikel vaak wordt gereserveerd.</span><span class="sxs-lookup"><span data-stu-id="099ac-148">Do not use if the item is often reserved.</span></span>|<span data-ttu-id="099ac-149">C-artikelen, zoals theekopjes, zijn artikelen met een lage waarde en een hoge en regelmatige bestelsnelheid.</span><span class="sxs-lookup"><span data-stu-id="099ac-149">C items, such as tea cups, are low-value items with high and regular order velocity.</span></span> <span data-ttu-id="099ac-150">Het beste bestelbeleid voor C-artikelen is daarom een beleid dat constante beschikbaarheid garandeert door altijd boven het bestelpunt te blijven.</span><span class="sxs-lookup"><span data-stu-id="099ac-150">The best reordering policy for C items is therefore one that guarantees constant availability by always staying above a reorder point.</span></span><br /><br /> <span data-ttu-id="099ac-151">Als de gebruiker een hoeveelheid reserveert voor een onzekere vraag, raakt de planning verstoord.</span><span class="sxs-lookup"><span data-stu-id="099ac-151">If the user reserves a quantity for some distant demand, then the planning foundation will be disturbed.</span></span> <span data-ttu-id="099ac-152">Zelfs als de geplande voorraad met betrekking tot het bestelpunt aanvaardbaar is, zijn de hoeveelheden mogelijk niet beschikbaar vanwege de reservering.</span><span class="sxs-lookup"><span data-stu-id="099ac-152">Even if the projected inventory level is acceptable with regard to the reorder point, the quantities may not be available because of the reservation.</span></span>|  
|<span data-ttu-id="099ac-153">**Maximum aantal**</span><span class="sxs-lookup"><span data-stu-id="099ac-153">**Maximum Qty.**</span></span>|<span data-ttu-id="099ac-154">Gebruiken voor C-artikelen met hoge transportkosten of opslagbeperkingen.</span><span class="sxs-lookup"><span data-stu-id="099ac-154">Use for C items with high carrying costs or storing limitations.</span></span><br /><br /> <span data-ttu-id="099ac-155">Combineren met een of meer orderwijzigingen (Minimum/Maximum bestelaantal of lotgrootte).</span><span class="sxs-lookup"><span data-stu-id="099ac-155">Combine with one or more order modifiers (Minimum/Maximum Order Quantity or Order Multiple).</span></span>|<span data-ttu-id="099ac-156">C-artikelen, zoals theekopjes, zijn artikelen met een lage waarde en een hoge en regelmatige bestelsnelheid.</span><span class="sxs-lookup"><span data-stu-id="099ac-156">C items, such as tea cups, are low-value items with high and regular order velocity.</span></span> <span data-ttu-id="099ac-157">Het beste bestelbeleid voor C-artikelen is daarom een beleid dat constante beschikbaarheid garandeert door altijd boven het bestelpunt te blijven, maar onder een maximum voorraadhoeveelheid.</span><span class="sxs-lookup"><span data-stu-id="099ac-157">The best reordering policy for C items is therefore one that guarantees constant availability by always staying above a reorder point, but below a maximum inventory quantity.</span></span><br /><br /> <span data-ttu-id="099ac-158">Om het voorgestelde order te wijzigen, kunt u het bestelaantal verlagen tot een opgegeven maximum bestelaantal, verhoogd tot een opgegeven minimum bestelaantal of afgerond tot het voldoet aan een opgegeven lotgrootte.</span><span class="sxs-lookup"><span data-stu-id="099ac-158">To modify the suggested order, you may want the order quantity to be decreased to a specified maximum order quantity, increased to a specified minimum order quantity, or rounded up to meet a specified order multiple.</span></span> <span data-ttu-id="099ac-159">**Opmerking:** als dit in combinatie met een bestelpunt wordt gebruikt, blijft de voorraad tussen bestelpunt en het maximum aantal.</span><span class="sxs-lookup"><span data-stu-id="099ac-159">**Note:**  If used with a reorder point, then inventory stays between the reorder point and the maximum quantity.</span></span>|  

## <a name="see-also"></a><span data-ttu-id="099ac-160">Zie ook</span><span class="sxs-lookup"><span data-stu-id="099ac-160">See Also</span></span>  
 <span data-ttu-id="099ac-161">[Aanbevolen procedures instellen: Voorraadplanning](setup-best-practices-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="099ac-161">[Setup Best Practices: Supply Planning](setup-best-practices-supply-planning.md) </span></span>  
 <span data-ttu-id="099ac-162">[Ontwerpdetails: Bestelbeleid](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="099ac-162">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
 <span data-ttu-id="099ac-163">[Ontwerpdetails: Order](design-details-order.md) </span><span class="sxs-lookup"><span data-stu-id="099ac-163">[Design Details: Order](design-details-order.md) </span></span>  
 <span data-ttu-id="099ac-164">[Ontwerpdetails: Lot-voor-lot](design-details-lot-for-lot.md) </span><span class="sxs-lookup"><span data-stu-id="099ac-164">[Design Details: Lot-for-Lot](design-details-lot-for-lot.md) </span></span>  
 <span data-ttu-id="099ac-165">[Ontwerpdetails: Vast bestelaantal](design-details-fixed-reorder-qty.md) </span><span class="sxs-lookup"><span data-stu-id="099ac-165">[Design Details: Fixed Reorder Qty.](design-details-fixed-reorder-qty.md) </span></span>  
 <span data-ttu-id="099ac-166">[Ontwerpdetails: Maximaal aantal](design-details-maximum-qty.md) </span><span class="sxs-lookup"><span data-stu-id="099ac-166">[Design Details: Maximum Qty.](design-details-maximum-qty.md) </span></span>  
 [<span data-ttu-id="099ac-167">Complexe toepassingsgebieden instellen met aanbevolen procedures</span><span class="sxs-lookup"><span data-stu-id="099ac-167">Set Up Complex Application Areas Using Best Practices</span></span>](set-up-complex-application-areas-using-best-practices.md)  
 <span data-ttu-id="099ac-168">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="099ac-168">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

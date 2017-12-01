---
title: Relaties tussen vraag en aanbod bijhouden
description: Vanuit elk document voor aanbod of vraag in het zogenaamde ordernetwerk kunt u de ordervraag (getraceerd aantal), prognose , raamverkooporder of planningsparameter (niet-getraceerd aantal) traceren die een planningregel heeft doen stijgen.
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
ms.openlocfilehash: 60672b1b88bff5a5e4de920f346d7d4942f835e9
ms.contentlocale: nl-nl
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-track-relations-between-demand-and-supply"></a><span data-ttu-id="21182-103">Procedure: Relatie tussen vraag en aanbod bijhouden</span><span class="sxs-lookup"><span data-stu-id="21182-103">How to: Track Relations Between Demand and Supply</span></span>
<span data-ttu-id="21182-104">Vanuit elk document voor aanbod of vraag in het zogenaamde ordernetwerk kunt u de ordervraag (getraceerd aantal), prognose , raamverkooporder of planningsparameter (niet-getraceerd aantal) traceren die een planningregel heeft doen stijgen.</span><span class="sxs-lookup"><span data-stu-id="21182-104">From any supply or demand document in the so-called order network, you can track the order demand (tracked quantity), forecast, blanket sales order, or planning parameter (untracked quantity) that has given rise to the planning line in question.</span></span>

<span data-ttu-id="21182-105">De planningsvoorstellen bevatten ook ondersteunende planninginformatie over entiteiten die geen orders zijn om de planner te helpen een optimaal leveringsplan op te stellen.</span><span class="sxs-lookup"><span data-stu-id="21182-105">The planning worksheets also offers supporting planning information about non-order entities to help the planner obtain an optimal supply plan.</span></span> <span data-ttu-id="21182-106">Zie de sectie Niet-getraceerde planningselementen voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="21182-106">For more information, see the "Untracked Planning Elements" section.</span></span>

## <a name="to-track-linked-items"></a><span data-ttu-id="21182-107">Gekoppelde artikelen traceren</span><span class="sxs-lookup"><span data-stu-id="21182-107">To track linked items</span></span>
<span data-ttu-id="21182-108">Met behulp van ordertracering kunt u nagaan hoe verkooporders, productieorders en inkooporders aan de productieorder zijn gekoppeld via de plannings- en reserveringssystemen.</span><span class="sxs-lookup"><span data-stu-id="21182-108">Order tracking shows how sales orders, production orders, and purchase orders are related to the manufacturing order through the planning and reservation systems.</span></span>

<span data-ttu-id="21182-109">Hieronder wordt beschreven hoe u gekoppelde artikelen in een vast geplande productieorder traceert.</span><span class="sxs-lookup"><span data-stu-id="21182-109">The following describes how to track linked items on a firm planned production order.</span></span> <span data-ttu-id="21182-110">De stappen voor alle andere soorten orders en vanuit planningsvoorstelregels zijn vergelijkbaar.</span><span class="sxs-lookup"><span data-stu-id="21182-110">The steps are similar for all other order types, and from planning worksheet lines.</span></span>

1. <span data-ttu-id="21182-111">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Vast geplande productieorder** in en klik op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="21182-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Firm Planned Prod. Order**, and then choose the related link.</span></span>
2. <span data-ttu-id="21182-112">Open de betreffende vast geplande productieorder in de lijst.</span><span class="sxs-lookup"><span data-stu-id="21182-112">Open the relevant firm planned production order from the list.</span></span>
3. <span data-ttu-id="21182-113">Op het sneltabblad **Regels** kiest u de actie **Functies** en vervolgens **Ordertracering**.</span><span class="sxs-lookup"><span data-stu-id="21182-113">On the **Lines** FastTab, choose the **Functions** action, and then choose the **Order Tracking** action.</span></span>

<span data-ttu-id="21182-114">Op de regels in het venster **Ordertracering** worden de documenten weergegeven die zijn gekoppeld aan de huidige productieorderregel.</span><span class="sxs-lookup"><span data-stu-id="21182-114">The lines in the **Order Tracking** display the documents that are related to the current production order line.</span></span>

## <a name="untracked-planning-elements"></a><span data-ttu-id="21182-115">Niet-getraceerde planningselementen</span><span class="sxs-lookup"><span data-stu-id="21182-115">Untracked Planning Elements</span></span>
<span data-ttu-id="21182-116">Het venster **Niet-getraceerde planningselementen** wordt geopend wanneer u het veld **Niet-getraceerd aantal** in het venster **Orderplanning** kiest.</span><span class="sxs-lookup"><span data-stu-id="21182-116">The **Untracked Planning Elements** window opens when you choose the **Untracked Qty.** field in the **order Planning** window.</span></span> <span data-ttu-id="21182-117">Dit dient twee doelen:</span><span class="sxs-lookup"><span data-stu-id="21182-117">It serves two purposes:</span></span>

1. <span data-ttu-id="21182-118">De tabel bevat informatie over ongetraceerde hoeveelheden die worden weergegeven wanneer de gebruiker opzoekt in het venster Ordertracering om de ongetraceerde aantallen weer te geven.</span><span class="sxs-lookup"><span data-stu-id="21182-118">To hold information about untracked quantities displayed when the user looks up from the Order Tracking window to see untracked quantities.</span></span>
2. <span data-ttu-id="21182-119">De tabel bevat waarschuwingsberichten die worden weergegeven wanneer de gebruiker op het pictogram **Waarschuwing** in het venster **Planningsvoorstel** klikt.</span><span class="sxs-lookup"><span data-stu-id="21182-119">To hold warning messages displayed when the user chooses the **Warning** icon in the **Planning Worksheet** window.</span></span>

<span data-ttu-id="21182-120">Het venster bevat posten die een verklaring kunnen geven voor niet-getraceerde overschotaantallen in het ordertraceringsnetwerk.</span><span class="sxs-lookup"><span data-stu-id="21182-120">The window contains entries which account for an untracked surplus quantity in order tracking network.</span></span> <span data-ttu-id="21182-121">Deze posten worden gegenereerd tijdens het planningsproces en verklaren waar het niet-getraceerde overschotaantal in de ordertraceringsregels vandaan kwam.</span><span class="sxs-lookup"><span data-stu-id="21182-121">These entries are generated during the planning run and explain where the untracked surplus quantity in the order tracking lines came from.</span></span> <span data-ttu-id="21182-122">Dit niet-getraceerde overschot kan afkomstig zijn uit:</span><span class="sxs-lookup"><span data-stu-id="21182-122">This untracked surplus can come from:</span></span>

- <span data-ttu-id="21182-123">Productieprognose</span><span class="sxs-lookup"><span data-stu-id="21182-123">Production forecast</span></span>
- <span data-ttu-id="21182-124">Raamcontractenorders</span><span class="sxs-lookup"><span data-stu-id="21182-124">Blanket orders</span></span>
- <span data-ttu-id="21182-125">Veiligheidsvoorraad</span><span class="sxs-lookup"><span data-stu-id="21182-125">Safety stock quantity</span></span>
- <span data-ttu-id="21182-126">Bestelpunt</span><span class="sxs-lookup"><span data-stu-id="21182-126">Reorder point</span></span>
- <span data-ttu-id="21182-127">Maximale voorraad</span><span class="sxs-lookup"><span data-stu-id="21182-127">Maximum inventory</span></span>
- <span data-ttu-id="21182-128">Bestelaantal</span><span class="sxs-lookup"><span data-stu-id="21182-128">Reorder quantity</span></span>
- <span data-ttu-id="21182-129">Max. bestelaantal</span><span class="sxs-lookup"><span data-stu-id="21182-129">Maximum order quantity</span></span>
- <span data-ttu-id="21182-130">Min. bestelaantal</span><span class="sxs-lookup"><span data-stu-id="21182-130">Minimum order quantity</span></span>
- <span data-ttu-id="21182-131">Vaste lotgrootte</span><span class="sxs-lookup"><span data-stu-id="21182-131">Order multiple</span></span>
- <span data-ttu-id="21182-132">Demping (% van lotgrootte)</span><span class="sxs-lookup"><span data-stu-id="21182-132">Dampener (% of lot size)</span></span>

## <a name="see-also"></a><span data-ttu-id="21182-133">Zie ook</span><span class="sxs-lookup"><span data-stu-id="21182-133">See Also</span></span>  
<span data-ttu-id="21182-134">[Gepland](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="21182-134">[Planning](production-planning.md) </span></span>  
[<span data-ttu-id="21182-135">Productie instellen</span><span class="sxs-lookup"><span data-stu-id="21182-135">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="21182-136">[Productie](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="21182-136">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="21182-137">Voorraad</span><span class="sxs-lookup"><span data-stu-id="21182-137">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="21182-138">Inkoop</span><span class="sxs-lookup"><span data-stu-id="21182-138">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="21182-139">Ontwerpdetails: Reservering, tracering en planningsboodschappen</span><span class="sxs-lookup"><span data-stu-id="21182-139">Design Details: Reservation, Tracking, and Action Messaging</span></span>](design-details-reservation-order-tracking-and-action-messaging.md)  
<span data-ttu-id="21182-140">[Ontwerpdetails: Voorzieningsplanning](design-details-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="21182-140">[Design Details: Supply Planning](design-details-supply-planning.md) </span></span>  
[<span data-ttu-id="21182-141">Aanbevolen procedures instellen: voorraadplanning</span><span class="sxs-lookup"><span data-stu-id="21182-141">Setup Best Practices: Supply Planning</span></span>](setup-best-practices-supply-planning.md)  
<span data-ttu-id="21182-142">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="21182-142">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>


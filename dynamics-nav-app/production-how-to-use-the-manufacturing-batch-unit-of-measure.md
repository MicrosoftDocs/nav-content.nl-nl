---
title: De productiebatcheenheid gebruiken
description: "Als een artikel in één eenheid in voorraad is, maar in een andere eenheid wordt geproduceerd, moet de productieorder gebruikmaken van een productiebatcheenheid voor het berekenen van het juiste aantal onderdelen. Een voorbeeld van een berekening van een productiebatcheenheid is wanneer een geproduceerd artikel als stukgoed in voorraad is maar in tonnen gewicht wordt geproduceerd."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/14/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: cf0c91b076f473c12e61ce82d870a66e352c1920
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-work-with-manufacturing-batch-units-of-measure"></a><span data-ttu-id="aa91d-104">Procedure: Werken met productiebatcheenheden</span><span class="sxs-lookup"><span data-stu-id="aa91d-104">How to: Work with Manufacturing Batch Units of Measure</span></span>
<span data-ttu-id="aa91d-105">Als een artikel in één eenheid in voorraad is, maar in een andere eenheid wordt geproduceerd, kan een productieorder worden gemaakt die gebruikmaakt van een productiebatcheenheid voor het berekenen van het juiste aantal onderdelen tijdens de batchverwerking **Productieorder vernieuwen**.</span><span class="sxs-lookup"><span data-stu-id="aa91d-105">If an item is stocked in one unit of measure but produced in another, a production order is created that uses a manufacturing batch unit of measure to calculate the correct quantity of the components during the **Refresh Production Order** batch job.</span></span> <span data-ttu-id="aa91d-106">Een voorbeeld van een berekening van een productiebatcheenheid is wanneer een geproduceerd artikel als stukgoed in voorraad is maar in tonnen gewicht wordt geproduceerd.</span><span class="sxs-lookup"><span data-stu-id="aa91d-106">An example of a manufacturing batch unit of measure calculation is when a manufactured item is stocked in pieces but produced in tons.</span></span>  

## <a name="to-create-a-production-bom-using-a-batch-unit-of-measure"></a><span data-ttu-id="aa91d-107">Een productiestuklijst maken met behulp van een batcheenheid</span><span class="sxs-lookup"><span data-stu-id="aa91d-107">To create a production BOM using a batch unit of measure</span></span>  
1.  <span data-ttu-id="aa91d-108">De productiebatcheenheid wordt ingesteld als alternatieve eenheid in het venster **Artikeleenheden** bij het artikel dat moet worden geproduceerd.</span><span class="sxs-lookup"><span data-stu-id="aa91d-108">The manufacturing batch unit of measure is set up as an alternative unit of measure in the **Item Units of Measure** window on the item to be produced.</span></span> <span data-ttu-id="aa91d-109">De batcheenheid komt niet in de plaats van de basiseenheid van het artikel.</span><span class="sxs-lookup"><span data-stu-id="aa91d-109">The batch unit of measure will not replace the base unit of measure on the item.</span></span>  
2.  <span data-ttu-id="aa91d-110">Maak een productiestuklijst voor het artikel dat is ingesteld met de productiebatcheenheid.</span><span class="sxs-lookup"><span data-stu-id="aa91d-110">Create a production BOM for the item set up with the manufacturing batch unit of measure.</span></span> <span data-ttu-id="aa91d-111">Zie voor meer informatie [Procedure: productiestuklijsten maken](production-how-to-create-production-boms.md).</span><span class="sxs-lookup"><span data-stu-id="aa91d-111">For more information, see [How to: Create Production BOMs](production-how-to-create-production-boms.md).</span></span>  
3.  <span data-ttu-id="aa91d-112">Selecteer de eenheidscode voor de productiebatcheenheid in het veld **Eenheidscode**.</span><span class="sxs-lookup"><span data-stu-id="aa91d-112">In the **Unit of Measure Code** field, select the manufacturing batch unit of measure.</span></span>  
4.  <span data-ttu-id="aa91d-113">Voer voor elke productiestuklijstregel in het veld **Aantal per** het aantal van dit onderdeelartikel in dat nodig is om deze batcheenheid te maken.</span><span class="sxs-lookup"><span data-stu-id="aa91d-113">For each production BOM line, in the **Quantity Per** field, enter the quantity of this component item that is required to create this batch unit of measure.</span></span>  
5.  <span data-ttu-id="aa91d-114">Open **Artikel** voor het betreffende artikel.</span><span class="sxs-lookup"><span data-stu-id="aa91d-114">Open the **Item Card** for the related item.</span></span>  

    <span data-ttu-id="aa91d-115">Selecteer op het sneltabblad **Aanvulling** in de groep **Prod.-stuklijstnr.** de hierboven gemaakte productiestuklijst.</span><span class="sxs-lookup"><span data-stu-id="aa91d-115">On the **Replenishment** FastTab, in the **Production BOM No.** field, select the production BOM created above.</span></span>  
6.  <span data-ttu-id="aa91d-116">Maak een productieorderkop met het artikel dat is ingesteld met de productiebatcheenheid.</span><span class="sxs-lookup"><span data-stu-id="aa91d-116">Create a production order header using the item set up with the manufacturing batch unit of measure.</span></span> <span data-ttu-id="aa91d-117">Zie voor meer informatie [Procedure: productieorders maken](production-how-to-create-production-orders.md).</span><span class="sxs-lookup"><span data-stu-id="aa91d-117">For more information, see [How to: Create Production Orders](production-how-to-create-production-orders.md).</span></span>  
7.  <span data-ttu-id="aa91d-118">Kies de actie **Vernieuwen** en kies vervolgens de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="aa91d-118">Choose the **Refresh** action, and then choose  the **OK** button.</span></span>  

<span data-ttu-id="aa91d-119">Kies op het sneltabblad **Regels** de actie **Regel** en kies vervolgens de actie **Materialen** om het resultaat te bekijken.</span><span class="sxs-lookup"><span data-stu-id="aa91d-119">On the **Lines** FastTab, choose the **Line** action, and then choose the **Components** action to view the result.</span></span> <span data-ttu-id="aa91d-120">Het programma berekent het juiste aantal materialen dat nodig is om aan de productiestuklijst te voldoen op basis van de productiebatcheenheid.</span><span class="sxs-lookup"><span data-stu-id="aa91d-120">The program calculates the correct quantity of the components needed to satisfy the production BOM based on the manufacturing batch unit of measure.</span></span>  

## <a name="to-calculate-a-manufacturing-batch-unit-of-measure-on-a-production-order"></a><span data-ttu-id="aa91d-121">Een productiebatcheenheid berekenen in een productieorder</span><span class="sxs-lookup"><span data-stu-id="aa91d-121">To calculate a manufacturing batch unit of measure on a production order</span></span>  
1.  <span data-ttu-id="aa91d-122">Maak een productieorderkop met het artikel dat is ingesteld met de productiebatcheenheid.</span><span class="sxs-lookup"><span data-stu-id="aa91d-122">Create a production order header using the item set up with the manufacturing batch unit of measure.</span></span>  
2.  <span data-ttu-id="aa91d-123">Typ in het veld **Artikelnr.** in de productieorderregel hetzelfde artikelnummer dat wordt gebruikt in de kop.</span><span class="sxs-lookup"><span data-stu-id="aa91d-123">In the **Item No.** field in the Production Order line, type the same item number used in the header.</span></span>  
3.  <span data-ttu-id="aa91d-124">Voer in het veld **Aantal** hetzelfde aantal in dat wordt gebruikt in de kop.</span><span class="sxs-lookup"><span data-stu-id="aa91d-124">In the **Quantity** field, enter the same quantity used in the header.</span></span>  
4.  <span data-ttu-id="aa91d-125">Selecteer de eenheidscode voor de productiebatcheenheid in het veld **Eenheidscode**.</span><span class="sxs-lookup"><span data-stu-id="aa91d-125">In the **Unit of Measure Code** field, select the manufacturing batch unit of measure code.</span></span>  
5.  <span data-ttu-id="aa91d-126">Kies de actie **Vernieuwen**.</span><span class="sxs-lookup"><span data-stu-id="aa91d-126">Choose the **Refresh** action.</span></span>
6.  <span data-ttu-id="aa91d-127">Schakel op het sneltabblad **Berekenen** het selectievakje **Regels** uit.</span><span class="sxs-lookup"><span data-stu-id="aa91d-127">On the **Calculate** FastTab, clear the **Lines** check box.</span></span>  
7.  <span data-ttu-id="aa91d-128">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="aa91d-128">Choose the **OK** button.</span></span>  
8.  <span data-ttu-id="aa91d-129">Kies op het sneltabblad **Regels** de actie **Regel** en kies vervolgens de actie **Materialen** om het resultaat te bekijken.</span><span class="sxs-lookup"><span data-stu-id="aa91d-129">On the **Lines** FastTab, choose the **Line** action, and then choose the **Components** action to view the result.</span></span> <span data-ttu-id="aa91d-130">Het juiste aantal materialen dat nodig is om aan de productiestuklijst te voldoen wordt berekend op basis van de productiebatcheenheid.</span><span class="sxs-lookup"><span data-stu-id="aa91d-130">The correct quantity of the components needed to satisfy the production BOM is calculated based on the manufacturing batch unit of measure.</span></span>  

## <a name="see-also"></a><span data-ttu-id="aa91d-131">Zie ook</span><span class="sxs-lookup"><span data-stu-id="aa91d-131">See Also</span></span>  
[<span data-ttu-id="aa91d-132">Procedure: bewerkingsplannen maken</span><span class="sxs-lookup"><span data-stu-id="aa91d-132">How to: Create Routings</span></span>](production-how-to-create-routings.md)  
<span data-ttu-id="aa91d-133">[Procedure: productiestuklijsten maken](production-how-to-create-production-boms.md)   </span><span class="sxs-lookup"><span data-stu-id="aa91d-133">[How to: Create Production BOMs](production-how-to-create-production-boms.md)   </span></span>  
[<span data-ttu-id="aa91d-134">Productie instellen</span><span class="sxs-lookup"><span data-stu-id="aa91d-134">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="aa91d-135">[Productie](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="aa91d-135">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
<span data-ttu-id="aa91d-136">[Gepland](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="aa91d-136">[Planning](production-planning.md) </span></span>  
[<span data-ttu-id="aa91d-137">Voorraad</span><span class="sxs-lookup"><span data-stu-id="aa91d-137">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="aa91d-138">Inkoop</span><span class="sxs-lookup"><span data-stu-id="aa91d-138">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="aa91d-139">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="aa91d-139">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

---
title: Materialen afboeken op basis van de uitvoer van een bewerking
description: Voor artikelen die zijn ingesteld met de achterwaartse afboekingsmethode wordt standaard het verbruik van onderdelen berekend en geboekt wanneer u de status van een vrijgegeven productieorder wijzigt in **Voltooid**. Zie voor meer informatie Afboekingsmethode.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 48645ff5d943b2f7093224289ff3cad6cfa6537e
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-flush-components-according-to-operation-output"></a><span data-ttu-id="2cf33-104">Procedure: materialen afboeken op basis van de uitvoer van een bewerking</span><span class="sxs-lookup"><span data-stu-id="2cf33-104">How to: Flush Components According to Operation Output</span></span>
<span data-ttu-id="2cf33-105">Voor artikelen die zijn ingesteld met de achterwaartse afboekingsmethode wordt standaard het verbruik van onderdelen berekend en geboekt wanneer u de status van een vrijgegeven productieorder wijzigt in **Voltooid**.</span><span class="sxs-lookup"><span data-stu-id="2cf33-105">For items that are set up with backward flushing method, the default behavior is to calculate and post component consumption when you change the status of a released production order to **Finished**.</span></span>  

<span data-ttu-id="2cf33-106">Als u ook bewerkingsplankoppelingen definieert, vinden berekening en boeking plaats wanneer elke bewerking is voltooid en wordt de hoeveelheid geboekt die daadwerkelijk is verbruikt in de bewerking.</span><span class="sxs-lookup"><span data-stu-id="2cf33-106">If you also define routing link codes, then calculation and posting occurs when each operation is finished, and the quantity that was actually consumed in the operation is posted.</span></span> <span data-ttu-id="2cf33-107">Zie [Procedure: Bewerkingsplannen maken](production-how-to-create-routings.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="2cf33-107">For more information, see [How to: Create Routings](production-how-to-create-routings.md).</span></span>  

<span data-ttu-id="2cf33-108">Als bijvoorbeeld een productieorder voor het vervaardigen van 800 meter 8 kg van een component vereist, worden als u 200 meter als uitvoer boekt automatisch 2 kg als verbruik geboekt.</span><span class="sxs-lookup"><span data-stu-id="2cf33-108">For example, if a production order to produce 800 meters requires 8 kg of a component, then when you post 200 meters as output, 2 kg are automatically posted as consumption.</span></span>  

<span data-ttu-id="2cf33-109">Deze functionaliteit is handig om de volgende redenen:</span><span class="sxs-lookup"><span data-stu-id="2cf33-109">This functionality is useful for the following reasons:</span></span>  

-   <span data-ttu-id="2cf33-110">**Voorraadwaardering** - Waardeposten voor uitvoer en verbruik worden parallel geproduceerd naarmate de productieorder vordert.</span><span class="sxs-lookup"><span data-stu-id="2cf33-110">**Inventory Valuation** - Value entries for output and consumption are created in parallel as the production order progresses.</span></span> <span data-ttu-id="2cf33-111">Zonder bewerkingsplankoppelingen neemt de voorraadwaarde toe als uitvoer wordt geboekt en vervolgens op een later tijdstip weer af wanneer de waarde van het materiaalverbruik wordt geboekt samen met de gereedgemelde productieorder.</span><span class="sxs-lookup"><span data-stu-id="2cf33-111">Without routing link codes, the inventory value will increase as output is posted and then decrease at a later point in time when the value of component consumption is posted together with the finished production order.</span></span>  
-   <span data-ttu-id="2cf33-112">**Beschikbaarheid van voorraad** - Bij geleidelijke verbruiksboeking is de beschikbaarheid van artikelonderdelen meer actueel, hetgeen belangrijk is voor het handhaven van het interne evenwicht tussen vraag en aanbod.</span><span class="sxs-lookup"><span data-stu-id="2cf33-112">**Inventory Availability** - With gradual consumption posting, the availability of component items is more up-to-date, which is important to maintain the internal balance between demand and supply.</span></span> <span data-ttu-id="2cf33-113">Zonder bewerkingsplankoppelingen kan bij andere vraag naar het materiaal de misvatting ontstaan dat het materiaal beschikbaar is zolang een vertraagde verbruiksboeking uitstaat.</span><span class="sxs-lookup"><span data-stu-id="2cf33-113">Without routing link codes, other demands for the component may believe that it is available as long as it is pending a delayed consumption posting.</span></span>  
-   <span data-ttu-id="2cf33-114">**Just-In-Time** – Via de mogelijkheid om producten aan te passen aan de vraag van de klant kunt u verspilling tot een minimum beperken door ervoor te zorgen dat werk en systeemwijzigingen alleen optreden wanneer het nodig is.</span><span class="sxs-lookup"><span data-stu-id="2cf33-114">**Just-in-Time** – With the ability to customize products to customer requests, you can minimize waste by making sure that work and system changes only occur when it is necessary.</span></span>  

<span data-ttu-id="2cf33-115">In de volgende procedure ziet u hoe achterwaarts afboeken en bewerkingsplankoppelingen kunnen worden gecombineerd zodat het aantal dat per bewerking wordt afgeboekt, in verhouding staat tot de werkelijke uitvoer van de voltooide bewerking.</span><span class="sxs-lookup"><span data-stu-id="2cf33-115">The following procedure shows how to combine backward flushing and routing link codes so that the quantity that is flushed for each operation is proportional to the actual output of the finished operation.</span></span>  

## <a name="to-flush-components-according-to-operation-output"></a><span data-ttu-id="2cf33-116">Onderdelen afboeken op basis van de uitvoer van een bewerking</span><span class="sxs-lookup"><span data-stu-id="2cf33-116">To flush components according to operation output</span></span>  
1.  <span data-ttu-id="2cf33-117">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Artikelen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="2cf33-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Items**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="2cf33-118">Kies de actie **Bewerken**.</span><span class="sxs-lookup"><span data-stu-id="2cf33-118">Choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="2cf33-119">Selecteer op het sneltabblad **Aanvulling** in het veld **Methode** de optie **Voorwaarts**.</span><span class="sxs-lookup"><span data-stu-id="2cf33-119">On the **Replenishment** FastTab, in the **Flushing Method** field, select **Forward**.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="2cf33-120">Selecteer **Pick + Voorwaarts** als het onderdeel wordt gebruikt op een locatie die is ingesteld voor gestuurde opslag en pick.</span><span class="sxs-lookup"><span data-stu-id="2cf33-120">Select **Pick+ Forward** if the component is used in a location that is set up for directed put-away and pick.</span></span>  

4.  <span data-ttu-id="2cf33-121">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Bewerkingsplannen** in en klik op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="2cf33-121">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Routings**, and then choose the related link.</span></span>  
5.  <span data-ttu-id="2cf33-122">Definieer bewerkingsplankoppelingen voor elke bewerking waarbij het onderdeel wordt verbruikt.</span><span class="sxs-lookup"><span data-stu-id="2cf33-122">Define routing link codes for every operation that consumes the component.</span></span> <span data-ttu-id="2cf33-123">Zie [Procedure: Bewerkingsplannen maken](production-how-to-create-routings.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="2cf33-123">For more information, see [How to: Create Routings ](production-how-to-create-routings.md).</span></span>  
6.  <span data-ttu-id="2cf33-124">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Productiestuklijst** in en klik op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="2cf33-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Production BOM**, and then choose the related link.</span></span>  
7.  <span data-ttu-id="2cf33-125">Definieer bewerkingsplankoppelingen op basis van elk exemplaar van de component voor de bewerking waarbij de component wordt verbruikt.</span><span class="sxs-lookup"><span data-stu-id="2cf33-125">Define routing link codes from each instance of the component to the operation where it is consumed.</span></span>

    > [!IMPORTANT]  
    >  <span data-ttu-id="2cf33-126">Het onderdeel moet een bewerkingsplankoppeling naar de laatste bewerking in het bewerkingsplan hebben.</span><span class="sxs-lookup"><span data-stu-id="2cf33-126">The component must have a routing link to the last operation in the routing.</span></span>  

## <a name="see-also"></a><span data-ttu-id="2cf33-127">Zie ook</span><span class="sxs-lookup"><span data-stu-id="2cf33-127">See Also</span></span>  
[<span data-ttu-id="2cf33-128">Procedure: productiestuklijsten maken</span><span class="sxs-lookup"><span data-stu-id="2cf33-128">How to: Create Production BOMs</span></span>](production-how-to-create-production-boms.md)  
[<span data-ttu-id="2cf33-129">Productie instellen</span><span class="sxs-lookup"><span data-stu-id="2cf33-129">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="2cf33-130">[Productie](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="2cf33-130">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
<span data-ttu-id="2cf33-131">[Gepland](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="2cf33-131">[Planning](production-planning.md) </span></span>  
[<span data-ttu-id="2cf33-132">Voorraad</span><span class="sxs-lookup"><span data-stu-id="2cf33-132">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="2cf33-133">Inkoop</span><span class="sxs-lookup"><span data-stu-id="2cf33-133">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="2cf33-134">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2cf33-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>


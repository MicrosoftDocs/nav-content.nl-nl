---
title: Productie uitvoeren
description: Wanneer er voor vraag is gepland en de materialen zijn uitgegeven op basis van productiestuklijsten, kunnen de daadwerkelijke productiebewerkingen starten en vervolgens worden uitgevoerd in de volgorde die is gedefinieerd in het bewerkingsplan van de productieorder.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/26/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 1d3e6b49626aaf60f398b9f9cf8a656bd3dc4946
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="manufacturing"></a><span data-ttu-id="b24a8-103">Productie</span><span class="sxs-lookup"><span data-stu-id="b24a8-103">Manufacturing</span></span>
<span data-ttu-id="b24a8-104">Wanneer er voor vraag is gepland en de materialen zijn uitgegeven op basis van productiestuklijsten, kunnen de daadwerkelijke productiebewerkingen starten en vervolgens worden uitgevoerd in de volgorde die is gedefinieerd in het bewerkingsplan van de productieorder.</span><span class="sxs-lookup"><span data-stu-id="b24a8-104">When demand is planned for and the materials have been issued according to production BOMs, then the actual production operations can start and be executed in the sequence defined by the production order routing.</span></span>  

<span data-ttu-id="b24a8-105">Een uit systeemoogpunt belangrijk deel van de uitvoering van productie is het boeken van productie-output in de database om voortgang te melden en om de voorraad met de gereedgemelde artikelen bij te werken.</span><span class="sxs-lookup"><span data-stu-id="b24a8-105">An important part of executing production, from a system point of view, is to post production output to the database to report progress and to update inventory with the finished items.</span></span> <span data-ttu-id="b24a8-106">Output-boeking kan handmatig worden gedaan door na de productiebewerkingen dagboekregels in te vullen en te boeken.</span><span class="sxs-lookup"><span data-stu-id="b24a8-106">Output posting can be done manually, by filling and posting journal lines after production operations.</span></span> <span data-ttu-id="b24a8-107">Of het kan automatisch worden gedaan door middel van achterwaarts afboeken.</span><span class="sxs-lookup"><span data-stu-id="b24a8-107">Or, it can be done automatically with the use of backward flushing.</span></span> <span data-ttu-id="b24a8-108">In dat geval wordt materiaalverbruik automatisch samen met de output geboekt, wanneer de productieorder wordt gereedgemeld.</span><span class="sxs-lookup"><span data-stu-id="b24a8-108">In that case material consumption is automatically posted along with output when the production order changes to finished.</span></span>  

<span data-ttu-id="b24a8-109">Als alternatief voor het in batches boeken van output voor meerdere productieorders kunt u het venster **Productiedagboek** gebruiken om verbruik en/of output voor één productieorderregel te boeken.</span><span class="sxs-lookup"><span data-stu-id="b24a8-109">As an alternative to the batch journal for output posting for multiple production orders, you can use the **Production Journal** window to post consumption and/or output for one production order line.</span></span>

<span data-ttu-id="b24a8-110">Voordat u artikelen kunt gaan produceren, moet u verschillende zaken instellen, zoals afdelingen, bewerkingsplannen en productiestuklijsten.</span><span class="sxs-lookup"><span data-stu-id="b24a8-110">Before you can begin to produce items, you must make various setup, such as work centers, routings, and production BOMs.</span></span> <span data-ttu-id="b24a8-111">Zie [Productie instellen](production-configure-production-processes.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="b24a8-111">For more information, see [Setting Up Manufacturing](production-configure-production-processes.md).</span></span>

<span data-ttu-id="b24a8-112">In de volgende tabel wordt een reeks taken beschreven, met koppelingen naar de beschrijvende onderwerpen.</span><span class="sxs-lookup"><span data-stu-id="b24a8-112">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="b24a8-113">**Als u dit wilt doen**</span><span class="sxs-lookup"><span data-stu-id="b24a8-113">**To**</span></span>|<span data-ttu-id="b24a8-114">**Zie**</span><span class="sxs-lookup"><span data-stu-id="b24a8-114">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="b24a8-115">Begrijpen hoe de productieorders werken.</span><span class="sxs-lookup"><span data-stu-id="b24a8-115">Understand how production orders work.</span></span>|[<span data-ttu-id="b24a8-116">Informatie over productieorders</span><span class="sxs-lookup"><span data-stu-id="b24a8-116">About Production Orders</span></span>](production-about-production-orders.md)|
|<span data-ttu-id="b24a8-117">Handmatig productieorders maken.</span><span class="sxs-lookup"><span data-stu-id="b24a8-117">Create production orders manually.</span></span>|[<span data-ttu-id="b24a8-118">Procedure: Productieorders maken:</span><span class="sxs-lookup"><span data-stu-id="b24a8-118">How to: Create Production Orders</span></span>](production-how-to-create-production-orders.md)|
|<span data-ttu-id="b24a8-119">Alle of bepaalde bewerkingen in een productieorder uitbesteden aan een toeleverancier.</span><span class="sxs-lookup"><span data-stu-id="b24a8-119">Outsource all or selected operations in a production order to a subcontractor.</span></span>|[<span data-ttu-id="b24a8-120">Procedure: Productie uitbesteden</span><span class="sxs-lookup"><span data-stu-id="b24a8-120">How to: Subcontract Manufacturing</span></span>](production-how-to-subcontract-manufacturing.md)|
|<span data-ttu-id="b24a8-121">Productie-output en verbruikte materiaal en tijd vastleggen voor één vrijgegeven productieorderregel.</span><span class="sxs-lookup"><span data-stu-id="b24a8-121">Record and post production output along with material and time consumption for a single released production order line.</span></span>|[<span data-ttu-id="b24a8-122">Procedure: Verbruik en output boeken voor één vrijgegeven productieorderregel</span><span class="sxs-lookup"><span data-stu-id="b24a8-122">How to: Post Consumption and Output for One Released Production Order Line</span></span>](production-how-to-register-consumption-and-output.md)|  
|<span data-ttu-id="b24a8-123">Het aantal gebruikte onderdelen per bewerking in batches in een dagboek boeken waarin meerdere geplande productieorders kunnen worden verwerkt.</span><span class="sxs-lookup"><span data-stu-id="b24a8-123">Batch post the quantity of components used per operation in a journal that can processes multiple planned production orders.</span></span>|[<span data-ttu-id="b24a8-124">Procedure: Verbruik in batches boeken</span><span class="sxs-lookup"><span data-stu-id="b24a8-124">How to: Batch Post Consumption</span></span>](production-how-to-post-consumption.md)|
|<span data-ttu-id="b24a8-125">Het aantal voltooide artikelen en de bestede tijd per bewerking in een dagboek boeken waarin meerdere vrijgegeven productieorders kunnen worden verwerkt.</span><span class="sxs-lookup"><span data-stu-id="b24a8-125">Post the quantity of finished items and the time spent per operation in a journal that can processes multiple released production orders.</span></span>|[<span data-ttu-id="b24a8-126">Procedure: Output en bewerkingstijd in batches boeken</span><span class="sxs-lookup"><span data-stu-id="b24a8-126">How to: Batch Post Output and Run Times</span></span>](production-how-to-post-output-quantity.md)|  
|<span data-ttu-id="b24a8-127">Het aantal artikelen boeken dat is geproduceerd in elke voltooide bewerking, maar niet geldt als voltooide output maar als uitgevallen materiaal.</span><span class="sxs-lookup"><span data-stu-id="b24a8-127">Post the number of items produced in each finished operation which do not qualify as finished output, but as scrapped material.</span></span>|[<span data-ttu-id="b24a8-128">Procedure: Uitval boeken</span><span class="sxs-lookup"><span data-stu-id="b24a8-128">How to: Post Scrap</span></span>](production-how-to-post-scrap.md)|
|<span data-ttu-id="b24a8-129">De werklast voor de shopfloor als resultaat van geplande en vrijgegeven productieorders weergeven.</span><span class="sxs-lookup"><span data-stu-id="b24a8-129">View the shop floor load as a result of planned and released production orders.</span></span>|[<span data-ttu-id="b24a8-130">Procedure: De werklast in afdelingen en bewerkingsplaatsen weergeven</span><span class="sxs-lookup"><span data-stu-id="b24a8-130">How to: View the Load in Work and Machine Centers</span></span>](production-how-to-view-the-load-on-work-centers.md)|      
|<span data-ttu-id="b24a8-131">Het venster **Capaciteitsdagboek** gebruiken om verbruikte capaciteit te boeken die niet is toegewezen aan een productieorder, zoals onderhoudswerkzaamheden.</span><span class="sxs-lookup"><span data-stu-id="b24a8-131">Use the **Capacity Journal** window to post consumed capacities that are not assigned to a production order, such as maintenance work.</span></span>|[<span data-ttu-id="b24a8-132">Procedure: capaciteit boeken</span><span class="sxs-lookup"><span data-stu-id="b24a8-132">How to: Post Capacities</span></span>](production-how-to-post-capacities.md)|  
|<span data-ttu-id="b24a8-133">De kosten van gereedgemelde productieartikelen en verbruikte materialen berekenen en aanpassen voor financiële reconciliatie.</span><span class="sxs-lookup"><span data-stu-id="b24a8-133">Calculate and adjust the cost of finished production items and consumed components for financial reconciliation.</span></span>|[<span data-ttu-id="b24a8-134">Over de kosten van de gereedgemelde productieorder</span><span class="sxs-lookup"><span data-stu-id="b24a8-134">About Finished Production Order Costs</span></span>](finance-about-finished-production-order-costs.md)|  

## <a name="see-also"></a><span data-ttu-id="b24a8-135">Zie ook</span><span class="sxs-lookup"><span data-stu-id="b24a8-135">See Also</span></span>  
[<span data-ttu-id="b24a8-136">Productie instellen</span><span class="sxs-lookup"><span data-stu-id="b24a8-136">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="b24a8-137">[Gepland](production-planning.md)    </span><span class="sxs-lookup"><span data-stu-id="b24a8-137">[Planning](production-planning.md)    </span></span>  
[<span data-ttu-id="b24a8-138">Voorraad</span><span class="sxs-lookup"><span data-stu-id="b24a8-138">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="b24a8-139">Inkoop</span><span class="sxs-lookup"><span data-stu-id="b24a8-139">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="b24a8-140">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b24a8-140">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

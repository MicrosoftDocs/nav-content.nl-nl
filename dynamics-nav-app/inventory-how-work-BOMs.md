---
title: Werken met stuklijsten om onderdelen te beheren
description: U maakt een assemblagestuklijst om de onderdelen of resources op te geven die vereist zijn om het artikel samen te stellen dat de assemblagestuklijst vertegenwoordigt.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 09/04/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 9515ab4e5fc1003fd175c0946aeaceba33dac825
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-work-with-bills-of-material"></a><span data-ttu-id="26660-103">Procedure: Werken met stuklijsten</span><span class="sxs-lookup"><span data-stu-id="26660-103">How to: Work with Bills of Material</span></span>
<span data-ttu-id="26660-104">U gebruikt stuklijsten om bovenliggende artikelen te structureren die door resources of bewerkingsplaatsen moeten worden geassembleerd of geproduceerd van onderdelen.</span><span class="sxs-lookup"><span data-stu-id="26660-104">You use bills of materials (BOMs) to structure parent items that must be assembled or produced by resources or machine centers from components.</span></span> <span data-ttu-id="26660-105">Er kan ook een assemblagestuklijst worden gebruikt om een hoofdartikel als pakketten bestaande uit de onderdelen te verkopen.</span><span class="sxs-lookup"><span data-stu-id="26660-105">An assembly BOM can also be used to sell a parent item as a kit consisting of its components.</span></span>

## <a name="assembly-boms-or-production-boms"></a><span data-ttu-id="26660-106">Assemblagestuklijsten of productiestuklijsten</span><span class="sxs-lookup"><span data-stu-id="26660-106">Assembly BOMs or Production BOMs</span></span>
<span data-ttu-id="26660-107">U gebruikt assemblageorders voor het maken van eindartikelen van onderdelen in een eenvoudig proces dat kan worden uitgevoerd door een of meer standaardbronnen die geen bewerkingsplaatsen of -afdelingen betreffen of waarbij geen bronnen gebruikt worden.</span><span class="sxs-lookup"><span data-stu-id="26660-107">You use assembly orders for making end items from components in a simple process that can be performed by one or more basic resources, which are not machine or work centers, or without any resources.</span></span> <span data-ttu-id="26660-108">Een assemblageproces kan bijvoorbeeld zijn het picken van twee flessen wijn en één pak koffie en deze als een cadeau-item verpakken.</span><span class="sxs-lookup"><span data-stu-id="26660-108">For example, an assembly process could be to pick two wine bottles and one coffee sack and then pack them as a gift item.</span></span>  

<span data-ttu-id="26660-109">Een assemblagestuklijst betreft de hoofdgegevens die bepalen welke onderdelen gebruikt worden in een samengesteld eindartikel en welke bronnen gebruikt worden voor het samenstellen van het assemblageartikel.</span><span class="sxs-lookup"><span data-stu-id="26660-109">An assembly BOM is the master data that defines which component items go into an assembled end item and which resources are used to assemble the assembly item.</span></span> <span data-ttu-id="26660-110">Wanneer u een assemblageartikel en een aantal in een nieuwe assemblageorderkop invoert, worden de assemblageorderregels automatisch op basis van de assemblagestuklijst gevuld met één assemblageorderregel per onderdeel of bron.</span><span class="sxs-lookup"><span data-stu-id="26660-110">When you enter an assembly item and a quantity in the header of a new assembly order, then the assembly order lines are automatically filled according to the assembly BOM with one assembly order line per component or resource.</span></span> <span data-ttu-id="26660-111">Zie voor meer informatie [Assemblagebeheer](assembly-assemble-items.md).</span><span class="sxs-lookup"><span data-stu-id="26660-111">For more information, see [Assembly Management](assembly-assemble-items.md).</span></span>

<span data-ttu-id="26660-112">Assemblagestuklijsten worden in dit onderwerp beschreven.</span><span class="sxs-lookup"><span data-stu-id="26660-112">Assembly BOMs are described in this topic.</span></span>

<span data-ttu-id="26660-113">U gebruikt productieorders voor het maken van eindartikelen van onderdelen in een complex proces, waarvoor een productiebewerkingsplan en bewerkingsplaatsen of -afdelingen nodig zijn die productiecapaciteit vertegenwoordigen.</span><span class="sxs-lookup"><span data-stu-id="26660-113">You use production orders for making end items from components in a complex process that requires a production routing and work or machine centers, which represent production capacities.</span></span> <span data-ttu-id="26660-114">Een productieproces kan bijvoorbeeld zijn het knippen van stalen platen in één bewerking, deze lassen in een volgende bewerking en het eindartikel verfen in de laatste bewerking.</span><span class="sxs-lookup"><span data-stu-id="26660-114">For example, a production process could be to cut steel plates in one operation, weld them in the next operation, and paint the end item in the last operation.</span></span> <span data-ttu-id="26660-115">Zie [Productie](production-manage-manufacturing.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="26660-115">For more information, see [Manufacturing](production-manage-manufacturing.md).</span></span>  

<span data-ttu-id="26660-116">Een productiestuklijst is de stamgegevens die een productieartikel en de componenten erin definieert.</span><span class="sxs-lookup"><span data-stu-id="26660-116">A production BOM is the master data that defines a production item and the components that go into it.</span></span> <span data-ttu-id="26660-117">voor componenten moet de productiestuklijst worden gecertificeerd en toegewezen aan het productieartikel voordat het in een productieorder kan worden gebruikt.</span><span class="sxs-lookup"><span data-stu-id="26660-117">for assembly items, the production BOM must be certified and assigned to the production item before it can be used in a production order.</span></span> <span data-ttu-id="26660-118">Wanneer u het productieartikel op een productieorderregel handmatig of door het vernieuwen van de order invoert, wordt de inhoud van de productiestuklijst omgezet in de onderdelen van de productieorder .</span><span class="sxs-lookup"><span data-stu-id="26660-118">When you enter the production item on a production order line, either manually or by refreshing the order, then the production BOM content becomes the production order components.</span></span> <span data-ttu-id="26660-119">Zie voor meer informatie [Procedure: productiestuklijsten maken](production-how-to-create-production-boms.md).</span><span class="sxs-lookup"><span data-stu-id="26660-119">For more information, see [How to: Create Production BOMs](production-how-to-create-production-boms.md).</span></span>  

<span data-ttu-id="26660-120">Het concept van bronnen in de productie is veel geavanceerder dan in de assemblage.</span><span class="sxs-lookup"><span data-stu-id="26660-120">The concept of resources in production is much more advanced than in assembly management.</span></span> <span data-ttu-id="26660-121">Werkplaatsen en machinecentra fungeren als bronnen en productiestappen worden vertegenwoordigd door bewerkingen die zijn toegewezen aan bronnen in productiebewerkingsplannen.</span><span class="sxs-lookup"><span data-stu-id="26660-121">Work centers and machine centers function as resources, and production steps are represented by operations that are assigned to resources in production routings.</span></span> <span data-ttu-id="26660-122">Zie [Procedure: Bewerkingsplannen maken](production-how-to-create-routings.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="26660-122">For more information, see [How to: Create Routings](production-how-to-create-routings.md).</span></span>

<span data-ttu-id="26660-123">Zowel assemblage- als productieorders kunnen rechtstreeks aan verkooporders worden gekoppeld.</span><span class="sxs-lookup"><span data-stu-id="26660-123">Both assembly orders and production orders may be linked directly to sales orders.</span></span> <span data-ttu-id="26660-124">U kunt echter alleen assemblageorders gebruiken om het eindartikel rechtstreeks voor een klantverzoek aan de verkooporder te koppelen.</span><span class="sxs-lookup"><span data-stu-id="26660-124">However, you can only use assembly orders to customize the end item directly for a customer request with the sales order.</span></span>

## <a name="to-create-an-assembly-bom"></a><span data-ttu-id="26660-125">Een assemblagestuklijst maken</span><span class="sxs-lookup"><span data-stu-id="26660-125">To create an assembly BOM</span></span>
<span data-ttu-id="26660-126">Als u een bovenliggend artikel wilt definiëren dat bestaat uit andere artikelen, en mogelijk uit resources die nodig zijn om het bovenliggende artikel samen te stellen, moet u een assemblagestuklijst maken.</span><span class="sxs-lookup"><span data-stu-id="26660-126">To define a parent item that consists of other items, and potentially of resources required to put the parent together, you must create an assembly BOM.</span></span>  

<span data-ttu-id="26660-127">Assemblagestuklijsten bevatten gewoonlijk artikelen, maar kunnen ook een of meer resources bevatten die het assemblageartikel samenstellen.</span><span class="sxs-lookup"><span data-stu-id="26660-127">Assembly BOMs usually contain items but can also contain one or more resources that are required to put the assembly item together.</span></span>

<span data-ttu-id="26660-128">Assemblagestuklijsten kunnen meerdere niveaus bevatten, wat betekent dat een onderdeel op de assemblagestuklijst zelf ook een assemblageartikel kan zijn.</span><span class="sxs-lookup"><span data-stu-id="26660-128">Assembly BOMs can have multiple levels, which means that a component on the assembly BOM can be an assembly item itself.</span></span> <span data-ttu-id="26660-129">In dat geval bevat het veld **Assemblagestuklijst** op de assemblagestuklijstregel **Ja**.</span><span class="sxs-lookup"><span data-stu-id="26660-129">In that case, the **Assembly BOM** field on the assembly BOM line contains **Yes**.</span></span>

<span data-ttu-id="26660-130">Er gelden speciale vereisten voor artikelen op assemblagestuklijsten met betrekking tot beschikbaarheid.</span><span class="sxs-lookup"><span data-stu-id="26660-130">Special requirements apply to items on assembly BOMs with regards to availability.</span></span> <span data-ttu-id="26660-131">Zie het gedeelte 'De beschikbaarheid van een artikel bekijken op basis van het gebruik ervan in assemblagestuklijsten' in [Procedure: De beschikbaarheid van artikelen weergeven](inventory-how-availability-overview.md).</span><span class="sxs-lookup"><span data-stu-id="26660-131">For more information, see the "To see the availability of an item by its use in assembly BOMs" section in [How to: View the Availability of Items](inventory-how-availability-overview.md).</span></span>

<span data-ttu-id="26660-132">Het maken van een assemblagestuklijst bestaat uit twee delen:</span><span class="sxs-lookup"><span data-stu-id="26660-132">There are two parts to creating an assembly BOM:</span></span>
- <span data-ttu-id="26660-133">Een nieuw artikel instellen</span><span class="sxs-lookup"><span data-stu-id="26660-133">Setting up a new item</span></span>
- <span data-ttu-id="26660-134">De stuklijststructuur van het assemblageartikel definiëren.</span><span class="sxs-lookup"><span data-stu-id="26660-134">Defining the BOM structure of the assembly item.</span></span>

1. <span data-ttu-id="26660-135">Stel een nieuw artikel in.</span><span class="sxs-lookup"><span data-stu-id="26660-135">Set up a new item.</span></span> <span data-ttu-id="26660-136">Zie [Procedure: Nieuwe artikelen registreren](inventory-how-register-new-items.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="26660-136">For more information, see [How to: Register New Items](inventory-how-register-new-items.md).</span></span>

    <span data-ttu-id="26660-137">Ga verder om onderdelen of resources in de assemblagestuklijst in te voeren.</span><span class="sxs-lookup"><span data-stu-id="26660-137">Proceed to enter components or resources on the assembly BOM.</span></span>  
2. <span data-ttu-id="26660-138">Kies in het venster **Artikel** voor een assemblageartikel de actie **Assemblage** en kies vervolgens de actie **Assemblagestuklijst**.</span><span class="sxs-lookup"><span data-stu-id="26660-138">In the **Item Card** window for an assembly item, choose the **Assembly** action, and then choose the **Assembly BOM** action.</span></span>
3. <span data-ttu-id="26660-139">Vul indien nodig de velden in het venster **Assemblagestuklijst** in.</span><span class="sxs-lookup"><span data-stu-id="26660-139">In the **Assembly BOM** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-view-the-components-of-an-assembly-item-indented-according-to-the-bom-structure"></a><span data-ttu-id="26660-140">De onderdelen van een assemblageartikel weergeven terwijl het is ingesprongen volgens de stuklijststructuur</span><span class="sxs-lookup"><span data-stu-id="26660-140">To view the components of an assembly item indented according to the BOM structure</span></span>
<span data-ttu-id="26660-141">Vanuit het venster **Assemblagestuklijst** kunt u een afzonderlijk venster openen dat de onderdelen en resources bevat die zijn ingesprongen op basis van hun stuklijstpositie onder het assemblageartikel.</span><span class="sxs-lookup"><span data-stu-id="26660-141">From the **Assembly BOM** window, you can open a separate window that shows the components and any resources indented according to their BOM position under the assembly item.</span></span>

1. <span data-ttu-id="26660-142">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Artikelen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="26660-142">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="26660-143">Open de kaart voor een assemblageartikel.</span><span class="sxs-lookup"><span data-stu-id="26660-143">Open the card for an assembly item.</span></span> <span data-ttu-id="26660-144">(Het veld **Assemblagestuklijst** in het venster **Artikelen** bevat **Ja**.)</span><span class="sxs-lookup"><span data-stu-id="26660-144">(The **Assembly BOM** field in the **Items** window contains **Yes**.)</span></span>
3. <span data-ttu-id="26660-145">Kies in het venster **Artikel** de actie **Assemblage** en kies vervolgens de actie **Assemblagestuklijst**.</span><span class="sxs-lookup"><span data-stu-id="26660-145">In the **Item Card** window, choose the **Assembly** action, and then choose the **Assembly BOM** action.</span></span>
4. <span data-ttu-id="26660-146">Kies in het venster **Assemblagestuklijst** de actie **Stuklijst weergeven**.</span><span class="sxs-lookup"><span data-stu-id="26660-146">In the **Assembly BOM** window, choose the **Show BOM** action.</span></span>

## <a name="to-replace-the-assembly-item-with-its-components-on-document-lines"></a><span data-ttu-id="26660-147">Het assemblageartikel in documentregels vervangen door de samenstellende onderdelen</span><span class="sxs-lookup"><span data-stu-id="26660-147">To replace the assembly item with its components on document lines</span></span>
<span data-ttu-id="26660-148">Vanuit ieder in- of verkoopdocument dat een assemblageartikel bevat, kunt u de regel voor dit artikel door middel van een speciale functie vervangen door nieuwe regels voor de samenstellende onderdelen ervan.</span><span class="sxs-lookup"><span data-stu-id="26660-148">From any sales and purchase document that contains an assembly item, you can use a special function to replace the line for the assembly item with new lines for its components.</span></span> <span data-ttu-id="26660-149">Deze functie bijvoorbeeld nuttig als u de onderdelen wilt verkopen als een kit die samen het assemblageartikel vertegenwoordigen.</span><span class="sxs-lookup"><span data-stu-id="26660-149">This function is useful, for example, if you want to sell the components as a kit that represents the assembly item.</span></span>

<span data-ttu-id="26660-150">**Pas op**: Wanneer u de functie **Stuklijst weergeven** hebt gebruikt, kunt u dit niet gemakkelijk ongedaan maken.</span><span class="sxs-lookup"><span data-stu-id="26660-150">**Caution**: When you have used the **Explode BOM** function, you cannot easily undo it.</span></span> <span data-ttu-id="26660-151">U moet dan de verkooporderregels die de onderdelen vertegenwoordigen verwijderen, en vervolgens opnieuw een verkooporderregel voor het assemblageartikel invoeren.</span><span class="sxs-lookup"><span data-stu-id="26660-151">You must delete the sales order lines representing the components and then reenter a sales order line for the assembly item.</span></span>

<span data-ttu-id="26660-152">De volgende procedure is gebaseerd op een verkoopfactuur.</span><span class="sxs-lookup"><span data-stu-id="26660-152">The following procedure is based on a sales invoice.</span></span> <span data-ttu-id="26660-153">Dezelfde stappen zijn van toepassing op andere verkoopdocumenten en op alle inkoopdocumenten.</span><span class="sxs-lookup"><span data-stu-id="26660-153">The same steps apply to other sales documents and to all purchase documents.</span></span>

1. <span data-ttu-id="26660-154">Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Verkoopfacturen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="26660-154">In the top right corner, choose the **Search for Page or Report** icon, enter **Sales Invoices**, and then choose the related link.</span></span>
2. <span data-ttu-id="26660-155">Open een verkoopfactuur die een regel voor een assemblageartikel bevat.</span><span class="sxs-lookup"><span data-stu-id="26660-155">Open a sales invoice that contains a line for an assembly item.</span></span>
3. <span data-ttu-id="26660-156">Selecteer de regel een assemblageartikel en klik vervolgens op de regelactie **Stuklijst weergeven**.</span><span class="sxs-lookup"><span data-stu-id="26660-156">Choose the line for an assembly item, and then **Explode BOM** line action.</span></span>

<span data-ttu-id="26660-157">Alle velden op de verkoopfactuurregel voor het assemblageartikel worden worden gewist, behalve de velden **Artikel** en **Beschrijving**.</span><span class="sxs-lookup"><span data-stu-id="26660-157">All fields on the sales invoice line for the assembly item are cleared except for the **Item** and **Description** fields.</span></span> <span data-ttu-id="26660-158">Volledige verkoopfactuurregels worden ingevoegd voor de onderdelen en mogelijke resources, waaruit het assemblageartikel is opgebouwd.</span><span class="sxs-lookup"><span data-stu-id="26660-158">Complete sales invoice lines are inserted for the components and possible resources that comprise the assembly item.</span></span>

<span data-ttu-id="26660-159">**Opmerking**: De functie Stuklijst weergeven is ook beschikbaar in het venster **Assemblagestuklijst**.</span><span class="sxs-lookup"><span data-stu-id="26660-159">**Note**: The Explode BOM function is also available in the **Assembly BOM** window.</span></span>

## <a name="to-calculate-the-standard-cost-of-an-assembly-item"></a><span data-ttu-id="26660-160">De vaste verrekenprijs van een assemblageartikel berekenen</span><span class="sxs-lookup"><span data-stu-id="26660-160">To calculate the standard cost of an assembly item</span></span>
<span data-ttu-id="26660-161">U berekent de kostprijs van een assemblageartikel door de kostprijs van elk onderdeel en elke resource in de assemblagestuklijst bij elkaar op te tellen.</span><span class="sxs-lookup"><span data-stu-id="26660-161">You calculate the unit cost of an assembly item by rolling up the unit cost of each component and resource in the item’s assembly BOM.</span></span>

<span data-ttu-id="26660-162">U kunt de vaste verrekenprijs voor een of meerdere artikelen ook berekenen en bijwerken in het venster **Vaste-verrekenprijsvoorstel**.</span><span class="sxs-lookup"><span data-stu-id="26660-162">You can also calculate and update the standard cost for one or many items in the **Standard Cost Worksheet** window.</span></span> <span data-ttu-id="26660-163">Zie [Procedure: Vaste verrekenprijzen aanpassen](finance-how-to-update-standard-costs.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="26660-163">For more information, see [How to: Update Standard Costs](finance-how-to-update-standard-costs.md).</span></span>  

<span data-ttu-id="26660-164">De kostprijs van een assemblagestuklijst is altijd gelijk aan het totaal van de kostprijzen van de verschillende componenten, inclusief overige assemblagestuklijsten, en eventuele resources.</span><span class="sxs-lookup"><span data-stu-id="26660-164">The unit cost of an assembly BOM always equals the total of the unit costs of its components, including other assembly BOMs, and any resources.</span></span>

1. <span data-ttu-id="26660-165">Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Artikelen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="26660-165">In the top right corner, choose the **Search for Page or Report** icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="26660-166">Open de kaart voor een assemblageartikel.</span><span class="sxs-lookup"><span data-stu-id="26660-166">Open the card for an assembly item.</span></span> <span data-ttu-id="26660-167">(Het veld **Assemblagestuklijst** in het venster **Artikelen** bevat **Ja**.)</span><span class="sxs-lookup"><span data-stu-id="26660-167">(The **Assembly BOM** field in the **Items** window contains **Yes**.)</span></span>
3. <span data-ttu-id="26660-168">Kies in het venster **Artikel** de actie **Assemblage** en kies vervolgens de actie **Assemblagestuklijst**.</span><span class="sxs-lookup"><span data-stu-id="26660-168">In the **Item Card** window, choose the **Assembly** action, and then choose the **Assembly BOM** action.</span></span>
4. <span data-ttu-id="26660-169">Kies in het venster **Assemblagestuklijst** de actie **Vaste verrekenprijs berekenen**.</span><span class="sxs-lookup"><span data-stu-id="26660-169">In the **Assembly BOM** window, choose the **Calc. Standard Cost** action.</span></span>
5. <span data-ttu-id="26660-170">Selecteer een van de volgende opties en kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="26660-170">Select one of the following options, and then choose the **OK** button.</span></span>

|<span data-ttu-id="26660-171">Optie</span><span class="sxs-lookup"><span data-stu-id="26660-171">Option</span></span> |<span data-ttu-id="26660-172">Description</span><span class="sxs-lookup"><span data-stu-id="26660-172">Description</span></span> |
|-------|------------|
|<span data-ttu-id="26660-173">**Hoogste niveau**</span><span class="sxs-lookup"><span data-stu-id="26660-173">**Top Level**</span></span>|<span data-ttu-id="26660-174">Berekent de vaste verrekenprijs van het assemblageartikel als de totale kosten van alle gekochte of geassembleerde artikelen op die assemblagestuklijst, ongeacht eventuele onderliggende assemblagestuklijsten.</span><span class="sxs-lookup"><span data-stu-id="26660-174">Calculates the assembly item's standard cost as the total cost of all purchased or assembled items on that assembly BOM regardless of any underlying assembly BOMs.</span></span>|
|<span data-ttu-id="26660-175">**Alle niveaus**</span><span class="sxs-lookup"><span data-stu-id="26660-175">**All Levels**</span></span>|<span data-ttu-id="26660-176">Berekent de vaste verrekenprijs voor het assemblageartikel als de som van: 1) De berekende kosten van alle onderliggende assemblagestuklijsten op de assemblagestuklijst.</span><span class="sxs-lookup"><span data-stu-id="26660-176">Calculates the assembly's item standard cost as the sum of: 1) The calculated cost of all underlying assembly BOMs on the assembly BOM.</span></span> <span data-ttu-id="26660-177">2) De kosten van alle ingekochte artikelen op de assemblagestuklijst.</span><span class="sxs-lookup"><span data-stu-id="26660-177">2) The cost of all purchased items on the assembly BOM.</span></span>|



<span data-ttu-id="26660-178">De kosten van de artikelen waaruit de assemblagestuklijst bestaat, worden gekopieerd van artikelkaarten van de componenten.</span><span class="sxs-lookup"><span data-stu-id="26660-178">The costs of the items that make up the assembly BOM are copied from the component item cards.</span></span> <span data-ttu-id="26660-179">De kosten van elk artikel worden vermenigvuldigd met het aantal, en de totale kostprijs wordt weergegeven in het venster **Kostprijs** op de artikelkaart.</span><span class="sxs-lookup"><span data-stu-id="26660-179">The cost of each item is multiplied by the quantity, and the total cost is shown in the **Unit Cost** field on the item card.</span></span>

## <a name="see-also"></a><span data-ttu-id="26660-180">Zie ook</span><span class="sxs-lookup"><span data-stu-id="26660-180">See Also</span></span>
[<span data-ttu-id="26660-181">Procedure: Nieuwe artikelen registreren</span><span class="sxs-lookup"><span data-stu-id="26660-181">How to: Register New Items</span></span>](inventory-how-register-new-items.md)  
<span data-ttu-id="26660-182">[Procedure: beschikbaarheid van artikelen weergeven](inventory-how-availability-overview.md)   </span><span class="sxs-lookup"><span data-stu-id="26660-182">[How to: View the Availability of Items](inventory-how-availability-overview.md)   </span></span>  
[<span data-ttu-id="26660-183">Voorraad</span><span class="sxs-lookup"><span data-stu-id="26660-183">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="26660-184">[Werken met [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="26660-184">[Working with [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](ui-work-product.md)</span></span>

---
title: Artikelen verzenden
description: "Afhankelijk van de magazijnconfiguratie, kunt u de verzending direct registreren in het gerelateerde uitgaande bedrijfsdocument, zoals een verkooporder, of magazijnverzendingsdocumenten gebruiken die deel uitmaken van een werkstroom en met verschillende magazijnactiviteiten zijn geïntegreerd."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 121f1e32d1fa265d4e059dc0ee43fad22f732472
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-ship-items"></a><span data-ttu-id="983bd-103">Procedure: Artikelen verzenden</span><span class="sxs-lookup"><span data-stu-id="983bd-103">How to: Ship Items</span></span>
<span data-ttu-id="983bd-104">Wanneer u artikelen verzendt vanuit een magazijn waarvoor magazijnverzendingsverwerking niet is ingesteld, registreert u de verzending in het gerelateerde bedrijfsdocument, zoals een verkooporder, serviceorder, inkoopretourorder of uitgaande transferorder.</span><span class="sxs-lookup"><span data-stu-id="983bd-104">When you ship items from a warehouse that is not set up for warehouse shipment processing, you simply record the shipment on the related business document, such as a sales order, service order, purchase return order, or outbound transfer order.</span></span>

<span data-ttu-id="983bd-105">Als u artikelen verzendt vanuit een magazijn met magazijnverzendingsverwerking, kunt u artikelen alleen verzenden op basis van brondocumenten die door andere afdelingen zijn vrijgegeven voor magazijnactiviteiten.</span><span class="sxs-lookup"><span data-stu-id="983bd-105">When you ship items from a warehouse that is set up warehouse shipment processing, you can ship items only on the basis of source documents that other company units have released to the warehouse for action.</span></span>

> [!NOTE]
> <span data-ttu-id="983bd-106">Als u in uw magazijn met cross-docking en opslaglocaties werkt, kunt u voor elke regel u zien hoeveel artikelen in de cross-dockopslaglocaties zijn geplaatst. Deze aantallen worden automatisch berekend wanneer de velden op de verzending worden bijgewerkt.</span><span class="sxs-lookup"><span data-stu-id="983bd-106">If your warehouse uses cross-docking and bins, for each line, you can view the quantity of items that have been placed in the cross-dock bins. The program calculates these quantities automatically whenever the fields on the shipment are updated.</span></span> <span data-ttu-id="983bd-107">Als dit de artikelen voor de voorbereide verzending zijn, kunt u een pick maken voor alle regels en de verzendingen vervolgens voltooien.</span><span class="sxs-lookup"><span data-stu-id="983bd-107">If they are the items that apply to the shipment you are preparing, you can create a pick for all the lines and then complete the shipment.</span></span> <span data-ttu-id="983bd-108">Zie [Procedure: Artikelen cross-docken](warehouse-how-to-cross-dock-items.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="983bd-108">For more information, see [How to: Cross-Dock Items](warehouse-how-to-cross-dock-items.md).</span></span>

## <a name="to-ship-items-with-a-sales-order"></a><span data-ttu-id="983bd-109">Artikelen verzenden met een verkooporder</span><span class="sxs-lookup"><span data-stu-id="983bd-109">To ship items with a sales order</span></span>
<span data-ttu-id="983bd-110">Hieronder wordt beschreven hoe u artikelen ontvangt met een inkooporder.</span><span class="sxs-lookup"><span data-stu-id="983bd-110">The following describes how to receive items with a purchase order.</span></span> <span data-ttu-id="983bd-111">De stappen zijn vergelijkbaar voor inkoopretourorders, serviceorders en uitgaande transferorders.</span><span class="sxs-lookup"><span data-stu-id="983bd-111">The steps are similar for purchase return orders, service orders, and outbound transfer orders.</span></span>  
1. <span data-ttu-id="983bd-112">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Verkooporders** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="983bd-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="983bd-113">Open een bestaande verkooporder of maak een nieuwe.</span><span class="sxs-lookup"><span data-stu-id="983bd-113">Open an existing sales order, or create a new one.</span></span> <span data-ttu-id="983bd-114">Zie [Procedure: Producten verkopen](sales-how-sell-products.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="983bd-114">For more information, see [How to: Sell Products](sales-how-sell-products.md).</span></span>
3. <span data-ttu-id="983bd-115">Voer in het veld **Te verzenden aantal** het aantal in dat u hebt ontvangen.</span><span class="sxs-lookup"><span data-stu-id="983bd-115">In the **Qty. to Ship** field, enter the received quantity.</span></span>

    <span data-ttu-id="983bd-116">De waarde in het veld **Verzonden aantal** wordt dienovereenkomstig bijgewerkt.</span><span class="sxs-lookup"><span data-stu-id="983bd-116">The value in the **Qty. Shipped** field is updated.</span></span> <span data-ttu-id="983bd-117">Als het een gedeeltelijke verzending is, is de waarde lager dan de waarde in het veld **Aantal**.</span><span class="sxs-lookup"><span data-stu-id="983bd-117">If this is a partial shipment, then the value is lower than the value in the **Quantity** field.</span></span>
4. <span data-ttu-id="983bd-118">Kies de actie **Boeken**.</span><span class="sxs-lookup"><span data-stu-id="983bd-118">Choose the **Post** action.</span></span>

## <a name="to-ship-items-with-a-warehouse-shipment"></a><span data-ttu-id="983bd-119">Artikelen verzenden met een magazijnverzending</span><span class="sxs-lookup"><span data-stu-id="983bd-119">To ship items with a warehouse shipment</span></span>
<span data-ttu-id="983bd-120">Eerst maakt u een verzendingsdocument op basis van een bedrijfsbrondocument.</span><span class="sxs-lookup"><span data-stu-id="983bd-120">First you create a shipment document from a business source document.</span></span> <span data-ttu-id="983bd-121">Vervolgens pickt u de opgegeven artikelen voor de verzending.</span><span class="sxs-lookup"><span data-stu-id="983bd-121">Then you pick the specified items for the shipment.</span></span>

### <a name="to-create-a-warehouse-shipment"></a><span data-ttu-id="983bd-122">Een magazijnverzending maken</span><span class="sxs-lookup"><span data-stu-id="983bd-122">To create a warehouse shipment</span></span>
<span data-ttu-id="983bd-123">Gewoonlijk maakt de werknemer die verantwoordelijk voor verzendingen is een magazijnverzending.</span><span class="sxs-lookup"><span data-stu-id="983bd-123">Typically, employee responsible for shipping creates a warehouse shipment.</span></span>
1.  <span data-ttu-id="983bd-124">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Magazijnverzendingen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="983bd-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Warehouse Shipments**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="983bd-125">Kies de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="983bd-125">Choose the **New** action.</span></span>  

    <span data-ttu-id="983bd-126">Vul de velden op het sneltabblad **Algemeen** in.</span><span class="sxs-lookup"><span data-stu-id="983bd-126">Fill in the fields on **General** FastTab.</span></span> <span data-ttu-id="983bd-127">Bij het ophalen van brondocumentregels worden bepaalde gegevens automatisch naar elke regel gekopieerd.</span><span class="sxs-lookup"><span data-stu-id="983bd-127">When you retrieve source document lines, some of the information is copied to each line.</span></span>  

    <span data-ttu-id="983bd-128">Voor magazijnconfiguraties met gestuurde opslag en pick: als de vestiging een standaardzone en -opslaglocatie voor verzendingen heeft, worden de velden **Zone** en **Opslaglocatie** automatisch ingevuld. U kunt deze waarden desgewenst wijzigen.</span><span class="sxs-lookup"><span data-stu-id="983bd-128">For warehouse configuration with directed put-away and pick, if the location has a default zone and bin for shipments, the **Zone Code** and **Bin Code** fields are filled in automatically, but you can change them as appropriate.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="983bd-129">Als u artikelen wilt verzenden met andere magazijnklassen dan de magazijnklasse van de opslaglocatie in het veld **Opslaglocatie** in de documentkop, moet u de inhoud van het veld **Opslaglocatie** in de kop verwijderen voordat u de brondocumentregels voor de artikelen ophaalt.</span><span class="sxs-lookup"><span data-stu-id="983bd-129">If you wish to ship items with warehouse class codes other than the class code of the bin in the **Bin Code** field on the document header, you must delete the contents of the **Bin Code** field on the header before you retrieve source document lines for the items.</span></span>  
3.  <span data-ttu-id="983bd-130">Kies de actie **Brondocumenten ophalen**.</span><span class="sxs-lookup"><span data-stu-id="983bd-130">Choose the **Get Source Documents** action.</span></span> <span data-ttu-id="983bd-131">Het venster **Brondocumenten** verschijnt.</span><span class="sxs-lookup"><span data-stu-id="983bd-131">The **Source Documents** window opens.</span></span>

    <span data-ttu-id="983bd-132">U kunt vanuit een nieuwe of geopende magazijnverzending het venster **Filters om brondoc. op te halen** gebruiken voor het ophalen van de vrijgegeven brondocumentregels die bepalen welke artikelen moeten worden verzonden.</span><span class="sxs-lookup"><span data-stu-id="983bd-132">From a new or an open warehouse shipment, you can use the **Filters to Get Source Docs.** window to retrieve the released source document lines that define which items to ship.</span></span>

    1. <span data-ttu-id="983bd-133">Kies de actie **Filters om brondoc. op te halen gebruiken**.</span><span class="sxs-lookup"><span data-stu-id="983bd-133">Choose the **Use Filters to Get Src. Docs.** action.</span></span>  
    2. <span data-ttu-id="983bd-134">U stelt een nieuw filter in door een omschrijvende code in te voeren in het veld **Code** en vervolgens de actie **Wijzigen** te kiezen.</span><span class="sxs-lookup"><span data-stu-id="983bd-134">To set up a new filter, enter a descriptive code in the **Code** field, and then choose the **Modify** action.</span></span>  
    3. <span data-ttu-id="983bd-135">Definieer het soort brondocumentregels dat u wilt ophalen door de relevante filtervelden in te vullen.</span><span class="sxs-lookup"><span data-stu-id="983bd-135">Define the type of source document lines that you want to retrieve by filling in the relevant filter fields.</span></span>  
    4. <span data-ttu-id="983bd-136">Kies de actie **Uitvoeren**.</span><span class="sxs-lookup"><span data-stu-id="983bd-136">Choose the **Run** action.</span></span>  

    <span data-ttu-id="983bd-137">Alle vrijgegeven brondocumentregels die voldoen aan de filtercriteria worden nu ingevoegd in het venster **Mag. -verzending** van waaruit u de filterfunctie hebt geactiveerd.</span><span class="sxs-lookup"><span data-stu-id="983bd-137">All released source document lines that fulfill the filter criteria are now inserted in **Warehouse Shipment** window from which you activated the filter function.</span></span>  

    <span data-ttu-id="983bd-138">De filtercombinaties die u definieert, worden opgeslagen in het venster **Filters om brondoc. op te halen** tot de volgende keer dat u deze nodig hebt.</span><span class="sxs-lookup"><span data-stu-id="983bd-138">The filter combinations that you define are saved in the **Filters to Get Source Docs.** window until the next time you need it.</span></span> <span data-ttu-id="983bd-139">U kunt een onbeperkt aantal filtercombinaties maken.</span><span class="sxs-lookup"><span data-stu-id="983bd-139">You can make an unlimited number of filter combinations.</span></span> <span data-ttu-id="983bd-140">U kunt de criteria op elk moment wijzigen door de actie **Wijzigen** te kiezen.</span><span class="sxs-lookup"><span data-stu-id="983bd-140">You can change the criteria at any time by choosing the **Modify** action.</span></span>

4.  <span data-ttu-id="983bd-141">Selecteer de brondocumenten waarvoor u artikelen wilt verzenden en klik op **OK**.</span><span class="sxs-lookup"><span data-stu-id="983bd-141">Select the source documents for which you want to ship items, and then choose the **OK** button.</span></span>  

<span data-ttu-id="983bd-142">De regels van de brondocumenten verschijnen in het venster **Mag. -verzending**.</span><span class="sxs-lookup"><span data-stu-id="983bd-142">The lines of the source documents appear in the **Warehouse Shipment** window.</span></span> <span data-ttu-id="983bd-143">Het veld **Te verzenden aantal** is ingevuld met de openstaande hoeveelheid voor elke regel, maar u kunt het aantal wijzigen indien nodig.</span><span class="sxs-lookup"><span data-stu-id="983bd-143">The **Qty. to Ship** field is filled with the quantity outstanding for each line, but you can change the quantity as necessary.</span></span> <span data-ttu-id="983bd-144">Als u de inhoud van het veld **Opslaglocatie** op het sneltabblad **Algemeen** verwijdert voordat u de regels ophaalt, moet u op elke verzendregel een opslaglocatie invullen.</span><span class="sxs-lookup"><span data-stu-id="983bd-144">If you deleted the contents of the **Bin Code** field on the **General** FastTab before getting the lines, you must fill in an appropriate bin code on each shipment line.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="983bd-145">U kunt niet meer artikelen verzenden dan het aantal in het veld **Openstaand aantal** op de brondocumentregel.</span><span class="sxs-lookup"><span data-stu-id="983bd-145">You cannot ship more items than the number in the **Qty. Outstanding** field on the source document line.</span></span> <span data-ttu-id="983bd-146">Als u meer artikelen wilt verzenden, haalt u een ander brondocument op dat een regel voor het item bevat. U gebruikt de filterfunctie om brondocumenten met het artikel op te halen.</span><span class="sxs-lookup"><span data-stu-id="983bd-146">To ship more items, retrieve another source document that contains a line for the item by using the filter function to get source documents with the item.</span></span>  

<span data-ttu-id="983bd-147">Als u alle regels voor de verzending hebt, kunt u het proces starten dat deze doorstuurt naar het magazijnpersoneel om te picken.</span><span class="sxs-lookup"><span data-stu-id="983bd-147">When you have the lines you want to ship, you can start the process that sends the lines to warehouse employees to pick.</span></span>

### <a name="to-pick-and-ship"></a><span data-ttu-id="983bd-148">U kunt als volgt een verzending picken en verzenden</span><span class="sxs-lookup"><span data-stu-id="983bd-148">To pick and ship</span></span>
<span data-ttu-id="983bd-149">Doorgaans wordt een nieuw pickdocument gemaakt of een bestaand pickdocument geopend door een magazijnmedewerker die verantwoordelijk is voor pickactiviteiten.</span><span class="sxs-lookup"><span data-stu-id="983bd-149">Typically, a warehouse worker responsible for picking creates a pick document, or opens an already created pick document.</span></span>
1. <span data-ttu-id="983bd-150">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Magazijnverzendingen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="983bd-150">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Warehouse Shipments**, and then choose the related link.</span></span>
2. <span data-ttu-id="983bd-151">Selecteer de magazijnverzending waarvoor u wilt picken en kies de actie **Pick maken**.</span><span class="sxs-lookup"><span data-stu-id="983bd-151">Select the warehouse shipment that you want to pick for, and then choose the **Create Pick** action.</span></span>
3. <span data-ttu-id="983bd-152">Vul de velden in het venster in en klik vervolgens op de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="983bd-152">Fill in the fields in the request window, and then choose the **OK** button.</span></span> <span data-ttu-id="983bd-153">Het opgegeven magazijnpickdocument wordt gemaakt.</span><span class="sxs-lookup"><span data-stu-id="983bd-153">The specified warehouse pick document is created.</span></span>

    <span data-ttu-id="983bd-154">U kunt ook een bestaande magazijnpick openen.</span><span class="sxs-lookup"><span data-stu-id="983bd-154">Alternatively, open an existing warehouse pick.</span></span>
4. <span data-ttu-id="983bd-155">Klik op het pictogram ![pictogram Zoeken naar pagina of rapport](media/ui-search/search_small.png "Zoeken naar pagina of rapport"), voer **Magazijnpicks** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="983bd-155">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Picks**, and then choose the related link.</span></span> <span data-ttu-id="983bd-156">Selecteer de magazijnpick waaraan u wilt werken.</span><span class="sxs-lookup"><span data-stu-id="983bd-156">Select the warehouse pick that you want to work on.</span></span>

    <span data-ttu-id="983bd-157">Als het magazijn met opslaglocaties werkt, zijn de pickregels omgezet in Nemen- en Plaatsen-regels.</span><span class="sxs-lookup"><span data-stu-id="983bd-157">If the warehouse is set up to use bins, then the pick lines have been converted to Take and Place action lines.</span></span>

    <span data-ttu-id="983bd-158">U kunt deze regels sorteren, een werknemer aan de pick toewijzen, een breakbulkfilter instellen als u met gestuurde opslag en pick werkt en de pickinstructies afdrukken.</span><span class="sxs-lookup"><span data-stu-id="983bd-158">You can sort the lines, assign an employee to the pick, set a break-bulk filter, if you are using directed put-away and pick, and print the pick instructions.</span></span>

5. <span data-ttu-id="983bd-159">Voer de pick uit en plaats de artikelen in de opgegeven opslaglocatie voor verzending of in de verzendruimte als u niet met opslaglocaties werkt.</span><span class="sxs-lookup"><span data-stu-id="983bd-159">Perform the actual picking of items and place them in the specified shipping bin, or in the shipping area, if you do not have bins.</span></span>
6. <span data-ttu-id="983bd-160">Kies de actie **Pick registreren**.</span><span class="sxs-lookup"><span data-stu-id="983bd-160">Choose the **Register Pick** action.</span></span>

    <span data-ttu-id="983bd-161">De velden **Te verzenden aantal** en **Documentstatus** op de kop van het verzenddocument worden bijgewerkt.</span><span class="sxs-lookup"><span data-stu-id="983bd-161">The **Qty. to Ship** field and the **Document Status** field on the header of the shipment document are updated.</span></span> <span data-ttu-id="983bd-162">De gepickte artikelen zijn niet meer beschikbaar voor een andere verzending of voor interne bewerkingen.</span><span class="sxs-lookup"><span data-stu-id="983bd-162">The items you have picked are no longer available for picking for other shipments or for internal operations.</span></span>
7. <span data-ttu-id="983bd-163">Druk de verzenddocumenten af, bereid de zending voor en boek de zending.</span><span class="sxs-lookup"><span data-stu-id="983bd-163">Print your shipping documents, prepare the shipment packages, and then post the shipment.</span></span>

<span data-ttu-id="983bd-164">Zie [Procedure: Artikelen picken voor magazijnverzending](warehouse-how-to-pick-items-for-warehouse-shipment.md) voor meer informatie over het picken voor magazijnverzendingen.</span><span class="sxs-lookup"><span data-stu-id="983bd-164">For more information about picking for warehouse shipments, see [How to: Pick Items for Warehouse Shipment](warehouse-how-to-pick-items-for-warehouse-shipment.md).</span></span>

<span data-ttu-id="983bd-165">U kunt in het pickvoorstel verschillende pickinstructies combineren tot één instructie (voor verschillende verzendingen) en zo de artikelen in het magazijn nog efficiënter picken.</span><span class="sxs-lookup"><span data-stu-id="983bd-165">You can also use the pick worksheet to make several pick instructions into one instruction (for several shipments) and thereby improve the efficiency of picking in the warehouse.</span></span> <span data-ttu-id="983bd-166">Zie [Procedure: picks plannen in het voorstel](warehouse-how-to-plan-picks-in-worksheets.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="983bd-166">For more information, see [How to: Plan Pick in Worksheets](warehouse-how-to-plan-picks-in-worksheets.md).</span></span>

> [!NOTE]
> <span data-ttu-id="983bd-167">Als u de ontvangst van bepaalde artikelen in het magazijn afwacht en met cross-docken werkt, berekent [!INCLUDE[d365fin](includes/d365fin_md.md)] voor elke verzend- of pickvoorstelregel het aantal van het artikel in de cross-dockopslaglocatie.</span><span class="sxs-lookup"><span data-stu-id="983bd-167">If you are waiting for particular items to arrive at the warehouse, and you use cross-dock functionality, then [!INCLUDE[d365fin](includes/d365fin_md.md)] calculates on each shipment or pick worksheet line the quantity of the item that is in the cross-dock bin.</span></span> <span data-ttu-id="983bd-168">Dit veld wordt bijgewerkt telkens wanneer u het verzenddocument of het voorstel opent of sluit.</span><span class="sxs-lookup"><span data-stu-id="983bd-168">It updates this field each time you leave and open the shipment document or worksheet.</span></span> <span data-ttu-id="983bd-169">Zie [Procedure: Artikelen cross-docken](warehouse-how-to-cross-dock-items.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="983bd-169">For more information, see [How to: Cross-Dock Items](warehouse-how-to-cross-dock-items.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="983bd-170">Zie ook</span><span class="sxs-lookup"><span data-stu-id="983bd-170">See Also</span></span>  
[<span data-ttu-id="983bd-171">Magazijnbeheer</span><span class="sxs-lookup"><span data-stu-id="983bd-171">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="983bd-172">Voorraad</span><span class="sxs-lookup"><span data-stu-id="983bd-172">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="983bd-173">[Magazijnbeheer instellen](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="983bd-173">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="983bd-174">[Assemblagebeheer](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="983bd-174">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="983bd-175">Ontwerpdetails: Magazijnbeheer</span><span class="sxs-lookup"><span data-stu-id="983bd-175">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="983bd-176">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="983bd-176">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

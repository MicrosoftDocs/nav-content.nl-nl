---
title: Serviceorders maken
description: In het venster **Serviceorder** kunt u documenten maken waarin u op aanvraag van de klant voor serviceartikelen gegevens invoert over een service, bijvoorbeeld herstel en onderhoud.
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
ms.openlocfilehash: ca6e6f1fd6bf6c9d9a26a9e42fca8b9c4931f89d
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-service-orders"></a><span data-ttu-id="fb46e-103">Procedure: Serviceorders maken</span><span class="sxs-lookup"><span data-stu-id="fb46e-103">How to: Create Service Orders</span></span>
<span data-ttu-id="fb46e-104">In het venster **Serviceorder** kunt u documenten maken waarin u op aanvraag van de klant voor serviceartikelen gegevens invoert over een service, als bijvoorbeeld herstel en onderhoud.</span><span class="sxs-lookup"><span data-stu-id="fb46e-104">You can use the **Service Order** window to create documents where you enter information about a service, such as repairs and maintenance, on service items by customer request.</span></span>  
  
<span data-ttu-id="fb46e-105">Wanneer u een serviceorder maakt, hoeft u slechts een paar velden in te vullen.</span><span class="sxs-lookup"><span data-stu-id="fb46e-105">When creating a service order, you only have to fill in a few fields.</span></span> <span data-ttu-id="fb46e-106">Sommige velden zijn optioneel en veel worden automatisch ingevuld wanneer u verwante velden invult.</span><span class="sxs-lookup"><span data-stu-id="fb46e-106">Some fields are optional and many are automatically filled in when you fill in related fields.</span></span>  
  
## <a name="to-create-a-service-order"></a><span data-ttu-id="fb46e-107">Serviceorders maken</span><span class="sxs-lookup"><span data-stu-id="fb46e-107">To create a service order</span></span>    
1. <span data-ttu-id="fb46e-108">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Serviceorders** in en klik op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="fb46e-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="fb46e-109">Maak een nieuwe serviceorder.</span><span class="sxs-lookup"><span data-stu-id="fb46e-109">Create a new service order.</span></span>  
3. <span data-ttu-id="fb46e-110">Selecteer in het veld **Nr.**</span><span class="sxs-lookup"><span data-stu-id="fb46e-110">In the **No.**</span></span> <span data-ttu-id="fb46e-111">een nummer voor de serviceorder in.</span><span class="sxs-lookup"><span data-stu-id="fb46e-111">field, enter a number for the service order.</span></span>  
  
     <span data-ttu-id="fb46e-112">Als u in het venster **Servicebeheerinstellingen** nummerreeksen voor serviceorders hebt ingesteld, kunt u ook op Enter drukken om het eerstvolgende beschikbare serviceordernummer in te voeren.</span><span class="sxs-lookup"><span data-stu-id="fb46e-112">Alternatively, if you have set up number series for service orders in the **Service Mgt. Setup** window, you can press Enter to select the next available service order number.</span></span>  
  
4. <span data-ttu-id="fb46e-113">Voer in het veld **Klantnr.**</span><span class="sxs-lookup"><span data-stu-id="fb46e-113">In the **Customer No.**</span></span> <span data-ttu-id="fb46e-114">de betreffende klant uit de lijst.</span><span class="sxs-lookup"><span data-stu-id="fb46e-114">field, select the relevant customer from the list.</span></span> <span data-ttu-id="fb46e-115">De betreffende velden voor de klant worden automatisch ingevuld met gegevens uit de tabel **Klant**.</span><span class="sxs-lookup"><span data-stu-id="fb46e-115">The customer-relevant fields are filled in with information from the **Customer** table.</span></span>  
  
5. <span data-ttu-id="fb46e-116">Afhankelijk van de instellingen op het sneltabblad **Verplichte velden** in het venster **CRM - Service-instellingen** moet u wellicht het veld **Serviceordersoort** en het veld **Verkoper** invullen.</span><span class="sxs-lookup"><span data-stu-id="fb46e-116">Depending on the settings on the **Mandatory Fields** FastTab in the **Service Mgt. Setup** window, you may need to fill in the **Service Order Type** field and the **Salesperson Code** field.</span></span>  
6. <span data-ttu-id="fb46e-117">Het invullen van de overige velden is optioneel.</span><span class="sxs-lookup"><span data-stu-id="fb46e-117">Optionally, fill in the rest of the fields.</span></span>  
7. <span data-ttu-id="fb46e-118">Registreer de serviceartikelregels.</span><span class="sxs-lookup"><span data-stu-id="fb46e-118">Register the service item lines.</span></span>  

## <a name="to-create-a-service-order-from-a-contract"></a><span data-ttu-id="fb46e-119">Serviceorders maken van contracten</span><span class="sxs-lookup"><span data-stu-id="fb46e-119">To create a service order from a contract</span></span>  
<span data-ttu-id="fb46e-120">U kunt automatisch serviceorders voor het onderhoud van serviceartikelen maken op basis van servicecontracten.</span><span class="sxs-lookup"><span data-stu-id="fb46e-120">You can automatically create service orders for the maintenance of service items based on service contracts.</span></span>  
  
1. <span data-ttu-id="fb46e-121">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Contractserviceorders maken** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="fb46e-121">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Create Contract Service Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="fb46e-122">Stel op het sneltabblad **Servicecontractkop** de gewenste filters in.</span><span class="sxs-lookup"><span data-stu-id="fb46e-122">On the **Service Contract Header** FastTab, set the filters you want to apply.</span></span>  
3. <span data-ttu-id="fb46e-123">Op het Sneltabblad **Opties** vult u de velden **Begindatum** en **Einddatum** in met de begindatum en einddatum van de periode waarvoor u contractserviceorders wilt maken.</span><span class="sxs-lookup"><span data-stu-id="fb46e-123">On the **Options** FastTab, fill in the **Starting Date** and **Ending Date** fields with the starting date and ending date for the period that you want to create contract service orders for.</span></span> <span data-ttu-id="fb46e-124">Met de batchverwerking maakt u serviceorders waarin serviceartikelen in servicecontracten zijn opgenomen met de volgende geplande servicedatums in deze periode.</span><span class="sxs-lookup"><span data-stu-id="fb46e-124">The batch job creates service orders that include service items in service contracts with next planned service dates within this period.</span></span>  
  
    > [!NOTE]  
    >  <span data-ttu-id="fb46e-125">Er is een limiet aan het aantal dagen dat u als het datuminterval voor de batchtaak kunt gebruiken.</span><span class="sxs-lookup"><span data-stu-id="fb46e-125">There is a limit to the number of days you can use as the date range each time you use this batch job.</span></span> <span data-ttu-id="fb46e-126">U bepaalt de beperking in het veld **Max. dagen contractserviceorder** in het venster **Servicebeheerinstellingen**.</span><span class="sxs-lookup"><span data-stu-id="fb46e-126">You set this limit in the **Contract Serv. Ord. Max. Days** field in the **Service Mgt. Setup** window.</span></span>  
  
4. <span data-ttu-id="fb46e-127">Kies in het veld **Actie** de optie **Serviceorder maken**.</span><span class="sxs-lookup"><span data-stu-id="fb46e-127">In the **Action** field, choose **Create Service Order**.</span></span>  

## <a name="to-convert-a-service-quote-to-a-service-order"></a><span data-ttu-id="fb46e-128">Een serviceofferte omzetten in een serviceorder</span><span class="sxs-lookup"><span data-stu-id="fb46e-128">To convert a service quote to a service order</span></span>
<span data-ttu-id="fb46e-129">Wanneer een klant een servicecontractofferte heeft geaccepteerd, zet u deze om in een serviceorder.</span><span class="sxs-lookup"><span data-stu-id="fb46e-129">When a customer has accepted a service quote, you convert it to a service order.</span></span> <span data-ttu-id="fb46e-130">De offerte wordt verwijderd en er wordt een nieuwe serviceorder ingesteld met dezelfde omschrijving als de serviceofferte.</span><span class="sxs-lookup"><span data-stu-id="fb46e-130">The quote is deleted and a new service order is set up with the same description as the service quote.</span></span> <span data-ttu-id="fb46e-131">De responsdatum en -tijd worden opnieuw berekend voor de serviceorder en de status van de serviceorder wordt ingesteld op **In behandeling**.</span><span class="sxs-lookup"><span data-stu-id="fb46e-131">The response date and time are recalculated for the service order and the status is set to **Pending**.</span></span> <span data-ttu-id="fb46e-132">De herstelstatus van de serviceartikelen in de order wordt gewijzigd in **Eerste**.</span><span class="sxs-lookup"><span data-stu-id="fb46e-132">The repair status of the service items in the order are changed to **Initial**.</span></span>  
  
<span data-ttu-id="fb46e-133">In [!INCLUDE[d365fin](includes/d365fin_md.md)] wordt gezocht naar toewijzingsposten voor alle serviceartikelen met de status **Actief** in de serviceofferte.</span><span class="sxs-lookup"><span data-stu-id="fb46e-133">[!INCLUDE[d365fin](includes/d365fin_md.md)] searches for allocation entries for all the service items in the service quote that have the status **Active**.</span></span> <span data-ttu-id="fb46e-134">Als dergelijke toewijzingsposten worden gevonden, wordt de toewijzingsstatus gewijzigd in **Hertoewijzing vereist**.</span><span class="sxs-lookup"><span data-stu-id="fb46e-134">If it finds such allocation entries, their allocation status is updated to **Reallocation Needed**.</span></span> <span data-ttu-id="fb46e-135">Wanneer u de serviceartikelen in de serviceorder opnieuw toewijst, wordt de status van de geregistreerde toewijzingsposten voor de order gewijzigd in **Gereedgemeld**.</span><span class="sxs-lookup"><span data-stu-id="fb46e-135">When you reallocate the service items in the service order, the status of the allocation entries registered for the quote are updated to **Finished**.</span></span>   

1. <span data-ttu-id="fb46e-136">Kies het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Servicecontractoffertes** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="fb46e-136">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Contract Quotes**, and then choose the related link.</span></span>  
2. <span data-ttu-id="fb46e-137">Kies de serviceofferte die u wilt omzetten in een serviceorder.</span><span class="sxs-lookup"><span data-stu-id="fb46e-137">Choose the service quote to convert to a service order.</span></span>  
3. <span data-ttu-id="fb46e-138">Kies de actie **Order maken**.</span><span class="sxs-lookup"><span data-stu-id="fb46e-138">Choose the **Make Order** action.</span></span>  

## <a name="to-check-item-availability-for-one-or-more-orders"></a><span data-ttu-id="fb46e-139">Artikelbeschikbaarheid voor een of meer orders controleren</span><span class="sxs-lookup"><span data-stu-id="fb46e-139">To check item availability for one or more orders</span></span>  
<span data-ttu-id="fb46e-140">U kunt controleren en bekijken of een artikel dat u nodig hebt om een order af te handelen op voorraad is en als dat niet het geval is, wanneer het artikel beschikbaar zal zijn.</span><span class="sxs-lookup"><span data-stu-id="fb46e-140">You can check and see if an item you need to fulfill an order is in stock, and if it is not, when the item will be in stock.</span></span> <span data-ttu-id="fb46e-141">Daarna kunt u dan, als een artikel beschikbaar is voor reservering, dit artikel reserveren om er zeker van te zijn dat het beschikbaar is voor uw gebruik.</span><span class="sxs-lookup"><span data-stu-id="fb46e-141">In addition, if an item is available to reserve, you can reserve it to make sure it is available for your use.</span></span> <span data-ttu-id="fb46e-142">U kunt de beschikbaarheid voor een bepaalde order of voor alle orders controleren.</span><span class="sxs-lookup"><span data-stu-id="fb46e-142">You can check availability for a particular order, or for all orders.</span></span>  

1.  <span data-ttu-id="fb46e-143">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Planbord** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="fb46e-143">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Dispatch Board**, and then choose the related link.</span></span>  
2. <span data-ttu-id="fb46e-144">Ga op een van de volgende manieren te werk:</span><span class="sxs-lookup"><span data-stu-id="fb46e-144">Do one of the following:</span></span>  
  
    * <span data-ttu-id="fb46e-145">Als u de beschikbaarheid voor een bepaalde order wilt controleren, kiest u de actie **Vraagoverzicht**.</span><span class="sxs-lookup"><span data-stu-id="fb46e-145">For a particular order, choose the order, and then choose the **Demand Overview** action.</span></span>  
    * <span data-ttu-id="fb46e-146">Voor alle orders kiest u **Document weergeven**.</span><span class="sxs-lookup"><span data-stu-id="fb46e-146">For all orders, choose **Show Document**.</span></span> <span data-ttu-id="fb46e-147">Het venster **Serviceorder** wordt geopend.</span><span class="sxs-lookup"><span data-stu-id="fb46e-147">The **Service Order** window opens.</span></span>  
  
3. <span data-ttu-id="fb46e-148">Vouw op de pagina **Vraagoverzicht** de artikelgroepering uit en bekijk informatie over de beschikbaarheid van het artikel.</span><span class="sxs-lookup"><span data-stu-id="fb46e-148">On the **Demand Overview** page, expand the item grouping, and view information about the availability of the item.</span></span> <span data-ttu-id="fb46e-149">U kunt bijvoorbeeld zien hoeveel artikelen op voorraad zijn.</span><span class="sxs-lookup"><span data-stu-id="fb46e-149">For example, you can see how many items are in inventory.</span></span> <span data-ttu-id="fb46e-150">U kunt ook zien of een artikel beschikbaar is of dat het is nabesteld, dat betekent Type bron = aankoop, of wanneer deze is gereserveerd.</span><span class="sxs-lookup"><span data-stu-id="fb46e-150">You can also see if and when an item will be available if it is on back order, that is, Source Type = Purchase, or whether it has been reserved.</span></span> 

## <a name="to-reserve-an-item-for-a-service-order"></a><span data-ttu-id="fb46e-151">Een artikel voor een serviceorder reserveren</span><span class="sxs-lookup"><span data-stu-id="fb46e-151">To reserve an item for a service order</span></span>
<span data-ttu-id="fb46e-152">Als u er zeker van wilt zijn dat een artikel voor een serviceorder beschikbaar is, kunt u het artikel reserveren.</span><span class="sxs-lookup"><span data-stu-id="fb46e-152">If you need to be sure that an item is available for a service order, you can reserve the item.</span></span> 

1. <span data-ttu-id="fb46e-153">Geef in het venster **Zoeken** **Serviceorders** op en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="fb46e-153">In the **Search** box, enter **Service Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="fb46e-154">Kies de serviceorder en kies **Bewerken**.</span><span class="sxs-lookup"><span data-stu-id="fb46e-154">Choose the service order, and then choose **Edit**.</span></span>  
3. <span data-ttu-id="fb46e-155">Kies **Acties**, kies **Order** en kies **Serviceregels**.</span><span class="sxs-lookup"><span data-stu-id="fb46e-155">Choose **Actions**, choose **Order**, and then choose **Service Lines**.</span></span>  
4. <span data-ttu-id="fb46e-156">Op de pagina **Serviceregels** kiest u het artikel dat u wilt reserveren en vervolgens kiest u de actie **Reserveren**.</span><span class="sxs-lookup"><span data-stu-id="fb46e-156">On the **Service Lines** page, choose the item to reserve, and then choose the **Reserve** action.</span></span>  
5. <span data-ttu-id="fb46e-157">Op de pagina **Reservering** kiest u **Huidige regel reserveren**.</span><span class="sxs-lookup"><span data-stu-id="fb46e-157">On the **Reservation** page, choose **Reserve from Current Line**.</span></span> 

## <a name="to-insert-lines-based-on-standard-service-codes"></a><span data-ttu-id="fb46e-158">Regels invoegen op basis van standaardservicecodes</span><span class="sxs-lookup"><span data-stu-id="fb46e-158">To insert lines based on standard service codes</span></span>  
<span data-ttu-id="fb46e-159">Als u standaardservicecodes hebt ingesteld en deze hebt toegewezen aan serviceartikelgroepen, kunt u de standaardregels invoegen die zijn gekoppeld aan de standaardservicecodes op servicedocumenten.</span><span class="sxs-lookup"><span data-stu-id="fb46e-159">If you have set up standard service codes and assigned them to service item groups, you can insert the standard lines linked to the standard service codes on service documents.</span></span> <span data-ttu-id="fb46e-160">Zie voor meer informatie [Procedure: Standaardservicecodes instellen](service-how-setup-service-coding.md).</span><span class="sxs-lookup"><span data-stu-id="fb46e-160">For more information, see [How to: Set Up Standard Service Codes](service-how-setup-service-coding.md).</span></span>   

1. <span data-ttu-id="fb46e-161">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Serviceorders** in en klik op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="fb46e-161">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="fb46e-162">Maak een nieuwe serviceorder.</span><span class="sxs-lookup"><span data-stu-id="fb46e-162">Create a new service order.</span></span>  
3. <span data-ttu-id="fb46e-163">Vul de velden in.</span><span class="sxs-lookup"><span data-stu-id="fb46e-163">Fill in the fields as necessary..</span></span>  
4. <span data-ttu-id="fb46e-164">Vul de vereiste gegevens in op de serviceartikelregels.</span><span class="sxs-lookup"><span data-stu-id="fb46e-164">Fill in the service item lines with the required information.</span></span>  
5. <span data-ttu-id="fb46e-165">Kies de regel met het serviceartikel waarvoor u serviceregels wilt maken en kies **Std. servicecodes ophalen**.</span><span class="sxs-lookup"><span data-stu-id="fb46e-165">Choose the line with the service item that you want to create service lines for, and then choose **Get Std. Service Codes**.</span></span> <span data-ttu-id="fb46e-166">Het venster **Std. serviceartikelgroepcodes** wordt geopend met de standaardcodes voor de serviceartikelgroep die op de regel zijn opgegeven.</span><span class="sxs-lookup"><span data-stu-id="fb46e-166">The **Standard Serv. Item Gr. Codes** window opens with the standard codes for the service item group specified on the line.</span></span>  
6. <span data-ttu-id="fb46e-167">Kies de juiste code en kies de knop **OK** om de standaardserviceregels in te voeren.</span><span class="sxs-lookup"><span data-stu-id="fb46e-167">Choose the appropriate code, and choose the **OK** button to enter standard service lines.</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="fb46e-168">Als het veld **Serviceartikelgroepcode** op de serviceartikelregel van het document leeg is, betekent dit dat het serviceartikel niet tot een serviceartikelgroep behoort.</span><span class="sxs-lookup"><span data-stu-id="fb46e-168">If the **Service Item Group Code** field on the service item line of the document is blank, this means that the service item does not belong to any service item group.</span></span> <span data-ttu-id="fb46e-169">In dit geval bevat het venster **Std. serviceartikelgroepcodes** een overzicht van alle standaard servicecodes.</span><span class="sxs-lookup"><span data-stu-id="fb46e-169">In this case, the **Standard Serv. Item Gr. Codes** window will contain a list of all standard service codes.</span></span> <span data-ttu-id="fb46e-170">Selecteer uit de lijst om standaardserviceregels in het document in te voegen.</span><span class="sxs-lookup"><span data-stu-id="fb46e-170">You should select from the list to insert standard service lines in the document.</span></span> <span data-ttu-id="fb46e-171">U kunt ook selecteren uit de lijst met standaard service-codes toegewezen aan een bepaald serviceartikelgroep.</span><span class="sxs-lookup"><span data-stu-id="fb46e-171">You may also select from the list of standard service codes assigned to a specific service item group.</span></span> <span data-ttu-id="fb46e-172">Om de lijst weer te geven, selecteert u de relevante code in het veld **Serviceartikelgroepcode** in het venster **Std. serviceartikelgroepcodes**.</span><span class="sxs-lookup"><span data-stu-id="fb46e-172">To view the list, select the relevant code in the **Service Item Group Code** field in the **Standard Serv. Item Gr. Codes** window.</span></span>  

## <a name="to-register-internal-or-public-comments"></a><span data-ttu-id="fb46e-173">Interne of openbare opmerkingen registreren</span><span class="sxs-lookup"><span data-stu-id="fb46e-173">To register internal or public comments</span></span>
<span data-ttu-id="fb46e-174">U kunt opmerkingen toevoegen die op serviceorders en serviceoffertes kunnen worden afgedrukt om extra informatie te bieden.</span><span class="sxs-lookup"><span data-stu-id="fb46e-174">You can add comments that will be printed on service orders and service quotes to provide additional information.</span></span> <span data-ttu-id="fb46e-175">U kunt maximaal 80 tekens, inclusief spaties, toevoegen.</span><span class="sxs-lookup"><span data-stu-id="fb46e-175">You can add up to 80 characters, including spaces.</span></span> <span data-ttu-id="fb46e-176">Als u extra tekst wilt invoeren, kiest u een andere regel.</span><span class="sxs-lookup"><span data-stu-id="fb46e-176">If you need to enter additional text, choose another line.</span></span> <span data-ttu-id="fb46e-177">Als u een opmerking wilt registreren, kiest u een regel en kiest u de actie **Opmerkingen**.</span><span class="sxs-lookup"><span data-stu-id="fb46e-177">To register a comment, choose a line, and then choose the **Comments** action.</span></span>  

## <a name="to-delete-invoiced-service-orders"></a><span data-ttu-id="fb46e-178">Gefactureerde serviceorders verwijderen</span><span class="sxs-lookup"><span data-stu-id="fb46e-178">To delete invoiced service orders</span></span>  
<span data-ttu-id="fb46e-179">Wanneer orders volledig zijn gefactureerd, worden ze doorgaans automatisch verwijderd.</span><span class="sxs-lookup"><span data-stu-id="fb46e-179">Orders are usually deleted automatically after having been fully invoiced.</span></span> <span data-ttu-id="fb46e-180">Wanneer een factuur wordt geboekt, wordt een bijbehorende post gemaakt in het venster **Geboekte servicefacturen**.</span><span class="sxs-lookup"><span data-stu-id="fb46e-180">When an invoice is posted, a corresponding entry is created in the **Posted Service Invoices** window.</span></span> <span data-ttu-id="fb46e-181">U kunt het geboekte document bekijken op de pagina **Geboekte servicefactuur**.</span><span class="sxs-lookup"><span data-stu-id="fb46e-181">The posted document can be viewed on the **Posted Service Invoice** page.</span></span>  
  
<span data-ttu-id="fb46e-182">Serviceorders worden echter niet automatisch verwijderd als het totale aantal op de order niet vanuit de serviceorder zelf is geboekt, maar vanuit het venster **Servicefactuur**.</span><span class="sxs-lookup"><span data-stu-id="fb46e-182">Service orders are not deleted automatically, however, if the total quantity on the order has been posted not from the service order itself, but from the **Service Invoice** window.</span></span> <span data-ttu-id="fb46e-183">In dit geval zult u wellicht gefactureerde orders die niet zijn verwijderd, zelf moeten verwijderen.</span><span class="sxs-lookup"><span data-stu-id="fb46e-183">Then you may need to delete invoiced orders that were not deleted.</span></span> <span data-ttu-id="fb46e-184">Hiervoor kunt u de batchverwerking **Gefactureerde serviceorders verwijderen** uitvoeren.</span><span class="sxs-lookup"><span data-stu-id="fb46e-184">You can do this by running the **Delete Invoiced Service Orders** batch job.</span></span>  

1. <span data-ttu-id="fb46e-185">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Gefactureerde serviceorders verwijderen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="fb46e-185">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delete Invoiced Service Orders**, and then choose the related link.</span></span> <span data-ttu-id="fb46e-186">Het opvraagvenster voor de batchverwerking **Gefactureerde serviceorders verwijderen** wordt geopend.</span><span class="sxs-lookup"><span data-stu-id="fb46e-186">The **Delete Invoiced Service Orders** batch job request window opens.</span></span>  
2. <span data-ttu-id="fb46e-187">U kunt de orders selecteren die u wilt verwijderen door filters in te stellen in de velden **Nr.**, **Klantnr.** en **Factureren aan**.</span><span class="sxs-lookup"><span data-stu-id="fb46e-187">To select the orders to be deleted, you can set filters in the **No.**, **Customer No.**, and **Bill-to Customer No.**</span></span> <span data-ttu-id="fb46e-188">in.</span><span class="sxs-lookup"><span data-stu-id="fb46e-188">fields.</span></span>  
3. <span data-ttu-id="fb46e-189">Klik op **OK**.</span><span class="sxs-lookup"><span data-stu-id="fb46e-189">Choose **OK**.</span></span>  


## <a name="see-also"></a><span data-ttu-id="fb46e-190">Zie ook</span><span class="sxs-lookup"><span data-stu-id="fb46e-190">See Also</span></span>  
[<span data-ttu-id="fb46e-191">Serviceboekingen</span><span class="sxs-lookup"><span data-stu-id="fb46e-191">Service Posting</span></span>](service-service-posting.md)  
[<span data-ttu-id="fb46e-192">Procedure: Een serviceorder boeken</span><span class="sxs-lookup"><span data-stu-id="fb46e-192">How to: Post a Service Order</span></span>](service-how-to-post-service-orders.md)  
[<span data-ttu-id="fb46e-193">CRM - Service instellen</span><span class="sxs-lookup"><span data-stu-id="fb46e-193">Setting Up Service Management</span></span>](service-setup-service.md)  
[<span data-ttu-id="fb46e-194">Procedure: Werken aan servicetaken</span><span class="sxs-lookup"><span data-stu-id="fb46e-194">How to: Work on Service Tasks</span></span>](service-how-to-work-on-service-tasks.md)  
[<span data-ttu-id="fb46e-195">Procedure: Resources toewijzen</span><span class="sxs-lookup"><span data-stu-id="fb46e-195">How to: Allocate Resources</span></span>](service-how-to-allocate-resources.md)  

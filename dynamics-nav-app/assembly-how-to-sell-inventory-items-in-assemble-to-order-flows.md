---
title: Voorraadartikelen in assembleren voor order-stromen verkopen
description: Als het artikel is ingesteld voor assembleren-op-order, neemt het standaardproces voor de verkooporder aan dat het item niet in voorraad is en voor deze verkooporder geassembleerd moet worden. Daarom wordt er automatisch een gekoppelde assemblageorder gemaakt wanneer u een artikel aan de verkooporderregel wilt toevoegen.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 0d907c5f96c4af0e28a04292bee2c21865346593
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-sell-inventory-items-in-assemble-to-order-flows"></a><span data-ttu-id="0fc0e-104">Procedure: voorraadartikelen in assembleren-op-order-stromen verkopen</span><span class="sxs-lookup"><span data-stu-id="0fc0e-104">How to: Sell Inventory Items in Assemble-to-Order Flows</span></span>
<span data-ttu-id="0fc0e-105">Als het veld **Assemblagebeleid** op de artikelkaart van assemblageartikel **Op order assembleren** bevat, neemt het standaardproces voor de verkooporder aan dat het item niet in voorraad is en voor deze verkooporder geassembleerd moet worden.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-105">If the **Assembly Policy** field on the item card of an assembly item contains **Assemble-to-Order**, then the default sales order process assumes that the item is not in inventory and must be assembled for that specific sales order.</span></span> <span data-ttu-id="0fc0e-106">Daarom wordt er automatisch een gekoppelde assemblageorder gemaakt wanneer u een artikel aan de verkooporderregel wilt toevoegen.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-106">Therefore, a linked assembly order is automatically created when you add the item to a sales order line.</span></span> <span data-ttu-id="0fc0e-107">Zie voor meer informatie [Procedure: op order geassembleerde artikelen verkopen](assembly-how-to-sell-items-assembled-to-order.md).</span><span class="sxs-lookup"><span data-stu-id="0fc0e-107">For more information, see [How to: Sell Items Assembled to Order](assembly-how-to-sell-items-assembled-to-order.md).</span></span> <span data-ttu-id="0fc0e-108">Echter als een deel van de hoeveelheid van de verkooporder al beschikbaar in voorraad is, kunt u de assemblageorder verkleinen door het veld **Aantal voor op order assembleren** op de verkooporderregel te veranderen.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-108">However, if a part of the sales order quantity is already available in inventory, then you can decrease the assembly order quantity by changing the **Qty. to Assemble to Order** field on the sales order line.</span></span>  

<span data-ttu-id="0fc0e-109">Dit scenario is zeldzaam omdat op-order-assembleren-artikelen altijd worden aangepast en de kans dat ze in voorraad zijn in de configuratie die is aangevraagd door een andere klant laag is.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-109">This scenario is rare because assemble-to-order items are expected to always be customized, and the chance that they are in inventory in the configuration that is requested by another customer is low.</span></span> <span data-ttu-id="0fc0e-110">Maar als een bedrijf aantallen voor assembleren op basis van orders in voorraad heeft als gevolg van retouren of annuleringen, moeten deze hoeveelheden worden verzameld en verkocht voordat nieuwe worden samengesteld.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-110">However, if a company does have assemble-to-order quantities in inventory because of returns or order cancellations, then these quantities should be picked and sold before new ones are assembled.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="0fc0e-111">Er bestaat geen functionaliteit op verkooporders die automatisch waarschuwen of u helpt assemblyorderhoeveelheden die reeds beschikbaar zijn af te trekken.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-111">No functionality exists on sales orders that automatically alerts or helps you deduct assembly order quantities that are already available.</span></span> <span data-ttu-id="0fc0e-112">In plaats daarvan moet u de beschikbaarheidsinformatie controleren, zoals het feitenblok **Verkoopregeldetails**.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-112">Instead, you must monitor availability information, such as in the **Sales Line Details** FactBox.</span></span>  

<span data-ttu-id="0fc0e-113">Vergelijkbare functionaliteit is beschikbaar wanneer u assemblageartikelen uit voorraad verkoopt en een deel of de gehele hoeveelheid is niet beschikbaar en kan worden geleverd door een assemblageorder.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-113">Similar functionality is available when you are selling assembly items from inventory and a part or all of the quantity is unavailable and can be supplied by an assembly order.</span></span> <span data-ttu-id="0fc0e-114">Zie voor meer informatie [Procedure: op-order-assembleren-artikelen en voorraadartikelen samen verkopen](assembly-how-to-sell-assemble-to-order-items-and-inventory-items-together.md).</span><span class="sxs-lookup"><span data-stu-id="0fc0e-114">For more information, see [How to: Sell Assemble-to-Order Items and Inventory Items Together](assembly-how-to-sell-assemble-to-order-items-and-inventory-items-together.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="0fc0e-115">Bepaalde regels zijn van toepassing op het veld **Te verzenden aantal** op verkooporderregels die een combinatie van het op-order-assembleren-aantallen en voorraadaantallen bevatten.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-115">Certain rules apply to the **Qty. to Ship** field on sales order lines that contain a combination of assemble-to-order quantities and inventory quantities.</span></span> <span data-ttu-id="0fc0e-116">Zie voor meer informatie de sectie Combinatiescenario's in [Op voorraad assembleren of Op order assembleren begrijpen](assembly-assemble-to-order-or-assemble-to-stock.md).</span><span class="sxs-lookup"><span data-stu-id="0fc0e-116">For more information, see the Combination Scenarios section in [Understanding Assemble to Order and Assemble to Stock](assembly-assemble-to-order-or-assemble-to-stock.md).</span></span>  

<span data-ttu-id="0fc0e-117">Vervang in deze procedure de aantallen voor assembleren op basis van orders met de voorraadaantallen op een verkooporderregel.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-117">In this procedure, you replace assemble-to-order quantities with inventory quantities on a sales order line.</span></span> <span data-ttu-id="0fc0e-118">De stappen omvatten het opsporen of beschikbaarheid bestaat, het aftrekken van die hoeveelheid van de gekoppelde assemblageorder en vervolgens het reserveren van de voorraadhoeveelheid om ervoor te zorgen dat deze wordt gepickt en voor de order worden verzonden.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-118">The steps include detecting that availability exists, deducting that quantity from the linked assembly order, and then reserving the inventory quantity to make sure that it is picked and shipped for the order.</span></span>  

## <a name="to-sell-inventory-items-in-assemble-to-order-flows"></a><span data-ttu-id="0fc0e-119">Voorraadartikelen in assembleren-op-order-stromen verkopen</span><span class="sxs-lookup"><span data-stu-id="0fc0e-119">To sell inventory items in assemble-to-order flows</span></span>  
1.  <span data-ttu-id="0fc0e-120">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Verkooporders** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-120">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="0fc0e-121">Een verkooporder maken.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-121">Create a sales order.</span></span> <span data-ttu-id="0fc0e-122">Zie [Procedure: Producten verkopen](sales-how-sell-products.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-122">For more information, see [How to: Sell Products](sales-how-sell-products.md).</span></span>  
3.  <span data-ttu-id="0fc0e-123">Op een verkooporderregel voor een op-order-assembleren-artikel voert u in het veld **Hoeveelheid** de gevraagde hoeveelheid in.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-123">On a sales order line for an assemble-to-order item, in the **Quantity** field, enter the demanded quantity.</span></span>  
4.  <span data-ttu-id="0fc0e-124">In het feitenblok **Verkoopregeldetails** bepaalt u of de gevraagde hoeveelheid geheel of gedeeltelijk beschikbaar is.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-124">In the **Sales Line Details** FactBox, determine if all or some of the demanded quantity is available.</span></span>  
5.  <span data-ttu-id="0fc0e-125">In het veld **Aantal voor op order assembleren** trekt u de beschikbare hoeveelheid af zodat alleen niet-beschikbare hoeveelheid op de order wordt geassembleerd.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-125">In the **Qty. to Assemble to Order** field, deduct the available quantity so that only the unavailable quantity is assembled to the order.</span></span> <span data-ttu-id="0fc0e-126">Het veld **Gereserveerde hoeveelheid** wordt dienovereenkomstig verlaagd om aan te geven dat de order-naar-order-koppeling of reservering alleen van toepassing is op de te assembleren hoeveelheid.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-126">The **Reserved Quantity** field is decreased accordingly to reflect that the order-to-order link, or reservation, only applies to the quantity to be assembled.</span></span>  
6.  <span data-ttu-id="0fc0e-127">Op het sneltabblad **Regels** kiest u **Functies** en vervolgens kiest u de actie **Reserveren**.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-127">On the **Lines** FastTab, choose **Functions**, and then choose the **Reserve** action.</span></span>  
7.  <span data-ttu-id="0fc0e-128">Selecteer in het venster **Reservering** de artikelpostregel of -regels die de beschikbare hoeveelheden bevatten, kies de actie **Vanuit huidige regel reserveren** en kies vervolgens de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-128">In the **Reservation** window, select the item ledger entry line or lines that contain the available quantities, choose the **Reserve from Current Line** action, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="0fc0e-129">In het veld **Verkooporder** toont het veld **Gereserveerd aantal** nu dat het gehele aantal op de orderregel is gereserveerd.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-129">In the **Sales Order** window, the **Reserved Quantity** field now shows that the whole order line quantity is reserved.</span></span> <span data-ttu-id="0fc0e-130">Het veld **Aantal voor op order assembleren** weerspiegelt nog steeds de subhoeveelheid die moet worden geassembleerd.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-130">The **Qty. to Assemble to Order** field still reflects the subquantity that has to be assembled.</span></span>  

8.  <span data-ttu-id="0fc0e-131">Geef de verkooporder vrij voor het picken van de voorraadartikelen en assemblage van de niet beschikbare artikelen.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-131">Release the sales order for picking of the inventory items and for assembly of the unavailable items.</span></span> <span data-ttu-id="0fc0e-132">Zie [Procedure: Artikelen assembleren](assembly-how-to-assemble-items.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-132">For more information, see [How to: Assemble Items](assembly-how-to-assemble-items.md).</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="0fc0e-133">Het veld **Opslaglocatie** in de verkooporder kan al vooraf zijn ingevuld volgens het veld **Opslaglocatiecode assembleren-op-order verzending** of **Opslagloc.code Vanuit-assembl.** op de locatiekaart.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-133">The **Bin Code** field on the sales order may be prefilled according to the **Assemble-to-Order Shpt. Bin Code** or the **From-Assembly Bin Code** field on the location card.</span></span> <span data-ttu-id="0fc0e-134">In dat geval is het veld **Opslaglocatie** op de verkooporderregel mogelijk onjuist in deze combinatie van hoeveelheden assembleren voor order en assembleren voor voorraad.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-134">In that case, the **Bin Code** field on the sales order line may be incorrect in this combination of assemble-to-order and assemble-to-stock quantities.</span></span> <span data-ttu-id="0fc0e-135">Het is verstandig om het veld **Opslaglocatie** te bekijken en te controleren of de plaatsing voor alle hoeveelheden werkt.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-135">It is a good idea to look in the **Bin Code** field and ensure that the placement works for all quantities.</span></span> <span data-ttu-id="0fc0e-136">U kunt ook twee verschillende hoeveelheden invoeren op aparte verkooporderregels.</span><span class="sxs-lookup"><span data-stu-id="0fc0e-136">Alternatively, enter the two different quantities on separate sales order lines.</span></span>  

## <a name="see-also"></a><span data-ttu-id="0fc0e-137">Zie ook</span><span class="sxs-lookup"><span data-stu-id="0fc0e-137">See Also</span></span>  
[<span data-ttu-id="0fc0e-138">Assemblagebeheer</span><span class="sxs-lookup"><span data-stu-id="0fc0e-138">Assembly Management</span></span>](assembly-assemble-items.md)  
[<span data-ttu-id="0fc0e-139">Procedure: Artikelen reserveren</span><span class="sxs-lookup"><span data-stu-id="0fc0e-139">How to: Reserve Items</span></span>](inventory-how-to-reserve-items.md)  
[<span data-ttu-id="0fc0e-140">Procedure: Werken met stuklijsten</span><span class="sxs-lookup"><span data-stu-id="0fc0e-140">How to: Work with Bills of Material</span></span>](inventory-how-work-BOMs.md)  
[<span data-ttu-id="0fc0e-141">Voorraad</span><span class="sxs-lookup"><span data-stu-id="0fc0e-141">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="0fc0e-142">Ontwerpdetails: Magazijnbeheer</span><span class="sxs-lookup"><span data-stu-id="0fc0e-142">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="0fc0e-143">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="0fc0e-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

---
title: Een verkooporder maken die is gekoppeld aan een inkooporder voor een directe verzending
description: Hierin wordt beschreven hoe u een verkooporder kunt maken die is gekoppeld aan een inkooporder om verzending direct van de leverancier naar de klant mogelijk te maken.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: direct shipment
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 6a8210808532ff8945660c23f0bf91719e2f2963
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-make-drop-shipments"></a><span data-ttu-id="06de9-103">Procedure: Doorverzendingen maken</span><span class="sxs-lookup"><span data-stu-id="06de9-103">How to: Make Drop Shipments</span></span>
<span data-ttu-id="06de9-104">Een doorverzending is de directe verzending van artikelen van een van uw leveranciers naar een van uw klanten.</span><span class="sxs-lookup"><span data-stu-id="06de9-104">A drop shipment is the shipment of items from one of your vendors directly to one of your customers.</span></span>

<span data-ttu-id="06de9-105">Wanneer een verkooporder voor doorverzending is gemarkeerd en u maakt een inkooporder waarin de klant in het veld **Orderklantnr.**</span><span class="sxs-lookup"><span data-stu-id="06de9-105">When a sales order is marked for drop shipment, and you create a purchase order specifying the customer in the **Sell-to Customer No.**</span></span> <span data-ttu-id="06de9-106">is opgegeven, kunt u de twee documenten koppelen en daarbij de leverancier opdragen om direct naar de klant te verzenden.</span><span class="sxs-lookup"><span data-stu-id="06de9-106">field, you can link the two documents and thereby instruct the vendor to ship directly to the customer.</span></span>

## <a name="to-create-a-sales-order-for-drop-shipment"></a><span data-ttu-id="06de9-107">Een verkooporder voor doorverzending maken</span><span class="sxs-lookup"><span data-stu-id="06de9-107">To create a sales order for drop shipment</span></span>
<span data-ttu-id="06de9-108">Ter voorbereiding op een doorverzending maakt u een verkooporder voor een artikel zoals u dat normaal doet, maar u moet wel op de verkoopregel aangeven dat voor de verkoop doorverzending vereist is.</span><span class="sxs-lookup"><span data-stu-id="06de9-108">To prepare a drop shipment, you create a sales order for an item as normal, except you must indicate on the sales line that the sale requires drop shipment.</span></span>

1. <span data-ttu-id="06de9-109">Maak een verkooporder voor een artikel.</span><span class="sxs-lookup"><span data-stu-id="06de9-109">Create a sales order for an item.</span></span> <span data-ttu-id="06de9-110">Zie [Procedure: Producten verkopen](sales-how-sell-products.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="06de9-110">For more information, see [How to: Sell Products](sales-how-sell-products.md).</span></span>
2. <span data-ttu-id="06de9-111">Op de verkooporderregel voor de doorverzending schakelt u het selectievakje **Doorverzending** in.</span><span class="sxs-lookup"><span data-stu-id="06de9-111">On the sales order line for the drop shipment, select the **Drop Shipment** check box.</span></span> <span data-ttu-id="06de9-112">Gebruik de functie **Kolommen kiezen** als het veld niet zichtbaar is.</span><span class="sxs-lookup"><span data-stu-id="06de9-112">Use the **Choose Columns** function if the field is not visible.</span></span> <span data-ttu-id="06de9-113">Zie [Persoonlijke gebruikersinstellingen](ui-user-personalization.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="06de9-113">For more information, see [User Personalization](ui-user-personalization.md).</span></span>

## <a name="to-create-the-purchase-order-for-drop-shipment"></a><span data-ttu-id="06de9-114">De inkooporder voor doorverzendingen maken</span><span class="sxs-lookup"><span data-stu-id="06de9-114">To create the purchase order for drop shipment</span></span>
<span data-ttu-id="06de9-115">Ter voorbereiding op een doorverzending van het artikel dat u wilt verkopen, maakt u een inkooporder zoals u dat normaal doet, maar u moet op de inkooporder wel aangeven dat het artikel naar de klant moet worden verzonden en niet naar uzelf.</span><span class="sxs-lookup"><span data-stu-id="06de9-115">To prepare a drop shipment for the item to be sold, you create a purchase order as normal, except you must indicate on the purchase order that it must be shipped to your customer, not to yourself.</span></span>

1. <span data-ttu-id="06de9-116">Inkooporder maken.</span><span class="sxs-lookup"><span data-stu-id="06de9-116">Create a purchase order.</span></span> <span data-ttu-id="06de9-117">Vul geen velden op de regels in.</span><span class="sxs-lookup"><span data-stu-id="06de9-117">Do not fill any fields on the lines.</span></span> <span data-ttu-id="06de9-118">Zie voor meer informatie [Procedure: Inkopen vastleggen](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="06de9-118">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>
2. <span data-ttu-id="06de9-119">Selecteer in het veld **Orderklantnr.**</span><span class="sxs-lookup"><span data-stu-id="06de9-119">In the **Sell-to Customer No.**</span></span> <span data-ttu-id="06de9-120">de klant aan wie u verkoopt.</span><span class="sxs-lookup"><span data-stu-id="06de9-120">field, select the customer that you are selling to.</span></span>
3. <span data-ttu-id="06de9-121">Kies de actie **Doorverzendingen** en kies vervolgens de actie **Verkooporder ophalen**.</span><span class="sxs-lookup"><span data-stu-id="06de9-121">Choose the **Drop Shipments** action, and then choose the **Get Sales Order** action.</span></span>
4. <span data-ttu-id="06de9-122">Selecteer in het venster **Verkoopoverzicht** de verkooporder die u hebt voorbereid in de sectie "Een verkooporder voor doorverzending maken".</span><span class="sxs-lookup"><span data-stu-id="06de9-122">In the **Sales List** window, select the sales order that you prepared in the "To create a sales order for drop shipment" section.</span></span>
5. <span data-ttu-id="06de9-123">Kies de knop **Ok**.</span><span class="sxs-lookup"><span data-stu-id="06de9-123">Choose the **OK** button.</span></span>

<span data-ttu-id="06de9-124">De regelgegevens van de verkooporder worden ingevoegd op de inkooporderregel(s).</span><span class="sxs-lookup"><span data-stu-id="06de9-124">The line information from the sales order is inserted on the purchase order line(s).</span></span>

<span data-ttu-id="06de9-125">U kunt de leverancier nu opdragen om de artikelen naar de klant te verzenden, bijvoorbeeld door de inkooporder als een PDF via e-mail te verzenden.</span><span class="sxs-lookup"><span data-stu-id="06de9-125">You can now instruct the vendor to ship the items to your customer, for example, by mailing the purchase order as a PDF.</span></span>     

## <a name="to-view-the-linked-purchase-order-from-the-sales-order"></a><span data-ttu-id="06de9-126">De gekoppelde inkooporder weergeven op basis van de verkooporder</span><span class="sxs-lookup"><span data-stu-id="06de9-126">To view the linked purchase order from the sales order</span></span>
* <span data-ttu-id="06de9-127">Selecteer de verkooporderregel van de doorverzending, kies de actie **Order**, kies de actie **Doorverzending** en kies vervolgens de actie **Inkooporder**.</span><span class="sxs-lookup"><span data-stu-id="06de9-127">Select the drop-shipment sales order line, choose the **Order** action, choose the **Drop Shipment** action, and then choose the **Purchase Order** action.</span></span>

## <a name="to-post-a-drop-shipment"></a><span data-ttu-id="06de9-128">Een doorverzending boeken</span><span class="sxs-lookup"><span data-stu-id="06de9-128">To post a drop shipment</span></span>
<span data-ttu-id="06de9-129">Nadat de leverancier de artikelen heeft verzonden, kunt u de verkooporder boeken als verzonden.</span><span class="sxs-lookup"><span data-stu-id="06de9-129">After the vendor ships the items, you can post the sales order as shipped.</span></span> <span data-ttu-id="06de9-130">U kunt de inkooporder ook boeken, maar alleen met de optie **Ontvangen**, totdat de verkooporder is gefactureerd.</span><span class="sxs-lookup"><span data-stu-id="06de9-130">You can also post the purchase order, but only with the **Receive** option until the sales order has been invoiced.</span></span>

1. <span data-ttu-id="06de9-131">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Verkooporders** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="06de9-131">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="06de9-132">Open de verkooporder die u hebt gemaakt in de sectie "Een verkooporder voor een doorverzending maken".</span><span class="sxs-lookup"><span data-stu-id="06de9-132">Open the sales order that you created in the "To create a sales order for a drop shipment" section.</span></span>
3. <span data-ttu-id="06de9-133">Geef in het veld **Te verzenden aantal** op hoeveel van de orderhoeveelheid moet worden verzonden, de volledige of gedeeltelijke orderhoeveelheid.</span><span class="sxs-lookup"><span data-stu-id="06de9-133">In the **Qty. to Ship** field, specify how many of the order quantity to ship, the full or a partial order quantity.</span></span>
4. <span data-ttu-id="06de9-134">Kies de actie **Boeken** of **Boeken en verzenden**.</span><span class="sxs-lookup"><span data-stu-id="06de9-134">Choose the **Post** or **Post and Send** action.</span></span>
5. <span data-ttu-id="06de9-135">Kies vervolgens **de optie Verzenden** om later te factureren of de optie **Verzenden en factureren** om meteen te factureren.</span><span class="sxs-lookup"><span data-stu-id="06de9-135">Choose either the **Ship** option to invoice later, or the **Ship and Invoice** option to invoice immediately.</span></span>

## <a name="see-also"></a><span data-ttu-id="06de9-136">Zie ook</span><span class="sxs-lookup"><span data-stu-id="06de9-136">See Also</span></span>
<span data-ttu-id="06de9-137">[Procedure: Speciale orders maken](sales-how-to-create-special-orders.md)|</span><span class="sxs-lookup"><span data-stu-id="06de9-137">[How to: Create Special Orders](sales-how-to-create-special-orders.md)|</span></span>  
[<span data-ttu-id="06de9-138">Procedure: Producten verkopen</span><span class="sxs-lookup"><span data-stu-id="06de9-138">How to: Sell Products</span></span>](sales-how-sell-products.md)  
[<span data-ttu-id="06de9-139">Procedure: Inkopen vastleggen</span><span class="sxs-lookup"><span data-stu-id="06de9-139">How to: Record Purchases</span></span>](purchasing-how-record-purchases.md)  
[<span data-ttu-id="06de9-140">Verkoop</span><span class="sxs-lookup"><span data-stu-id="06de9-140">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="06de9-141">Voorraad</span><span class="sxs-lookup"><span data-stu-id="06de9-141">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="06de9-142">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="06de9-142">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>


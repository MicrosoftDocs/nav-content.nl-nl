---
title: 'Procedure: Doorverzendingen maken'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: a726c8c24d8f843b33b4df4d85ad2b5eab3790e7
ms.contentlocale: nl-nl
ms.lasthandoff: 09/11/2017

---

# <a name="how-to-make-drop-shipments"></a><span data-ttu-id="01b64-102">Procedure: Doorverzendingen maken</span><span class="sxs-lookup"><span data-stu-id="01b64-102">How to: Make Drop Shipments</span></span>
<span data-ttu-id="01b64-103">Een doorverzending is de directe verzending van artikelen van een van uw leveranciers naar een van uw klanten.</span><span class="sxs-lookup"><span data-stu-id="01b64-103">A drop shipment is the shipment of items from one of your vendors directly to one of your customers.</span></span>

<span data-ttu-id="01b64-104">Wanneer een verkooporder voor doorverzending is gemarkeerd en u maakt een inkooporder waarin de klant in het veld **Orderklantnr.**</span><span class="sxs-lookup"><span data-stu-id="01b64-104">When a sales order is marked for drop shipment, and you create a purchase order specifying the customer in the **Sell-to Customer No.**</span></span> <span data-ttu-id="01b64-105">is opgegeven, kunt u de twee documenten koppelen en daarbij de leverancier opdragen om direct naar de klant te verzenden.</span><span class="sxs-lookup"><span data-stu-id="01b64-105">field, then you can link the two documents and thereby instruct the vendor to ship directly to the customer.</span></span>

## <a name="to-create-a-sales-order-for-drop-shipment"></a><span data-ttu-id="01b64-106">Een verkooporder voor doorverzending maken</span><span class="sxs-lookup"><span data-stu-id="01b64-106">To create a sales order for drop shipment</span></span>
<span data-ttu-id="01b64-107">Ter voorbereiding op een doorverzending maakt u een verkooporder voor een artikel zoals u dat normaal doet, maar u moet wel op de verkoopregel aangeven dat voor de verkoop doorverzending vereist is.</span><span class="sxs-lookup"><span data-stu-id="01b64-107">To prepare a drop shipment, you create a sales order for an item as normal, except you must indicate on the sales line that the sale requires drop shipment.</span></span>

1. <span data-ttu-id="01b64-108">Maak een verkooporder voor een artikel.</span><span class="sxs-lookup"><span data-stu-id="01b64-108">Create a sales order for an item.</span></span> <span data-ttu-id="01b64-109">Zie [Procedure: Producten verkopen](sales-how-sell-products.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="01b64-109">For more information, see [How to: Sell Products](sales-how-sell-products.md).</span></span>
2. <span data-ttu-id="01b64-110">Op de verkooporderregel voor het doorverzendingsartikel schakelt u het selectievakje **Doorverzending** in.</span><span class="sxs-lookup"><span data-stu-id="01b64-110">On the sales order line for the drop-shipment item, select the **Drop Shipment** check box.</span></span>

## <a name="to-create-the-purchase-order-for-drop-shipment"></a><span data-ttu-id="01b64-111">De inkooporder voor doorverzendingen maken</span><span class="sxs-lookup"><span data-stu-id="01b64-111">To create the purchase order for drop shipment</span></span>
<span data-ttu-id="01b64-112">Ter voorbereiding op een doorverzending van het artikel dat u wilt verkopen, maakt u een inkooporder zoals u dat normaal doet, maar u moet op de inkooporder wel aangeven dat het artikel naar de klant moet worden verzonden en niet naar uzelf.</span><span class="sxs-lookup"><span data-stu-id="01b64-112">To prepare a drop shipment for the item to be sold, you create a purchase order as normal, except you must indicate on the purchase order that it must be shipped to your customer, not to yourself.</span></span>

1. <span data-ttu-id="01b64-113">Inkooporder maken.</span><span class="sxs-lookup"><span data-stu-id="01b64-113">Create a purchase order.</span></span> <span data-ttu-id="01b64-114">Vul geen velden op de regels in.</span><span class="sxs-lookup"><span data-stu-id="01b64-114">Do not fill any fields on the lines.</span></span> <span data-ttu-id="01b64-115">Zie voor meer informatie [Procedure: Inkopen vastleggen](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="01b64-115">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>
2. <span data-ttu-id="01b64-116">Selecteer in het veld **Orderklantnr.**</span><span class="sxs-lookup"><span data-stu-id="01b64-116">In the **Sell-to Customer No.**</span></span> <span data-ttu-id="01b64-117">de klant aan wie u verkoopt.</span><span class="sxs-lookup"><span data-stu-id="01b64-117">field, select the customer that you are selling to.</span></span>
3. <span data-ttu-id="01b64-118">Kies de actie **Doorverzendingen** en kies vervolgens de actie **Verkooporder ophalen**.</span><span class="sxs-lookup"><span data-stu-id="01b64-118">Choose the **Drop Shipments** action, and then choose the **Get Sales Order** action.</span></span>
4. <span data-ttu-id="01b64-119">Selecteer in het venster **Verkoopoverzicht** de verkooporder die u hebt voorbereid in de sectie "Een verkooporder voor doorverzending maken".</span><span class="sxs-lookup"><span data-stu-id="01b64-119">In the **Sales List** window, select the sales order that you prepared in the "To create a sales order for drop shipment" section.</span></span>
5. <span data-ttu-id="01b64-120">Kies de knop **Ok**.</span><span class="sxs-lookup"><span data-stu-id="01b64-120">Choose the **OK** button.</span></span>

<span data-ttu-id="01b64-121">De regelgegevens van de verkooporder worden ingevoegd op de inkooporderregel(s).</span><span class="sxs-lookup"><span data-stu-id="01b64-121">The line information from the sales order is inserted on the purchase order line(s).</span></span>

<span data-ttu-id="01b64-122">U kunt de leverancier nu opdragen om de artikelen naar de klant te verzenden, bijvoorbeeld door de inkooporder als een PDF via e-mail te verzenden.</span><span class="sxs-lookup"><span data-stu-id="01b64-122">You can now instruct the vendor to ship the items to your customer, for example, by mailing the purchase order as a PDF.</span></span>     

## <a name="to-view-the-linked-purchase-order-from-the-sales-order"></a><span data-ttu-id="01b64-123">De gekoppelde inkooporder weergeven op basis van de verkooporder</span><span class="sxs-lookup"><span data-stu-id="01b64-123">To view the linked purchase order from the sales order</span></span>
1. <span data-ttu-id="01b64-124">Selecteer de verkooporderregel van de doorverzending, kies de actie **Order**, kies de actie **Doorverzending** en kies vervolgens de actie **Inkooporder**.</span><span class="sxs-lookup"><span data-stu-id="01b64-124">Select the drop-shipment sales order line, choose the **Order** action, choose the **Drop Shipment** action, and then choose the **Purchase Order** action.</span></span>

<span data-ttu-id="01b64-125">De gekoppelde inkooporder wordt geopend.</span><span class="sxs-lookup"><span data-stu-id="01b64-125">The linked purchase order opens.</span></span>

## <a name="to-post-a-drop-shipment"></a><span data-ttu-id="01b64-126">Een doorverzending boeken</span><span class="sxs-lookup"><span data-stu-id="01b64-126">To post a drop shipment</span></span>
<span data-ttu-id="01b64-127">Als de leverancier de artikelen heeft verzonden, kunt u de verkooporder boeken als verzonden.</span><span class="sxs-lookup"><span data-stu-id="01b64-127">When the vendor has shipped the items, you can post the sales order as shipped.</span></span> <span data-ttu-id="01b64-128">U kunt de inkooporder ook boeken, maar alleen met de optie **Ontvangen**, totdat de verkooporder is gefactureerd.</span><span class="sxs-lookup"><span data-stu-id="01b64-128">You can also post the purchase order, but only with the **Receive** option until the sales order has been invoiced.</span></span>
1. <span data-ttu-id="01b64-129">Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Verkooporders** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="01b64-129">In the top right corner, choose the **Search for Page or Report** icon, enter **Sales orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="01b64-130">Open de verkooporder die u hebt gemaakt in de sectie "Een verkooporder voor een doorverzending maken".</span><span class="sxs-lookup"><span data-stu-id="01b64-130">Open the sales order that you created in the "To create a sales order for a drop shipment" section.</span></span>
3. <span data-ttu-id="01b64-131">Geef in het veld **Te verzenden aantal** op hoeveel van de orderhoeveelheid moet worden verzonden, de volledige of gedeeltelijke orderhoeveelheid.</span><span class="sxs-lookup"><span data-stu-id="01b64-131">In the **Qty. to Ship** field, specify how many of the order quantity to ship, the full or a partial order quantity.</span></span>
3. <span data-ttu-id="01b64-132">Kies de actie **Boeken** of **Boeken en verzenden**.</span><span class="sxs-lookup"><span data-stu-id="01b64-132">Choose the **Post** or **Post and Send** action.</span></span>
4. <span data-ttu-id="01b64-133">Kies vervolgens **de optie Verzenden** om later te factureren of de optie **Verzenden en factureren** om meteen te factureren.</span><span class="sxs-lookup"><span data-stu-id="01b64-133">Choose either the **Ship** option to invoice later, or the **Ship and Invoice** option to invoice immediately.</span></span>

## <a name="see-also"></a><span data-ttu-id="01b64-134">Zie ook</span><span class="sxs-lookup"><span data-stu-id="01b64-134">See Also</span></span>
<span data-ttu-id="01b64-135">[Procedure: Producten verkopen](sales-how-sell-products.md)  </span><span class="sxs-lookup"><span data-stu-id="01b64-135">[How to: Sell Products](sales-how-sell-products.md)  </span></span>  
[<span data-ttu-id="01b64-136">Procedure: Inkopen vastleggen</span><span class="sxs-lookup"><span data-stu-id="01b64-136">How to: Record Purchases</span></span>](purchasing-how-record-purchases.md)  
[<span data-ttu-id="01b64-137">Verkoop beheren</span><span class="sxs-lookup"><span data-stu-id="01b64-137">Manage Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="01b64-138">[Voorraad beheren](inventory-manage-inventory.md)    </span><span class="sxs-lookup"><span data-stu-id="01b64-138">[Manage Inventory](inventory-manage-inventory.md)    </span></span>  
[<span data-ttu-id="01b64-139">Werken met Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="01b64-139">Work with Dynamics NAV</span></span>](ui-work-product.md)


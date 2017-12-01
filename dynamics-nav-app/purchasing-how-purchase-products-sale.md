---
title: Een inkoopfactuur maken van een verkoopfactuur om artikelen te kopen voor een verkoop
description: Vanuit een verkoopfactuur kunt u, om producten te kopen, een inkoopfactuur maken voor een leverancier.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: supply planning, sales demand, replenish
ms.date: 05/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 0ba1fa771a0853c2a2cabe4d368cc09902496b01
ms.contentlocale: nl-nl
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-purchase-items-for-a-sale"></a><span data-ttu-id="4af0d-103">Procedure: Producten kopen voor een verkoop</span><span class="sxs-lookup"><span data-stu-id="4af0d-103">How to: Purchase Items for a Sale</span></span>
<span data-ttu-id="4af0d-104">Vanuit verkooporders en verkoopfacturen kunt u functie gebruiken om snel inkoopdocumenten te maken voor ontbrekende artikelaantallen die vereist worden door de verkoop.</span><span class="sxs-lookup"><span data-stu-id="4af0d-104">From sales orders and sales invoices, you can use functions to quickly create purchase documents for missing item quantities that are required by the sale.</span></span> <span data-ttu-id="4af0d-105">U kunt twee verschillende functies gebruiken, afhankelijk van de documentsoort.</span><span class="sxs-lookup"><span data-stu-id="4af0d-105">You can use two different functions depending on the document type.</span></span>
|<span data-ttu-id="4af0d-106">Functie</span><span class="sxs-lookup"><span data-stu-id="4af0d-106">Function</span></span>|<span data-ttu-id="4af0d-107">Description</span><span class="sxs-lookup"><span data-stu-id="4af0d-107">Description</span></span>|
|--------|-----------|
|<span data-ttu-id="4af0d-108">**Inkooporders maken**</span><span class="sxs-lookup"><span data-stu-id="4af0d-108">**Create Purchase Orders**</span></span>|<span data-ttu-id="4af0d-109">Vanuit een verkooporder maakt deze functie een inkooporder voor elk van de artikelen op de verkooporder.</span><span class="sxs-lookup"><span data-stu-id="4af0d-109">From a sales order, this function creates a purchase order for each vendor of items on the sales order.</span></span> <span data-ttu-id="4af0d-110">U kunt het inkoopaantal wijzigen voordat u de inkooporders maakt.</span><span class="sxs-lookup"><span data-stu-id="4af0d-110">You can edit the purchase quantity before you create the purchase orders.</span></span> <span data-ttu-id="4af0d-111">Alleen niet-beschikbare verkoopaantallen worden voorgesteld.</span><span class="sxs-lookup"><span data-stu-id="4af0d-111">Only unavailable sales quantities are suggested.</span></span>
|<span data-ttu-id="4af0d-112">**Inkoopfactuur maken**</span><span class="sxs-lookup"><span data-stu-id="4af0d-112">**Create Purchase Invoice**</span></span>|<span data-ttu-id="4af0d-113">Vanuit een verkooporder en vanuit een verkoopfactuur maakt deze functie een inkoopfactuur voor een geselecteerde leverancier voor alle regels of geselecteerde regels op het verkoopdocument.</span><span class="sxs-lookup"><span data-stu-id="4af0d-113">From a sales order and from a sales invoice, this function creates a purchase invoice for a selected vendor for all lines or selected lines on the sales document.</span></span> <span data-ttu-id="4af0d-114">Het volledige verkoopaantal wordt voorgesteld.</span><span class="sxs-lookup"><span data-stu-id="4af0d-114">The full sales quantity is suggested.</span></span>|

## <a name="to-create-one-or-more-purchase-orders-from-a-sales-order"></a><span data-ttu-id="4af0d-115">Een of meerdere inkooporders van een verkooporder maken</span><span class="sxs-lookup"><span data-stu-id="4af0d-115">To create one or more purchase orders from a sales order</span></span>
<span data-ttu-id="4af0d-116">Als u een inkooporder wilt maken voor elk niet-beschikbaar artikelaantal op de verkooporder, gebruikt u de functie **Inkooporders maken**.</span><span class="sxs-lookup"><span data-stu-id="4af0d-116">To create a purchase order for each unavailable item quantity on the sales order, you use the **Create Purchase Orders** function.</span></span>

1. <span data-ttu-id="4af0d-117">Kies op de startpagina de tegel **Doorlopende verkooporders**.</span><span class="sxs-lookup"><span data-stu-id="4af0d-117">On the Home page, choose the **Ongoing Sales Orders** tile.</span></span>
2. <span data-ttu-id="4af0d-118">Open een verkooporder waarvoor u artikelen wilt inkopen.</span><span class="sxs-lookup"><span data-stu-id="4af0d-118">Open a sales order that you want to purchase items for.</span></span>
3. <span data-ttu-id="4af0d-119">Kies de actie **Inkooporders maken**.</span><span class="sxs-lookup"><span data-stu-id="4af0d-119">Choose the **Create Purchase Orders** action.</span></span>

    <span data-ttu-id="4af0d-120">Het venster **Inkooporders maken** wordt geopend met een regel voor elk ander artikel op de verkooporder.</span><span class="sxs-lookup"><span data-stu-id="4af0d-120">The **Create Purchase Orders** window opens showing a line for each different item on the sales order.</span></span> <span data-ttu-id="4af0d-121">Regels voor volledig beschikbare verkoopaantallen en niet-beschikbare verkoopaantallen (grijs) worden standaard weergegeven.</span><span class="sxs-lookup"><span data-stu-id="4af0d-121">Lines for both fully available sales quantities and unavailable sales quantities (grayed) are shown by default.</span></span> <span data-ttu-id="4af0d-122">U kunt de actie **Niet-beschikbare weergeven** kiezen om alleen regels weer te geven voor niet-beschikbare verkoopaantallen.</span><span class="sxs-lookup"><span data-stu-id="4af0d-122">You can choose the **Show Unavailable** action to only see lines for unavailable sales quantities.</span></span>

    <span data-ttu-id="4af0d-123">Het veld **In te kopen aantal** bevat standaard het niet-beschikbare verkoopaantal.</span><span class="sxs-lookup"><span data-stu-id="4af0d-123">The **Quantity to Purchase** field contains the unavailable sales quantity by default.</span></span>
4. <span data-ttu-id="4af0d-124">Als u een ander aantal wilt aanschaffen dan het niet-beschikbare verkoopaantal, bewerkt u de waarde in het veld **In te kopen aantal**.</span><span class="sxs-lookup"><span data-stu-id="4af0d-124">To purchase another quantity than the unavailable sales quantity, edit the value in the **Quantity to Purchase** field.</span></span>

    > [!NOTE]  
>   <span data-ttu-id="4af0d-125">U kunt ook het veld **In te kopen aantal** wijzigen op grijze regels, ook al vertegenwoordigen deze volledig beschikbare verkoopaantallen.</span><span class="sxs-lookup"><span data-stu-id="4af0d-125">You can also change the **Quantity to Purchase** field on grayed lines even though they represent fully available sales quantities.</span></span>
5. <span data-ttu-id="4af0d-126">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="4af0d-126">Choose the **OK** button.</span></span>

    <span data-ttu-id="4af0d-127">Een inkooporder wordt gemaakt voor elke leverancier van artikelen op de verkooporder, inclusief aantalwijzigingen die u aanbrengt in het venster **Inkooporders maken**.</span><span class="sxs-lookup"><span data-stu-id="4af0d-127">A purchase order is created for each vendor of items on the sales order, including any quantity changes that you made in the **Create Purchase Orders** window.</span></span>
7. <span data-ttu-id="4af0d-128">Ga verder met het verwerken van de inkooporder of -orders, bijvoorbeeld door inkooporderregels te bewerken of toe te voegen.</span><span class="sxs-lookup"><span data-stu-id="4af0d-128">Proceed to process the purchase order or orders, for example, by editing or adding purchase order lines.</span></span> <span data-ttu-id="4af0d-129">Zie voor meer informatie [Procedure: Inkopen vastleggen](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="4af0d-129">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>


## <a name="to-create-a-purchase-invoice-from-a-sales-order-or-sales-invoice"></a><span data-ttu-id="4af0d-130">Een inkoopfactuur van een verkooporder of verkoopfactuur maken</span><span class="sxs-lookup"><span data-stu-id="4af0d-130">To create a purchase invoice from a sales order or sales invoice</span></span>
<span data-ttu-id="4af0d-131">Als u één inkoopfactuur wilt maken voor een of meer regels in een verkoopdocument door eerst te selecteren van welke leverancier wordt gekocht, gebruikt u de functie **Inkoopfactuur maken**.</span><span class="sxs-lookup"><span data-stu-id="4af0d-131">To create a single purchase invoice for one or more lines on a sales document by first selecting which vendor to buy from, you use the **Create Purchase Invoice** function.</span></span>

> [!NOTE]  
>   <span data-ttu-id="4af0d-132">Deze functie maakt een inkoopfactuur voor het exacte artikelaantal op het geselecteerde verkoopdocument.</span><span class="sxs-lookup"><span data-stu-id="4af0d-132">This function creates a purchase invoice for the exact item quantity on the selected sales document.</span></span> <span data-ttu-id="4af0d-133">Als u het inkoopaantal wilt wijzigen, moet u de inkoopfactuur wijzigen nadat deze is gemaakt.</span><span class="sxs-lookup"><span data-stu-id="4af0d-133">To change the purchase quantity, you must edit the purchase invoice after it is created.</span></span>  

1. <span data-ttu-id="4af0d-134">Kies op de startpagina de tegel **Doorlopende verkoopfacturen**.</span><span class="sxs-lookup"><span data-stu-id="4af0d-134">On the Home page, choose the **Ongoing Sales Invoices** tile.</span></span>
2. <span data-ttu-id="4af0d-135">Open een verkoopfactuur waarvoor u artikelen wilt inkopen.</span><span class="sxs-lookup"><span data-stu-id="4af0d-135">Open a sales invoice that you want to purchase items for.</span></span>
3. <span data-ttu-id="4af0d-136">Selecteer een of meer verkoopfactuurregels die u wilt gebruiken op de inkoopfactuur.</span><span class="sxs-lookup"><span data-stu-id="4af0d-136">Select one or more sales invoice lines that you want to use on the purchase invoice.</span></span> <span data-ttu-id="4af0d-137">Als u alle verkoopfactuurregels wilt gebruiken, selecteert u ze allemaal of selecteert u helemaal geen regels.</span><span class="sxs-lookup"><span data-stu-id="4af0d-137">To use all the sales invoice lines, select either all of them or do not select any lines.</span></span>
4. <span data-ttu-id="4af0d-138">Kies de actie **Inkoopfactuur maken**.</span><span class="sxs-lookup"><span data-stu-id="4af0d-138">Choose the **Create Purchase Invoice** action.</span></span>
5. <span data-ttu-id="4af0d-139">Selecteer **Alle regels** of **Geselecteerde regels** en kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="4af0d-139">Select either **All Lines** or **Selected Lines**, and then choose the **OK** button.</span></span>  
6. <span data-ttu-id="4af0d-140">Selecteer in de lijst met leveranciers die wordt weergegeven, de leverancier van wie u alle artikelen wilt kopen en kies vervolgens de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="4af0d-140">In the list of vendors that appears, select the vendor that you want to buy all the items from, and then choose the **OK** button.</span></span>

    <span data-ttu-id="4af0d-141">Er wordt een inkoopfactuur gemaakt die één, meerdere of alle regels op de verkoopfactuur bevat.</span><span class="sxs-lookup"><span data-stu-id="4af0d-141">A purchase invoice is created that contains one, more, or all the lines on the sales invoice.</span></span>
7. <span data-ttu-id="4af0d-142">Ga verder met het verwerken van de inkoopfactuur, bijvoorbeeld door inkoopfactuurregels te bewerken of toe te voegen.</span><span class="sxs-lookup"><span data-stu-id="4af0d-142">Proceed to process the purchase invoice, for example, by editing or adding purchase invoice lines.</span></span> <span data-ttu-id="4af0d-143">Zie voor meer informatie [Procedure: Inkopen vastleggen](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="4af0d-143">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="4af0d-144">Zie ook</span><span class="sxs-lookup"><span data-stu-id="4af0d-144">See Also</span></span>
[<span data-ttu-id="4af0d-145">Inkoop</span><span class="sxs-lookup"><span data-stu-id="4af0d-145">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="4af0d-146">Procedure: Inkopen vastleggen</span><span class="sxs-lookup"><span data-stu-id="4af0d-146">How to: Record Purchases</span></span>](purchasing-how-record-purchases.md)  
[<span data-ttu-id="4af0d-147">Procedure: Verkopen factureren</span><span class="sxs-lookup"><span data-stu-id="4af0d-147">How to: Invoice Sales</span></span>](sales-how-invoice-sales.md)  
[<span data-ttu-id="4af0d-148">Procedure: Nieuwe leveranciers registreren</span><span class="sxs-lookup"><span data-stu-id="4af0d-148">How to: Register New Vendors</span></span>](purchasing-how-register-new-vendors.md)  
<span data-ttu-id="4af0d-149">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="4af0d-149">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>


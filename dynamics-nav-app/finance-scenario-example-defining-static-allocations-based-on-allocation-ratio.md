---
title: "Statische toewijzingen op basis van de verdeelsleutel definiëren"
description: De methode voor statische toewijzingen baseert zich op een vaste waarde voor bijvoorbeeld gebruikte vierkante meters of een vastgestelde verdeelsleutel, zoals 5:2:4.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 9471cc39baa5f3b6aae705ab1eff22c0a7f304be
ms.contentlocale: nl-nl
ms.lasthandoff: 12/01/2017

---
# <a name="scenario-example-defining-static-allocations-based-on-allocation-ratio"></a><span data-ttu-id="48080-103">Voorbeeld scenario: statische toewijzingen op basis van de verdeelsleutel definiëren</span><span class="sxs-lookup"><span data-stu-id="48080-103">Scenario Example: Defining Static Allocations Based on Allocation Ratio</span></span>
<span data-ttu-id="48080-104">De methode voor statische toewijzingen baseert zich op een vaste waarde voor bijvoorbeeld gebruikte vierkante meters of een vastgestelde verdeelsleutel, zoals 5:2:4.</span><span class="sxs-lookup"><span data-stu-id="48080-104">Static allocation method is based on a definite value, such as square meters used, or an established allocation ratio such as 5:2:4.</span></span>  

<span data-ttu-id="48080-105">In dit onderwerp wordt beschreven hoe u drie nieuwe verdeeldoelen voor kostenobjecten kunt definiëren voor de verdelingsbron van kostenplaats PROD met behulp van de vastgestelde verdeelsleutel 5: 2: 4.</span><span class="sxs-lookup"><span data-stu-id="48080-105">This topic describes how to define three new allocation target cost objects for the allocation source PROD cost center using the established allocation ratio 5:2:4.</span></span> <span data-ttu-id="48080-106">De drie doelkostenobjecten zijn ACCESSO, VERF en TOEBEHOREN.</span><span class="sxs-lookup"><span data-stu-id="48080-106">The three target cost objects are ACCESSO, PAINT, and FITTINGS.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="48080-107">In het voorbeeld worden de demogegevens in de [!INCLUDE[d365fin](includes/d365fin_md.md)] gebruikt.</span><span class="sxs-lookup"><span data-stu-id="48080-107">The example uses the demo data in the [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

## <a name="to-define-the-allocation-source-prod-cost-center-on-the-general-fasttab"></a><span data-ttu-id="48080-108">De verdelingsbron van kostenplaats PROD op het sneltabblad Algemeen definiëren</span><span class="sxs-lookup"><span data-stu-id="48080-108">To define the allocation source PROD cost center on the General FastTab</span></span>  

1.  <span data-ttu-id="48080-109">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Kostenverdeling** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="48080-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Cost Allocation**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="48080-110">Kies in het venster **Kostenverdeling** de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="48080-110">In the **Cost Allocation** window, choose the **New** action.</span></span>  
3.  <span data-ttu-id="48080-111">Druk in het veld **ID** op Enter of voer een id in.</span><span class="sxs-lookup"><span data-stu-id="48080-111">In the **ID** field, press Enter or enter an ID.</span></span>  
4.  <span data-ttu-id="48080-112">Geef **1** op in het veld **Niveau**.</span><span class="sxs-lookup"><span data-stu-id="48080-112">In the **Level** field, enter **1**.</span></span>  
5.  <span data-ttu-id="48080-113">Voer in de velden **Geldig vanaf** en **Geldig tot** juiste datums in.</span><span class="sxs-lookup"><span data-stu-id="48080-113">In the **Valid From** and **Valid To** fields, enter appropriate dates.</span></span>  
6.  <span data-ttu-id="48080-114">Voer in het veld **Kostenplaatscode** **PROD** in.</span><span class="sxs-lookup"><span data-stu-id="48080-114">In the **Cost Center Code** field, enter **PROD**.</span></span>  
7.  <span data-ttu-id="48080-115">Voer in het veld **Credit naar kostensoort** het kostensoort **9903** in.</span><span class="sxs-lookup"><span data-stu-id="48080-115">In the **Credit to Cost Type** field, enter the cost type **9903**.</span></span>  

## <a name="to-define-the-allocation-target-cost-objects-on-the-lines-fasttab"></a><span data-ttu-id="48080-116">Verdeeldoelen voor kostenobjecten op de sneltabblad Regels definiëren</span><span class="sxs-lookup"><span data-stu-id="48080-116">To define the allocation target cost objects on the Lines FastTab</span></span>  

1.  <span data-ttu-id="48080-117">Voer op de eerste regel in het veld **Doelkostensoort** **9903** in.</span><span class="sxs-lookup"><span data-stu-id="48080-117">On the first line, in the **Target Cost Type** field, enter **9903**.</span></span>  
2.  <span data-ttu-id="48080-118">Selecteer op de eerste regel in het veld **Doelkostenobject** **ACCESSO**.</span><span class="sxs-lookup"><span data-stu-id="48080-118">On the first line, in the **Target Cost Object** field, select **ACCESSO**.</span></span>  
3.  <span data-ttu-id="48080-119">Selecteer op de eerste regel in het veld **Verdelingsdoelsoort** de optie **Alle kosten** om te definiëren hoe te betalen kosten moeten worden toegewezen.</span><span class="sxs-lookup"><span data-stu-id="48080-119">On the first line, in the **Allocation Target Type** field, select **All Costs** to define how all accrued costs are allocated.</span></span>  
4.  <span data-ttu-id="48080-120">Op de eerste regel in het veld **Basis** selecteert u **Statisch** om de statische toewijzingsmethode te gebruiken.</span><span class="sxs-lookup"><span data-stu-id="48080-120">On the first line, in the **Base** field, select **Static** to use the static allocation method.</span></span>  
5.  <span data-ttu-id="48080-121">Op de eerste regel in het veld **Deel** voert u de verdeelsleutel **5** in.</span><span class="sxs-lookup"><span data-stu-id="48080-121">On the first line, in the **Share** field, enter the allocation ratio **5**.</span></span>  
6.  <span data-ttu-id="48080-122">Voer op de tweede regel in het veld **Doelkostensoort** **9903** in.</span><span class="sxs-lookup"><span data-stu-id="48080-122">On the second line, in the **Target Cost Type** field, enter **9903**.</span></span>  
7.  <span data-ttu-id="48080-123">Selecteer op de tweede regel in het veld **Doelkostenobject** **PAINT**.</span><span class="sxs-lookup"><span data-stu-id="48080-123">On the second line, in the **Target Cost Object** field, select **PAINT**.</span></span>  
8.  <span data-ttu-id="48080-124">Selecteer op de tweede regel in het veld **Verdelingsdoelsoort** de optie **Alle kosten** om te definiëren hoe te betalen kosten moeten worden toegewezen.</span><span class="sxs-lookup"><span data-stu-id="48080-124">On the second line, in the **Allocation Target Type** field, select **All Costs** to define how all accrued costs are allocated.</span></span>  
9. <span data-ttu-id="48080-125">Op de tweede regel in het veld **Basis** selecteert u **Statisch** om de statische toewijzingsmethode te gebruiken.</span><span class="sxs-lookup"><span data-stu-id="48080-125">On the second line, in the **Base** field, select **Static** to use the static allocation method.</span></span>  
10. <span data-ttu-id="48080-126">Op de tweede regel in het veld **Deel** voert u de verdeelsleutel **2** in.</span><span class="sxs-lookup"><span data-stu-id="48080-126">On the second line, in the **Share** field, enter the allocation ratio **2**.</span></span>  
11. <span data-ttu-id="48080-127">Voer op de derde regel in het veld **Doelkostensoort** **9903** in.</span><span class="sxs-lookup"><span data-stu-id="48080-127">On the third line, in the **Target Cost Type** field, enter **9903**.</span></span>  
12. <span data-ttu-id="48080-128">Selecteer op de derde regel in het veld **Doelkostenobject** **FITTINGS**.</span><span class="sxs-lookup"><span data-stu-id="48080-128">On the third line, in the **Target Cost Object** field, select **FITTINGS**.</span></span>  
13. <span data-ttu-id="48080-129">Selecteer op de derde regel in het veld **Verdelingsdoelsoort** de optie **Alle kosten** om te definiëren hoe te betalen kosten moeten worden toegewezen.</span><span class="sxs-lookup"><span data-stu-id="48080-129">On the third line, in the **Allocation Target Type** field, select **All Costs** to define how all accrued costs are allocated.</span></span>  
14. <span data-ttu-id="48080-130">Op de derde regel in het veld **Basis** selecteert u **Statisch** om de statische toewijzingsmethode te gebruiken.</span><span class="sxs-lookup"><span data-stu-id="48080-130">On the third line, in the **Base** field, select **Static** to use the static allocation method.</span></span>  
15. <span data-ttu-id="48080-131">Op de derde regel in het veld **Deel** voert u de verdeelsleutel **4** in.</span><span class="sxs-lookup"><span data-stu-id="48080-131">On the third line, in the **Share** field, enter the allocation ratio **4**.</span></span>  

> [!IMPORTANT]  
>  [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="48080-132"> berekent automatisch het veld **Percentage** met een percentage dat wordt bepaald door alle drie de verdeelsleutels die zijn ingevoerd in het veld **Deel** voor alle drie de regels.</span><span class="sxs-lookup"><span data-stu-id="48080-132"> automatically calculates the **Percent** field using a percentage rate that is dependent on all three allocation ratios that are entered in the **Share** field for all three lines.</span></span>  

## <a name="see-also"></a><span data-ttu-id="48080-133">Zie ook</span><span class="sxs-lookup"><span data-stu-id="48080-133">See Also</span></span>  
<span data-ttu-id="48080-134">[Procedure: een verdelingsbron en verdeeldoelen instellen.](finance-how-to-set-up-allocation-source-and-targets.md) </span><span class="sxs-lookup"><span data-stu-id="48080-134">[How to: Set Up Allocation Source and Targets](finance-how-to-set-up-allocation-source-and-targets.md) </span></span>  
<span data-ttu-id="48080-135">[Kosten definiëren en toewijzen](finance-define-and-allocate-costs.md) </span><span class="sxs-lookup"><span data-stu-id="48080-135">[Defining and Allocating Costs](finance-define-and-allocate-costs.md) </span></span>  
<span data-ttu-id="48080-136">[Voorbeeldscenario: dynamische toewijzingen op basis van de verkochte artikelen definiëren](finance-scenario-example-defining-dynamic-allocations-based-on-items-sold.md) </span><span class="sxs-lookup"><span data-stu-id="48080-136">[Scenario Example: Defining Dynamic Allocations Based on Items Sold](finance-scenario-example-defining-dynamic-allocations-based-on-items-sold.md) </span></span>  
[<span data-ttu-id="48080-137">Kosten definiëren en toewijzen</span><span class="sxs-lookup"><span data-stu-id="48080-137">Defining and Allocating Costs</span></span>](finance-define-and-allocate-costs.md)


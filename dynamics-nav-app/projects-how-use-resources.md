---
title: 'Procedure: Resources gebruiken voor projecten'
author: SorenGP
ms.custom: na
ms.date: 12/14/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: cced4bca42b74c2664fd18770f1616c57286e1c3
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-use-resources-for-jobs"></a><span data-ttu-id="40051-102">Procedure: Resources gebruiken voor projecten</span><span class="sxs-lookup"><span data-stu-id="40051-102">How to: Use Resources for Jobs</span></span>
<span data-ttu-id="40051-103">U legt het gebruik van resources vast in het projectdagboek om kosten, prijzen en de werksoorten bij te houden die zijn gekoppeld aan projecten.</span><span class="sxs-lookup"><span data-stu-id="40051-103">You record the usage of resources in the job journal to keep track of costs, prices, and the work types that are linked to jobs.</span></span> <span data-ttu-id="40051-104">Zie voor meer informatie [Procedure: Gebruik vastleggen voor projecten](projects-how-record-job-usage.md).</span><span class="sxs-lookup"><span data-stu-id="40051-104">For more information, see [How to: Record Usage for Jobs](projects-how-record-job-usage.md).</span></span>

<span data-ttu-id="40051-105">U kunt ook het verbruik van een resource boeken in een resourcedagboek.</span><span class="sxs-lookup"><span data-stu-id="40051-105">You can also post the usage of a resource in a resource journal.</span></span> <span data-ttu-id="40051-106">Posten die in een resourcedagboek zijn geboekt, werken niet door in het grootboek.</span><span class="sxs-lookup"><span data-stu-id="40051-106">Entries posted in a resource journal have no effect on the general ledger.</span></span>

## <a name="to-assign-resources-to-jobs"></a><span data-ttu-id="40051-107">Resources toewijzen aan projecten</span><span class="sxs-lookup"><span data-stu-id="40051-107">To assign resources to jobs</span></span>
<span data-ttu-id="40051-108">U wijst resources aan projecten toe door projectplanningsregels voor het project te maken.</span><span class="sxs-lookup"><span data-stu-id="40051-108">You assign resources to jobs by creating job planning lines for the job.</span></span> <span data-ttu-id="40051-109">Zie [Procedure: Projecten maken](projects-how-create-jobs.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="40051-109">For more information, see [How to: Create Jobs](projects-how-create-jobs.md).</span></span>

## <a name="to-record-resource-usage-for-a-job"></a><span data-ttu-id="40051-110">Resourceverbruik voor een project vastleggen</span><span class="sxs-lookup"><span data-stu-id="40051-110">To record resource usage for a job</span></span>

1. <span data-ttu-id="40051-111">Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Projectdagboeken** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="40051-111">In the top right corner, choose the **Search for Page or Report** icon, enter **Job Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="40051-112">Open een relevante projectdagboekbatch en vul indien nodig de velden in.</span><span class="sxs-lookup"><span data-stu-id="40051-112">Open a relevant job journal batch, and then fill in the fields as necessary.</span></span> <span data-ttu-id="40051-113">Kies een veld om een korte omschrijving van het veld of een koppeling naar meer informatie te lezen.</span><span class="sxs-lookup"><span data-stu-id="40051-113">Choose a field to read a short description of the field or link to more information.</span></span>
3. <span data-ttu-id="40051-114">Wanneer het dagboek compleet is, kiest u de actie **Boeken**.</span><span class="sxs-lookup"><span data-stu-id="40051-114">When the journal is complete, choose the **Post** action.</span></span>

## <a name="to-adjust-resource-prices"></a><span data-ttu-id="40051-115">Resourceprijzen aanpassen</span><span class="sxs-lookup"><span data-stu-id="40051-115">To adjust resource prices</span></span>  
<span data-ttu-id="40051-116">Als u kost- of verkoopprijzen wilt wijzigen voor een groot aantal resources, kunt u een batchverwerking gebruiken.</span><span class="sxs-lookup"><span data-stu-id="40051-116">If you want to change costs or prices for a large number of resources, you can use a batch job.</span></span>  

1. <span data-ttu-id="40051-117">Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Resourceprijzen herwaarderen** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="40051-117">In the top right corner, choose the **Search for Page or Report** icon, enter **Adjust Resource Costs/Prices**, and then choose the related link.</span></span>
2. <span data-ttu-id="40051-118">Vul de overige velden op een regel desgewenst in en kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="40051-118">Fill in the fields on a line as necessary, and then choose the **OK** button.</span></span>

<span data-ttu-id="40051-119">**Opmerking**: met deze batchverwerking worden geen alternatieve kost- of verkoopprijzen voor resources gemaakt of aangepast.</span><span class="sxs-lookup"><span data-stu-id="40051-119">**Note**: This batch job does not create or adjust alternate costs or prices for resources.</span></span> <span data-ttu-id="40051-120">Dit verandert alleen de inhoud van het veld op de resourcekaart voor het veld **Aan te passen prijs** dat u hebt geselecteerd in de batchtaak.</span><span class="sxs-lookup"><span data-stu-id="40051-120">It only changes the contents of the field on the resource card for the **Adjust Field** field that you selected in the batch job.</span></span> <span data-ttu-id="40051-121">De aanpassing werkt onmiddellijk door voor de resources. Controleer daarom uw herwaarderingsfactoren zorgvuldig voordat u de batchverwerking uitvoert.</span><span class="sxs-lookup"><span data-stu-id="40051-121">The adjustment will take effect immediately for resources, so check your adjustment factors before you run the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-existing-alternate-prices"></a><span data-ttu-id="40051-122">Suggesties voor wijzigingen van resourceprijzen krijgen op basis van bestaande alternatieve prijzen</span><span class="sxs-lookup"><span data-stu-id="40051-122">To get resource price change suggestions based on existing alternate prices</span></span>  
<span data-ttu-id="40051-123">Als u al alternatieve resourceprijzen hebt ingesteld voor bepaalde resources, kunt u een batchverwerking gebruiken om meerdere alternatieve resourceprijzen in te stellen.</span><span class="sxs-lookup"><span data-stu-id="40051-123">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span></span>

1. <span data-ttu-id="40051-124">Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Resourceprijswijzigingen** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="40051-124">In the top right corner, choose the **Search for Page or Report** icon, enter **Resource Price Changes**, and then choose the related link.</span></span>
2. <span data-ttu-id="40051-125">Kies de actie **Res.prijsvoorstellen (Prijs)** en vul indien nodig de velden in.</span><span class="sxs-lookup"><span data-stu-id="40051-125">Choose the **Suggest Res. Price Chg. (Price)** action, and then fill in the fields as necessary.</span></span>
3. <span data-ttu-id="40051-126">Kies de knop **Ok**.</span><span class="sxs-lookup"><span data-stu-id="40051-126">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="40051-127">Nadat de batchverwerking is voltooid, bevat het venster **Resourceprijswijzigingen** de resultaten van de batchverwerking.</span><span class="sxs-lookup"><span data-stu-id="40051-127">When the batch job is finished, the **Resource Price Changes** window shows the results of the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-standard-prices"></a><span data-ttu-id="40051-128">Resourceprijsvoorstellen ophalen op basis van standaardverkoopprijzen</span><span class="sxs-lookup"><span data-stu-id="40051-128">To get resource price change suggestions based on standard prices</span></span>  
<span data-ttu-id="40051-129">Als u meerdere alternatieve resourceprijzen wilt instellen op basis van de standaardverkoopprijzen op de resourcekaarten, kunt u een batchverwerking gebruiken.</span><span class="sxs-lookup"><span data-stu-id="40051-129">If you want to set up multiple alternate resource prices based on the standard prices on the resource cards, you can use a batch job.</span></span>  

1. <span data-ttu-id="40051-130">Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Resourceprijswijzigingen** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="40051-130">In the top right corner, choose the **Search for Page or Report** icon, enter **Resource Price Changes**, and then choose the related link.</span></span>
2. <span data-ttu-id="40051-131">Kies de actie **Res.prijsvoorstellen (Res.)** en vul indien nodig de velden in.</span><span class="sxs-lookup"><span data-stu-id="40051-131">Choose the **Suggest Res. Price Chg. (Res.)** action, and then fill in the fields as necessary.</span></span>  
3. <span data-ttu-id="40051-132">Kies de knop **Ok**.</span><span class="sxs-lookup"><span data-stu-id="40051-132">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="40051-133">Nadat de batchverwerking is voltooid, opent u het venster **Resourceprijswijzigingen** om de resultaten van de batchverwerking te bekijken.</span><span class="sxs-lookup"><span data-stu-id="40051-133">When the batch job is finished, open the **Resource Price Changes** window to see the results of the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-alternate-prices"></a><span data-ttu-id="40051-134">Suggesties voor wijzigingen van resourceprijzen krijgen op basis van alternatieve prijzen</span><span class="sxs-lookup"><span data-stu-id="40051-134">To get resource price change suggestions based on alternate prices</span></span>  
<span data-ttu-id="40051-135">Als u al alternatieve resourceprijzen hebt ingesteld voor bepaalde resources, kunt u een batchverwerking gebruiken om meerdere alternatieve resourceprijzen in te stellen.</span><span class="sxs-lookup"><span data-stu-id="40051-135">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span></span>

1. <span data-ttu-id="40051-136">Voer **Res.prijsvoorstellen (Prijs)** in het tekstvak **Zoeken** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="40051-136">In the **Search** box, enter **Suggest Res. Price Chg. (Price)**, and then choose the related link.</span></span>  
2. <span data-ttu-id="40051-137">Vul indien nodig de velden in.</span><span class="sxs-lookup"><span data-stu-id="40051-137">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="40051-138">Kies de knop **Ok**.</span><span class="sxs-lookup"><span data-stu-id="40051-138">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="40051-139">Nadat de batchverwerking is voltooid, opent u het venster **Resourceprijswijzigingen** om de resultaten van de batchverwerking te bekijken.</span><span class="sxs-lookup"><span data-stu-id="40051-139">When the batch job is finished, open the **Resource Price Changes** window to see the results of the batch job.</span></span>

## <a name="see-also"></a><span data-ttu-id="40051-140">Zie ook</span><span class="sxs-lookup"><span data-stu-id="40051-140">See Also</span></span>
[<span data-ttu-id="40051-141">Projecten beheren</span><span class="sxs-lookup"><span data-stu-id="40051-141">Manage Projects</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="40051-142">Financiën</span><span class="sxs-lookup"><span data-stu-id="40051-142">Finance</span></span>](finance-setup.md)  
<span data-ttu-id="40051-143">[Inkoop beheren](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="40051-143">[Manage Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="40051-144">[Verkoop beheren](sales-manage-sales.md)   </span><span class="sxs-lookup"><span data-stu-id="40051-144">[Manage Sales](sales-manage-sales.md)   </span></span>  
[<span data-ttu-id="40051-145">Werken met Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="40051-145">Work With Dynamics NAV</span></span>](ui-work-product.md)  


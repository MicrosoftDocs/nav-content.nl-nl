---
title: Gegevens analyseren per dimensie
description: Beschrijft hoe u diverse bedrijfsgegevens analyseert per dimensie.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bi, power BI, analysis, KPI
ms.date: 06/13/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: a86031e20e7a5de266405166ee8025cde7221602
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
#  <a name="how-to-analyze-data-by-dimensions"></a><span data-ttu-id="9cc25-103">Procedure: Gegevens analyseren per dimensie</span><span class="sxs-lookup"><span data-stu-id="9cc25-103">How to: Analyze Data by Dimensions</span></span>
<span data-ttu-id="9cc25-104">In financiële analyses is een dimensie informatie die u kunt toevoegen aan een post als een soort kenteken.</span><span class="sxs-lookup"><span data-stu-id="9cc25-104">In financial analysis, a dimension is data that you can add to an entry as a kind of marker.</span></span> <span data-ttu-id="9cc25-105">Deze informatie wordt gebruikt om posten met vergelijkbare kenmerken te groeperen, zoals klanten, regio's, producten en verkopers, en om deze groepen eenvoudig op te kunnen roepen voor analyse.</span><span class="sxs-lookup"><span data-stu-id="9cc25-105">This data is used to group entries with similar characteristics, such as customers, regions, products, and salesperson, and easily retrieve these groups for analysis.</span></span> <span data-ttu-id="9cc25-106">Dimensies kunnen worden gebruikt op posten in dagboeken, documenten en budgetten.</span><span class="sxs-lookup"><span data-stu-id="9cc25-106">Dimensions can be used on entries in journals, documents, and budgets.</span></span> <span data-ttu-id="9cc25-107">De term dimensie beschrijft hoe analyse plaatsvindt.</span><span class="sxs-lookup"><span data-stu-id="9cc25-107">The term dimension describes how analysis occurs.</span></span> <span data-ttu-id="9cc25-108">Een tweedimensionale analyse is bijvoorbeeld verkoop per gebied.</span><span class="sxs-lookup"><span data-stu-id="9cc25-108">A two-dimensional analysis, for example, would be sales per area.</span></span> <span data-ttu-id="9cc25-109">Door echter meer dan twee dimensies te gebruiken bij het maken van een post, kunt u complexere analyses uitvoeren, zoals verkoop per verkoopcampagne per klantengroep per gebied.</span><span class="sxs-lookup"><span data-stu-id="9cc25-109">However, by using more than two dimensions when creating an entry, you can carry out a more complex analysis, such as sales per sales campaign per customer group per area.</span></span> <span data-ttu-id="9cc25-110">Zie voor meer informatie [Werken met dimensies](finance-dimensions.md).</span><span class="sxs-lookup"><span data-stu-id="9cc25-110">For more information, see [Working with Dimensions](finance-dimensions.md).</span></span>

<span data-ttu-id="9cc25-111">Door gegevens met dimensies te analyseren krijgt u een beter inzicht in uw bedrijf, zodat u informatie kunt evalueren, zoals hoe goed uw bedrijf draait, waar de zaken floreren en waar juist niet en waar meer resources moeten worden ingezet.</span><span class="sxs-lookup"><span data-stu-id="9cc25-111">Analyzing data by dimensions gives you greater insight into your business, so you can evaluate information, such as how well your business is operating, where it is thriving and where it is not, and where more resources should be allocated.</span></span>

> [!TIP]
> <span data-ttu-id="9cc25-112">Als snelle manier om transactiegegevens te analyseren per dimensie kunt u totalen in het rekeningschema en posten in de vensters **Posten** filteren op dimensie.</span><span class="sxs-lookup"><span data-stu-id="9cc25-112">As a quick way to analyze transactional data by dimensions, you can filter totals in the chart of accounts and entries in all **Entries** windows by dimensions.</span></span> <span data-ttu-id="9cc25-113">Zoek de actie **Dimensiefilter instellen**.</span><span class="sxs-lookup"><span data-stu-id="9cc25-113">Look for the **Set Dimension Filter** action.</span></span>

## <a name="to-set-up-an-analysis-view"></a><span data-ttu-id="9cc25-114">Een analyseweergave instellen</span><span class="sxs-lookup"><span data-stu-id="9cc25-114">To set up an analysis view</span></span>  
<span data-ttu-id="9cc25-115">Met een analyse op basis van dimensies geeft u een geselecteerde combinatie van dimensies weer.</span><span class="sxs-lookup"><span data-stu-id="9cc25-115">An analysis by dimensions displays a selected combination of dimensions.</span></span> <span data-ttu-id="9cc25-116">U kunt elke ingestelde analyse opslaan en ophalen.</span><span class="sxs-lookup"><span data-stu-id="9cc25-116">You can store and retrieve each analysis you have set up.</span></span> <span data-ttu-id="9cc25-117">De gegevens voor het instellen van een analyse worden op een **Analyseweergave**kaart opgeslagen om analyse in de toekomst te vereenvoudigen.</span><span class="sxs-lookup"><span data-stu-id="9cc25-117">The information for setting up an analysis is stored on an **Analysis View** card to simplify future analysis.</span></span>  

1. <span data-ttu-id="9cc25-118">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Analyseweergaven** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="9cc25-118">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Analysis Views**, and then choose the related link.</span></span>  
2. <span data-ttu-id="9cc25-119">Kies in het venster **Analyseweergaveoverzicht** de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="9cc25-119">In the **Analysis View List** window, choose the **New** action.</span></span>
3. <span data-ttu-id="9cc25-120">Vul indien nodig de velden in.</span><span class="sxs-lookup"><span data-stu-id="9cc25-120">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="9cc25-121">Als u andere dimensiecodes wilt toevoegen naast de vier op het sneltabblad **Dimensies**, kiest u de actie **Filteren**, vult u de velden in en kiest u de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="9cc25-121">To add other dimension codes in addition to the four on the **Dimensions** FastTab, choose the **Filter** action, fill in the fields, and then choose the **OK** button.</span></span>  
5. <span data-ttu-id="9cc25-122">Als u de weergave wilt bijwerken, kiest u de actie **Bijwerken**.</span><span class="sxs-lookup"><span data-stu-id="9cc25-122">To update the view, choose the **Update** action.</span></span>

## <a name="to-analyze-by-dimensions"></a><span data-ttu-id="9cc25-123">Analyseren per dimensie</span><span class="sxs-lookup"><span data-stu-id="9cc25-123">To analyze by dimensions</span></span>
<span data-ttu-id="9cc25-124">U kunt de matrix **Analyse per dimensie** gebruiken om de bedragen in uw grootboek te bekijken met de analyseweergaven die u al hebt ingesteld.</span><span class="sxs-lookup"><span data-stu-id="9cc25-124">You can use the **Analysis by Dimensions** matrix to view the amounts in your general ledger by using the analysis views that you have already set up.</span></span> <span data-ttu-id="9cc25-125">U vult het venster **Analyse per dimensie** in om te bepalen wat wordt weergegeven in de matrix en kiest vervolgens de actie **Matrix weergeven** om de matrix weer te geven..</span><span class="sxs-lookup"><span data-stu-id="9cc25-125">You fill in the **Analysis by Dimensions** window to define what will be shown in the matrix, and then you choose the **Show Matrix** action to view the matrix.</span></span>  

- <span data-ttu-id="9cc25-126">De kolommen aan de verre linkerzijde bevatten gegevens op basis van de selectie in het veld **Als regels weergeven** in de kop.</span><span class="sxs-lookup"><span data-stu-id="9cc25-126">The leftmost columns contain information based on what you have selected in the **Show as Lines** field in the header.</span></span>  
- <span data-ttu-id="9cc25-127">De kolommen aan de verre rechterzijde bevatten gegevens op basis van de selectie in het veld **Als kolommen weergeven** in de kop.</span><span class="sxs-lookup"><span data-stu-id="9cc25-127">The rightmost columns contain information based on to what you have selected in the **Show as Columns** field in the header.</span></span>  

1. <span data-ttu-id="9cc25-128">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Analyse per dimensie** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="9cc25-128">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Analysis by Dimensions**, and then choose the related link.</span></span>  
2. <span data-ttu-id="9cc25-129">Selecteer de relevante analyseweergave en kies vervolgens de actie **Analyseweergave bewerken**.</span><span class="sxs-lookup"><span data-stu-id="9cc25-129">Select the relevant analysis view,  and then choose the **Edit Analysis View** action.</span></span>
3. <span data-ttu-id="9cc25-130">Vul boven in het venster **Analyse per dimensie** de velden in om te definiëren wat wordt weergegeven.</span><span class="sxs-lookup"><span data-stu-id="9cc25-130">At the top of the **Analysis by Dimensions** window, fill in the fields to define what is shown.</span></span>
4. 5. <span data-ttu-id="9cc25-131">Als u wilt weten uit welke bedragen een bedrag in de matrix bestaat, selecteert u het bedrag.</span><span class="sxs-lookup"><span data-stu-id="9cc25-131">To see a specification of an amount shown in the matrix window, choose the amount.</span></span>  

> [!IMPORTANT]  
>   <span data-ttu-id="9cc25-132">U kunt geen periode selecteren die korter is dan de opgegeven periode voor datumcompressie op de **Analyseweergave**-kaart.</span><span class="sxs-lookup"><span data-stu-id="9cc25-132">You cannot select a period length shorter than the period specified for the date compression on the **Analysis View** card.</span></span> <span data-ttu-id="9cc25-133">De opdrachten **Volgende set** en **Vorige set** zijn niet ingeschakeld als u **Periode** hebt geselecteerd in het veld **Als regels weergeven** of **Als kolommen weergeven**.</span><span class="sxs-lookup"><span data-stu-id="9cc25-133">The **Next Set** and **Previous Set** commands are inactive if you have selected **Period** in either the **Show as Lines** or the **Show as Columns** field.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="9cc25-134">Met de lijst **Dimensies - detail** kunt u een gedetailleerde classificatie weergeven van de wijze waarop dimensies zijn gebruikt voor posten gedurende een geselecteerde periode.</span><span class="sxs-lookup"><span data-stu-id="9cc25-134">You can use the **Dimensions - Detail** report to display a detailed classification of how dimensions have been used on entries over a selected period.</span></span> <span data-ttu-id="9cc25-135">Met de lijst **Dimensies - totaal** kunt u alleen de totale bedragen weergeven.</span><span class="sxs-lookup"><span data-stu-id="9cc25-135">You can use the **Dimensions - Total ** report to display only the total amounts.</span></span>  

> [!TIP]  
>   <span data-ttu-id="9cc25-136">U kunt de weergave ook wijzigen door de inhoud van het veld **Als regels weergeven** en het veld **Als kolommen weergeven** te veranderen.</span><span class="sxs-lookup"><span data-stu-id="9cc25-136">You can also change the view by changing the contents of the **Show as Lines** field and **Show as Columns** field.</span></span> <span data-ttu-id="9cc25-137">Als u een weergave-instelling wilt omkeren, kiest u de actie **Regels en kolommen omkeren**.</span><span class="sxs-lookup"><span data-stu-id="9cc25-137">To reverse a view setting, choose the **Reverse Lines and Columns** action.</span></span>

## <a name="to-update-an-analysis-view"></a><span data-ttu-id="9cc25-138">Analyseweergave bijwerken</span><span class="sxs-lookup"><span data-stu-id="9cc25-138">To update an analysis view</span></span>  
<span data-ttu-id="9cc25-139">Met de bedragen die worden weergegeven in het venster **Analyse per dimensies**, krijgt u een overzicht van de status van het bedrijf die gold op het moment dat u voor het laatst hebt bijgewerkt.</span><span class="sxs-lookup"><span data-stu-id="9cc25-139">The amounts that are displayed in the **Analysis by Dimensions** window give you a picture of the company’s state at the time of the last update.</span></span> <span data-ttu-id="9cc25-140">Als u de huidige status wilt weten, moet u de analyseweergave bijwerken.</span><span class="sxs-lookup"><span data-stu-id="9cc25-140">To get a picture of the current state, you must update the analysis view by running the update function.</span></span>

<span data-ttu-id="9cc25-141">Met de volgende procedure kunt u een analyseweergave bijwerken vanuit het venster **Analyse per dimensies**.</span><span class="sxs-lookup"><span data-stu-id="9cc25-141">The following procedure is for updating an analysis view from the **Analysis by Dimensions** window.</span></span> <span data-ttu-id="9cc25-142">De stappen zijn vergelijkbaar vanuit het venster **Analyseweergave** en **Analyseweergaveoverzicht**.</span><span class="sxs-lookup"><span data-stu-id="9cc25-142">The steps are similar from the **Analysis View Card** and the **Analysis View List** windows.</span></span>  

1. <span data-ttu-id="9cc25-143">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Analyse per dimensie** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="9cc25-143">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Analysis by Dimensions**, and then choose the related link.</span></span>  
2. <span data-ttu-id="9cc25-144">Kies in het venster **Analyse per dimensie** het veld **Analyseweergavecode**.</span><span class="sxs-lookup"><span data-stu-id="9cc25-144">In the **Analysis by Dimensions** window, choose the **Analysis View Code** field.</span></span>  
3. <span data-ttu-id="9cc25-145">Selecteer de regel met de gewenste analyseweergave.</span><span class="sxs-lookup"><span data-stu-id="9cc25-145">Select the line with the relevant analysis view.</span></span>  
4. <span data-ttu-id="9cc25-146">Kies de actie **Bijwerken**.</span><span class="sxs-lookup"><span data-stu-id="9cc25-146">Choose the **Update** action.</span></span>  

> [!TIP]  
>   <span data-ttu-id="9cc25-147">Als u het selectievakje **Bijwerken bij boeking** op een analyseweergavekaart selecteert, wordt de weergave automatisch bijgewerkt wanneer een desbetreffende transactie wordt geboekt.</span><span class="sxs-lookup"><span data-stu-id="9cc25-147">If you select the **Update on Posting** check box on an analysis view card, the view is automatically updated when an involved transaction is posted.</span></span>

> [!NOTE]  
>   <span data-ttu-id="9cc25-148">Als u bepaalde of alle analyseweergaven tegelijk wilt bijwerken, moet u de batchverwerking **Analyseweergaven bijwerken** gebruiken.</span><span class="sxs-lookup"><span data-stu-id="9cc25-148">To update some or all analysis views at the same time, you must use the **Update Analysis Views** batch job.</span></span>  

## <a name="see-also"></a><span data-ttu-id="9cc25-149">Zie ook</span><span class="sxs-lookup"><span data-stu-id="9cc25-149">See Also</span></span>
[<span data-ttu-id="9cc25-150">Bedrijfsinformatie</span><span class="sxs-lookup"><span data-stu-id="9cc25-150">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="9cc25-151">Financiën</span><span class="sxs-lookup"><span data-stu-id="9cc25-151">Finance</span></span>](finance.md)  
[<span data-ttu-id="9cc25-152">Financiën instellen</span><span class="sxs-lookup"><span data-stu-id="9cc25-152">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="9cc25-153">Het grootboek en het rekeningschema</span><span class="sxs-lookup"><span data-stu-id="9cc25-153">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
[<span data-ttu-id="9cc25-154">Werken met dimensies</span><span class="sxs-lookup"><span data-stu-id="9cc25-154">Working with Dimensions</span></span>](finance-dimensions.md)  
<span data-ttu-id="9cc25-155">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9cc25-155">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

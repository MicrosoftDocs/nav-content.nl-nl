---
title: Werken met rekeningschema's
description: "Beschrijft hoe u rapportageschema's gebruikt om diverse weergaven en lijsten te maken om financiële prestatiegegevens te analyseren."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bi, power BI, analysis, KPI
ms.date: 08/11/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: f0d979b41ea498b157241c94d557b325a5b19f67
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-work-with-account-schedules"></a><span data-ttu-id="243da-103">Procedure: Werken met rapportageschema's</span><span class="sxs-lookup"><span data-stu-id="243da-103">How to: Work with Account Schedules</span></span>
<span data-ttu-id="243da-104">Gebruik rapportageschema's om inzicht te krijgen in de financiële gegevens die in uw rekeningschema zijn opgeslagen.</span><span class="sxs-lookup"><span data-stu-id="243da-104">Use account schedules to get insight into the financial data stored in your chart of accounts.</span></span> <span data-ttu-id="243da-105">Met rapportageschema's worden cijfers geanalyseerd in grootboekrekeningen en worden grootboekposten vergeleken met budgetposten voor het grootboek.</span><span class="sxs-lookup"><span data-stu-id="243da-105">Account schedules analyze figures in G/L accounts, and compare general ledger entries with general ledger budget entries.</span></span> <span data-ttu-id="243da-106">De resultaten worden weergegeven in diagrammen op uw startpagina, zoals het cashflowdiagram.</span><span class="sxs-lookup"><span data-stu-id="243da-106">The results display in charts on your Home page, such as the Cash Flow chart.</span></span>  

[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="243da-107"> biedt een aantal voorbeeldrapportageschema's die u direct kunt gebruiken, of u kunt uw eigen rijen en kolommen instellen om de te vergelijken cijfers op te geven.</span><span class="sxs-lookup"><span data-stu-id="243da-107"> provides a few sample account schedules that you can use right away, or you can set up your own rows and columns to specify the figures to compare.</span></span> <span data-ttu-id="243da-108">U kunt bijvoorbeeld rapportageschema's maken om winstmarges te berekenen voor dimensies, zoals afdelingen of klantengroepen.</span><span class="sxs-lookup"><span data-stu-id="243da-108">For example, you can create account schedules to calculate profit margins on dimensions like departments or customer groups.</span></span> <span data-ttu-id="243da-109">U kunt zoveel aangepaste financiële overzichten maken als u wilt.</span><span class="sxs-lookup"><span data-stu-id="243da-109">You can create as many customized financial statements as you want.</span></span>  

<span data-ttu-id="243da-110">Het instellen van rapportageschema's vereist begrip van de financiële gegevens in het rekeningschema.</span><span class="sxs-lookup"><span data-stu-id="243da-110">Setting up account schedules requires an understanding of the financial data in the chart of accounts.</span></span> <span data-ttu-id="243da-111">U kunt bijvoorbeeld grootboekposten weergeven als percentages van budgetposten.</span><span class="sxs-lookup"><span data-stu-id="243da-111">For example, you can view general ledger entries as percentages of budget entries.</span></span> <span data-ttu-id="243da-112">Hiertoe moeten budgetten worden gemaakt.</span><span class="sxs-lookup"><span data-stu-id="243da-112">This requires that budgets are created.</span></span> <span data-ttu-id="243da-113">Zie [Procedure: Budgetten maken](finance-how-create-budgets.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="243da-113">For more information, see [How to: Create Budgets](finance-how-create-budgets.md).</span></span>

## <a name="account-categories-and-account-schedules"></a><span data-ttu-id="243da-114">Rekeningcategorieën en rekeningschema's</span><span class="sxs-lookup"><span data-stu-id="243da-114">Account Categories and Account Schedules</span></span>
<span data-ttu-id="243da-115">U kunt rekeningcategorieën gebruiken om de indeling te wijzigen van uw financiële overzichten.</span><span class="sxs-lookup"><span data-stu-id="243da-115">You can use account categories to change the layout of your financial statements.</span></span> <span data-ttu-id="243da-116">Nadat u de rekeningcategorieën hebt ingesteld in het venster **GB-rekeningcategorieën** en u kiest de actie **Rapportageschema's genereren**, worden de onderliggende rapportageschema's voor de financiële kernrapporten bijgewerkt.</span><span class="sxs-lookup"><span data-stu-id="243da-116">After you set up your account categories in the **G/L Account Categories** window, and you choose the **Generate Account Schedules** action, the underlying account schedules for the core financial reports are updated.</span></span> <span data-ttu-id="243da-117">De volgende keer dat u een van deze rapporten uitvoert, zoals het saldo-overzicht, worden nieuwe totalen en subposten toegevoegd op basis van uw wijzigingen.</span><span class="sxs-lookup"><span data-stu-id="243da-117">The next time you run one of these reports, such as the balance statement, new totals and subentries are added, based on your changes.</span></span> <span data-ttu-id="243da-118">Zie voor meer informatie [Het grootboek en het rekeningschema](finance-general-ledger.md).</span><span class="sxs-lookup"><span data-stu-id="243da-118">For more information, see [The General Ledger and the Chart of Accounts](finance-general-ledger.md).</span></span>  

## <a name="to-create-new-account-schedules"></a><span data-ttu-id="243da-119">Nieuwe rekeningstelsels maken</span><span class="sxs-lookup"><span data-stu-id="243da-119">To create new account schedules</span></span>  
 <span data-ttu-id="243da-120">U kunt rekeningstelsels gebruiken om de cijfers in grootboekrekeningen te analyseren, of om grootboekposten te vergelijken met grootboekbegrotingsposten.</span><span class="sxs-lookup"><span data-stu-id="243da-120">You use account schedules to analyze figures in general ledger accounts or to compare general ledger entries with general ledger budget entries.</span></span> <span data-ttu-id="243da-121">U kunt bijvoorbeeld de grootboekposten weergeven als percentages van de begrotingsposten.</span><span class="sxs-lookup"><span data-stu-id="243da-121">For example, you can view the general ledger entries as percentages of the budget entries.</span></span>

1. <span data-ttu-id="243da-122">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Rapportageschema's** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="243da-122">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedules**, and then choose the related link.</span></span>  
2. <span data-ttu-id="243da-123">Kies in het venster **Rapportageschema's** de actie **Nieuw** om een nieuwe naam voor een rekeningschema te maken.</span><span class="sxs-lookup"><span data-stu-id="243da-123">In the **Account Schedule Names** window, choose the **New** action to create a new account schedule name.</span></span>
3. <span data-ttu-id="243da-124">Vul indien nodig de velden in.</span><span class="sxs-lookup"><span data-stu-id="243da-124">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="243da-125">Kies de actie **Rapportageschema bewerken**.</span><span class="sxs-lookup"><span data-stu-id="243da-125">Choose the **Edit Account Schedule** action.</span></span>
5. <span data-ttu-id="243da-126">Vul de benodigde velden in het venster **Rapportageschema** in.</span><span class="sxs-lookup"><span data-stu-id="243da-126">In the **Account Schedule** window, fill in the fields as necessary.</span></span>  

    <span data-ttu-id="243da-127">Nadat u een nieuw rapportageschema hebt gemaakt en de rijen hebt ingesteld, moet u kolommen instellen.</span><span class="sxs-lookup"><span data-stu-id="243da-127">When you have created a new account schedule and set up the rows, you must set up columns.</span></span> <span data-ttu-id="243da-128">U kunt de kolommen handmatig instellen of een vooraf gedefinieerde kolomindeling toewijzen aan het rapportageschema.</span><span class="sxs-lookup"><span data-stu-id="243da-128">You can either set them up manually or assign a predefined column layout to your account schedule.</span></span>
6. <span data-ttu-id="243da-129">Kies de actie **Instellingen kolomindeling bewerken**.</span><span class="sxs-lookup"><span data-stu-id="243da-129">Choose the **Edit Column Layout Setup** action.</span></span>
7. <span data-ttu-id="243da-130">Vul indien nodig in het venster **Kolomindeling** de velden in.</span><span class="sxs-lookup"><span data-stu-id="243da-130">In the **Column Layout** window, fill in the fields as necessary.</span></span>

> [!NOTE]  
>   <span data-ttu-id="243da-131">Als u geen standaardkolomindeling hebt toegewezen aan het rapportageschema, moet u de kolommen handmatig instellen.</span><span class="sxs-lookup"><span data-stu-id="243da-131">If you did not assign a default column layout to the account schedule, you must set the columns up manually.</span></span>   

### <a name="to-create-a-column-that-calculates-percentages"></a><span data-ttu-id="243da-132">Een kolom maken die percentages berekent</span><span class="sxs-lookup"><span data-stu-id="243da-132">To create a column that calculates percentages</span></span>  
<span data-ttu-id="243da-133">U wilt mogelijk soms een kolom opnemen in een rekeningschema om percentages van een totaal te berekenen.</span><span class="sxs-lookup"><span data-stu-id="243da-133">Sometimes you may want to include a column in an account schedule to calculate percentages of a total.</span></span> <span data-ttu-id="243da-134">U hebt bijvoorbeeld een aantal rijen die zijn onderverdeeld op dimensie, en u wilt wellicht een kolom maken om het percentage aan te geven van de totale verkoop van elke rij.</span><span class="sxs-lookup"><span data-stu-id="243da-134">For example, if you have a number of rows that break down sales by dimension, you may want a column to indicate the percentage of total sales that each row represents.</span></span>

1. <span data-ttu-id="243da-135">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Rapportageschema's** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="243da-135">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedules**, and then choose the related link.</span></span>
2. <span data-ttu-id="243da-136">Selecteer een rapportageschema in het venster **Rapportageschema's**.</span><span class="sxs-lookup"><span data-stu-id="243da-136">In the **Account Schedule Names** window, select an account schedule.</span></span>  
3. <span data-ttu-id="243da-137">Kies de actie **Rapportageschema bewerken** om een rapportageschemarij te definiëren die de totalen moet berekenen waarop de percentages worden gebaseerd.</span><span class="sxs-lookup"><span data-stu-id="243da-137">Choose the **Edit Account Schedule** action to set up an account schedule row to calculate the total on which the percentages will be based.</span></span>  
4. <span data-ttu-id="243da-138">Voeg een regel in rechtstreeks boven de eerste rij waarvoor u een percentage wilt weergeven.</span><span class="sxs-lookup"><span data-stu-id="243da-138">Insert a line immediately above the first row for which you want to display a percentage.</span></span>  
5. <span data-ttu-id="243da-139">Vul de velden als volgt op de regel in: voer in het veld **Samentellingssoort** **Basis voor percentage** in.</span><span class="sxs-lookup"><span data-stu-id="243da-139">Fill in the fields on the line as follows: In the **Totaling Type** field, enter **Set Base for Percent**.</span></span> <span data-ttu-id="243da-140">Voer in het veld **Samentelling** een formule in voor het totaal waarop het percentage wordt gebaseerd.</span><span class="sxs-lookup"><span data-stu-id="243da-140">In the **Totaling** field, enter a formula for the total that the percentage will be based on.</span></span> <span data-ttu-id="243da-141">Als bijvoorbeeld rij 11 de totale omzet bevat, voert u **11** in.</span><span class="sxs-lookup"><span data-stu-id="243da-141">For example, if row 11 contains the total sales, enter **11**.</span></span>  
6. <span data-ttu-id="243da-142">Kies de actie **Instellingen kolomindeling bewerken** om een kolom in te stellen.</span><span class="sxs-lookup"><span data-stu-id="243da-142">Choose the **Edit Column Layout Setup** action to set up a column.</span></span>  
7. <span data-ttu-id="243da-143">Vul de velden als volgt op de regel in: selecteer in het veld **Kolomsoort** **Formule**.</span><span class="sxs-lookup"><span data-stu-id="243da-143">Fill in the fields on the line as follows: In the **Column Type** field, select **Formula**.</span></span> <span data-ttu-id="243da-144">Voer in het veld **Formule** een formule in voor het bedrag waarvoor u een percentage wilt berekenen, gevolgd door %.</span><span class="sxs-lookup"><span data-stu-id="243da-144">In the **Formula** field, enter a formula for the amount that you want to calculate a percentage for, followed by %.</span></span> <span data-ttu-id="243da-145">Bijvoorbeeld, als kolomnummer N de mutatie bevat, voert u **N%** in.</span><span class="sxs-lookup"><span data-stu-id="243da-145">For example, if column number N contains the net change, enter **N%**.</span></span>  
8. <span data-ttu-id="243da-146">Herhaal stap 4 tot en met 7 voor elke groep rijen die u wilt uitsplitsen op percentage.</span><span class="sxs-lookup"><span data-stu-id="243da-146">Repeat steps 4 through 7 for each group of rows that you want to break down by percentage.</span></span>

## <a name="to-set-up-account-schedules-with-overviews"></a><span data-ttu-id="243da-147">Rekeningstelsels met overzichten instellen</span><span class="sxs-lookup"><span data-stu-id="243da-147">To set up account schedules with overviews</span></span>  
<span data-ttu-id="243da-148">U kunt een rekeningstelsel gebruiken om een rekeningoverzicht te maken waarin grootboekcijfers en begrotingscijfers van grootboeken worden vergeleken.</span><span class="sxs-lookup"><span data-stu-id="243da-148">You can use an account schedule to create a statement comparing general ledger figures and general leger budget figures.</span></span>

1. <span data-ttu-id="243da-149">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Rapportageschema's** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="243da-149">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedules**, and then choose the related link.</span></span>
2. <span data-ttu-id="243da-150">Selecteer een rapportageschema in het venster **Rapportageschema's**.</span><span class="sxs-lookup"><span data-stu-id="243da-150">In the **Account Schedule Names** window, select an account schedule.</span></span>  
3. <span data-ttu-id="243da-151">Kies de actie **Rapportageschema bewerken**</span><span class="sxs-lookup"><span data-stu-id="243da-151">Choose the **Edit Account Schedule** action</span></span>  
4. <span data-ttu-id="243da-152">Selecteer in het venster **Rapportageschema** in het veld **Naam** de naam van het standaardrapportageschema.</span><span class="sxs-lookup"><span data-stu-id="243da-152">In the **Account Schedule** window, in the **Name** field, select the default account schedule name.</span></span>
5. <span data-ttu-id="243da-153">Kies de actie **Rekeningen invoegen**.</span><span class="sxs-lookup"><span data-stu-id="243da-153">Choose the **Insert Accounts** action.</span></span>  
6. <span data-ttu-id="243da-154">Selecteer de rekeningen die u wilt opnemen in uw overzicht en klik vervolgens op **OK**.</span><span class="sxs-lookup"><span data-stu-id="243da-154">Select the accounts that you want to include in your statement, and then choose the **OK** button.</span></span>

    <span data-ttu-id="243da-155">De rekeningen worden nu opgenomen in het rapportageschema.</span><span class="sxs-lookup"><span data-stu-id="243da-155">The accounts are now inserted into your account schedule.</span></span> <span data-ttu-id="243da-156">Indien gewenst kunt u ook de kolomindeling wijzigen.</span><span class="sxs-lookup"><span data-stu-id="243da-156">If you want you can also change the column layout.</span></span>  
7. <span data-ttu-id="243da-157">Kies de actie **Overzicht**.</span><span class="sxs-lookup"><span data-stu-id="243da-157">Choose the **Overview** action.</span></span>  
8. <span data-ttu-id="243da-158">Stel op het sneltabblad **Dimensiefilters** het begrotingsfilter in met de gewenste filternaam.</span><span class="sxs-lookup"><span data-stu-id="243da-158">On the **Dimension Filters** FastTab, set the budget filter to the desired filter name.</span></span>  
9. <span data-ttu-id="243da-159">Kies de knop **Ok**.</span><span class="sxs-lookup"><span data-stu-id="243da-159">Choose the **OK** button.</span></span>  

<span data-ttu-id="243da-160">Nu kunt u het budgetoverzicht kopiëren en in een spreadsheet plakken.</span><span class="sxs-lookup"><span data-stu-id="243da-160">Now you can copy and paste your budget statement into a spreadsheet.</span></span>

## <a name="see-also"></a><span data-ttu-id="243da-161">Zie ook</span><span class="sxs-lookup"><span data-stu-id="243da-161">See Also</span></span>
[<span data-ttu-id="243da-162">Bedrijfsinformatie</span><span class="sxs-lookup"><span data-stu-id="243da-162">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="243da-163">Financiën</span><span class="sxs-lookup"><span data-stu-id="243da-163">Finance</span></span>](finance.md)  
[<span data-ttu-id="243da-164">Financiën instellen</span><span class="sxs-lookup"><span data-stu-id="243da-164">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="243da-165">Het grootboek en het rekeningschema</span><span class="sxs-lookup"><span data-stu-id="243da-165">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
<span data-ttu-id="243da-166">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="243da-166">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

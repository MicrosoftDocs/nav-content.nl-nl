---
title: 'Procedure: Onderhanden werk voor een project berekenen'
description: Met projecten kunt u het verbruik van de bedrijfsresources plannen en de diverse kosten bijhouden die samenhangen met het resourceverbruik voor een bepaald project. Projecten brengen het verbruik met zich mee van arbeidsuren, machine-uren, voorraadartikelen en andere soorten verbruik die moeten worden bijgehouden terwijl het project voortduurt.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: ea0953192454302a83a9187cd6569905723fd150
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="walkthrough-calculating-work-in-process-for-a-job"></a><span data-ttu-id="6d9ce-104">Procedure: Onderhanden werk voor een project berekenen</span><span class="sxs-lookup"><span data-stu-id="6d9ce-104">Walkthrough: Calculating Work in Process for a Job</span></span>
<span data-ttu-id="6d9ce-105">Met projecten kunt u het verbruik van de bedrijfsresources plannen en de diverse kosten bijhouden die samenhangen met het resourceverbruik voor een bepaald project.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-105">With jobs, you can schedule the usage of your company's resources and keep track of the various costs associated with the usage of resources on a specific project.</span></span> <span data-ttu-id="6d9ce-106">Projecten brengen het verbruik met zich mee van arbeidsuren, machine-uren, voorraadartikelen en andere soorten verbruik die moeten worden bijgehouden terwijl het project voortduurt.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-106">Jobs involve the consumption of employee hours, machine hours, inventory items, and other types of usage that have to be tracked as a job progresses.</span></span> <span data-ttu-id="6d9ce-107">Als een project over langere tijd loopt, moet u deze kosten mogelijk overdragen naar een OHW-rekening (Onderhanden werk) op de balans terwijl het project wordt voltooid.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-107">If a job runs over a long period, you may want to transfer these costs to a Work in Process (WIP) account on the balance sheet while the job is being completed.</span></span> <span data-ttu-id="6d9ce-108">Vervolgens kunt u de kosten en verkopen indien van toepassing verantwoorden in uw resultatenrekeningen.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-108">You can then recognize the costs and sales in your income statement accounts when it is appropriate.</span></span>  

## <a name="about-this-walkthrough"></a><span data-ttu-id="6d9ce-109">Informatie over deze procedure</span><span class="sxs-lookup"><span data-stu-id="6d9ce-109">About This Walkthrough</span></span>  
 <span data-ttu-id="6d9ce-110">In deze procedure worden de volgende taken beschreven:</span><span class="sxs-lookup"><span data-stu-id="6d9ce-110">This walkthrough illustrates the following tasks:</span></span>  

-   <span data-ttu-id="6d9ce-111">OHW berekenen.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-111">Calculating WIP.</span></span>  
-   <span data-ttu-id="6d9ce-112">Een OHW-berekeningsmethode kiezen.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-112">Selecting a WIP calculation method.</span></span>  
-   <span data-ttu-id="6d9ce-113">Een deel van een project uitsluiten van OHW.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-113">Excluding part of a job from the WIP.</span></span>  
-   <span data-ttu-id="6d9ce-114">OHW boeken naar de grootboekrekening.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-114">Posting the WIP to the general ledger.</span></span>  
-   <span data-ttu-id="6d9ce-115">Een OHW-boeking terugdraaien.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-115">Reversing a WIP posting.</span></span>  

 <span data-ttu-id="6d9ce-116">In elke stap van het proces wordt de waarde berekend en worden de projecttransacties naar het grootboek verplaatst.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-116">Each step of the process calculates the value and moves the job transactions to the general ledger.</span></span> <span data-ttu-id="6d9ce-117">De berekenings- en boekingsstappen zijn van elkaar gescheiden zodat u uw gegevens kunt controleren en wijzigingen kunt aanbrengen voordat de posten naar het grootboek worden geboekt.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-117">The calculation and posting steps are separated to help you review your data and to make modifications before posting to the general ledger.</span></span> <span data-ttu-id="6d9ce-118">Daarom moet u controleren of alle gegevens correct zijn nadat u de batchverwerking voor berekening hebt uitgevoerd en voordat u de batchverwerking voor boeking hebt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-118">Therefore, you should make sure that all information is correct after you run the calculation batch jobs and before you run the posting batch jobs.</span></span>  

## <a name="roles"></a><span data-ttu-id="6d9ce-119">Rollen</span><span class="sxs-lookup"><span data-stu-id="6d9ce-119">Roles</span></span>  
 <span data-ttu-id="6d9ce-120">In deze procedure is projectteamlid Tricia de hoofdpersoon.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-120">This walkthrough uses the project team member (Tricia) as the persona.</span></span>  

## <a name="prerequisites"></a><span data-ttu-id="6d9ce-121">Vereisten</span><span class="sxs-lookup"><span data-stu-id="6d9ce-121">Prerequisites</span></span>  
 <span data-ttu-id="6d9ce-122">Voordat u de stappen in dit overzicht kunt uitvoeren, moet [!INCLUDE[d365fin](includes/d365fin_md.md)] op uw computer zijn geïnstalleerd.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-122">Before you can perform the tasks in the walkthrough, the [!INCLUDE[d365fin](includes/d365fin_md.md)] must be installed on your computer.</span></span>  

## <a name="story"></a><span data-ttu-id="6d9ce-123">Scenario</span><span class="sxs-lookup"><span data-stu-id="6d9ce-123">Story</span></span>  
 <span data-ttu-id="6d9ce-124">In dit scenario gaat het om het bedrijf Cronus International Ltd., een design- en consultancyfirma die nieuwe infrastructuren ontwerpt (conferentiezalen en kantoren) en inricht met meubels, accessoires en opslagruimten.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-124">This walkthrough focuses on CRONUS International Ltd., a design and consultancy firm that designs and fits new infrastructures, such as conference halls and offices, with furniture, accessories, and storage units.</span></span> <span data-ttu-id="6d9ce-125">Het werk bij CRONUS is voor het grootste deel projectgericht en projectteamlid Tricia gebruikt projecten om een overzicht te krijgen van de lopende projecten waaraan CRONUS werkt en de projecten die zijn voltooid.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-125">Most of the work at CRONUS is project-oriented and Tricia, a project team member, uses jobs to have an overview of each ongoing job that CRONUS has started and also the jobs that are completed.</span></span> <span data-ttu-id="6d9ce-126">De projecten kunnen soms tamelijk lang zijn en meerdere maanden lopen.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-126">Some of the jobs can be very lengthy and can run over months.</span></span> <span data-ttu-id="6d9ce-127">Tricia gebruikt een OHW-rekening voor het vastleggen van het onderhanden werk en het bijhouden van de kosten gedurende het project.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-127">Tricia can use a WIP account to record the work in process and to track the costs throughout the job.</span></span>  

## <a name="calculating-wip"></a><span data-ttu-id="6d9ce-128">OHW berekenen</span><span class="sxs-lookup"><span data-stu-id="6d9ce-128">Calculating WIP</span></span>  
 <span data-ttu-id="6d9ce-129">CRONUS heeft een langdurig project aangenomen dat nu is uitgebreid tot over meerdere rapportageperioden.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-129">CRONUS has taken on a lengthy project that has now extended across reporting periods.</span></span> <span data-ttu-id="6d9ce-130">Tricia, een lid van het projectteam berekent het onderhanden werk (OHW) om ervoor te zorgen dat de financiële rapportage van het bedrijf accuraat is.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-130">Tricia, a project team member, calculates the work in process (WIP) to make sure that the financial statement of the company will be accurate.</span></span>  

 <span data-ttu-id="6d9ce-131">Tijdens deze procedure selecteert Tricia een bepaalde groep taken die wordt opgenomen in de OHW-berekening.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-131">During this procedure, Tricia will select a specific group of tasks that will be included in the WIP calculation.</span></span> <span data-ttu-id="6d9ce-132">In het venster **Projecttaakregels** kan ze deze regels opgeven in de kolom **OHW-totaal**.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-132">In the **Job Task Lines** window, she can specify these lines in the **WIP-Total** column.</span></span>  

 <span data-ttu-id="6d9ce-133">De volgende tabel beschrijft de volgende drie opties.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-133">The following table describes the three options.</span></span>  

|<span data-ttu-id="6d9ce-134">Veld</span><span class="sxs-lookup"><span data-stu-id="6d9ce-134">Field</span></span>|<span data-ttu-id="6d9ce-135">Description</span><span class="sxs-lookup"><span data-stu-id="6d9ce-135">Description</span></span>|  
|-------------------------------------|---------------------------------------|  
|**<blank>**|<span data-ttu-id="6d9ce-136">Leeg laten als de projecttaak deel uitmaakt van een groep taken.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-136">Leave blank if the job task is a part of a group of tasks.</span></span>|  
|<span data-ttu-id="6d9ce-137">**Totaal**</span><span class="sxs-lookup"><span data-stu-id="6d9ce-137">**Total**</span></span>|<span data-ttu-id="6d9ce-138">Definieert de reeks of groep taken die zijn opgenomen in de berekening van OHW en verantwoording.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-138">Defines the range or group of tasks that are included in the WIP and recognition calculation.</span></span> <span data-ttu-id="6d9ce-139">Binnen de groep wordt elke projecttaak waarvoor **Taaksoort project** is ingesteld op **Boeken**, opgenomen in het OHW-totaal tenzij het veld **OHW-totaal** is ingesteld op **Uitgesloten**.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-139">Within the group, any job task with **Job Task Type** set to **Posting** will be included in the WIP Total, unless its **WIP-Total** field is set to **Excluded**.</span></span>|  
|<span data-ttu-id="6d9ce-140">**Uitgesloten**</span><span class="sxs-lookup"><span data-stu-id="6d9ce-140">**Excluded**</span></span>|<span data-ttu-id="6d9ce-141">Geldt alleen voor een taak met **Taaksoortproject** **Boeken**.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-141">Applies only to a task with **Job Task Type** of **Posting**.</span></span> <span data-ttu-id="6d9ce-142">De taak wordt niet meegenomen wanneer OHW en verantwoording worden berekend.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-142">The task is not included when WIP and recognition are calculated.</span></span>|  

 <span data-ttu-id="6d9ce-143">In het volgende scenario past Tricia de methode Kostprijs toe, die door haar bedrijf standaard wordt gebruikt, om het OHW berekenen.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-143">In the following walkthrough, Tricia applies the Cost Value method, her company standard, to calculate WIP.</span></span> <span data-ttu-id="6d9ce-144">Zij geeft aan welk deel van het project wordt meegenomen in de OHW-berekening door OHW-totaalwaarden toe te wijzen aan verschillende projecttaakregels.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-144">She specifies what part of the job will be included in the WIP calculation by assigning WIP-Total values to various job task lines.</span></span>  

### <a name="to-calculate-wip"></a><span data-ttu-id="6d9ce-145">OHW berekenen</span><span class="sxs-lookup"><span data-stu-id="6d9ce-145">To calculate WIP</span></span>  

1.  <span data-ttu-id="6d9ce-146">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Projecten** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-146">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Jobs**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="6d9ce-147">Selecteer in de lijst **Projecten** het project **Deerfield** en kies de actie **Bewerken**.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-147">In the **Jobs** list, select the **Deerfield** job, and then choose the **Edit** action.</span></span> <span data-ttu-id="6d9ce-148">Hiermee opent u de projectkaart in de bewerkmodus.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-148">This will open the job card in edit mode.</span></span>  

     <span data-ttu-id="6d9ce-149">OHW kan worden berekend op basis van Kostprijs, Verkoopprijs, Kostprijs van omzet, Percentage voltooid of Contract voltooid.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-149">WIP can be calculated based on Cost Value, Sales Value, Cost of Sales, Percentage of Completion, or Completed Contract.</span></span> <span data-ttu-id="6d9ce-150">In dit voorbeeld wordt door CRONUS de methode Kostprijs toegepast.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-150">In this example, CRONUS uses the Cost Value method.</span></span>  

3.  <span data-ttu-id="6d9ce-151">Kies op het sneltabblad **Boeking** het veld **OHW-methode** en selecteer **Kostprijs**.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-151">On the **Posting** FastTab, choose the **WIP Method** field, and then select **Cost Value**.</span></span>  
4.  <span data-ttu-id="6d9ce-152">Kies de actie **Projecttaakregels** en stel de volgende waarden in het veld **OHW-totaal** in.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-152">Choose the **Job Task Lines** action and set the following values in the **WIP-Total** field.</span></span>  

     <span data-ttu-id="6d9ce-153">De volgende tabel beschrijft de waarden.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-153">The following table describes the values.</span></span>  

    |<span data-ttu-id="6d9ce-154">Projecttaaknr.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-154">Job Task No.</span></span>|<span data-ttu-id="6d9ce-155">Veld OHW-totaal</span><span class="sxs-lookup"><span data-stu-id="6d9ce-155">WIP-Total Field</span></span>|  
    |------------------|----------------------|  
    |<span data-ttu-id="6d9ce-156">1130</span><span class="sxs-lookup"><span data-stu-id="6d9ce-156">1130</span></span>|<span data-ttu-id="6d9ce-157">Exclusief</span><span class="sxs-lookup"><span data-stu-id="6d9ce-157">Excluded</span></span>|  
    |<span data-ttu-id="6d9ce-158">1190</span><span class="sxs-lookup"><span data-stu-id="6d9ce-158">1190</span></span>|<span data-ttu-id="6d9ce-159">Totaal</span><span class="sxs-lookup"><span data-stu-id="6d9ce-159">Total</span></span>|  
    |<span data-ttu-id="6d9ce-160">1210</span><span class="sxs-lookup"><span data-stu-id="6d9ce-160">1210</span></span>|<span data-ttu-id="6d9ce-161">Exclusief</span><span class="sxs-lookup"><span data-stu-id="6d9ce-161">Excluded</span></span>|  
    |<span data-ttu-id="6d9ce-162">1310</span><span class="sxs-lookup"><span data-stu-id="6d9ce-162">1310</span></span>|<span data-ttu-id="6d9ce-163">Exclusief</span><span class="sxs-lookup"><span data-stu-id="6d9ce-163">Excluded</span></span>|  

5.  <span data-ttu-id="6d9ce-164">Kies de actie **OHW** en kies vervolgens de actie **OHW berekenen**.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-164">Choose the **WIP** action, and then choose the **Calculate WIP** action.</span></span>  
6.  <span data-ttu-id="6d9ce-165">In het venster **OHW voor project berekenen** kunt u een project selecteren waarvoor u OHW wilt berekenen.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-165">In the **Job Calculate WIP** window, you can select a job that you want to calculate WIP.</span></span> <span data-ttu-id="6d9ce-166">Selecteer op het sneltabblad **Project** **Deerfield** in het veld **Nr.**.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-166">On the **Job** FastTab, select **Deerfield** in the **No.**</span></span> <span data-ttu-id="6d9ce-167">te kiezen.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-167">field.</span></span>  
7.  <span data-ttu-id="6d9ce-168">Voer in het veld **Boekingsdatum** een datum in die na de werkdatum ligt.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-168">In the **Posting Date** field, enter a date that is later than the work date.</span></span>
8.  <span data-ttu-id="6d9ce-169">Typ **1** in het veld **Documentnr.**.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-169">In the **Document No.** field, enter **1**.</span></span> <span data-ttu-id="6d9ce-170">Hiermee maakt u een document waar u later, als u het wilt traceren, naar kunt verwijzen.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-170">This creates a document that you can refer to later for traceability.</span></span>  
9. <span data-ttu-id="6d9ce-171">Kies **OK** om de batchverwerking te starten.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-171">Choose the **OK** button to run the batch job.</span></span> <span data-ttu-id="6d9ce-172">Er wordt een bericht weergegeven.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-172">A message is displayed.</span></span> <span data-ttu-id="6d9ce-173">Kies de knop **OK** om door te gaan.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-173">Choose the **OK** button to continue.</span></span> <span data-ttu-id="6d9ce-174">Sluit het venster **Projecttaakregels**.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-174">Close the **Job Task Lines** window.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="6d9ce-175">Het bericht geeft aan dat er waarschuwingen zijn in verband met de OHW-berekening.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-175">The message states that there are warnings associated with the WIP calculation.</span></span> <span data-ttu-id="6d9ce-176">U gaat de waarschuwingen bekijken in de volgende procedure.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-176">You will review the warnings in the next procedure.</span></span>  

10. <span data-ttu-id="6d9ce-177">Vouw op de kaart **Project** het sneltabblad **OHW en verantwoording** uit om de berekende waarden weer te geven.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-177">On the **Job** card, expand the **WIP and Recognition** FastTab to see the calculated values.</span></span> <span data-ttu-id="6d9ce-178">U kunt ook de **Boekingsdatum OHW** bekijken en eventuele waarden die naar het grootboek zijn geboekt.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-178">You can also see the **WIP Posting Date** and the values that have been posted to the general ledger, if any.</span></span>  

 <span data-ttu-id="6d9ce-179">Zoals u ziet, bedraagt de waarde voor **Verantw. totale kosten** 215,60 in de kolom **Te boeken**.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-179">Notice that the value for **Recog. Costs Amount** is 215.60 in the **To Post** column.</span></span> <span data-ttu-id="6d9ce-180">Dit reflecteert de totale kostprijs van twee van de artikelen in groep projecttaken 1110 – 1130.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-180">This reflects the total costs of two of the items in the group of job tasks 1110 – 1130.</span></span> <span data-ttu-id="6d9ce-181">Het derde artikel was ingesteld op **Uitgesloten** en dus is niet opgenomen in de OHW-berekening.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-181">The third item was set to **Excluded**, and therefore is not included in the WIP calculation.</span></span>  

### <a name="to-review-wip-warnings"></a><span data-ttu-id="6d9ce-182">OHW-waarschuwingen bekijken</span><span class="sxs-lookup"><span data-stu-id="6d9ce-182">To review WIP warnings</span></span>  

1.  <span data-ttu-id="6d9ce-183">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Cockpit OHW taak** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-183">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Job WIP Cockpit**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="6d9ce-184">Selecteer het project **Deerfield** en kies vervolgens de actie **Waarschuwingen weergeven**.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-184">Select the **Deerfield** job, and then choose the **Show Warnings** action.</span></span>  
3.  <span data-ttu-id="6d9ce-185">Controleer in het venster **OHW-waarschuwingen project** de waarschuwing waaraan de taak is gekoppeld.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-185">In the **Job WIP Warnings** window, review the warning associated with the job.</span></span>  

 <span data-ttu-id="6d9ce-186">Na deze boekingsperiode moet Tricia het OHW opnieuw berekenen om het tot dan toe voltooide werk op te nemen.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-186">After the accounting period ends, Tricia has to recalculate the WIP to include completed work to this point.</span></span>  

### <a name="to-recalculate-wip"></a><span data-ttu-id="6d9ce-187">OHW opnieuw berekenen</span><span class="sxs-lookup"><span data-stu-id="6d9ce-187">To recalculate WIP</span></span>  

1.  <span data-ttu-id="6d9ce-188">Op de kaart **Project** kiest u de actie **OHW-posten** om de OHW-berekening weer te geven.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-188">On the **Job** card, choose the **WIP Entries** action to view the WIP calculation.</span></span>  

     <span data-ttu-id="6d9ce-189">In het venster **OHW-posten project** ziet u de OHW-posten die de laatste keer zijn berekend voor een project ook als het OHW nog niet in het grootboek is geboekt.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-189">The **Job WIP Entries** window shows the WIP entries that were last calculated on a job, even if WIP has not yet been posted to the general ledger.</span></span>  

2.  <span data-ttu-id="6d9ce-190">U kunt de stappen volgen in de procedure waarin wordt uitgelegd hoe u OHW kunt herberekenen.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-190">You can follow the steps in the procedure that explains how to calculate WIP to recalculate WIP.</span></span> <span data-ttu-id="6d9ce-191">Elke keer als het OHW wordt berekend, wordt een post gemaakt in het venster **OHW-posten project**.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-191">Every time WIP is calculated, an entry is created in the **Job WIP Entries** window.</span></span>  
3.  <span data-ttu-id="6d9ce-192">Sluit het venster.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-192">Close the window.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="6d9ce-193">Onderhanden werk en Verantwoording worden alleen berekend.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-193">Work in Process and Recognition is only calculated.</span></span> <span data-ttu-id="6d9ce-194">Het wordt niet geboekt in het grootboek.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-194">It is not posted to the general ledger.</span></span> <span data-ttu-id="6d9ce-195">Als u dat wel wilt doen, moet u de batchverwerking **OHW naar GB boeken** uitvoeren nadat u OHW en verantwoording hebt berekend.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-195">To do so, you must run **Post WIP to G/L** batch job after you have calculated the WIP and Recognition.</span></span>

## <a name="posting-wip-to-general-ledger"></a><span data-ttu-id="6d9ce-196">OHW boeken naar het grootboek</span><span class="sxs-lookup"><span data-stu-id="6d9ce-196">Posting WIP to General Ledger</span></span>  
 <span data-ttu-id="6d9ce-197">Nadat Tricia het OHW voor dit project heeft berekend, kan ze het naar het grootboek boeken.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-197">Now that Tricia has calculated WIP for this job, she can post it to the general ledger.</span></span>  

### <a name="to-post-wip-to-general-ledger"></a><span data-ttu-id="6d9ce-198">OHW naar het grootboek boeken</span><span class="sxs-lookup"><span data-stu-id="6d9ce-198">To post WIP to general ledger</span></span>  

1.  <span data-ttu-id="6d9ce-199">Selecteer het project **Deerfield** in de lijst **Projecten**.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-199">From the **Jobs** list, select the **Deerfield** job.</span></span>  
2.  <span data-ttu-id="6d9ce-200">Kies de actie **OHW** en kies vervolgens de actie **OHW naar GB boeken**.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-200">Choose the **WIP** action, and then choose the **Post WIP to G/L** action.</span></span>  
3.  <span data-ttu-id="6d9ce-201">Selecteer in het venster **Project-OHW naar GB boeken** de waarde **Deerfield** in het veld **Nr.** op het sneltabblad **Project**.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-201">In the **Job Post WIP to G/L** window, on the **Job** FastTab, select **Deerfield** in the **No.**</span></span> <span data-ttu-id="6d9ce-202">veld.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-202">field.</span></span>  
4.  <span data-ttu-id="6d9ce-203">Geef in het sneltabblad **Opties** in het veld **Tegenboekingsdocumentnr.** **1** op.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-203">On the **Options** FastTab, in the **Reversal Document No.** field, enter **1**.</span></span>  
5.  <span data-ttu-id="6d9ce-204">Kies de knop **OK** om OHW naar het grootboek te boeken.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-204">Choose the **OK** button to post WIP to the general ledger.</span></span>  
6.  <span data-ttu-id="6d9ce-205">Klik op **OK** om het bevestigingsvenster af te sluiten.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-205">Choose the **OK** button to close the confirmation window.</span></span>  

     <span data-ttu-id="6d9ce-206">Nadat u de boeking hebt voltooid, kunt u de boekingsinformatie bekijken in het venster **GB-posten OHW**.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-206">After you have completed the posting, you can view the posting information in the **WIP G/L Entries** window.</span></span>  

7.  <span data-ttu-id="6d9ce-207">Selecteer in de lijst **Projecten** het project **Deerfield** en kies de actie **GB-posten OHW**.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-207">In the **Jobs** list, select the **Deerfield** job, and then choose the **WIP G/L Entries** action.</span></span>  

     <span data-ttu-id="6d9ce-208">In het venster **GB-posten OHW project** ziet u dat het OHW naar het grootboek is geboekt.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-208">In the **Job WIP G/L Entries** window, verify that the WIP has been posted to the general ledger.</span></span>  

8.  <span data-ttu-id="6d9ce-209">Sluit het venster.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-209">Close the window.</span></span>  
9. <span data-ttu-id="6d9ce-210">Open de kaart **Project** voor het project **Deerfield**.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-210">Open the **Job** card for the **Deerfield** job.</span></span>  
10. <span data-ttu-id="6d9ce-211">Zoals u ziet is nu op het sneltabblad **OHW en verantwoording** in de kolom **Geboekt** het veld **Verantw. totale kosten GB** ingevuld, waarmee wordt aangegeven met het OHW met succes naar het grootboek is geboekt.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-211">On the **WIP and Recognition** FastTab, notice that in the **Posted** column, the **Recog. Costs G/L Amount** field is now filled in, which indicates that WIP was posted to the general ledger successfully.</span></span>  
11. <span data-ttu-id="6d9ce-212">Kies de knop **OK** om de kaart te sluiten.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-212">Choose the **OK** button to close the card.</span></span>  

## <a name="reversing-a-wip-posting"></a><span data-ttu-id="6d9ce-213">Een OHW-boeking tegenboeken</span><span class="sxs-lookup"><span data-stu-id="6d9ce-213">Reversing a WIP Posting</span></span>  
 <span data-ttu-id="6d9ce-214">Tricia bepaalt dat de projecttaken die zijn uitgesloten van de berekening van OHW hadden moeten worden berekend in OHW.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-214">Tricia determines that the job tasks that were excluded from the calculation of WIP should have been calculated in WIP.</span></span> <span data-ttu-id="6d9ce-215">Gelukkig kan ze de onjuiste boeking terugdraaien zonder dat ze nieuwe OHW-boekingen hoeft te boeken.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-215">She can reverse the incorrect postings without having to post new WIP postings.</span></span>  

### <a name="to-reverse-a-wip-posting"></a><span data-ttu-id="6d9ce-216">Een OHW-boeking tegenboeken</span><span class="sxs-lookup"><span data-stu-id="6d9ce-216">To reverse a WIP posting</span></span>  

1.  <span data-ttu-id="6d9ce-217">Selecteer het project **Deerfield** in de lijst **Projecten**.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-217">From the **Jobs** list, select the **Deerfield** job.</span></span>  
2.  <span data-ttu-id="6d9ce-218">Kies de actie **OHW** en kies vervolgens de actie **OHW naar GB boeken**.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-218">Choose the **WIP** action, and then choose the **Post WIP to G/L** action.</span></span>  
3.  <span data-ttu-id="6d9ce-219">Selecteer in het venster **Project-OHW naar GB boeken** de waarde **Deerfield** in het veld **Nr.** op het sneltabblad **Project**.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-219">In the **Job Post to WIP to G/L** window, on the **Job** FastTab, select **Deerfield** in the **No.**</span></span> <span data-ttu-id="6d9ce-220">veld.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-220">field.</span></span>  
4.  <span data-ttu-id="6d9ce-221">Geef in het sneltabblad **Opties** in het veld **Tegenboekingsdocumentnr.** **1** op.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-221">On the **Options** FastTab, in the **Reversal Document No.** field, enter **1**.</span></span>  
5.  <span data-ttu-id="6d9ce-222">Geef de oorspronkelijke boekingsdatum op in het veld **Tegenboekingsdatum**.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-222">In the **Reversal Posting Date** field, enter the original posting date.</span></span> <span data-ttu-id="6d9ce-223">Dit moet dezelfde datum zijn als u hebt gebruikt toen u voor het eerst het OHW berekende.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-223">It should be the same date that you used to calculate WIP the first time.</span></span>  
6.  <span data-ttu-id="6d9ce-224">Schakel het selectievakje **Alleen tegenboeken** in.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-224">Select the **Reverse Only** check box.</span></span> <span data-ttu-id="6d9ce-225">Hiermee wordt het eerder geboekte OHW teruggedraaid en het nieuwe OHW naar het grootboek geboekt.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-225">This will reverse previously posted WIP, but does post new WIP to the general ledger.</span></span>  
7.  <span data-ttu-id="6d9ce-226">Kies de knop **OK** om de batchverwerking uit te voeren en kies vervolgens de knop **OK** om het bevestigingsvenster te sluiten.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-226">Choose the **OK** button to run the batch job, and choose the **OK** button to close the confirmation window.</span></span>  
8.  <span data-ttu-id="6d9ce-227">Open de kaart **Project** voor **Deerfield**.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-227">Open the **Job** card for **Deerfield**.</span></span>  
9. <span data-ttu-id="6d9ce-228">Controleer op het sneltabblad **OHW en verantwoording** of er geen geboekte OHW-posten zijn.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-228">On the **WIP and Recognition** FastTab, verify that there are no posted WIP entries.</span></span>  
10. <span data-ttu-id="6d9ce-229">Sluit dit venster.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-229">Close this window.</span></span>  
11. <span data-ttu-id="6d9ce-230">Selecteer in de lijst **Projecten** het project **Deerfield**, kies de actie **OHW** en kies vervolgens de actie **GB-posten OHW**.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-230">In the **Jobs** list, select the **Deerfield** job, choose the **WIP** action, and then choose the **WIP G/L Entries** action.</span></span> <span data-ttu-id="6d9ce-231">Bij de OHW-posten is het selectievakje **Omgekeerd** ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-231">The WIP entries have the **Reversed** check box selected.</span></span>  
12. <span data-ttu-id="6d9ce-232">Sluit dit venster.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-232">Close this window.</span></span>  
13. <span data-ttu-id="6d9ce-233">U kunt teruggaan naar de **Projecttaakregels** voor het project, de vereiste onderdelen van het project in de OHW-berekening opnemen, het OHW opnieuw berekenen en de nieuwe waarde naar het grootboek boeken.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-233">Open **Job Task Lines** for the job, include the parts of the job that should be in the WIP calculation, and then recalculate and post the new value to the general ledger.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="6d9ce-234">Stel Tricia OHW had berekend en geboekt voor een project met onjuiste datums.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-234">Suppose Tricia calculated and posted WIP for a job with incorrect dates.</span></span> <span data-ttu-id="6d9ce-235">Volgens de methode die eerder werd beschreven, kan zij de onjuiste boekingen tegenboeken, de datums corrigeren en de boekingen opnieuw naar het grootboek posten.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-235">Following the method that was discussed earlier, she can reverse the incorrect postings, correct the dates, and repost to the general ledger.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="6d9ce-236">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="6d9ce-236">Next Steps</span></span>  
 <span data-ttu-id="6d9ce-237">In dit scenario heeft u de stappen doorgenomen voor het berekenen van OHW in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="6d9ce-237">This walkthrough has taken you through the steps of calculating WIP in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="6d9ce-238">Bij grotere projecten kan het handig zijn om de kosten periodiek over te dragen naar een OHW-rekening terwijl het project wordt voltooid.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-238">In larger jobs, it may be useful to transfer the costs to a WIP account periodically while the job is being completed.</span></span> <span data-ttu-id="6d9ce-239">In dit overzicht hebt u gezien hoe u taakregels uitsluit van een berekening.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-239">This walkthrough has shown you how to exclude task lines from a calculation.</span></span> <span data-ttu-id="6d9ce-240">Ook hebt u gezien wanneer u een herberekening moet uitvoeren.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-240">It also shows you when you would have to recalculate.</span></span> <span data-ttu-id="6d9ce-241">En tot slot dit wordt in dit scenario aangegeven hoe u de OHW naar het grootboek boekt.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-241">And finally, this walkthrough demonstrates how to post the WIP to the general ledger.</span></span> <span data-ttu-id="6d9ce-242">Ook is een voorbeeld opgenomen van hoe u een OHW-post naar het grootboek kunt tegenboeken.</span><span class="sxs-lookup"><span data-stu-id="6d9ce-242">An example of how to reverse a WIP posting to the general ledger is also included.</span></span>  

## <a name="see-also"></a><span data-ttu-id="6d9ce-243">Zie ook</span><span class="sxs-lookup"><span data-stu-id="6d9ce-243">See Also</span></span>  
 [<span data-ttu-id="6d9ce-244">Procedures voor bedrijfsprocessen</span><span class="sxs-lookup"><span data-stu-id="6d9ce-244">Business Process Walkthroughs</span></span>](walkthrough-business-process-walkthroughs.md)  
 <span data-ttu-id="6d9ce-245">[Procedure: Projecten plannen](walkthrough-managing-projects-with-jobs.md) </span><span class="sxs-lookup"><span data-stu-id="6d9ce-245">[Walkthrough: Managing Projects with Jobs](walkthrough-managing-projects-with-jobs.md) </span></span>  
 <span data-ttu-id="6d9ce-246">[OHW-methoden](projects-understanding-wip.md) </span><span class="sxs-lookup"><span data-stu-id="6d9ce-246">[Understanding WIP Methods](projects-understanding-wip.md) </span></span>  
 [<span data-ttu-id="6d9ce-247">Voortgang en prestaties bewaken</span><span class="sxs-lookup"><span data-stu-id="6d9ce-247">Monitor Progress and Performance</span></span>](projects-how-monitor-progress-performance.md)  
 <span data-ttu-id="6d9ce-248">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="6d9ce-248">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

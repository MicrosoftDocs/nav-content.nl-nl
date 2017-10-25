---
title: Vakantieagenda's instellen
description: "Op een afdelingsagenda staan de werkdagen en -tijden, de diensten, vakanties en afwezigheid genoteerd die bepalend zijn voor de brutocapaciteit. gemeten in tijd, van de afdeling op basis van de gedefinieerde efficiëntie en capaciteitswaarden. Voordat er een afdelingsagenda kan worden gemaakt, moet diverse voorbereidingen worden getroffen:"
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/14/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 59131cdded4bf854aed02a7d835e8160342adb36
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-shop-calendars"></a><span data-ttu-id="eebde-104">Procedure: vakantieagenda's instellen</span><span class="sxs-lookup"><span data-stu-id="eebde-104">How to: Set Up Shop Calendars</span></span>
<span data-ttu-id="eebde-105">Een afdelings- of bewerkingsplaatsagenda bevat de werkdagen en -tijden, de diensten, vakanties en afwezigheid die bepalend zijn voor de brutocapaciteit, gemeten in tijd, van de afdeling op basis van de gedefinieerde efficiëntie- en capaciteitswaarden.</span><span class="sxs-lookup"><span data-stu-id="eebde-105">A work center or machine calendar specifies the working days and hours, shifts, holidays, and absences that determine the center’s gross available capacity, measured in time, according to its defined efficiency and capacity values.</span></span>

<span data-ttu-id="eebde-106">Voordat een bepaalde afdelings- of bewerkingsplaatsagenda kan worden berekend, moeten er eerst een of meer algemene productieagenda's worden ingesteld.</span><span class="sxs-lookup"><span data-stu-id="eebde-106">As a foundation for calculating a specific work or machine center calendar, you must first set up one or more general shop calendars.</span></span> <span data-ttu-id="eebde-107">In een productieagenda wordt een standaardwerkweek gedefinieerd in termen van begin- en eindtijden van een werkdag en de ploegen die er werkzaam zijn.</span><span class="sxs-lookup"><span data-stu-id="eebde-107">A shop calendar defines a standard work week according to start and end times of each working day and the work shift relation.</span></span> <span data-ttu-id="eebde-108">Bovendien zijn in een productieagenda de vastgestelde vakantiedagen gedurende het jaar opgenomen.</span><span class="sxs-lookup"><span data-stu-id="eebde-108">In addition, the shop calendar defines the fixed holidays during a year.</span></span>  

<span data-ttu-id="eebde-109">Hier wordt beschreven hoe u afdelingsagenda's instelt.</span><span class="sxs-lookup"><span data-stu-id="eebde-109">The following describes how to set up work center calendars.</span></span> <span data-ttu-id="eebde-110">Voor het instellen van bewerkingsplaatsagenda's zijn de stappen vergelijkbaar.</span><span class="sxs-lookup"><span data-stu-id="eebde-110">The steps are similar when setting up machine center calendars.</span></span>  

## <a name="to-create-work-shifts"></a><span data-ttu-id="eebde-111">Ploegen maken</span><span class="sxs-lookup"><span data-stu-id="eebde-111">To create work shifts</span></span>  
1.  <span data-ttu-id="eebde-112">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Ploegen** in en klik op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="eebde-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Work Shifts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="eebde-113">Geef op een lege regel in het veld **Code** een nummer op om de ploeg aan te duiden, bijvoorbeeld **1**.</span><span class="sxs-lookup"><span data-stu-id="eebde-113">On a blank line, enter a number in the **Code** field to identify the work shift, for example, **1**.</span></span>  
3.  <span data-ttu-id="eebde-114">Geef een omschrijving voor de ploeg in het veld **Omschrijving**, bijvoorbeeld **Vroege ploeg**.</span><span class="sxs-lookup"><span data-stu-id="eebde-114">Describe the work shift in the **Description** field, for example, **1st shift**.</span></span>  
4.  <span data-ttu-id="eebde-115">Vul eventueel regels voor een tweede of derde ploeg in.</span><span class="sxs-lookup"><span data-stu-id="eebde-115">Optionally, fill in lines for a second or third work shift.</span></span>  

<span data-ttu-id="eebde-116">Ook als de afdeling niet met ploegen werkt, moet er toch minstens één ploegcode worden opgegeven.</span><span class="sxs-lookup"><span data-stu-id="eebde-116">Even if your work centers do not work in different work shifts, enter at least one work shift code.</span></span>  

## <a name="to-set-up-a-shop-calendar"></a><span data-ttu-id="eebde-117">Een productieagenda instellen</span><span class="sxs-lookup"><span data-stu-id="eebde-117">To set up a shop calendar</span></span>  
1.  <span data-ttu-id="eebde-118">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Productieagenda's** in en klik op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="eebde-118">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Shop Calendars**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="eebde-119">Geef op een lege regel in het veld **Code** een nummer op ter aanduiding van de productieagenda.</span><span class="sxs-lookup"><span data-stu-id="eebde-119">On a blank line, enter a number in the **Code** field to identify the shop calendar.</span></span>  
3.  <span data-ttu-id="eebde-120">Beschrijf de productieagenda in het veld **Omschrijving**.</span><span class="sxs-lookup"><span data-stu-id="eebde-120">Describe the shop calendar in the **Description** field.</span></span>  
4.  <span data-ttu-id="eebde-121">Kies de actie **Werkdagen**.</span><span class="sxs-lookup"><span data-stu-id="eebde-121">Choose the **Working Days** action.</span></span>
5.  <span data-ttu-id="eebde-122">Geef in het venster **Productieagendawerkdagen** een volledige werkweek, met de begin- en eindtijden voor elke dag, op.</span><span class="sxs-lookup"><span data-stu-id="eebde-122">In the **Shop Calendar Working Days** window, define a complete work week, with the start and end times for each day.</span></span>  

    <span data-ttu-id="eebde-123">Selecteer in het veld **Ploeg** een van de ploegen die u eerder hebt gedefinieerd.</span><span class="sxs-lookup"><span data-stu-id="eebde-123">In the **Work Shift Code** field, select one of the shifts that you previously defined.</span></span> <span data-ttu-id="eebde-124">Voeg een regel toe voor elke werkdag en elke ploeg.</span><span class="sxs-lookup"><span data-stu-id="eebde-124">Add a line for every working day and every shift.</span></span> <span data-ttu-id="eebde-125">Voorbeeld:</span><span class="sxs-lookup"><span data-stu-id="eebde-125">For example:</span></span>  

    <span data-ttu-id="eebde-126">maandag 07:00 15:00 1</span><span class="sxs-lookup"><span data-stu-id="eebde-126">Monday  07:00 15:00 1</span></span>   
    <span data-ttu-id="eebde-127">dinsdag 07:00 15:00 1</span><span class="sxs-lookup"><span data-stu-id="eebde-127">Tuesday 07:00 15:00 1</span></span>  

    <span data-ttu-id="eebde-128">Als u een productieagenda met twee ploegen nodig hebt, gaat u op de volgende manier te werk:</span><span class="sxs-lookup"><span data-stu-id="eebde-128">If you need a shop calendar with two work shifts, you must fill it in in this manner:</span></span>  

    <span data-ttu-id="eebde-129">maandag 07:00 15:00 1</span><span class="sxs-lookup"><span data-stu-id="eebde-129">Monday 07:00 15:00 1</span></span>   
    <span data-ttu-id="eebde-130">maandag 15:00 23:00 2</span><span class="sxs-lookup"><span data-stu-id="eebde-130">Monday 15:00 23:00 2</span></span>  
    <span data-ttu-id="eebde-131">dinsdag 07:00 15:00 1</span><span class="sxs-lookup"><span data-stu-id="eebde-131">Tuesday 07:00 15:00 1</span></span>  
    <span data-ttu-id="eebde-132">dinsdag 15:00 23:00 2</span><span class="sxs-lookup"><span data-stu-id="eebde-132">Tuesday 15:00 23:00 2</span></span>  

    <span data-ttu-id="eebde-133">Weekdagen die u niet in de productieagenda definieert, zoals zaterdag en zondag, worden beschouwd als niet-werkdagen en hebben in een afdelingsagenda een beschikbare capaciteit van nul.</span><span class="sxs-lookup"><span data-stu-id="eebde-133">Any week days that you do not define in the shop calendar, such as Saturday and Sunday, are considered non-working days and will have zero available capacity in a work center calendar.</span></span>  

    <span data-ttu-id="eebde-134">Wanneer alle werkdagen van een week zijn gedefinieerd, kunt u het venster **Productieagendawerkdagen** sluiten en doorgaan met het invoeren van vakanties en vrije dagen.</span><span class="sxs-lookup"><span data-stu-id="eebde-134">When all the working days of a week are defined, you can close the **Shop Calendar Working Days** window and proceed to enter holidays.</span></span>  

6.  <span data-ttu-id="eebde-135">Selecteer in het venster **Productieagenda's** de productieagenda en kies de actie **Vakantiedagen**.</span><span class="sxs-lookup"><span data-stu-id="eebde-135">In the **Shop Calendars** window, select the shop calendar, and then choose the **Holidays** action.</span></span>
7. <span data-ttu-id="eebde-136">Definieer in het venster **Productieagendavakantiedagen** de vakantiedagen van het jaar door voor elke vakantiedag op afzonderlijke regels de begindatum en -tijd, de eindtijd en een omschrijving op te geven.</span><span class="sxs-lookup"><span data-stu-id="eebde-136">In the **Shop Calendar Holidays** window, define the holidays of the year by entering the start date and time, the end time, and description of each holiday on individual lines.</span></span> <span data-ttu-id="eebde-137">Voorbeeld:</span><span class="sxs-lookup"><span data-stu-id="eebde-137">For example:</span></span>  

    <span data-ttu-id="eebde-138">04 juli 2014 0:00:00 23:59:00 Zomervakantie</span><span class="sxs-lookup"><span data-stu-id="eebde-138">04/07/14 0:00:00 23:59:00 Summer Holiday</span></span>  
    <span data-ttu-id="eebde-139">05 juli 2014 0:00:00 23:59:00 Zomervakantie</span><span class="sxs-lookup"><span data-stu-id="eebde-139">05/07/14 0:00:00 23:59:00 Summer Holiday</span></span>  
    <span data-ttu-id="eebde-140">06 juli 2014 0:00:00 23:59:00 Zomervakantie</span><span class="sxs-lookup"><span data-stu-id="eebde-140">06/07/14 0:00:00 23:59:00 Summer Holiday</span></span>  

<span data-ttu-id="eebde-141">De gedefinieerde vakantiedagen hebben in een afdelingsagenda een beschikbare capaciteit van nul.</span><span class="sxs-lookup"><span data-stu-id="eebde-141">The defined holidays will have zero available capacity in a work center calendar.</span></span>  

<span data-ttu-id="eebde-142">Nu kan de productieagenda worden toegewezen aan een afdeling om de afdelingsagenda te berekenen waarop de volledige tijdsplanning van alle bewerkingen op die afdeling wordt gebaseerd.</span><span class="sxs-lookup"><span data-stu-id="eebde-142">The shop calendar can now be assigned to a work center to calculate the work shop calendar that will govern all operation scheduling at that work center.</span></span>  

## <a name="to-calculate-a-work-center-calendar"></a><span data-ttu-id="eebde-143">Een afdelingsagenda berekenen</span><span class="sxs-lookup"><span data-stu-id="eebde-143">To calculate a work center calendar</span></span>  

1.  <span data-ttu-id="eebde-144">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Afdelingen** in en klik op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="eebde-144">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Work Centers**, and then choose the related link.</span></span>
2. <span data-ttu-id="eebde-145">Open de afdeling die u wilt bijwerken.</span><span class="sxs-lookup"><span data-stu-id="eebde-145">Open the work center that you want to update.</span></span>  
3. <span data-ttu-id="eebde-146">Geef in het veld **Productieagendacode** op welke productieagenda moet worden gebruikt als basis voor de agenda van de afdeling.</span><span class="sxs-lookup"><span data-stu-id="eebde-146">In the **Shop Calendar Code** field, select which shop calendar to use as the foundation for a work center calendar.</span></span>  
4. <span data-ttu-id="eebde-147">Kies de actie **Agenda**.</span><span class="sxs-lookup"><span data-stu-id="eebde-147">Choose the **Calendar** action.</span></span>  
5. <span data-ttu-id="eebde-148">Kies in het venster **Afdelingsagenda** de actie **Matrix weergeven**.</span><span class="sxs-lookup"><span data-stu-id="eebde-148">In the **Work Center Calendar** window, choose the **Show Matrix** action.</span></span>  

    <span data-ttu-id="eebde-149">In het linkerdeel van het matrixvenster worden alle afdelingen weergegeven die zijn ingesteld.</span><span class="sxs-lookup"><span data-stu-id="eebde-149">The left side of the matrix window lists the work centers that are set up.</span></span> <span data-ttu-id="eebde-150">In het rechterdeel ziet u een agenda met daarop de beschikbare capaciteitswaarden voor elke werkdag in de gedefinieerde eenheid, bijvoorbeeld **480** minuten.</span><span class="sxs-lookup"><span data-stu-id="eebde-150">The right side shows a calendar displaying the available capacity values for each working day in the defined unit of measure, for example, **480** minutes.</span></span> <span data-ttu-id="eebde-151">Elke regel geeft de agenda van één afdeling weer.</span><span class="sxs-lookup"><span data-stu-id="eebde-151">Each line represents the calendar of one work center.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="eebde-152">U kunt de capaciteitswaarden voor elke week of maand ook bekijken door te schakelen tussen opties in het veld **Weergeven per** in het venster **Afdelingsagenda**.</span><span class="sxs-lookup"><span data-stu-id="eebde-152">You can also select to view the capacity values for each week or month by changing the selection in the **View By** field in the **Work Center Calendar** window.</span></span>  

    <span data-ttu-id="eebde-153">Als u de nieuwe productieagenda wilt weergeven als een lijn op de geselecteerde afdeling, moet deze productieagenda eerst worden berekend.</span><span class="sxs-lookup"><span data-stu-id="eebde-153">To reflect the new shop calendar as a line on the selected work center, it must first be calculated.</span></span>  

6.  <span data-ttu-id="eebde-154">Kies de actie **Berekenen**.</span><span class="sxs-lookup"><span data-stu-id="eebde-154">Choose the **Calculate** action.</span></span>  
7.  <span data-ttu-id="eebde-155">Op het sneltabblad **Afdeling** kunt u een filter instellen, zodat er maar voor één afdeling een berekening wordt gemaakt.</span><span class="sxs-lookup"><span data-stu-id="eebde-155">On the **Work Center** FastTab, you can set a filter to only calculate for one work center.</span></span> <span data-ttu-id="eebde-156">Stelt u geen filter in, dan worden alle bestaande afdelingsagenda's berekend.</span><span class="sxs-lookup"><span data-stu-id="eebde-156">If you do not set a filter, all existing work center calendars will be calculated.</span></span>  
8.  <span data-ttu-id="eebde-157">Definieer de begin- en einddatum van de agendaperiode die moet worden berekend, bijvoorbeeld één jaar, van 1 jan. 2004 tot 31 dec. 2004.</span><span class="sxs-lookup"><span data-stu-id="eebde-157">Define the starting and ending dates of the calendar period that should be calculated, for example, one year from 01/01/14 to 31/12/14.</span></span>
9. <span data-ttu-id="eebde-158">Kies de knop **OK** om de capaciteit te berekenen.</span><span class="sxs-lookup"><span data-stu-id="eebde-158">Choose the **OK** button to calculate capacity.</span></span>  

<span data-ttu-id="eebde-159">Er zijn nu agendaposten gemaakt (of bijgewerkt) waarin de beschikbare capaciteit per dag (of per andere periode) wordt weergegeven op basis van de volgende drie sets stamgegevens:</span><span class="sxs-lookup"><span data-stu-id="eebde-159">Calendar entries are now created or updated displaying the available capacity for each period according to the following three sets of master data:</span></span>  

- <span data-ttu-id="eebde-160">de in de productieagenda gedefinieerde werkdagen en ploeg</span><span class="sxs-lookup"><span data-stu-id="eebde-160">The working days and shift defined in the assigned shop calendar.</span></span>  
- <span data-ttu-id="eebde-161">de waarde in het veld **Capaciteit** op de afdelingskaart</span><span class="sxs-lookup"><span data-stu-id="eebde-161">The value in the **Capacity** field on the work center card.</span></span>  
- <span data-ttu-id="eebde-162">de waarde in het veld **Efficiëntie** op de afdelingskaart.</span><span class="sxs-lookup"><span data-stu-id="eebde-162">The value in the **Efficiency** field on the work center card.</span></span>  

<span data-ttu-id="eebde-163">De berekende afdelingsagenda bepaalt nu wanneer en hoe veel capaciteit beschikbaar is op deze afdeling.</span><span class="sxs-lookup"><span data-stu-id="eebde-163">The calculated work center calendar will now define when and how much capacity is available at this work center.</span></span> <span data-ttu-id="eebde-164">Hiermee bepaalt u de gedetailleerde planning van bewerkingen die worden uitgevoerd op de afdeling.</span><span class="sxs-lookup"><span data-stu-id="eebde-164">This controls the detailed scheduling of operations performed at the work center.</span></span>  

## <a name="to-record-work-center-absence"></a><span data-ttu-id="eebde-165">Afwezigheid op de afdeling registreren</span><span class="sxs-lookup"><span data-stu-id="eebde-165">To record work center absence</span></span>  
1.  <span data-ttu-id="eebde-166">Kies in het venster **Afdelingsagenda** de actie **Matrix weergeven**.</span><span class="sxs-lookup"><span data-stu-id="eebde-166">In the **Work Center Calendar** window, choose the **Show Matrix** action.</span></span>
2. <span data-ttu-id="eebde-167">Selecteer in het venster **Afdelingsagendamatrix** de afdeling en de agendadag waarop de afwezigheid moet worden geregistreerd en kies vervolgens de actie **Afwezigheid**.</span><span class="sxs-lookup"><span data-stu-id="eebde-167">In the **Work Center Calendar Matrix** window, select the work center and calendar day when the absence time should be recorded, and then choose the **Absence** action.</span></span>  
3.  <span data-ttu-id="eebde-168">Definieer in het venster **Afwezigheid** de begintijd, de eindtijd en de omschrijving van de afwezigheid van die dag, bijvoorbeeld:</span><span class="sxs-lookup"><span data-stu-id="eebde-168">In the **Absence** window, define the starting time, ending time, and description of that day’s absence.</span></span> <span data-ttu-id="eebde-169">Voorbeeld:</span><span class="sxs-lookup"><span data-stu-id="eebde-169">For example:</span></span>  

    <span data-ttu-id="eebde-170">25 jan. 2001 08:00 10:00 Onderhoud</span><span class="sxs-lookup"><span data-stu-id="eebde-170">25/01/01 08:00 10:00 Maintenance</span></span>  

4.  <span data-ttu-id="eebde-171">Kies de actie **Bijwerken** en sluit vervolgens het venster **Afwezigheid**.</span><span class="sxs-lookup"><span data-stu-id="eebde-171">Choose the **Update** action, and then close the **Absence** window.</span></span>  

<span data-ttu-id="eebde-172">De geregistreerde afwezigheid is nu in mindering gebracht op de capaciteit van de geselecteerde dag.</span><span class="sxs-lookup"><span data-stu-id="eebde-172">The capacity of the selected day has now decreased by the recorded absence time.</span></span>  

## <a name="see-also"></a><span data-ttu-id="eebde-173">Zie ook</span><span class="sxs-lookup"><span data-stu-id="eebde-173">See Also</span></span>  
[<span data-ttu-id="eebde-174">Procedure: basisagenda's instellen</span><span class="sxs-lookup"><span data-stu-id="eebde-174">How to: Set Up Base Calendars</span></span>](across-how-to-assign-base-calendars.md)  
[<span data-ttu-id="eebde-175">Procedure: Afdelingen en bewerkingsplaatsen instellen</span><span class="sxs-lookup"><span data-stu-id="eebde-175">How to: Set Up Work Centers and Machine Centers</span></span>](production-how-to-set-up-work-and-machine-centers.md)  
[<span data-ttu-id="eebde-176">Productie instellen</span><span class="sxs-lookup"><span data-stu-id="eebde-176">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
[<span data-ttu-id="eebde-177">Productie</span><span class="sxs-lookup"><span data-stu-id="eebde-177">Manufacturing</span></span>](production-manage-manufacturing.md)  
<span data-ttu-id="eebde-178">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="eebde-178">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  


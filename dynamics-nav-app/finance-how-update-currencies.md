---
title: Valutawisselkoersen bijwerken
description: Als u meerdere valuta's in uw bedrijf wilt gebruiken, kunt u een code voor elke gebruikte valuta instellen en een externe wisselkoersservice gebruiken, bijvoorbeeld Yahoo.
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: multiple currencies, Yahoo
ms.date: 07/02/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 50603747629eee61f9bdaed900dcfc0dfc96ab3b
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-update-currency-exchange-rates"></a><span data-ttu-id="6c737-103">Procedure: Valutawisselkoersen bijwerken</span><span class="sxs-lookup"><span data-stu-id="6c737-103">How to: Update Currency Exchange Rates</span></span>
<span data-ttu-id="6c737-104">U moet een code instellen voor elke gebruikte valuta als u in andere valuta's dan uw lokale valuta inkoopt of verkoopt, in een andere valuta tegoeden of schulden hebt of grootboektransacties in verschillende valuta's vastlegt.</span><span class="sxs-lookup"><span data-stu-id="6c737-104">You must set up a code for each currency you use if you buy or sell in currencies other than your local currency, have receivables or payables in other currencies, or record G/L transactions in different currencies.</span></span>  

<span data-ttu-id="6c737-105">Aangezien bedrijven steeds vaker in andere landen/regio's opereren, is het belangrijk dat zij de financiën in meer dan één valuta kunnen controleren of rapporteren.</span><span class="sxs-lookup"><span data-stu-id="6c737-105">As companies operate in increasingly more countries/regions, it becomes more important that they be able to review or report financials in more than one currency.</span></span> <span data-ttu-id="6c737-106">In het programma wordt het gebruik van meerdere valuta;s ondersteund.</span><span class="sxs-lookup"><span data-stu-id="6c737-106">The program supports use of multiple currencies.</span></span> <span data-ttu-id="6c737-107">Binnen het programma wordt uw grootboek ingesteld met uw lokale valuta (LV) en wordt een andere valuta ingesteld als een extra valuta, waaraan een huidige wisselkoers wordt toegewezen.</span><span class="sxs-lookup"><span data-stu-id="6c737-107">Within the program, your general ledger is set up using your local currency (LCY), and another currency is set up as an additional currency, with a current exchange rate assigned.</span></span>  

 <span data-ttu-id="6c737-108">Door een tweede valuta in te stellen als een aanvullende rapportagevaluta, slaat [!INCLUDE[d365fin](includes/d365fin_md.md)] automatisch bedragen op in de LV en in deze extra rapportagevaluta bij elke boeking in het grootboek en andere boekingen, zoals btw-boekingen.</span><span class="sxs-lookup"><span data-stu-id="6c737-108">By designating a second currency as an additional reporting currency, [!INCLUDE[d365fin](includes/d365fin_md.md)] will automatically record amounts in both LCY and this additional reporting currency on each G/L entry and on other entries, such as VAT entries.</span></span> <span data-ttu-id="6c737-109">Wanneer het programma grootboekpostenbedragen berekent in een extra rapportagevaluta, wordt de informatie gebruikt van het venster **Valutawisselkoersen** om de relevante wisselkoers te vinden.</span><span class="sxs-lookup"><span data-stu-id="6c737-109">When G/L entry amounts are calculated in an additional reporting currency, the information in the **Currency Exchange Rates** window is used to find the relevant exchange rate.</span></span>  

> [!WARNING]  
>  <span data-ttu-id="6c737-110">De functie Extra rapportagevaluta mag NIET worden gebruikt als basis voor de vertaling van een financieel overzicht.</span><span class="sxs-lookup"><span data-stu-id="6c737-110">The Additional Reporting Currency functionality should NOT be used as a basis for financial statement translation.</span></span> <span data-ttu-id="6c737-111">Het is geen programma dat een vertaling kan uitvoeren van financiële overzichten van buitenlandse dochterondernemingen als onderdeel van een bedrijfsconsolidatie.</span><span class="sxs-lookup"><span data-stu-id="6c737-111">It is not a tool that can perform translation of foreign subsidiary financial statements as part of a company consolidation.</span></span> <span data-ttu-id="6c737-112">De extra rapportagevalutafunctie biedt alleen de optie om rapporten in een andere valuta voor te bereiden, alsof die valuta de lokale valuta van het bedrijf was.</span><span class="sxs-lookup"><span data-stu-id="6c737-112">The additional reporting currency functionality only provides the option of preparing reports in another currency, as if that currency was the company’s local currency.</span></span>

## <a name="adjusting-exchange-rates"></a><span data-ttu-id="6c737-113">Wisselkoersen corrigeren</span><span class="sxs-lookup"><span data-stu-id="6c737-113">Adjusting Exchange Rates</span></span>  
<span data-ttu-id="6c737-114">Aangezien valutakoersen constant wisselen, moeten de extra valuta-equivalenten in uw systeem periodiek worden gecorrigeerd.</span><span class="sxs-lookup"><span data-stu-id="6c737-114">Because exchange rates fluctuate constantly, additional currency equivalents in your system must be adjusted periodically.</span></span> <span data-ttu-id="6c737-115">Als deze correcties niet worden uitgevoerd, kunnen de bedragen die omgerekend zijn van vreemde (of extra) valuta's en geboekt zijn in het grootboek in LV misleidend zijn.</span><span class="sxs-lookup"><span data-stu-id="6c737-115">If these adjustments are not done, amounts that have been converted from foreign (or additional) currencies and posted to the general ledger in LCY may be misleading.</span></span> <span data-ttu-id="6c737-116">Bovendien moeten dagelijkse posten die geboekt zijn doordat een dagwisselkoers is ingevoerd in het programma worden bijgewerkt nadat de dagwisselkoersgegevens zijn ingevoerd.</span><span class="sxs-lookup"><span data-stu-id="6c737-116">In addition, daily entries posted before a daily exchange rate is entered into the program must be updated after the daily exchange rate information is entered.</span></span> <span data-ttu-id="6c737-117">De batchverwerking Wisselkoers herwaarderen wordt gebruikt om de wisselkoersen van de geboekte klant, leverancier en bankrekeningposten te corrigeren.</span><span class="sxs-lookup"><span data-stu-id="6c737-117">The Adjust Exchange Rates batch job is used to adjust the exchange rates of posted customer, vendor and bank account entries.</span></span> <span data-ttu-id="6c737-118">U kunt er tevens extra rapportagevalutabedragen in grootboekposten mee bijwerken.</span><span class="sxs-lookup"><span data-stu-id="6c737-118">It can also update additional reporting currency amounts on G/L entries.</span></span>  

## <a name="displaying-reports-and-amounts-in-the-additional-reporting-currency"></a><span data-ttu-id="6c737-119">Rapporten en bedragen weergeven in de extra rapportagevaluta</span><span class="sxs-lookup"><span data-stu-id="6c737-119">Displaying Reports and Amounts in the Additional Reporting Currency</span></span>  
<span data-ttu-id="6c737-120">Het gebruik van een extra rapportagevaluta kan in de volgende gevallen hulp bieden bij het rapportageproces voor een bedrijf:</span><span class="sxs-lookup"><span data-stu-id="6c737-120">Using an additional reporting currency can assist the reporting process for a company in the following cases:</span></span>  

- <span data-ttu-id="6c737-121">Bedrijven in landen/regio's die niet bij de EU horen en die grote hoeveelheden transacties aangaan met bedrijven in EU-landen/regio's.</span><span class="sxs-lookup"><span data-stu-id="6c737-121">Companies in non-EU countries/regions that have a high proportion of transactions with EU country/region companies.</span></span> <span data-ttu-id="6c737-122">In dit geval wil het bedrijf buiten de EU mogelijk tevens in euro rapporteren om de financiële rapporten beter bruikbaar te maken voor haar handelspartners in de EU.</span><span class="sxs-lookup"><span data-stu-id="6c737-122">In this case, the non-EU company may also wish to report in euro to make its financial reports more usable for its EU trade partners.</span></span>  

- <span data-ttu-id="6c737-123">Bedrijven die tevens rapporten in een internationale handelsvaluta in plaats van hun eigen lokale valuta willen weergeven.</span><span class="sxs-lookup"><span data-stu-id="6c737-123">Companies that also wish to display reports in a more internationally traded currency than their own local currency.</span></span>  

<span data-ttu-id="6c737-124">Verschillende rapporten in de module Financieel zijn gebaseerd op grootboekposten.</span><span class="sxs-lookup"><span data-stu-id="6c737-124">Several reports in the General Ledger application area are based on G/L entries.</span></span> <span data-ttu-id="6c737-125">Als u de financiële gegevens in de lijst in de extra rapportagevaluta wilt weergeven, plaatst u eenvoudigweg een vinkje in het veld **Bedragen in rapp.-valuta weergeven** in het betreffende grootboeklijstvenster.</span><span class="sxs-lookup"><span data-stu-id="6c737-125">To display the financial data in the report in the additional reporting currency, you simply select the **Show in Add.-Currency** field in the relevant G/L report window.</span></span>  

## <a name="to-set-up-a-currency-exchange-rate-service"></a><span data-ttu-id="6c737-126">Een wisselkoersservice instellen</span><span class="sxs-lookup"><span data-stu-id="6c737-126">To set up a currency exchange rate service</span></span>
<span data-ttu-id="6c737-127">U kunt een externe service gebruiken om valutawisselkoersen actueel te houden.</span><span class="sxs-lookup"><span data-stu-id="6c737-127">You can use an external service to keep your currency exchange rates up to date.</span></span> <span data-ttu-id="6c737-128">De Yahoo Currency Exchange Rates-service is vooraf geïnstalleerd en kan worden ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="6c737-128">The Yahoo Currency Exchange Rates service is preinstalled and ready to enable.</span></span>

1. <span data-ttu-id="6c737-129">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Valutawisselkoersservices** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="6c737-129">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Currency Exchange Rate Services**, and then choose the related link.</span></span>
2. <span data-ttu-id="6c737-130">Kies de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="6c737-130">Choose the **New** action.</span></span>
3. <span data-ttu-id="6c737-131">Vul in het venster **Valutawisselkoersservice** indien nodig de velden in.</span><span class="sxs-lookup"><span data-stu-id="6c737-131">In the **Currency Exchange Rate Service** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="6c737-132">Kies het selectievakje **Ingeschakeld** om de service in te schakelen.</span><span class="sxs-lookup"><span data-stu-id="6c737-132">Choose the **Enabled** check box to enable the service.</span></span>

## <a name="to-update-currency-exchange-rates-through-a-service"></a><span data-ttu-id="6c737-133">Valutawisselkoersen bijwerken met een service</span><span class="sxs-lookup"><span data-stu-id="6c737-133">To update currency exchange rates through a service</span></span>
1. <span data-ttu-id="6c737-134">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Valuta's** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="6c737-134">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Currencies**, and then choose the related link.</span></span>
2. <span data-ttu-id="6c737-135">Kies de actie **Wisselkoersen bijwerken**.</span><span class="sxs-lookup"><span data-stu-id="6c737-135">Choose the **Update Exchange Rates** action.</span></span>

<span data-ttu-id="6c737-136">De waarde in het veld **Wisselkoers** in het venster **Valuta´s** wordt bijgewerkt met de laatste wisselkoers.</span><span class="sxs-lookup"><span data-stu-id="6c737-136">The value in the **Exchange Rate** field in the **Currencies** window is updated with the latest currency exchange rate.</span></span>

## <a name="see-also"></a><span data-ttu-id="6c737-137">Zie ook</span><span class="sxs-lookup"><span data-stu-id="6c737-137">See Also</span></span>
[<span data-ttu-id="6c737-138">Afsluitingsjaren en -perioden</span><span class="sxs-lookup"><span data-stu-id="6c737-138">Closing Years and Periods</span></span>](year-close-years-periods.md)  
<span data-ttu-id="6c737-139">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="6c737-139">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

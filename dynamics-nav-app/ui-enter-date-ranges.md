---
title: Datumbereiken instellen in Dynamics NAV
description: Leer hoe u een rapport kunt verkrijgen om gegevens te tonen uit specifieke tijdperioden met behulp van datumbereiken in Dynamics NAV.
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: dates, reporting, filter
ms.date: 05/29/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 2619095e8b9e48068aa9d8790a9699b4c7ff05ec
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="entering-date-ranges-in-dynamics-nav"></a><span data-ttu-id="9eedd-103">Datumbereiken invoeren in Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="9eedd-103">Entering Date Ranges in Dynamics NAV</span></span>
<span data-ttu-id="9eedd-104">U kunt filters met een begin- en einddatum instellen om alleen de gegevens in dat datumbereik of tijdsinterval in te stellen.</span><span class="sxs-lookup"><span data-stu-id="9eedd-104">You can set filters containing a start date and an end date to display only the data contained in that date range or time interval.</span></span> <span data-ttu-id="9eedd-105">Voor het instellen van een datumbereik gelden speciale regels.</span><span class="sxs-lookup"><span data-stu-id="9eedd-105">Special rules apply to the way you set date ranges.</span></span> <span data-ttu-id="9eedd-106">Neem als voorbeeld de **Klanten top 10**:</span><span class="sxs-lookup"><span data-stu-id="9eedd-106">Let's take the **Customer Top 10** as an example:</span></span>

![Een datumbereik instellen op de aanvraagpagina voor de lijst Klanten top 10](./media/ui-enter-date-ranges/customer-top10-list.png)

<span data-ttu-id="9eedd-108">Hier kunt u de lijst tot een datumbereik beperken, zoals de afgelopen 2 weken of een totaal van 6 weken, of wat voor bereik u ook nodig hebt.</span><span class="sxs-lookup"><span data-stu-id="9eedd-108">Here you can limit the report to a date range such as the past 2 weeks, or a total of 6 weeks, or whatever range you want.</span></span> <span data-ttu-id="9eedd-109">Als u datumbereiken wilt invoeren, voert u datums in en gebruikt u **..**</span><span class="sxs-lookup"><span data-stu-id="9eedd-109">To set date ranges, you enter dates and then use either **..**</span></span> <span data-ttu-id="9eedd-110">of **|** om het bereik in te stellen.</span><span class="sxs-lookup"><span data-stu-id="9eedd-110">or **|** to set the range.</span></span> <span data-ttu-id="9eedd-111">Als u in ons voorbeeld de top 10 klanten voor de eerste twee weken van mei wilt invoeren, stelt u het datumfilter in op *05 01 17..05 14 17*.</span><span class="sxs-lookup"><span data-stu-id="9eedd-111">In our example, to show the top 10 customers for the first two weeks of May, you would set the date filter to *05 01 17..05 14 17*.</span></span>
<span data-ttu-id="9eedd-112">Hier volgen enkele andere voorbeelden:</span><span class="sxs-lookup"><span data-stu-id="9eedd-112">Here are a couple of other examples:</span></span>

| <span data-ttu-id="9eedd-113">Betekenis</span><span class="sxs-lookup"><span data-stu-id="9eedd-113">Meaning</span></span> | <span data-ttu-id="9eedd-114">Opmerking</span><span class="sxs-lookup"><span data-stu-id="9eedd-114">Example</span></span> | <span data-ttu-id="9eedd-115">Opgenomen posten</span><span class="sxs-lookup"><span data-stu-id="9eedd-115">Entries included</span></span> |
|---|---|---|
|<span data-ttu-id="9eedd-116">Gelijk aan</span><span class="sxs-lookup"><span data-stu-id="9eedd-116">Equal to</span></span>| <span data-ttu-id="9eedd-117">12 15 16</span><span class="sxs-lookup"><span data-stu-id="9eedd-117">12 15 16</span></span> |<span data-ttu-id="9eedd-118">Alleen posten die zijn geboekt op 15 december 2016.</span><span class="sxs-lookup"><span data-stu-id="9eedd-118">Only those posted on December 15 2016.</span></span>|
|<span data-ttu-id="9eedd-119">Interval</span><span class="sxs-lookup"><span data-stu-id="9eedd-119">Interval</span></span>| <span data-ttu-id="9eedd-120">12 15 16..01 15 17</span><span class="sxs-lookup"><span data-stu-id="9eedd-120">12 15 16..01 15 17</span></span><br /><br /><span data-ttu-id="9eedd-121">..12 15 16</span><span class="sxs-lookup"><span data-stu-id="9eedd-121">..12 15 16</span></span>|<span data-ttu-id="9eedd-122">Posten die zijn geboekt in de periode tussen en tot en met 15 december 2016 en 15 januari 2017.</span><span class="sxs-lookup"><span data-stu-id="9eedd-122">Those posted on dates between and including December 15 2016 and January 15 2017.</span></span><br /><br /><span data-ttu-id="9eedd-123">Posten die zijn geboekt op 15 december 2016 of eerder.</span><span class="sxs-lookup"><span data-stu-id="9eedd-123">Those posted on December 15 2016 or earlier.</span></span>|
|<span data-ttu-id="9eedd-124">Of/of</span><span class="sxs-lookup"><span data-stu-id="9eedd-124">Either/or</span></span>|<span data-ttu-id="9eedd-125">12 15 16&#124;12 16 16</span><span class="sxs-lookup"><span data-stu-id="9eedd-125">12 15 16&#124;12 16 16</span></span>|<span data-ttu-id="9eedd-126">Posten die zijn geboekt op 15 december of 16 december 2016.</span><span class="sxs-lookup"><span data-stu-id="9eedd-126">Those posted on either December 15 or December 16 2016.</span></span> <span data-ttu-id="9eedd-127">Als deze posten zijn geboekt op beide dagen, worden ze allebei weergegeven.</span><span class="sxs-lookup"><span data-stu-id="9eedd-127">If there are entries posted on both days, they will all be displayed.</span></span>|

<span data-ttu-id="9eedd-128">U kunt de verschillende notatiesoorten ook combineren.</span><span class="sxs-lookup"><span data-stu-id="9eedd-128">You can also combine the various format types.</span></span>

| <span data-ttu-id="9eedd-129">Opmerking</span><span class="sxs-lookup"><span data-stu-id="9eedd-129">Example</span></span> | <span data-ttu-id="9eedd-130">Opgenomen posten</span><span class="sxs-lookup"><span data-stu-id="9eedd-130">Entries included</span></span> |
|---|---|
|<span data-ttu-id="9eedd-131">12 15 16&#124;12 01 16..05 31 17</span><span class="sxs-lookup"><span data-stu-id="9eedd-131">12 15 16&#124;12 01 16..05 31 17</span></span> | <span data-ttu-id="9eedd-132">Posten die zijn geboekt op 15 december 2016 of op datums tussen en tot en met 1 december 2016 en 31 mei 2017.</span><span class="sxs-lookup"><span data-stu-id="9eedd-132">Entries posted either on December 15 2016 or on dates between and including December 01 2016 and May 31 2017.</span></span> |
|<span data-ttu-id="9eedd-133">..12 14 16&#124;12 30 16..</span><span class="sxs-lookup"><span data-stu-id="9eedd-133">..12 14 16&#124;12 30 16..</span></span> | <span data-ttu-id="9eedd-134">Posten die zijn geboekt op 14 december of eerder, of posten die zijn geboekt op 30 december of later. Dit wil zeggen, alle posten behalve die zijn geboekt tussen 15 december en 29 december tot en met.</span><span class="sxs-lookup"><span data-stu-id="9eedd-134">Entries posted on December 14 or earlier, or entries posted on December 30 or later - that is, all entries except those posted on dates between and including December 15 and 29.</span></span> |

<span data-ttu-id="9eedd-135">U ziet dat we hier de Amerikaanse datumnotatie MMDDYY hebben gebruikt.</span><span class="sxs-lookup"><span data-stu-id="9eedd-135">Note that we have used the US date format MMDDYY here.</span></span> <span data-ttu-id="9eedd-136">Zodra [!INCLUDE[d365fin](includes/d365fin_md.md)] beschikbaar wordt in andere markten, zult u de indelingen kunnen gebruiken die u gewend bent.</span><span class="sxs-lookup"><span data-stu-id="9eedd-136">As [!INCLUDE[d365fin](includes/d365fin_md.md)] becomes available in other markets, you'll be able to use the formats that you are used to.</span></span>

## <a name="see-also"></a><span data-ttu-id="9eedd-137">Zie ook</span><span class="sxs-lookup"><span data-stu-id="9eedd-137">See Also</span></span>
<span data-ttu-id="9eedd-138">[Werken met [!INCLUDE[d365fin](includes/d365fin_long_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9eedd-138">[Working with [!INCLUDE[d365fin](includes/d365fin_long_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="9eedd-139">Criteria in filters invoeren</span><span class="sxs-lookup"><span data-stu-id="9eedd-139">Entering Criteria in Filters </span></span>](ui-enter-criteria-filters.md)  
[<span data-ttu-id="9eedd-140">Algemene bedrijfsfunctionaliteit</span><span class="sxs-lookup"><span data-stu-id="9eedd-140">General Business Functionality</span></span>](ui-across-business-areas.md)


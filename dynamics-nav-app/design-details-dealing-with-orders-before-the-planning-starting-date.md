---
title: 'Ontwerpdetails: Werken met orders voor de geplande begindatum'
description: In dit onderwerp worden de regels beschreven die door planning op orders worden toegepast in de vaste zone.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: planning, frozen, design serial, lot
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 9b15856d89be0c0fba18381cea730a8a388986a3
ms.contentlocale: nl-nl
ms.lasthandoff: 12/01/2017

---
# <a name="design-details-dealing-with-orders-before-the-planning-starting-date"></a><span data-ttu-id="d4300-103">Ontwerpdetails: Werken met orders voor de geplande begindatum</span><span class="sxs-lookup"><span data-stu-id="d4300-103">Design Details: Dealing with Orders Before the Planning Starting Date</span></span>
<span data-ttu-id="d4300-104">Om te voorkomen dat een voorzieningenplan onmogelijke en daarom nutteloze voorstellen toont, beschouwt het planningssysteem de periode tot de begindatum van de planning als een vaste zone waarvoor niets wordt gepland.</span><span class="sxs-lookup"><span data-stu-id="d4300-104">To avoid that a supply plan shows impossible and therefore useless suggestions, the planning system regards the period up until the planning starting date a frozen zone where nothing is planned for.</span></span> <span data-ttu-id="d4300-105">De volgende regel geldt voor de vaste zone:</span><span class="sxs-lookup"><span data-stu-id="d4300-105">The following rule applies to the frozen zone:</span></span>  
  
<span data-ttu-id="d4300-106">Alle vraag en aanbod vóór de begindatum van de planningsperiode wordt beschouwd als deel van de voorraad of wordt verzonden.</span><span class="sxs-lookup"><span data-stu-id="d4300-106">All supply and demand before the starting date of the planning period will be considered a part of inventory or shipped.</span></span>  
  
<span data-ttu-id="d4300-107">Het planningssysteem zal, met enkele uitzonderingen, geen wijzigingen in voorzieningenorders in de vaste zone voorstellen en er worden voor die periode geen ordertraceringskoppelingen gemaakt of onderhouden.</span><span class="sxs-lookup"><span data-stu-id="d4300-107">Accordingly, the planning system will not, with a few exceptions, suggest any changes to supply orders in the frozen zone, and no order tracking links are created or maintained for that period.</span></span>  
  
<span data-ttu-id="d4300-108">De uitzonderingen op deze regel zijn als volgt:</span><span class="sxs-lookup"><span data-stu-id="d4300-108">The exceptions to this rule are as follows:</span></span>  
  
* <span data-ttu-id="d4300-109">Als de verwachte beschikbare voorraad, inclusief totale vraag en aanbod in de vaste zone, lager is dan nul.</span><span class="sxs-lookup"><span data-stu-id="d4300-109">If the projected available inventory, including the sum of supply and demand in the frozen zone, is below zero.</span></span>  
* <span data-ttu-id="d4300-110">Als serie-/lotnummers vereist zijn op de geantidateerde order(s).</span><span class="sxs-lookup"><span data-stu-id="d4300-110">If serial/lot numbers are required on the backdated order(s).</span></span>  
* <span data-ttu-id="d4300-111">Als de aanbod/vraag-combinatie is gekoppeld door een order-aan-order beleid.</span><span class="sxs-lookup"><span data-stu-id="d4300-111">If the supply-demand set is linked by an order-to-order policy.</span></span>  
  
<span data-ttu-id="d4300-112">Als de eerste beschikbare voorraad onder nul is, wordt er op de dag vóór de planningsperiode door het planningssysteem een noodvoorzieningenorder voorgesteld voor het ontbrekende aantal.</span><span class="sxs-lookup"><span data-stu-id="d4300-112">If the initial available inventory is below zero, the planning system suggests an emergency supply order on the day before the planning period to cover the missing quantity.</span></span> <span data-ttu-id="d4300-113">Dus is de voorspelde en beschikbare voorraad altijd minstens nul wanneer het plannen voor de toekomstige periode begint.</span><span class="sxs-lookup"><span data-stu-id="d4300-113">Consequently, the projected and available inventory will always be at least zero when planning for the future period begins.</span></span> <span data-ttu-id="d4300-114">De planningsregel voor deze voorzieningenorder geeft een waarschuwingspictogram Noodgeval weer en er worden extra gegevens getoond bij het opzoeken.</span><span class="sxs-lookup"><span data-stu-id="d4300-114">The planning line for this supply order will display an Emergency warning icon and additional information is provided upon lookup.</span></span>  
  
## <a name="seriallot-numbers-and-order-to-order-links-are-exempt-from-the-frozen-zone"></a><span data-ttu-id="d4300-115">Serie-/lotnummers en order-naar-order koppelingen zijn vrijgesteld van de vaste zone</span><span class="sxs-lookup"><span data-stu-id="d4300-115">Serial/Lot Numbers and Order-to-Order Links are Exempt from the Frozen Zone</span></span>  
<span data-ttu-id="d4300-116">Als serie-/lotnummers vereist zijn of als een order-naar-order koppeling bestaat, zal het planningssysteem de vaste zone negeren en zulke aantallen opnemen die geantidateerd zijn vanaf de begindatum, en mogelijk corrigerende acties voorstellen als vraag en aanbod niet zijn gesynchroniseerd.</span><span class="sxs-lookup"><span data-stu-id="d4300-116">If serial/lot numbers are required or an order-to-order link exists, the planning system will disregard the frozen zone and incorporate such quantities that are back-dated from the starting date and potentially suggest corrective actions if demand and supply is not synchronized.</span></span> <span data-ttu-id="d4300-117">De bedrijfsreden voor dit principe is dat dergelijke specifieke vraag-voorzieningcombinaties moeten overeenkomen om te zorgen dat aan deze specifieke vraag wordt voldaan.</span><span class="sxs-lookup"><span data-stu-id="d4300-117">The business reason for this principle is that such specific demand-supply sets must match to ensure that this specific demand is fulfilled.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="d4300-118">Zie ook</span><span class="sxs-lookup"><span data-stu-id="d4300-118">See Also</span></span>  
<span data-ttu-id="d4300-119">[Ontwerpdetails: Vraag en aanbod afstemmen](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="d4300-119">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
<span data-ttu-id="d4300-120">[Ontwerpdetails: Centrale begrippen van het planningssysteem](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="d4300-120">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
[<span data-ttu-id="d4300-121">Ontwerpdetails: Voorraadplanning</span><span class="sxs-lookup"><span data-stu-id="d4300-121">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)

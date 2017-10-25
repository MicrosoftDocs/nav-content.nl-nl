---
title: 'Ontwerpdetails: Maximaal aantal'
description: Het beleid Maximum aantal is een manier om voorraad bij te houden met behulp van een bestelpunt.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: eb2dfa933cd80400e3143c2c0b5bc44691170baf
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-maximum-qty"></a><span data-ttu-id="f8bad-103">Ontwerpdetails: Maximaal aantal</span><span class="sxs-lookup"><span data-stu-id="f8bad-103">Design Details: Maximum Qty.</span></span>
<span data-ttu-id="f8bad-104">Het beleid Maximum aantal is een manier om voorraad bij te houden met behulp van een bestelpunt.</span><span class="sxs-lookup"><span data-stu-id="f8bad-104">The Maximum Quantity policy is a way to maintain inventory using a reorder point.</span></span>  
  
 <span data-ttu-id="f8bad-105">Alles over het beleid voor een vast bestelaantal geldt ook voor dit beleid.</span><span class="sxs-lookup"><span data-stu-id="f8bad-105">Everything regarding the Fixed Reorder Qty. policy also applies to this policy.</span></span> <span data-ttu-id="f8bad-106">Het enige verschil is de hoeveelheid van de voorgestelde voorziening.</span><span class="sxs-lookup"><span data-stu-id="f8bad-106">The only difference is the quantity of the suggested supply.</span></span> <span data-ttu-id="f8bad-107">Wanneer het beleid voor maximaal aantal wordt gebruikt, wordt het bestelaantal dynamisch bepaald op basis van het geplande voorraadniveau en verschilt daarom gewoonlijk per order.</span><span class="sxs-lookup"><span data-stu-id="f8bad-107">When using the maximum quantity policy, the reorder quantity will be defined dynamically based on the projected inventory level and will therefore usually differ from order to order.</span></span>  
  
## <a name="calculated-per-time-bucket"></a><span data-ttu-id="f8bad-108">Berekend per tijdsinterval</span><span class="sxs-lookup"><span data-stu-id="f8bad-108">Calculated per Time Bucket</span></span>  
 <span data-ttu-id="f8bad-109">Het bestelaantal wordt bepaald op het moment (het einde van het tijdsinterval) dat het planningssysteem detecteert dat het bestelpunt is overschreden.</span><span class="sxs-lookup"><span data-stu-id="f8bad-109">The reorder quantity is determined at the point of time (the end of a time bucket) when the planning system detects that the reorder point has been crossed.</span></span> <span data-ttu-id="f8bad-110">Op dit moment meet het systeem het verschil tussen het huidige geplande voorraadniveau en de opgegeven maximale voorraad.</span><span class="sxs-lookup"><span data-stu-id="f8bad-110">At this time, the system measures the gap from the current projected inventory level up to the specified maximum inventory.</span></span> <span data-ttu-id="f8bad-111">Dit vormt het aantal dat opnieuw moet worden besteld.</span><span class="sxs-lookup"><span data-stu-id="f8bad-111">This constitutes the quantity that should be reordered.</span></span> <span data-ttu-id="f8bad-112">Het systeem controleert vervolgens of de voorziening al elders is besteld voor ontvangst binnen de doorlooptijd. Als dit het geval is, wordt het aantal van de nieuwe voorzieningenorder verminderd met de reeds bestelde aantallen.</span><span class="sxs-lookup"><span data-stu-id="f8bad-112">The system then checks if supply has already been ordered elsewhere to be received within the lead time and, if so, reduces the quantity of the new supply order by already ordered quantities.</span></span>  
  
 <span data-ttu-id="f8bad-113">Het systeem zorgt dat de geplande voorraad ten minste het bestelpuntniveau bereikt, voor het geval dat de gebruiker is vergeten een maximaal voorraadaantal op te geven.</span><span class="sxs-lookup"><span data-stu-id="f8bad-113">The system will ensure that the projected inventory at least reaches the reorder point level – in case the user has forgotten to specify a maximum inventory quantity.</span></span>  
  
## <a name="combines-with-order-modifiers"></a><span data-ttu-id="f8bad-114">Combineert met orderaanpassingsfuncties</span><span class="sxs-lookup"><span data-stu-id="f8bad-114">Combines with Order Modifiers</span></span>  
 <span data-ttu-id="f8bad-115">Afhankelijk van de instellingen kan het het beste zijn om het maximale aantal-beleid te combineren met orderwijzigingen om een minimaal orderaantal te garanderen of af te ronden op een geheel aantal inkoopeenheden, of te splitsen in meerdere lots zoals bepaald door het maximale orderaantal.</span><span class="sxs-lookup"><span data-stu-id="f8bad-115">Depending on the setup, it may be best to combine the Maximum Quantity policy with order modifiers to ensure a minimum order quantity or round it to an integer number of purchase units of measure, or split it into more lots as defined by the maximum order quantity.</span></span>  
  
## <a name="combines-with-calendars"></a><span data-ttu-id="f8bad-116">Combineert met agenda's</span><span class="sxs-lookup"><span data-stu-id="f8bad-116">Combines with Calendars</span></span>  
 <span data-ttu-id="f8bad-117">Voordat het planningssysteem een nieuwe voorzieningenorder voorstelt, wordt gecontroleerd of de order is gepland voor een niet-werkdag, volgens agenda's die zijn gedefinieerd in het veld **Basisagendacode** in de vensters **Bedrijfsgegevens** en **Vestiging**.</span><span class="sxs-lookup"><span data-stu-id="f8bad-117">Before suggesting a new supply order to meet a reorder point, the planning system checks if the order is scheduled for a non-working day, according to any calendars that are  defined in the **Base Calendar Code** field in the **Company Information** and **Location Card** windows.</span></span>  
  
 <span data-ttu-id="f8bad-118">Als de verwachte datum een vrije dag is, verplaatst het planningssysteem de order voorwaarts naar de dichtstbijzijnde werkdatum.</span><span class="sxs-lookup"><span data-stu-id="f8bad-118">If the scheduled date is a non-working day, the planning system moves the order forward to the nearest working date.</span></span> <span data-ttu-id="f8bad-119">Dit kan resulteren in een order die voldoet een bestelpunt maar aan een bepaalde vraag niet voldoet.</span><span class="sxs-lookup"><span data-stu-id="f8bad-119">This may result in an order that meets a reorder point but does not meet some specific demand.</span></span> <span data-ttu-id="f8bad-120">Voor dergelijke vraag in onbalans maakt het systeem een extra voorziening.</span><span class="sxs-lookup"><span data-stu-id="f8bad-120">For such unbalanced demand, the planning system creates an extra supply.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="f8bad-121">Zie ook</span><span class="sxs-lookup"><span data-stu-id="f8bad-121">See Also</span></span>  
 <span data-ttu-id="f8bad-122">[Ontwerpdetails: Bestelbeleid](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="f8bad-122">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
 <span data-ttu-id="f8bad-123">[Ontwerpdetails: Planningsparameters](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="f8bad-123">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
 <span data-ttu-id="f8bad-124">[Ontwerpdetails: Bestelbeleid verwerken](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="f8bad-124">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
 [<span data-ttu-id="f8bad-125">Ontwerpdetails: Voorraadplanning</span><span class="sxs-lookup"><span data-stu-id="f8bad-125">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)

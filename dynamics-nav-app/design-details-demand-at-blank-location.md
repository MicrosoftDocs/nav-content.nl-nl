---
title: 'Ontwerpdetails: Vraag en aanbod'
description: In dit onderwerp worden de concepten van vraag beschreven, de verzamelterm voor elk soort brutovraag, zoals een verkooporder en materiaalbehoefte van een productieorder.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, demand, supply, inventory, planning
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: d744b55835f5553e249a536e0fca0eb0046fda7b
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-demand-and-supply"></a><span data-ttu-id="9f63d-103">Ontwerpdetails: Vraag en aanbod</span><span class="sxs-lookup"><span data-stu-id="9f63d-103">Design Details: Demand and Supply</span></span>
<span data-ttu-id="9f63d-104">Vraag is de verzamelterm voor elk soort brutovraag, zoals een verkooporder en materiaalbehoefte van een productieorder.</span><span class="sxs-lookup"><span data-stu-id="9f63d-104">Demand is the common term used for any kind of gross demand, such as a sales order and component need from a production order.</span></span> <span data-ttu-id="9f63d-105">Bovendien staat het programma meer technische soorten vraag toe, zoals negatieve voorraad en inkoopretouren</span><span class="sxs-lookup"><span data-stu-id="9f63d-105">In addition, the program allows more technical types of demand, such as negative inventory and purchase returns.</span></span>  
  
<span data-ttu-id="9f63d-106">Voorziening is de algemene term voor elke soort positief of inkomend aantal, zoals voorraad, inkopen, assemblage, productie of inkomende transfers.</span><span class="sxs-lookup"><span data-stu-id="9f63d-106">Supply is the common term used for any kind of positive or inbound quantity, such as inventory, purchases, assembly, production, or inbound transfers.</span></span> <span data-ttu-id="9f63d-107">Een verkoopretour kan bovendien ook voorziening vertegenwoordigen.</span><span class="sxs-lookup"><span data-stu-id="9f63d-107">In addition, a sales return may also represent supply.</span></span>  
  
<span data-ttu-id="9f63d-108">Om de vele bronnen van vraag en voorzieningen te sorteren, ordent het planningssysteem deze op twee tijdpaden die voorraadprofielen worden genoemd.</span><span class="sxs-lookup"><span data-stu-id="9f63d-108">To sort out the many sources of demand and supply, the planning system organizes them on two time lines called inventory profiles.</span></span> <span data-ttu-id="9f63d-109">Eén profiel bevat vraaggebeurtenissen en het andere bevat de corresponderende voorzieninggebeurtenissen.</span><span class="sxs-lookup"><span data-stu-id="9f63d-109">One profile holds demand events, and the other holds the corresponding supply events.</span></span> <span data-ttu-id="9f63d-110">Elke gebeurtenis vertegenwoordigt een entiteit uit het ordernetwerk, bijvoorbeeld een verkooporderregel, een artikelpost of een productieorderregel.</span><span class="sxs-lookup"><span data-stu-id="9f63d-110">Each event represents one order network entity, such as a sales order line, an item ledger entry, or a production order line.</span></span>  
  
<span data-ttu-id="9f63d-111">Wanneer voorraadprofielen worden geladen, worden de verschillende vraag-voorzieningcombinaties vereffend om een voorzieningenplan uit te voeren dat aan de genoemde doelstellingen voldoet.</span><span class="sxs-lookup"><span data-stu-id="9f63d-111">When inventory profiles are loaded, the different demand-supply sets are balanced to output a supply plan that fulfills the listed goals.</span></span>  
  
<span data-ttu-id="9f63d-112">Planningsparameters en voorraadniveaus zijn respectievelijk andere soorten vraag en aanbod, die geïntegreerde afstemming ondergaan om voorraadartikelen aan te vullen.</span><span class="sxs-lookup"><span data-stu-id="9f63d-112">Planning parameters and inventory levels are other types of demand and supply respectively, which undergo integrated balancing to replenish stock items.</span></span> <span data-ttu-id="9f63d-113">Zie voor meer informatie [Ontwerpdetails: Bestelbeleid verwerken](design-details-handling-reordering-policies.md).</span><span class="sxs-lookup"><span data-stu-id="9f63d-113">For more information, see [Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md).</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="9f63d-114">Zie ook</span><span class="sxs-lookup"><span data-stu-id="9f63d-114">See Also</span></span>  
<span data-ttu-id="9f63d-115">[Ontwerpdetails: Vraag en aanbod afstemmen](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="9f63d-115">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
<span data-ttu-id="9f63d-116">[Ontwerpdetails: Centrale begrippen van het planningssysteem](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="9f63d-116">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
[<span data-ttu-id="9f63d-117">Ontwerpdetails: Voorraadplanning</span><span class="sxs-lookup"><span data-stu-id="9f63d-117">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)

---
title: 'Ontwerpdetails: Voorzieningsplanning'
description: Dit onderwerp biedt een overzicht van de concepten en principes die worden gebruikt binnen de functies voor voorraadplanning in [!INCLUDE[d365fin](includes/d365fin_md.md)].
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, supply, planning, reordering, replenishment
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: a362452c7ee7a115751ce665e5ea6c3c96b1f27c
ms.contentlocale: nl-nl
ms.lasthandoff: 12/01/2017

---
# <a name="design-details-supply-planning"></a><span data-ttu-id="a3170-103">Ontwerpdetails: Voorzieningsplanning</span><span class="sxs-lookup"><span data-stu-id="a3170-103">Design Details: Supply Planning</span></span>
<span data-ttu-id="a3170-104">Deze documentatie biedt gedetailleerde technische inzichten in de concepten en principes die worden gebruikt binnen de functies voor voorraadplanning in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="a3170-104">This documentation provides detailed technical insight to the concepts and principles that are used within the Supply Planning features in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

<span data-ttu-id="a3170-105">Er wordt uitgelegd hoe het planningssysteem werkt en hoe de algoritmen kunnen worden aangepast om te voldoen aan planningsvereisten in verschillende omgevingen.</span><span class="sxs-lookup"><span data-stu-id="a3170-105">It explains how the planning system works and how to adjust the algorithms to meet planning requirements in different environments.</span></span> <span data-ttu-id="a3170-106">Eerst worden de centrale oplossingsconcepten geïntroduceerd en vervolgens wordt de logica beschreven van het centrale mechanisme, de afstemming van voorzieningen, waarna wordt uitgelegd hoe voorraadplanning wordt uitgevoerd met gebruikmaking van bestelbeleid.</span><span class="sxs-lookup"><span data-stu-id="a3170-106">It first introduces central solution concepts and then describes the logic of the central mechanism, supply balancing, before proceeding to explain how inventory planning is performed with the use of reordering policies.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="a3170-107">In dit gedeelte</span><span class="sxs-lookup"><span data-stu-id="a3170-107">In This Section</span></span>  
[<span data-ttu-id="a3170-108">Ontwerpdetails: Centrale begrippen van het planningssysteem</span><span class="sxs-lookup"><span data-stu-id="a3170-108">Design Details: Central Concepts of the Planning System</span></span>](design-details-central-concepts-of-the-planning-system.md)  
[<span data-ttu-id="a3170-109">Ontwerpdetails: Reservering, ordertracering en planningsboodschappen</span><span class="sxs-lookup"><span data-stu-id="a3170-109">Design Details: Reservation, Order Tracking, and Action Messaging</span></span>](design-details-reservation-order-tracking-and-action-messaging.md)  
[<span data-ttu-id="a3170-110">Ontwerpdetails: Vraag en aanbod afstemmen</span><span class="sxs-lookup"><span data-stu-id="a3170-110">Design Details: Balancing Demand and Supply</span></span>](design-details-balancing-demand-and-supply.md)  
[<span data-ttu-id="a3170-111">Ontwerpdetails: Bestelbeleid verwerken</span><span class="sxs-lookup"><span data-stu-id="a3170-111">Design Details: Handling Reordering Policies</span></span>](design-details-handling-reordering-policies.md)  
[<span data-ttu-id="a3170-112">Ontwerpdetails: Planningsparameters</span><span class="sxs-lookup"><span data-stu-id="a3170-112">Design Details: Planning Parameters</span></span>](design-details-planning-parameters.md)  
[<span data-ttu-id="a3170-113">Ontwerpdetails: Tabel Planningstoewijzing</span><span class="sxs-lookup"><span data-stu-id="a3170-113">Design Details: Planning Assignment Table</span></span>](design-details-planning-assignment-table.md)  
[<span data-ttu-id="a3170-114">Ontwerpdetails: Vraag op lege vestiging</span><span class="sxs-lookup"><span data-stu-id="a3170-114">Design Details: Demand at Blank Location</span></span>](design-details-demand-at-blank-location.md)  
[<span data-ttu-id="a3170-115">Ontwerpdetails: Transfers in planning</span><span class="sxs-lookup"><span data-stu-id="a3170-115">Design Details: Transfers in Planning</span></span>](design-details-transfers-in-planning.md)


---
title: Voorraadkosten beheren
description: Kostenbeheer heeft betrekking op het vastleggen en rapporteren van operationele bedrijfskosten. Dit omvat de rapportage van productie- en voorraadkosten (dus de waarde van artikelen).
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 8fb7ea86ff0a14ca279b5d7527a5714482b0a95e
ms.contentlocale: nl-nl
ms.lasthandoff: 12/01/2017

---
# <a name="managing-inventory-costs"></a><span data-ttu-id="0e323-104">Voorraadkosten beheren</span><span class="sxs-lookup"><span data-stu-id="0e323-104">Managing Inventory Costs</span></span>
<span data-ttu-id="0e323-105">Kostenbeheer heeft betrekking op het vastleggen en rapporteren van operationele bedrijfskosten.</span><span class="sxs-lookup"><span data-stu-id="0e323-105">Cost management, also referred to as “costing”, is concerned with recording and reporting business operating costs.</span></span> <span data-ttu-id="0e323-106">Dit omvat de rapportage van productie- en voorraadkosten (dus de waarde van artikelen).</span><span class="sxs-lookup"><span data-stu-id="0e323-106">It includes the reporting of manufacturing costs and inventory costs, that is, the value of items.</span></span>   

<span data-ttu-id="0e323-107">U dient de volgende centrale principes te begrijpen: met waarderingsmethoden wordt gedefinieerd hoe artikelen worden gewaardeerd wanneer ze de voorraad verlaten, met een herwaardering van kosten worden de kosten bijgewerkt van goederen die worden verkocht met gerelateerde inkoopkosten die na de verkoop zijn geboekt en de voorraadwaarden moeten regelmatig worden geboekt naar speciale grootboekrekeningen.</span><span class="sxs-lookup"><span data-stu-id="0e323-107">Central principles to understand are that costing methods define how items are valued when they leave inventory, that cost adjustment updates the cost of goods sold with related purchase costs posted after the sale, and that inventory values must be posted to dedicated G/L accounts at regular intervals.</span></span>

<span data-ttu-id="0e323-108">In de volgende tabel wordt een reeks taken beschreven, met koppelingen naar de beschrijvende onderwerpen.</span><span class="sxs-lookup"><span data-stu-id="0e323-108">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

|<span data-ttu-id="0e323-109">**Als u dit wilt doen**</span><span class="sxs-lookup"><span data-stu-id="0e323-109">**To**</span></span>|<span data-ttu-id="0e323-110">**Zie**</span><span class="sxs-lookup"><span data-stu-id="0e323-110">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="0e323-111">Lees conceptuele informatie voor het begrip van de principes en definities die functionaliteit voor voorraadwaarderingsboekhouding in [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)] beheren.</span><span class="sxs-lookup"><span data-stu-id="0e323-111">Read various conceptual information to understand the principles and definitions that govern the inventory costing accounting functionality in [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)].</span></span>|[<span data-ttu-id="0e323-112">Over voorraadwaardering</span><span class="sxs-lookup"><span data-stu-id="0e323-112">About Inventory Costing</span></span>](finance-learn-about-costing.md)|  
|<span data-ttu-id="0e323-113">Stel voorraadperioden, waarderingsmethoden en afrondingsmethoden in.</span><span class="sxs-lookup"><span data-stu-id="0e323-113">Set up inventory periods, costing methods, and rounding methods.</span></span>|[<span data-ttu-id="0e323-114">Voorraadwaardering en kostprijsberekening instellen</span><span class="sxs-lookup"><span data-stu-id="0e323-114">Setting Up Inventory Valuation and Costing</span></span>](finance-set-up-inventory-valuation-and-costing.md)|
|<span data-ttu-id="0e323-115">Vermeerder of verminder de waarde van een of meer artikelen in voorraad door de huidige, berekende waarde ervan te boeken.</span><span class="sxs-lookup"><span data-stu-id="0e323-115">Appreciate or depreciate the value of one or more items in inventory by posting their current, calculated value.</span></span>|[<span data-ttu-id="0e323-116">Procedure: Voorraad herwaarderen</span><span class="sxs-lookup"><span data-stu-id="0e323-116">How to: Revalue Inventory</span></span>](inventory-how-revalue-inventory.md)|
|<span data-ttu-id="0e323-117">Herwaardeer artikelkosten, automatisch of handmatig, om kostenwijzigingen door te sturen van inkomende posten naar de gerelateerde uitgaande posten.</span><span class="sxs-lookup"><span data-stu-id="0e323-117">Adjust item costs, either automatically or manually, to forward cost changes from inbound entries to their related outbound entries.</span></span>|[<span data-ttu-id="0e323-118">Procedure: Artikelkosten herwaarderen</span><span class="sxs-lookup"><span data-stu-id="0e323-118">How to: Adjust Item Costs</span></span>](inventory-how-adjust-item-costs.md)|
|<span data-ttu-id="0e323-119">Speciale waarderingsfuncties gebruiken voor dagelijkse artikeltransacties in de artikelbewerkingen.</span><span class="sxs-lookup"><span data-stu-id="0e323-119">Use special costing functions for every-day item transactions in the item operations.</span></span>|[<span data-ttu-id="0e323-120">Voorraad- en productiekosten verwerken</span><span class="sxs-lookup"><span data-stu-id="0e323-120">Handling Inventory and Manufacturing Costs</span></span>](finance-handle-inventory-and-manufacturing-costs.md)|  
|<span data-ttu-id="0e323-121">U moet regelmatig de vaste verrekenprijzen van onderdelen bijwerken in assemblage- of productiestuklijsten en de nieuwe kosten tot aan het hoofdartikel berekenen.</span><span class="sxs-lookup"><span data-stu-id="0e323-121">Periodically update the standard costs of components, in assembly or production BOMs, and roll the new costs up to the parent item.</span></span>|[<span data-ttu-id="0e323-122">Procedure: vaste verrekenprijzen aanpassen</span><span class="sxs-lookup"><span data-stu-id="0e323-122">How to: Update Standard Costs</span></span>](finance-how-to-update-standard-costs.md)|
|<span data-ttu-id="0e323-123">Controle- en rapportagetaken uit te voeren voor een periode-einde, zoals het berekenen van de voorraadwaarde en het boeken van kosten in het grootboek.</span><span class="sxs-lookup"><span data-stu-id="0e323-123">Perform period-end control and reporting tasks, such calculate the value of inventory and post costs to the general ledger.</span></span>|[<span data-ttu-id="0e323-124">Kosten rapporteren en afstemmen met het grootboek</span><span class="sxs-lookup"><span data-stu-id="0e323-124">Reporting Costs and Reconciling with the General Ledger</span></span>](finance-report-costs-and-reconcile-with-the-general-ledger.md)|  
|<span data-ttu-id="0e323-125">Meer informatie over alle mechanisme in het kostprijsberekeningsysteem.</span><span class="sxs-lookup"><span data-stu-id="0e323-125">Learn about all mechanisms in the costing system.</span></span>|[<span data-ttu-id="0e323-126">Ontwerpdetails: Voorraadwaardering</span><span class="sxs-lookup"><span data-stu-id="0e323-126">Design Details: Inventory Costing</span></span>](design-details-inventory-costing.md)|  

## <a name="see-also"></a><span data-ttu-id="0e323-127">Zie ook</span><span class="sxs-lookup"><span data-stu-id="0e323-127">See Also</span></span>  
 [<span data-ttu-id="0e323-128">Financiën</span><span class="sxs-lookup"><span data-stu-id="0e323-128">Finance</span></span>](finance.md)  
 <span data-ttu-id="0e323-129">[Voorraad](inventory-manage-inventory.md) </span><span class="sxs-lookup"><span data-stu-id="0e323-129">[Inventory](inventory-manage-inventory.md) </span></span>  
 <span data-ttu-id="0e323-130">[Verkoop](sales-manage-sales.md) </span><span class="sxs-lookup"><span data-stu-id="0e323-130">[Sales](sales-manage-sales.md) </span></span>  
 [<span data-ttu-id="0e323-131">Inkoop</span><span class="sxs-lookup"><span data-stu-id="0e323-131">Purchasing</span></span>](purchasing-manage-purchasing.md)  
 <span data-ttu-id="0e323-132">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="0e323-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>


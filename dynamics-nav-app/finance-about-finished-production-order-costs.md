---
title: Over de kosten van de gereedgemelde productieorder
description: Het gereedmelden van de productieorder is een belangrijke taak in het voltooien van de levenscyclus van de waardering van het artikel dat wordt geproduceerd. De uiteindelijke kosten, inclusief verschillen in een standaardwaarderingsomgeving, werkelijke kosten in een FIFO, gemiddelde of LIFO-waarderingsomgeving, worden berekend met behulp van de batchverwerking **Kostprijs herwaarderen - Artikelposten**.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: cc1467bf1fd23668e3c080679277a89796a3b81b
ms.contentlocale: nl-nl
ms.lasthandoff: 12/01/2017

---
# <a name="about-finished-production-order-costs"></a><span data-ttu-id="ea1b4-104">Over de kosten van de gereedgemelde productieorder</span><span class="sxs-lookup"><span data-stu-id="ea1b4-104">About Finished Production Order Costs</span></span>
<span data-ttu-id="ea1b4-105">Het gereedmelden van de productieorder is een belangrijke taak in het voltooien van de levenscyclus van de waardering van het artikel dat wordt geproduceerd.</span><span class="sxs-lookup"><span data-stu-id="ea1b4-105">Finishing the production order is an important task in completing the costing lifecycle of the item that is being produced.</span></span> <span data-ttu-id="ea1b4-106">De uiteindelijke kosten (inclusief verschillen in een standaard waarderingsomgeving; werkelijke kosten in een FIFO, gemiddelde, of LIFO waarderingsomgeving) worden berekend met behulp van de batchverwerking **Kostprijs herwaarderen - Artikelposten**, die voorziet in financiële reconciliatie van de kostprijzen van artikelproductie.</span><span class="sxs-lookup"><span data-stu-id="ea1b4-106">Final costs, including variances in a standard cost environment, actuals in a FIFO, Average, or LIFO cost environment, are calculated using the **Adjust Cost - Item Entries** batch job, which allows for financial reconciliation of the costs of item production.</span></span> <span data-ttu-id="ea1b4-107">Een productieorder kan alleen in aanmerking komen voor kostenwaardering als de status **Gereedgemeld** is.</span><span class="sxs-lookup"><span data-stu-id="ea1b4-107">For a production order to be considered for cost adjustment, the status must be **Finished**.</span></span> <span data-ttu-id="ea1b4-108">Het is daarom van groot belang dat na voltooiing de status van een productieorder wordt gewijzigd in **Gereedgemeld**.</span><span class="sxs-lookup"><span data-stu-id="ea1b4-108">It is therefore critical that upon completion, the status of a production order is changed to **Finished**.</span></span>  

## <a name="example"></a><span data-ttu-id="ea1b4-109">Opmerking</span><span class="sxs-lookup"><span data-stu-id="ea1b4-109">Example</span></span>  
 <span data-ttu-id="ea1b4-110">Als u in een omgeving met vaste verrekenprijzen materiaal verbruikt voor het produceren van een artikel, worden de kosten van het artikel plus arbeid en overhead simpelweg naar OHW overgebracht.</span><span class="sxs-lookup"><span data-stu-id="ea1b4-110">In a standard cost environment, when you consume material to produce an item, stated simply, the cost of the item plus labor and overhead go into WIP.</span></span> <span data-ttu-id="ea1b4-111">Wanneer het item wordt geproduceerd, wordt OHW verminderd met het bedrag van de vaste verrekenprijs van het artikel.</span><span class="sxs-lookup"><span data-stu-id="ea1b4-111">When the item is produced, WIP is reduced by the amount of the standard cost of the item.</span></span> <span data-ttu-id="ea1b4-112">Gewoonlijk is het saldo hiervan niet nul.</span><span class="sxs-lookup"><span data-stu-id="ea1b4-112">Typically, these costs do not net to zero.</span></span> <span data-ttu-id="ea1b4-113">Om met deze kosten op nul uit te komen, moet u de batchverwerking **Kostprijs herwaarderen - Artikelposten** uitvoeren, waarbij u erop moet letten dat alleen productieorders met de status **Gereedgemeld** in aanmerking komen voor herwaardering.</span><span class="sxs-lookup"><span data-stu-id="ea1b4-113">So that these costs can net to zero, you must run the **Adjust Cost - Item Entries** batch job, noting that only production orders with the status of **Finished** will be considered for adjustment.</span></span>  

## <a name="see-also"></a><span data-ttu-id="ea1b4-114">Zie ook</span><span class="sxs-lookup"><span data-stu-id="ea1b4-114">See Also</span></span>  
[<span data-ttu-id="ea1b4-115">Voorraadkosten beheren</span><span class="sxs-lookup"><span data-stu-id="ea1b4-115">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
[<span data-ttu-id="ea1b4-116">Productie</span><span class="sxs-lookup"><span data-stu-id="ea1b4-116">Manufacturing</span></span>](production-manage-manufacturing.md)  
<span data-ttu-id="ea1b4-117">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="ea1b4-117">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>


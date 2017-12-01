---
title: Datumberekening voor verkoop
description: Het programma berekent automatisch de datum waarop u een artikel moet bestellen zodat u het op een bepaalde datum in voorraad hebt. Dit is de datum waarop u kunt verwachten dat artikelen die op een bepaalde datum zijn besteld beschikbaar zijn om te worden gepickt.
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
ms.openlocfilehash: c59bfb43a43fb53309e79d6dbde1d95decf050e8
ms.contentlocale: nl-nl
ms.lasthandoff: 12/01/2017

---
# <a name="date-calculation-for-sales"></a><span data-ttu-id="2b79f-104">Datumberekening voor verkoop</span><span class="sxs-lookup"><span data-stu-id="2b79f-104">Date Calculation for Sales</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="2b79f-105"> berekent automatisch de vroegst mogelijke datum waarop een artikel op een verkooporderregel kan worden verzonden.</span><span class="sxs-lookup"><span data-stu-id="2b79f-105"> automatically calculates the earliest possible date that an item on a sales order line can be shipped.</span></span>

<span data-ttu-id="2b79f-106">Als de klant om een specifieke leverdatum heeft verzocht, wordt berekend op welke datum de artikelen moeten kunnen worden gepickt, zodat ze op deze datum kunnen worden geleverd.</span><span class="sxs-lookup"><span data-stu-id="2b79f-106">If the customer has requested a specific delivery date, then the date on which the items must be available to pick to meet that delivery date is calculated.</span></span>

<span data-ttu-id="2b79f-107">Als de klant geen specifieke leverdatum heeft aangevraagd, wordt berekend op welke datum de artikelen kunnen worden geleverd op basis van de datum waarop de artikelen kunnen worden gepickt.</span><span class="sxs-lookup"><span data-stu-id="2b79f-107">If the customer does not request a specific delivery date, then the date on which the items can be delivered is calculated, starting from the date on which the items are available for picking.</span></span>

## <a name="calculating-a-requested-delivery-date"></a><span data-ttu-id="2b79f-108">Een verzochte leverdatum berekenen</span><span class="sxs-lookup"><span data-stu-id="2b79f-108">Calculating a Requested Delivery Date</span></span>
<span data-ttu-id="2b79f-109">Als u een aangevraagde leverdatum op de verkooporderregel plaatst, wordt automatisch deze datum gebruikt als uitgangspunt voor de volgende berekeningen.</span><span class="sxs-lookup"><span data-stu-id="2b79f-109">If you specify a requested delivery date on the sales order line, then that date is used as the starting point for the following calculations.</span></span>

- <span data-ttu-id="2b79f-110">verzochte leverdatum - verzendtijd = geplande verzenddatum</span><span class="sxs-lookup"><span data-stu-id="2b79f-110">requested delivery date - shipping time = planned shipment date</span></span>
- <span data-ttu-id="2b79f-111">geplande verzenddatum - verwerkingstijd uitgaand magazijn = verzenddatum</span><span class="sxs-lookup"><span data-stu-id="2b79f-111">planned shipment date - outbound whse. handling time = shipment date</span></span>

<span data-ttu-id="2b79f-112">Als de artikelen op de verzenddatum kunnen worden gepickt, kan het verkoopproces worden voortgezet.</span><span class="sxs-lookup"><span data-stu-id="2b79f-112">If the items are available to pick on the shipment date, then the sales process can continue.</span></span>

<span data-ttu-id="2b79f-113">Als de artikelen niet op de verzenddatum kunnen worden gepickt, wordt een voorraadwaarschuwing gegeven.</span><span class="sxs-lookup"><span data-stu-id="2b79f-113">If the items are not available to be picked on the shipment date, then a stock-out warning is displayed.</span></span>

## <a name="calculating-the-earliest-possible-delivery-date"></a><span data-ttu-id="2b79f-114">De eerst mogelijke leverdatum berekenen</span><span class="sxs-lookup"><span data-stu-id="2b79f-114">Calculating the Earliest Possible Delivery Date</span></span>
<span data-ttu-id="2b79f-115">Als u geen aangevraagde leverdatum op de verkooporderregel hebt opgegeven of als u niet aan de aangevraagde leverdatum kunt voldoen, wordt gezocht naar de vroegste datum waarop de artikelen beschikbaar zijn.</span><span class="sxs-lookup"><span data-stu-id="2b79f-115">If you do not specify a requested delivery date on the sales order line, or if the requested delivery date cannot be met, then the earliest date on which that the items are available is calculated.</span></span> <span data-ttu-id="2b79f-116">Vervolgens wordt deze datum ingevuld op de regel in het veld Verzenddatum waarna de volgende formules worden gebruikt om te bepalen op welke datum de artikelen volgens planning worden verzonden en geleverd aan de klant.</span><span class="sxs-lookup"><span data-stu-id="2b79f-116">That date is then entered in the Shipment Date field on the line, and the date on which you plan to ship the items as well as the date on which they will be delivered to the customer are calculated using the following formulas.</span></span>

- <span data-ttu-id="2b79f-117">verzenddatum + verwerkingstijd uitgaand magazijn = geplande verzenddatum</span><span class="sxs-lookup"><span data-stu-id="2b79f-117">shipment date + outbound whse. handling time = planned shipment date</span></span>
- <span data-ttu-id="2b79f-118">Geplande verzenddatum + Verzendtijd = Geplande leverdatum</span><span class="sxs-lookup"><span data-stu-id="2b79f-118">planned shipment date + shipping time = planned delivery date</span></span>


## <a name="see-also"></a><span data-ttu-id="2b79f-119">Zie ook</span><span class="sxs-lookup"><span data-stu-id="2b79f-119">See Also</span></span>  
 <span data-ttu-id="2b79f-120">[Datumberekening voor inkoop](purchasing-date-calculation-for-purchases.md) </span><span class="sxs-lookup"><span data-stu-id="2b79f-120">[Date Calculation for Purchases](purchasing-date-calculation-for-purchases.md) </span></span>  
 [<span data-ttu-id="2b79f-121">Procedure: ordertoezeggingsdatums berekenen</span><span class="sxs-lookup"><span data-stu-id="2b79f-121">How to: Calculate Order Promising Dates</span></span>](sales-how-to-calculate-order-promising-dates.md)  
 <span data-ttu-id="2b79f-122">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2b79f-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>


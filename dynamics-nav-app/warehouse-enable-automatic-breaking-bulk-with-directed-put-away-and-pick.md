---
title: Automatisch splitsen van bulkgoederen met gestuurde opslag en pick
description: Voor locaties die gebruikmaken van gestuurde opslag en pick, kunt u eenheden opsplitsen in kleinere eenheden wanneer er magazijninstructies worden gemaakt die voldoen aan de eisen met betrekking tot brondocumenten, -productieorders of interne picks en opslag.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 67b292438c0b262e7baecd622909ce3fc0f7f233
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-enable-automatic-breaking-bulk-with-directed-put-away-and-pick"></a><span data-ttu-id="9bc83-103">Procedure: Automatisch splitsen van bulkgoederen met gestuurde opslag en pick inschakelen</span><span class="sxs-lookup"><span data-stu-id="9bc83-103">How to: Enable Automatic Breaking Bulk with Directed Put-away and Pick</span></span>
<span data-ttu-id="9bc83-104">Voor locaties die gebruikmaken van gestuurde opslag en pick, kan [!INCLUDE[d365fin](includes/d365fin_md.md)] in allerlei situaties, bulkgoederen automatisch splitsen (dit houdt in dat een bepaalde eenheid wordt opgesplitst in kleinere eenheden) wanneer er magazijninstructies worden gemaakt die voldoen aan de eisen met betrekking tot brondocumenten, -productieorders of interne picks en opslag.</span><span class="sxs-lookup"><span data-stu-id="9bc83-104">For locations that use directed put-away and pick, [!INCLUDE[d365fin](includes/d365fin_md.md)] can, in various situations, automatically breakbulk, that is, break a larger unit of measure into smaller units of measure, when it creates warehouse instructions that fulfill the needs of source documents, production orders, or internal picks and put-aways.</span></span> <span data-ttu-id="9bc83-105">Bulksplitsing betekent soms ook het verzamelen van kleinere eenheden, indien nodig, om te voldoen aan uitgaande verzoeken door de grotere eenheid op het brondocument of de productieorder te splitsen in kleinere eenheden die in het magazijn beschikbaar zijn.</span><span class="sxs-lookup"><span data-stu-id="9bc83-105">To breakbulk sometimes also means gathering smaller units of measure, if necessary, to meet outbound requests by breaking the larger unit of measure on the source document or production order into the smaller units of measure that are available in the warehouse.</span></span>   

## <a name="breakbulking-in-picks"></a><span data-ttu-id="9bc83-106">Bulksplitsing in picks</span><span class="sxs-lookup"><span data-stu-id="9bc83-106">Breakbulking in Picks</span></span>  
<span data-ttu-id="9bc83-107">Als u artikelen wilt opslaan in een aantal verschillende eenheden en deze, zo nodig automatisch wilt laten combineren tijdens het pickproces, selecteert u het veld **Breakbulk toestaan** op de vestigingskaart.</span><span class="sxs-lookup"><span data-stu-id="9bc83-107">If you want to store items in several different units of measure and allow them to be automatically combined as needed in the picking process, select the **Allow Breakbulk** field on the location card.</span></span>  

<span data-ttu-id="9bc83-108">Als u een taak wilt uitvoeren, zoekt het programma automatisch naar een artikel in dezelfde eenheid.</span><span class="sxs-lookup"><span data-stu-id="9bc83-108">To fulfill a task, the program automatically looks for an item in the same unit of measure.</span></span> <span data-ttu-id="9bc83-109">Als deze vorm van het artikel echter niet wordt gevonden en u dit veld hebt geselecteerd, wordt u gevraagd een bepaalde eenheid op te splitsen in de vereiste eenheid.</span><span class="sxs-lookup"><span data-stu-id="9bc83-109">But if it cannot find this form of the item, and this field is selected, the program will suggest that you break a larger unit of measure into the unit of measure that is needed.</span></span>  

<span data-ttu-id="9bc83-110">Als het systeem alleen kleinere eenheden kan vinden, wordt u gevraagd artikelen te verzamelen om aan de hoeveelheid op de verzending of productieorder te kunnen voldoen.</span><span class="sxs-lookup"><span data-stu-id="9bc83-110">If the system can only find smaller units of measure, it will suggest that you gather items to fulfill the quantity on the shipment or production order.</span></span> <span data-ttu-id="9bc83-111">In de praktijk wordt de grotere eenheid op het brondocument opgesplitst in kleinere pickeenheden.</span><span class="sxs-lookup"><span data-stu-id="9bc83-111">In effect, it breaks the larger unit of measure on the source document into smaller units for picking.</span></span>  

## <a name="breakbulking-in-put-aways"></a><span data-ttu-id="9bc83-112">Bulksplitsing in opslag</span><span class="sxs-lookup"><span data-stu-id="9bc83-112">Breakbulking in Put-aways</span></span>  
<span data-ttu-id="9bc83-113">Bij de magazijnopslag stelt het programma automatisch Plaatsen-actieregels voor in de opslageenheid, bijvoorbeeld stuks, hoewel de artikelen in een andere eenheid arriveren.</span><span class="sxs-lookup"><span data-stu-id="9bc83-113">In the warehouse put-away, the program automatically suggests Place action lines in the put-away unit of measure, for example, pieces, even though the items arrive in a different unit of measure.</span></span>  

## <a name="breakbulking-in-movements"></a><span data-ttu-id="9bc83-114">Bulksplitsing in verplaatsingen</span><span class="sxs-lookup"><span data-stu-id="9bc83-114">Breakbulking in Movements</span></span>  
<span data-ttu-id="9bc83-115">Het programma past ook automatisch bulksplitsing toe op aanvullingsverplaatsingen, als u het standaard ingeschakelde selectievakje **Breakbulk toestaan** op het sneltabblad **Optie** van het venster **Opslagloc.-aanvulling** berekenen niet uitschakelt.</span><span class="sxs-lookup"><span data-stu-id="9bc83-115">The program also breakbulks automatically in replenishment movements, if the **Allow Breakbulk** field is selected on the **Option** FastTab in the **Calculate Bin Replenishment** window.</span></span>  

<span data-ttu-id="9bc83-116">U kunt de resultaten van de omzetting van de ene eenheid in de andere weergeven als tussenliggende bulksplitsingsregels in de opslag-, pick- of verplaatsingsinstructies.</span><span class="sxs-lookup"><span data-stu-id="9bc83-116">You can view the results of the conversion process from one unit of measure to another as intermediate breakbulk lines in the put-away, pick, or movement instructions.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="9bc83-117">Als u het veld **Breakbulkfilter** in de kop van de magazijninstructie selecteert, worden de bulksplitsingsregels verborgen wanneer de grotere eenheid volledig wordt gebruikt.</span><span class="sxs-lookup"><span data-stu-id="9bc83-117">If you select the **Set Breakbulk Filter** field on the warehouse instruction header, the program will hide the breakbulk lines whenever the larger unit of measure is going to be completely used.</span></span> <span data-ttu-id="9bc83-118">Bijvoorbeeld: als een pallet 12 stuks bevat en u alle 12 stuks gaat gebruiken, wordt u gevraagd 1 pallet te nemen en 12 stuks te plaatsen.</span><span class="sxs-lookup"><span data-stu-id="9bc83-118">For example, if a pallet is 12 pieces and you are going to use all 12 pieces, the pick will then direct you to take 1 pallet and place 12 pieces.</span></span> <span data-ttu-id="9bc83-119">Als u echter maar 9 stuks nodig hebt, worden de opsplitsingsregels niet verborgen, zelfs niet als u het veld **Breakbulkfilter** hebt geselecteerd omdat u de resterende drie stuks ergens in het magazijn moet plaatsen.</span><span class="sxs-lookup"><span data-stu-id="9bc83-119">However, if you have to pick only 9 pieces, then the breakbulk lines will not be hidden, even if you have selected the **Breakbulk Filter** field, because you have to place the remaining three pieces somewhere in the warehouse.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="9bc83-120">Als u wilt dat uw eenheden optimaal presteren in het magazijn, ook in verband met de bulksplitsingsfunctionaliteit, moet u waar mogelijk proberen om:</span><span class="sxs-lookup"><span data-stu-id="9bc83-120">If you want your units of measure to perform optimally in the warehouse, also in connection with the breakbulk functionality, you should wherever possible try to:</span></span>  
>   
> - <span data-ttu-id="9bc83-121">De basiseenheid voor een artikel in te stellen als de kleinste eenheid die u denkt nodig te hebben in de magazijnprocessen.</span><span class="sxs-lookup"><span data-stu-id="9bc83-121">Set up the base unit of measure for an item as the smallest unit of measure that you expect to handle in your warehouse processes.</span></span>  
> - <span data-ttu-id="9bc83-122">Alternatieve eenheden voor het artikel instellen als veelvouden van de basiseenheid.</span><span class="sxs-lookup"><span data-stu-id="9bc83-122">Set up your alternative units of measure for the item as multiples of the base unit of measure.</span></span>  

## <a name="see-also"></a><span data-ttu-id="9bc83-123">Zie ook</span><span class="sxs-lookup"><span data-stu-id="9bc83-123">See Also</span></span>  
[<span data-ttu-id="9bc83-124">Magazijnbeheer</span><span class="sxs-lookup"><span data-stu-id="9bc83-124">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="9bc83-125">Voorraad</span><span class="sxs-lookup"><span data-stu-id="9bc83-125">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="9bc83-126">[Magazijnbeheer instellen](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="9bc83-126">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="9bc83-127">[Assemblagebeheer](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="9bc83-127">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="9bc83-128">Ontwerpdetails: Magazijnbeheer</span><span class="sxs-lookup"><span data-stu-id="9bc83-128">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="9bc83-129">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9bc83-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  


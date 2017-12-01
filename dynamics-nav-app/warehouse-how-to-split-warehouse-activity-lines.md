---
title: Magazijnactiviteitsregels splitsen
description: Voor magazijnopslag en magazijnverplaatsingen of -picks en voor voorraadopslag en voorraadpicks worden opslaglocaties voorgesteld voor het opslaan en picken van artikelen. Het werkelijke aantal artikelen in de voorgestelde opslaglocatie is mogelijk onvoldoende of er is te weinig ruimte in de voorgestelde opslaglocatie om het vereiste aantal op te slaan. Als dat het geval is, moet u de desbetreffende regel splitsen, zodat de artikelen voor de regel in meerdere opslaglocaties worden geplaatst of uit meerdere opslaglocaties worden gepickt.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 8b2ab806f9499f9d54ed3ec79ca2874a71d8c730
ms.contentlocale: nl-nl
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-split-warehouse-activity-lines"></a><span data-ttu-id="e9fdf-105">Procedure: magazijnactiviteitsregels splitsen</span><span class="sxs-lookup"><span data-stu-id="e9fdf-105">How to: Split Warehouse Activity Lines</span></span>
<span data-ttu-id="e9fdf-106">Voor magazijnopslag en magazijnverplaatsingen of -picks en voor voorraadopslag en voorraadpicks worden opslaglocaties voorgesteld voor het opslaan en picken van artikelen.</span><span class="sxs-lookup"><span data-stu-id="e9fdf-106">In warehouse put-aways, movements, or picks, and in inventory put-aways and inventory picks, bins are suggested for the picking or putting away of items.</span></span> <span data-ttu-id="e9fdf-107">Het werkelijke aantal artikelen in de voorgestelde opslaglocatie is mogelijk onvoldoende of er is te weinig ruimte in de voorgestelde opslaglocatie om het vereiste aantal op te slaan.</span><span class="sxs-lookup"><span data-stu-id="e9fdf-107">The actual quantity in the bin suggested may not be sufficient, or there is not enough room in the suggested bin to put away the required quantity.</span></span> <span data-ttu-id="e9fdf-108">Als dat het geval is, moet u de desbetreffende regel splitsen, zodat de artikelen voor de regel in meerdere opslaglocaties worden geplaatst of uit meerdere opslaglocaties worden gepickt.</span><span class="sxs-lookup"><span data-stu-id="e9fdf-108">In these cases, you need to split the line, so that the items for one line are either taken from or placed into more than one bin.</span></span>  

<span data-ttu-id="e9fdf-109">De volgende procedure geldt voor magazijndocumenten, zoals magazijnopslag, -verplaatsing en -pickregels of voorraadopslag, -verplaatsing en -pickregels.</span><span class="sxs-lookup"><span data-stu-id="e9fdf-109">The following procedure applies to warehouse documents, such as warehouse put-away, movement, and pick lines, or inventory put-away, movement, and pick lines.</span></span>  

## <a name="to-split-warehouse-activity-lines"></a><span data-ttu-id="e9fdf-110">Magazijnactiviteitsregels splitsen</span><span class="sxs-lookup"><span data-stu-id="e9fdf-110">To split warehouse activity lines</span></span>  
1.  <span data-ttu-id="e9fdf-111">Open een magazijnactiviteitsregel waar u probeert een ontoereikend aantal te verwerken.</span><span class="sxs-lookup"><span data-stu-id="e9fdf-111">Open a warehouse activity line where you are trying to handle an insufficient quantity.</span></span>  
2.  <span data-ttu-id="e9fdf-112">Voer in het veld **Te verwerken aantal** het verlaagde aantal in dat u kunt verwerken.</span><span class="sxs-lookup"><span data-stu-id="e9fdf-112">In the **Qty. to Handle** field, enter the reduced quantity that you are able to handle.</span></span>  
3.  <span data-ttu-id="e9fdf-113">Kies op het sneltabblad **Regels** de actie **Acties**, kies **Functies** en kies vervolgens **Regel splitsen**.</span><span class="sxs-lookup"><span data-stu-id="e9fdf-113">On the **Lines** FastTab, choose the **Actions** action, choose the **Functions** action, and then choose the **Split Line** action.</span></span> <span data-ttu-id="e9fdf-114">Er verschijnt een nieuwe regel. Dit is een kopie van de oorspronkelijke regel, met uitzondering van het veld **Te verwerken aantal**, dat het aantal bevat dat u uit de oorspronkelijke regel hebt verwijderd.</span><span class="sxs-lookup"><span data-stu-id="e9fdf-114">A new line appears, which is a copy of the original line, except that the **Qty. to Handle** field contains the quantity that you removed from the original line.</span></span>  
4.  <span data-ttu-id="e9fdf-115">Wijs een opslaglocatie en een zone, als u met gestuurde opslag en pick werkt, aan deze nieuwe regel toe of blijf de regel splitsen tot u het volledige aantal artikelen over verschillende opslaglocaties hebt verdeeld.</span><span class="sxs-lookup"><span data-stu-id="e9fdf-115">Assign an appropriate bin and, if you are using directed put-away and pick, a zone, to this new line, or continue splitting the line as necessary until you find appropriate bins for all of the quantity.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="e9fdf-116">Als voor de vestiging gestuurde opslag en pick is ingesteld en u regels splitst, moet u het magazijn kennen en een opslaglocatie kunnen kiezen die overeenkomt met de opslagvereisten van het desbetreffende artikel. De opslaglocatie moet bovendien voldoen aan de algemene vereisten van het magazijndocument.</span><span class="sxs-lookup"><span data-stu-id="e9fdf-116">If the location uses directed put-away and pick and you split the lines, you must be familiar with the warehouse and be able to choose a bin that matches the storage requirements of the item and that fulfills the general requirements of the warehouse document.</span></span> <span data-ttu-id="e9fdf-117">U zou bijvoorbeeld niet een regel op een pickdocument splitsen en enkele artikelen in de bulk-opslag plaatsen.</span><span class="sxs-lookup"><span data-stu-id="e9fdf-117">For example, you would not split a line on a pick document and place some items in the bulk storage.</span></span>  

## <a name="see-also"></a><span data-ttu-id="e9fdf-118">Zie ook</span><span class="sxs-lookup"><span data-stu-id="e9fdf-118">See Also</span></span>  
[<span data-ttu-id="e9fdf-119">Magazijnbeheer</span><span class="sxs-lookup"><span data-stu-id="e9fdf-119">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="e9fdf-120">Voorraad</span><span class="sxs-lookup"><span data-stu-id="e9fdf-120">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="e9fdf-121">[Magazijnbeheer instellen](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="e9fdf-121">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="e9fdf-122">[Assemblagebeheer](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="e9fdf-122">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="e9fdf-123">Ontwerpdetails: Magazijnbeheer</span><span class="sxs-lookup"><span data-stu-id="e9fdf-123">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="e9fdf-124">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e9fdf-124">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>


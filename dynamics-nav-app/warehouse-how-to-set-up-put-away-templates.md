---
title: Opslagsjablonen instellen
description: Dankzij gestuurde opslag en pick kan op elk tijdstip de meest geschikte opslaglocatie worden gevonden. Dit gebeurt op basis van de opslagsjabloon dat u voor het magazijn hebt ingesteld, de opslaglocatievolgorde die u aan de verschillende opslaglocaties hebt toegewezen en de minimum- en maximumaantallen die u voor vaste opslaglocaties hebt ingesteld.
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
ms.openlocfilehash: be51b4d1cfc4d2a54e5f44f6419ed4539c01e9df
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-put-away-templates"></a><span data-ttu-id="067cc-103">Procedure: Opslagsjablonen instellen</span><span class="sxs-lookup"><span data-stu-id="067cc-103">How to: Set Up Put-away Templates</span></span>
<span data-ttu-id="067cc-104">Dankzij gestuurde opslag en pick kan op elk tijdstip de meest geschikte opslaglocatie worden gevonden. Dit gebeurt op basis van de opslagsjabloon die u voor het magazijn hebt ingesteld, de opslaglocatievolgorde die u aan de verschillende opslaglocaties hebt toegewezen en de minimum- en maximumaantallen die u voor vaste opslaglocaties hebt ingesteld.</span><span class="sxs-lookup"><span data-stu-id="067cc-104">With directed put-away and pick functionality, the most appropriate bin for your items at any given time is suggested, according to the put-away template that you have set up for the warehouse, the bin rankings you have given to the bins, and the minimum and maximum quantities that you have set up for fixed bins.</span></span>  

<span data-ttu-id="067cc-105">U kunt een aantal opslagsjablonen instellen en er vervolgens een van selecteren als hoofdsjabloon voor opslagactiviteiten in uw magazijn.</span><span class="sxs-lookup"><span data-stu-id="067cc-105">You can set up a number of put-away templates and select one of them to govern put-aways in general in your warehouse.</span></span> <span data-ttu-id="067cc-106">U kunt ook een bepaalde opslagsjabloon koppelen aan een artikel of SKU waarvoor speciale opslagvereisten gelden.</span><span class="sxs-lookup"><span data-stu-id="067cc-106">You can also select a put-away template for any item or stockkeeping unit that might have special put-away requirements.</span></span>  

## <a name="to-set-up-put-away-templates"></a><span data-ttu-id="067cc-107">U kunt als volgt opslagsjablonen instellen</span><span class="sxs-lookup"><span data-stu-id="067cc-107">To set up put-away templates</span></span>  
1.  <span data-ttu-id="067cc-108">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Opslagsjablonen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="067cc-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Put-away Templates**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="067cc-109">Kies de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="067cc-109">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="067cc-110">Voer een unieke id in voor de sjabloon die u wilt maken.</span><span class="sxs-lookup"><span data-stu-id="067cc-110">Enter a code that is the unique identifier of the template you are about to create.</span></span>  
4.  <span data-ttu-id="067cc-111">Typ desgewenst een korte omschrijving.</span><span class="sxs-lookup"><span data-stu-id="067cc-111">Enter a short description, if you wish.</span></span>  
5.  <span data-ttu-id="067cc-112">Voer op de eerste regel de opslaglocatievereisten in die u de hoogste prioriteit wilt geven bij opslagactiviteiten in het programma.</span><span class="sxs-lookup"><span data-stu-id="067cc-112">Fill in the first line with the bin requirements that you want fulfilled first and foremost when suggesting a put-away.</span></span>  
6.  <span data-ttu-id="067cc-113">Op de tweede regel voert u de vereisten in die u van secundair belang acht bij het zoeken naar een opslaglocatie.</span><span class="sxs-lookup"><span data-stu-id="067cc-113">Fill in the second line with the bin requirements that would be your second choice to fulfill in finding a bin for put-away.</span></span> <span data-ttu-id="067cc-114">De tweede regel wordt alleen gebruikt indien een opslaglocatie die aan de voorwaarden van de eerste regel voldoet niet kan worden gevonden.</span><span class="sxs-lookup"><span data-stu-id="067cc-114">The second line is used only if a bin that meets the requirements of the first line cannot be found.</span></span>  
7.  <span data-ttu-id="067cc-115">Vul de regels in totdat u alle acceptabele plaatsingsvereisten hebt ingevoerd waaraan moet worden voldaan bij de opslag van artikelen.</span><span class="sxs-lookup"><span data-stu-id="067cc-115">Continue to fill in the lines until you have described all the acceptable bin placements that you want to use in the put-away process.</span></span>  
8.  <span data-ttu-id="067cc-116">Schakel het selectievakje **Vrije opslaglocatie zoeken** op de laatste regel van de opslagsjabloon in.</span><span class="sxs-lookup"><span data-stu-id="067cc-116">On the last line in the put-away template, select the **Find Floating Bin** check box.</span></span>  

<span data-ttu-id="067cc-117">U kunt verschillende opslagsjablonen maken en deze naar wens toepassen.</span><span class="sxs-lookup"><span data-stu-id="067cc-117">You can create various put-away templates and then apply them as you see fit.</span></span> <span data-ttu-id="067cc-118">Er wordt allereerst rekening gehouden met de opslagsjabloon die u hebt geselecteerd voor het artikel of de SKU.</span><span class="sxs-lookup"><span data-stu-id="067cc-118">The put-away template that you selected for the item or stockkeeping unit, if any is used first.</span></span> <span data-ttu-id="067cc-119">Als deze velden niet zijn ingevuld, wordt de opslagsjabloon gebruikt die u voor het magazijn hebt geselecteerd op het sneltabblad **Opslaglocatiebeleid** van de vestigingskaart.</span><span class="sxs-lookup"><span data-stu-id="067cc-119">If these fields are not filled in, then the put-away template that you selected for the warehouse on the **Bin Policies** FastTab on the location card is used.</span></span>  

## <a name="see-also"></a><span data-ttu-id="067cc-120">Zie ook</span><span class="sxs-lookup"><span data-stu-id="067cc-120">See Also</span></span>  
[<span data-ttu-id="067cc-121">Magazijnbeheer</span><span class="sxs-lookup"><span data-stu-id="067cc-121">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="067cc-122">Voorraad</span><span class="sxs-lookup"><span data-stu-id="067cc-122">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="067cc-123">[Magazijnbeheer instellen](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="067cc-123">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="067cc-124">[Assemblagebeheer](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="067cc-124">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="067cc-125">Ontwerpdetails: Magazijnbeheer</span><span class="sxs-lookup"><span data-stu-id="067cc-125">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="067cc-126">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="067cc-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>


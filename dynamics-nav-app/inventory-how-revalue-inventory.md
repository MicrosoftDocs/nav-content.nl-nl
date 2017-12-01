---
title: Nieuwe waardeposten maken voor artikelen in de voorraad
description: Beschrijft hoe u de waardeposten vermeerdert of vermindert van een of meer artikelen in de voorraad door de huidige, berekende waarde ervan te boeken.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: costing, inventory cost, value entries
ms.date: 08/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: f945b13f87dfbab07d4df59a43dd4daf26ff9cb0
ms.contentlocale: nl-nl
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-revalue-inventory"></a><span data-ttu-id="252ca-103">Procedure: Voorraad herwaarderen</span><span class="sxs-lookup"><span data-stu-id="252ca-103">How to: Revalue Inventory</span></span>
<span data-ttu-id="252ca-104">Gebruik het herwaarderingsdagboek als u de voorraadwaarde van een artikel of een bepaalde artikelpost wilt vermeerderen of verminderen.</span><span class="sxs-lookup"><span data-stu-id="252ca-104">If you want to appreciate or depreciate an item or a specific item ledger entry, you must use the revaluation journal.</span></span>

## <a name="to-revalue-inventory"></a><span data-ttu-id="252ca-105">Voorraad herwaarderen</span><span class="sxs-lookup"><span data-stu-id="252ca-105">To revalue inventory</span></span>
1. <span data-ttu-id="252ca-106">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Herwaarderingsdagboek** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="252ca-106">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Revaluation Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="252ca-107">Kies de actie **Voorraadwaarde berekenen**.</span><span class="sxs-lookup"><span data-stu-id="252ca-107">Choose the **Calculate Inventory Value** action.</span></span>
3. <span data-ttu-id="252ca-108">Vul in het venster **Voorraadwaarde berekenen** indien nodig de velden in.</span><span class="sxs-lookup"><span data-stu-id="252ca-108">In the **Calculate Inventory Value** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="252ca-109">Kies de knop **Ok**.</span><span class="sxs-lookup"><span data-stu-id="252ca-109">Choose the **OK** button.</span></span>
5. <span data-ttu-id="252ca-110">Voer op elke regel in het venster **Herwaarderingsdagboek** het veld **Kostprijs (Geherwaardeerd)** in en voer de nieuwe eenheidskosten in.</span><span class="sxs-lookup"><span data-stu-id="252ca-110">On each line in the **Revaluation Journal** window, in the **Unit Cost (Revalued)** field, enter the new unit cost.</span></span> <span data-ttu-id="252ca-111">U kunt ook het nieuwe totale bedrag in het veld **Voorraadwaarde (Geherwaardeerd)** invoeren.</span><span class="sxs-lookup"><span data-stu-id="252ca-111">Alternatively, enter the new total amount in the **Inventory Value (Revalued)** field.</span></span>

    <span data-ttu-id="252ca-112">De bijbehorende velden worden automatisch bijgewerkt.</span><span class="sxs-lookup"><span data-stu-id="252ca-112">The relevant fields are automatically updated.</span></span> <span data-ttu-id="252ca-113">In het veld **Bedrag** wordt de werkelijke wijziging in de voorraadwaarde voor de geselecteerde artikelpost weergegeven.</span><span class="sxs-lookup"><span data-stu-id="252ca-113">Note that the **Amount** field shows the actual change in inventory value for the selected item ledger entry.</span></span> <span data-ttu-id="252ca-114">Het verschil tussen de waarden in de velden **Voorraadwaarde (Berekend)** en **Voorraadwaarde (Geherwaardeerd)** wordt berekend.</span><span class="sxs-lookup"><span data-stu-id="252ca-114">It calculates the difference between the **Inventory Value (Calculated)** field and the **Inventory Value (Revalued)** field.</span></span>
6. <span data-ttu-id="252ca-115">Wanneer u alle regels in het herwaarderingsdagboek hebt ingevuld, kiest u de actie **Boeken**.</span><span class="sxs-lookup"><span data-stu-id="252ca-115">When you have completed all lines in the revaluation journal, choose the **Post** action.</span></span>

<span data-ttu-id="252ca-116">Nieuwe waardeposten worden nu gemaakt om de herwaarderingen weer te geven die u hebt geboekt.</span><span class="sxs-lookup"><span data-stu-id="252ca-116">New value entries are now created to reflect the revaluations that you have posted.</span></span> <span data-ttu-id="252ca-117">U kunt de nieuwe waarden op de desbetreffende artikelkaarten bekijken.</span><span class="sxs-lookup"><span data-stu-id="252ca-117">You can see the new values on the respective item cards.</span></span>

## <a name="see-also"></a><span data-ttu-id="252ca-118">Zie ook</span><span class="sxs-lookup"><span data-stu-id="252ca-118">See Also</span></span>
[<span data-ttu-id="252ca-119">Ontwerpdetails: Herwaardering</span><span class="sxs-lookup"><span data-stu-id="252ca-119">Design Details: Revaluation</span></span>](design-details-revaluation.md)  
[<span data-ttu-id="252ca-120">Voorraad</span><span class="sxs-lookup"><span data-stu-id="252ca-120">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="252ca-121">Verkoop</span><span class="sxs-lookup"><span data-stu-id="252ca-121">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="252ca-122">Inkoop</span><span class="sxs-lookup"><span data-stu-id="252ca-122">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="252ca-123">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="252ca-123">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>


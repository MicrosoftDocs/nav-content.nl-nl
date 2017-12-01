---
title: Verbruik in batches boeken
description: Als de afboekingsmethode **Handmatig** is, moet u de materialen handmatig boeken met behulp van een verbruiksdagboek.
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
ms.openlocfilehash: 765e315a5fd1b886e9e04222a6fcfa983f2df31a
ms.contentlocale: nl-nl
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-batch-post-production-consumption"></a><span data-ttu-id="86ef9-103">Procedure: Productieverbruik in batches boeken</span><span class="sxs-lookup"><span data-stu-id="86ef9-103">How to: Batch Post Production Consumption</span></span>
<span data-ttu-id="86ef9-104">Als de afboekingsmethode **Handmatig** is, moet u de materialen handmatig boeken met behulp van een verbruiksdagboek.</span><span class="sxs-lookup"><span data-stu-id="86ef9-104">If the flushing method is **Manual**, you must post the components manually, using a consumption journal.</span></span>

<span data-ttu-id="86ef9-105">U kunt het systeem ook zo instellen materialen automatisch worden geboekt (*afgeboekt**) als u productieorders start of voltooit.</span><span class="sxs-lookup"><span data-stu-id="86ef9-105">You can also set the system up to automatically post (*flush*) components when you start or finish production orders.</span></span> <span data-ttu-id="86ef9-106">Zie voor meer informatie [Afboeking van materialen op basis van de uitvoer van een bewerking inschakelen](production-how-to-flush-components-according-to-operation-output.md).</span><span class="sxs-lookup"><span data-stu-id="86ef9-106">For more information, see [Enable Flushing of Components According to Operation Output](production-how-to-flush-components-according-to-operation-output.md).</span></span>

## <a name="to-post-consumption-for-one-or-more-production-order-lines"></a><span data-ttu-id="86ef9-107">Verbruik boeken voor een of meer productieorderregels</span><span class="sxs-lookup"><span data-stu-id="86ef9-107">To post consumption for one or more production order lines</span></span>  
1.  <span data-ttu-id="86ef9-108">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Verbruiksdagboek** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="86ef9-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Consumption Journal**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="86ef9-109">Voer in de velden informatie over de productieorder en verbruik in.</span><span class="sxs-lookup"><span data-stu-id="86ef9-109">Fill in the fields with the production order data and the consumption data.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    <span data-ttu-id="86ef9-110">Als het magazijn waar de materialen zijn opgeslagen opslaglocaties gebruikt, maar geen pickverwerking vereist, kunt u een opslaglocatie toewijzen aan de dagboekregel om aan te geven waar de artikelen uit het magazijn moeten worden gehaald.</span><span class="sxs-lookup"><span data-stu-id="86ef9-110">If the warehouse location where the components are stored is set up to use bins but does not require pick processing, assign a bin code to the journal line to indicate where the items should be taken from in the warehouse.</span></span> <span data-ttu-id="86ef9-111">Zie [Procedure: Picken voor productie of assemblage](warehouse-how-to-pick-for-production.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="86ef9-111">For more information, see [How to: Pick for Production or Assembly](warehouse-how-to-pick-for-production.md).</span></span>  
3.  <span data-ttu-id="86ef9-112">Kies de actie **Boeken** om het verbruik te boeken.</span><span class="sxs-lookup"><span data-stu-id="86ef9-112">Choose the **Post** action to post the consumption.</span></span> <span data-ttu-id="86ef9-113">De betreffende artikelposten worden verminderd.</span><span class="sxs-lookup"><span data-stu-id="86ef9-113">The related item ledger entries are reduced.</span></span>

## <a name="see-also"></a><span data-ttu-id="86ef9-114">Zie ook</span><span class="sxs-lookup"><span data-stu-id="86ef9-114">See Also</span></span>  
<span data-ttu-id="86ef9-115">[Productie](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="86ef9-115">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="86ef9-116">Productie instellen</span><span class="sxs-lookup"><span data-stu-id="86ef9-116">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="86ef9-117">[Gepland](production-planning.md)    </span><span class="sxs-lookup"><span data-stu-id="86ef9-117">[Planning](production-planning.md)    </span></span>  
[<span data-ttu-id="86ef9-118">Voorraad</span><span class="sxs-lookup"><span data-stu-id="86ef9-118">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="86ef9-119">Inkoop</span><span class="sxs-lookup"><span data-stu-id="86ef9-119">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="86ef9-120">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="86ef9-120">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>


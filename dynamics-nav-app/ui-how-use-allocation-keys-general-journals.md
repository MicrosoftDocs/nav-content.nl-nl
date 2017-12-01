---
title: 'Procedure: verdeelsleutels in dagboeken gebruiken '
description: Leren hoe u verdeelsleutels in dagboeken gebruikt.
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cost accounting
ms.date: 03/29/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: a0dea4d1043766ed198002aba93a80882b1f16fe
ms.contentlocale: nl-nl
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-use-allocation-keys-in-general-journals"></a><span data-ttu-id="6b9b7-103">Procedure: verdeelsleutels in dagboeken gebruiken</span><span class="sxs-lookup"><span data-stu-id="6b9b7-103">How to: Use Allocation Keys in General Journals</span></span>
<span data-ttu-id="6b9b7-104">U kunt een post in een dagboek verdelen over verschillende rekeningen wanneer u het dagboek boekt.</span><span class="sxs-lookup"><span data-stu-id="6b9b7-104">You can allocate an entry in a general journal to several different accounts when you post the journal.</span></span> <span data-ttu-id="6b9b7-105">De verdeling kan plaatsvinden op basis van aantal, percentage of bedrag.</span><span class="sxs-lookup"><span data-stu-id="6b9b7-105">The allocation can be made by quantity, percentage, or amount.</span></span>

## <a name="to-set-up-allocation-keys"></a><span data-ttu-id="6b9b7-106">Verdeelsleutels instellen</span><span class="sxs-lookup"><span data-stu-id="6b9b7-106">To set up allocation keys</span></span>
1. <span data-ttu-id="6b9b7-107">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Periodiek dagboek** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="6b9b7-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Recurring General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="6b9b7-108">Kies het veld **Batchnaam** om het venster **Fin. dagboekbatches** te openen.</span><span class="sxs-lookup"><span data-stu-id="6b9b7-108">Choose the **Batch Name** field to open the **General Journal Batches** window.</span></span>
3. <span data-ttu-id="6b9b7-109">U kunt verdeelsleutels in een bestaande batch in de lijst wijzigen of u kunt een nieuwe batch met verdeelsleutels maken.</span><span class="sxs-lookup"><span data-stu-id="6b9b7-109">You can either modify allocations on an existing batch in the list or create a new batch with allocations.</span></span>
   * <span data-ttu-id="6b9b7-110">Als u een nieuwe batch wilt maken, kiest u de actie **Nieuw** en gaat u naar de volgende stap.</span><span class="sxs-lookup"><span data-stu-id="6b9b7-110">To create a new batch, choose the **New** action, and go to the next step.</span></span>
   * <span data-ttu-id="6b9b7-111">Als u de verdeelsleutels van een bestaand dagboek wilt wijzigen, selecteert u het dagboek en gaat u naar stap 7.</span><span class="sxs-lookup"><span data-stu-id="6b9b7-111">To change the allocations of an existing journal, select the journal and go to step 7.</span></span>    
4. <span data-ttu-id="6b9b7-112">Voer in het veld **Naam** een naam voor de batch in, bijvoorbeeld Schoonmaak.</span><span class="sxs-lookup"><span data-stu-id="6b9b7-112">In the **Name** field, enter a name for the batch, such as CLEANING.</span></span> <span data-ttu-id="6b9b7-113">Voer in het veld **Omschrijving** een omschrijving in, bijvoorbeeld Dagboek schoonmaakkosten.</span><span class="sxs-lookup"><span data-stu-id="6b9b7-113">In the **Description** field, enter a description, such as Cleaning Expenses Journal.</span></span>
5. <span data-ttu-id="6b9b7-114">Wanneer u klaar bent, sluit u het venster.</span><span class="sxs-lookup"><span data-stu-id="6b9b7-114">When you are done, close the window.</span></span> <span data-ttu-id="6b9b7-115">Er wordt een nieuw, leeg periodiek dagboek geopend.</span><span class="sxs-lookup"><span data-stu-id="6b9b7-115">A new, empty recurring journal opens.</span></span>
6. <span data-ttu-id="6b9b7-116">Vul de velden op de regel in.</span><span class="sxs-lookup"><span data-stu-id="6b9b7-116">Fill in the fields on the line.</span></span>
7. <span data-ttu-id="6b9b7-117">Kies de actie **Verdeelsleutels**.</span><span class="sxs-lookup"><span data-stu-id="6b9b7-117">Choose the **Allocations** action.</span></span>
8. <span data-ttu-id="6b9b7-118">Voeg voor elke verdeelsleutel een regel toe.</span><span class="sxs-lookup"><span data-stu-id="6b9b7-118">Add a line for each allocation.</span></span> <span data-ttu-id="6b9b7-119">U moet ofwel het veld **Verdeelsleutel %**, of **Verdeelsleutelaantal**, of **Bedrag** invullen.</span><span class="sxs-lookup"><span data-stu-id="6b9b7-119">You must fill in either the **Allocation %**, **Allocation Quantity**, or **Amount** field.</span></span> <span data-ttu-id="6b9b7-120">U moet ook het veld **Rekeningnr.** invullen. Als u de transactie wilt toewijzen aan verschillende globale dimensies, moet u ook de globale dimensievelden invullen.</span><span class="sxs-lookup"><span data-stu-id="6b9b7-120">You must also fill in the **Account No.** field and, if you are allocating the transaction among global dimensions, the global dimension fields.</span></span>
9. <span data-ttu-id="6b9b7-121">Als u een percentage op de regel invoert, wordt het bedrag in het veld **Bedrag** automatisch berekend.</span><span class="sxs-lookup"><span data-stu-id="6b9b7-121">If you enter a percentage on a line, the amount in the **Amount** field is calculated automatically.</span></span> <span data-ttu-id="6b9b7-122">Deze bedragen hebben het tegengestelde teken van het totale bedrag in het veld **Bedrag** in het periodieke dagboek.</span><span class="sxs-lookup"><span data-stu-id="6b9b7-122">These amounts have the opposite sign from the total amount in the **Amount** field in the recurring journal.</span></span>
10. <span data-ttu-id="6b9b7-123">Kies **OK** na het invoeren van de verdeelsleutelregels om terug te keren naar het venster **Periodiek dagboek**.</span><span class="sxs-lookup"><span data-stu-id="6b9b7-123">After entering the allocations lines, choose **OK** to return to the **Recurring General Journal** window.</span></span> <span data-ttu-id="6b9b7-124">Het veld **Verdeeld bedrag (LV)** wordt ingevuld en de inhoud komt overeen met het veld **Bedrag**.</span><span class="sxs-lookup"><span data-stu-id="6b9b7-124">The **Allocated Amt. (USD)** field is filled in and matches the **Amount** field.</span></span>
11. <span data-ttu-id="6b9b7-125">Boek het dagboek.</span><span class="sxs-lookup"><span data-stu-id="6b9b7-125">Post the journal.</span></span>

## <a name="to-change-an-allocation-key-that-has-already-been-set-up"></a><span data-ttu-id="6b9b7-126">Een reeds ingestelde verdeelsleutel wijzigen</span><span class="sxs-lookup"><span data-stu-id="6b9b7-126">To change an allocation key that has already been set up</span></span>
1. <span data-ttu-id="6b9b7-127">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Periodiek dagboek** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="6b9b7-127">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Recurring General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="6b9b7-128">Selecteer in het venster **Periodiek dagboek** het dagboek met de verdeling.</span><span class="sxs-lookup"><span data-stu-id="6b9b7-128">In the **Recurring General Journal** window, select the journal with the allocation.</span></span>
3. <span data-ttu-id="6b9b7-129">Kies de regel met de verdeelsleutel en kies vervolgens **Verdeelsleutels**.</span><span class="sxs-lookup"><span data-stu-id="6b9b7-129">Choose the line with the allocation, and then choose **Allocations** action.</span></span>
4. <span data-ttu-id="6b9b7-130">Pas de relevante velden aan en kies vervolgens de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="6b9b7-130">Change the relevant fields, and then choose the **OK** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="6b9b7-131">Zie ook</span><span class="sxs-lookup"><span data-stu-id="6b9b7-131">See Also</span></span>
[<span data-ttu-id="6b9b7-132">Werken met diversendagboeken</span><span class="sxs-lookup"><span data-stu-id="6b9b7-132">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="6b9b7-133">Documenten en dagboeken boeken</span><span class="sxs-lookup"><span data-stu-id="6b9b7-133">Posting Documents and Journals</span></span>](ui-post-documents-journals.md)  
<span data-ttu-id="6b9b7-134">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="6b9b7-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>


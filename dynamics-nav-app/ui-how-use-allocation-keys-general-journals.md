---
title: 'Procedure: verdeelsleutels in dagboeken gebruiken'
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: d239ab62c4be88ccc4a2ce2669dcc2c20a3c0126
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

#  <a name="how-to-use-allocation-keys-in-general-journals"></a><span data-ttu-id="300ab-102">Procedure: verdeelsleutels in dagboeken gebruiken</span><span class="sxs-lookup"><span data-stu-id="300ab-102">How to: Use Allocation Keys in General Journals</span></span>
<span data-ttu-id="300ab-103">U kunt een post in een dagboek verdelen over verschillende rekeningen wanneer u het dagboek boekt.</span><span class="sxs-lookup"><span data-stu-id="300ab-103">You can allocate an entry in a general journal to several different accounts when you post the journal.</span></span> <span data-ttu-id="300ab-104">De verdeling kan plaatsvinden op basis van aantal, percentage of bedrag.</span><span class="sxs-lookup"><span data-stu-id="300ab-104">The allocation can be made by quantity, percentage, or amount.</span></span>

## <a name="to-set-up-allocation-keys"></a><span data-ttu-id="300ab-105">Verdeelsleutels instellen</span><span class="sxs-lookup"><span data-stu-id="300ab-105">To set up allocation keys</span></span> 
1. <span data-ttu-id="300ab-106">Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Periodiek dagboek** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="300ab-106">In the top right corner, choose the **Search for Page or Report** icon, enter **Recurring General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="300ab-107">Kies het veld **Batchnaam** om het venster **Fin. dagboekbatches** te openen.</span><span class="sxs-lookup"><span data-stu-id="300ab-107">Choose the **Batch Name** field to open the **General Journal Batches** window.</span></span>
3. <span data-ttu-id="300ab-108">U kunt verdeelsleutels in een bestaande batch in de lijst wijzigen of u kunt een nieuwe batch met verdeelsleutels maken.</span><span class="sxs-lookup"><span data-stu-id="300ab-108">You can either modify allocations on an existing batch in the list or create a new batch with allocations.</span></span>
  * <span data-ttu-id="300ab-109">Als u een nieuwe batch wilt maken, kiest u de actie **Nieuw** en gaat u naar de volgende stap.</span><span class="sxs-lookup"><span data-stu-id="300ab-109">To create a new batch, choose the **New** action, and go to the next step.</span></span>
  * <span data-ttu-id="300ab-110">Als u de verdeelsleutels van een bestaand dagboek wilt wijzigen, selecteert u het dagboek en gaat u naar stap 7.</span><span class="sxs-lookup"><span data-stu-id="300ab-110">To change the allocations of an existing journal, select the journal and go to step 7.</span></span>    
4. <span data-ttu-id="300ab-111">Voer in het veld **Naam** een naam voor de batch in, bijvoorbeeld Schoonmaak.</span><span class="sxs-lookup"><span data-stu-id="300ab-111">In the **Name** field, enter a name for the batch, such as CLEANING.</span></span> <span data-ttu-id="300ab-112">Voer in het veld **Omschrijving** een omschrijving in, bijvoorbeeld Dagboek schoonmaakkosten.</span><span class="sxs-lookup"><span data-stu-id="300ab-112">In the **Description** field, enter a description, such as Cleaning Expenses Journal.</span></span>
5. <span data-ttu-id="300ab-113">Wanneer u klaar bent, sluit u het venster.</span><span class="sxs-lookup"><span data-stu-id="300ab-113">When you are done, close the window.</span></span> <span data-ttu-id="300ab-114">Er wordt een nieuw, leeg periodiek dagboek geopend.</span><span class="sxs-lookup"><span data-stu-id="300ab-114">A new, empty recurring journal opens.</span></span> 
6. <span data-ttu-id="300ab-115">Vul de velden op de regel in.</span><span class="sxs-lookup"><span data-stu-id="300ab-115">Fill in the fields in the line.</span></span>
7. <span data-ttu-id="300ab-116">Kies de actie **Verdeelsleutels**.</span><span class="sxs-lookup"><span data-stu-id="300ab-116">Choose the **Allocations** action.</span></span> 
8. <span data-ttu-id="300ab-117">Voeg voor elke verdeelsleutel een regel toe.</span><span class="sxs-lookup"><span data-stu-id="300ab-117">Add a line for each allocation.</span></span> <span data-ttu-id="300ab-118">U moet ofwel het veld **Verdeelsleutel %**, of **Verdeelsleutelaantal**, of **Bedrag** invullen.</span><span class="sxs-lookup"><span data-stu-id="300ab-118">You must fill in either the **Allocation %**, **Allocation Quantity**, or **Amount** field.</span></span> <span data-ttu-id="300ab-119">U moet ook het veld **Rekeningnr.** invullen</span><span class="sxs-lookup"><span data-stu-id="300ab-119">You must also fill in the **Account No.**</span></span> <span data-ttu-id="300ab-120">en, als u de transactie verdeelt over globale dimensies, ook de globale dimensievelden.</span><span class="sxs-lookup"><span data-stu-id="300ab-120">field and, if you are allocating the transaction among global dimensions, the global dimension fields.</span></span>
9. <span data-ttu-id="300ab-121">Als u een percentage op de regel invoert, wordt het bedrag in het veld **Bedrag** automatisch berekend.</span><span class="sxs-lookup"><span data-stu-id="300ab-121">If you enter a percentage on a line, the amount in the **Amount** field is calculated automatically.</span></span> <span data-ttu-id="300ab-122">Deze bedragen hebben het tegengestelde teken van het totale bedrag in het veld **Bedrag** in het periodieke dagboek.</span><span class="sxs-lookup"><span data-stu-id="300ab-122">These amounts have the opposite sign from the total amount in the **Amount** field in the recurring journal.</span></span>
10. <span data-ttu-id="300ab-123">Kies **OK** na het invoeren van de verdeelsleutelregels om terug te keren naar het venster **Periodiek dagboek**.</span><span class="sxs-lookup"><span data-stu-id="300ab-123">After entering the allocations lines, choose **OK** to return to the **Recurring General Journal** window.</span></span> <span data-ttu-id="300ab-124">Het veld **Verdeeld bedrag (LV)** wordt ingevuld en de inhoud komt overeen met het veld **Bedrag**.</span><span class="sxs-lookup"><span data-stu-id="300ab-124">The **Allocated Amt. (USD)** field is filled in and matches the **Amount** field.</span></span>
11. <span data-ttu-id="300ab-125">Boek het dagboek.</span><span class="sxs-lookup"><span data-stu-id="300ab-125">Post the journal.</span></span>

## <a name="to-change-an-allocation-key-that-has-already-been-set-up"></a><span data-ttu-id="300ab-126">Een reeds ingestelde verdeelsleutel wijzigen</span><span class="sxs-lookup"><span data-stu-id="300ab-126">To change an allocation key that has already been set up</span></span>
1. <span data-ttu-id="300ab-127">Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Periodiek dagboek** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="300ab-127">In the top right corner, choose the **Search for Page or Report** icon, enter **Recurring General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="300ab-128">Selecteer in het venster **Periodiek dagboek** het dagboek met de verdeling.</span><span class="sxs-lookup"><span data-stu-id="300ab-128">In the **Recurring General Journal** window, select the journal with the allocation.</span></span>
3. <span data-ttu-id="300ab-129">Kies de regel met de verdeelsleutel en kies vervolgens **Verdeelsleutels**.</span><span class="sxs-lookup"><span data-stu-id="300ab-129">Choose the line with the allocation, and then choose **Allocations** action.</span></span>
4. <span data-ttu-id="300ab-130">Wijzig de betreffende velden en sluit het venster.</span><span class="sxs-lookup"><span data-stu-id="300ab-130">Change the relevant fields, and close the window.</span></span>

## <a name="see-also"></a><span data-ttu-id="300ab-131">Zie ook</span><span class="sxs-lookup"><span data-stu-id="300ab-131">See Also</span></span>
[<span data-ttu-id="300ab-132">Werken met diversendagboeken</span><span class="sxs-lookup"><span data-stu-id="300ab-132">Work With General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="300ab-133">Documenten en dagboeken boeken</span><span class="sxs-lookup"><span data-stu-id="300ab-133">Post Documents and Journals</span></span>](ui-post-documents-journals.md)





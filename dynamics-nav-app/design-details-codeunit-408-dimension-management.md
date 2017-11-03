---
title: 'Ontwerpdetails: Codeunit 408 Dimensiebeheer'
description: "Codeunit 408 Dimensiebeheer is een functiebibliotheek die veel voorkomende taken afhandelt die verband houden met dimensies, zoals kopiëren van de ene tabel naar de andere of van het ene document naar het andere."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: c1b3c745597f96165aec92a08bba50ecb6727a84
ms.contentlocale: nl-nl
ms.lasthandoff: 10/23/2017

---
# <a name="design-details-codeunit-408-dimension-management"></a><span data-ttu-id="3e462-103">Ontwerpdetails: Codeunit 408 Dimensiebeheer</span><span class="sxs-lookup"><span data-stu-id="3e462-103">Design Details: Codeunit 408 Dimension Management</span></span>
<span data-ttu-id="3e462-104">Codeunit 408 Dimensiebeheer is een functiebibliotheek die veel voorkomende taken afhandelt die verband houden met dimensies, zoals kopiëren van de ene tabel naar de andere of van het ene document naar het andere.</span><span class="sxs-lookup"><span data-stu-id="3e462-104">Codeunit 408 Dimension Management is a function library that handles common tasks that are related to dimensions, such as copying from one table to another or from one document to another.</span></span> <span data-ttu-id="3e462-105">In dit onderwerp worden de functies genoemd die in Microsoft Dynamics NAV 2013 R2 zijn gewijzigd en er wordt aangegeven wat er met de functies moet gebeuren.</span><span class="sxs-lookup"><span data-stu-id="3e462-105">This topic lists the functions that are modified in Microsoft Dynamics NAV 2013 R2 and specifies what has to be done to the functions.</span></span> <span data-ttu-id="3e462-106">Veel functies zijn verwijderd omdat er geen reden is om te kopiëren tussen dimensietabellen.</span><span class="sxs-lookup"><span data-stu-id="3e462-106">Many functions are deleted because there is no need for copying between dimension tables.</span></span>  

## <a name="modified-functions"></a><span data-ttu-id="3e462-107">Gewijzigde functies</span><span class="sxs-lookup"><span data-stu-id="3e462-107">Modified Functions</span></span>  

|<span data-ttu-id="3e462-108">Functienaam</span><span class="sxs-lookup"><span data-stu-id="3e462-108">Function Name</span></span>|<span data-ttu-id="3e462-109">Beschrijving wijziging</span><span class="sxs-lookup"><span data-stu-id="3e462-109">Modification Description</span></span>|  
|-------------------|------------------------------|  
|<span data-ttu-id="3e462-110">CheckDimSetIDComb</span><span class="sxs-lookup"><span data-stu-id="3e462-110">CheckDimSetIDComb</span></span>|<span data-ttu-id="3e462-111">Nieuwe functie die de overige controlefuncties vervangt en die een dimensieset-id als argument gebruikt in plaats van een dimensietabel.</span><span class="sxs-lookup"><span data-stu-id="3e462-111">New function that substitutes the other check functions and takes a Dimension Set ID as an argument instead of a dimension table.</span></span>|  
|<span data-ttu-id="3e462-112">CheckDimSetIDComb</span><span class="sxs-lookup"><span data-stu-id="3e462-112">CheckDimSetIDComb</span></span><br /><br /> <span data-ttu-id="3e462-113">CheckDocDimComb</span><span class="sxs-lookup"><span data-stu-id="3e462-113">CheckDocDimComb</span></span><br /><br /> <span data-ttu-id="3e462-114">CheckServContractDimComb</span><span class="sxs-lookup"><span data-stu-id="3e462-114">CheckServContractDimComb</span></span><br /><br /> <span data-ttu-id="3e462-115">CheckDimBuffer</span><span class="sxs-lookup"><span data-stu-id="3e462-115">CheckDimBuffer</span></span><br /><br /> <span data-ttu-id="3e462-116">CheckDimComb</span><span class="sxs-lookup"><span data-stu-id="3e462-116">CheckDimComb</span></span><br /><br /> <span data-ttu-id="3e462-117">CheckDimValueComb</span><span class="sxs-lookup"><span data-stu-id="3e462-117">CheckDimValueComb</span></span>|<span data-ttu-id="3e462-118">Wissen.</span><span class="sxs-lookup"><span data-stu-id="3e462-118">Delete.</span></span> <span data-ttu-id="3e462-119">Al het gebruik moet worden gewijzigd in CheckDimSetIDComb.</span><span class="sxs-lookup"><span data-stu-id="3e462-119">All usage should be changed to CheckDimSetIDComb.</span></span>|  
|<span data-ttu-id="3e462-120">GetDefaultDim</span><span class="sxs-lookup"><span data-stu-id="3e462-120">GetDefaultDim</span></span>|<span data-ttu-id="3e462-121">Wijzigen om een geheel-getal dimensieset-id te retourneren in plaats van een set records.</span><span class="sxs-lookup"><span data-stu-id="3e462-121">Modify to return an integer Dimension Set ID instead of a set of records.</span></span>|  
|<span data-ttu-id="3e462-122">CopyJnlLineDimToICJnlDim</span><span class="sxs-lookup"><span data-stu-id="3e462-122">CopyJnlLineDimToICJnlDim</span></span><br /><br /> <span data-ttu-id="3e462-123">CopyICJnlDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="3e462-123">CopyICJnlDimToJnlLineDim</span></span><br /><br /> <span data-ttu-id="3e462-124">CopyDocDimtoICDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-124">CopyDocDimtoICDocDim</span></span><br /><br /> <span data-ttu-id="3e462-125">CopyICDocDimtoICDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-125">CopyICDocDimtoICDocDim</span></span>|<span data-ttu-id="3e462-126">Wijzigen voor gebruik met DimSetID > ICJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="3e462-126">Modify to work with DimSetID -> ICJnlLineDim</span></span>|  

## <a name="deleted-functions"></a><span data-ttu-id="3e462-127">Verwijderde functies</span><span class="sxs-lookup"><span data-stu-id="3e462-127">Deleted Functions</span></span>  
 <span data-ttu-id="3e462-128">De functies die uit codeunit 408 met de Dimensiesetpostenfunctie zijn verwijderd worden hieronder weergegeven.</span><span class="sxs-lookup"><span data-stu-id="3e462-128">Functions that are deleted from codeunit 408 in connection with the Dimension Set Entries feature are listed below.</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="3e462-129">Tijdens de upgrade van de vereffeningcode van Microsoft Dynamics NAV 2009 of eerdere versies naar Microsoft Dynamics NAV 2016 zijn de volgende functies niet beschikbaar in Microsoft Dynamics NAV 2016.</span><span class="sxs-lookup"><span data-stu-id="3e462-129">During the upgrade of application code from Microsoft Dynamics NAV 2009 or earlier versions to Microsoft Dynamics NAV 2016, the following functions are not available in Microsoft Dynamics NAV 2016.</span></span> <span data-ttu-id="3e462-130">Als u aanpassingen hebt die een of meer van de functies gebruiken, moet u die code upgraden.</span><span class="sxs-lookup"><span data-stu-id="3e462-130">If you have customizations that use one or more of the functions, you must upgrade that code accordingly.</span></span>

 <span data-ttu-id="3e462-131">InsertJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="3e462-131">InsertJnlLineDim</span></span>  

 <span data-ttu-id="3e462-132">UpdateJnlLineDefaultDim</span><span class="sxs-lookup"><span data-stu-id="3e462-132">UpdateJnlLineDefaultDim</span></span>  

 <span data-ttu-id="3e462-133">GetJnlLineDefaultDim</span><span class="sxs-lookup"><span data-stu-id="3e462-133">GetJnlLineDefaultDim</span></span>  

 <span data-ttu-id="3e462-134">GetPreviousDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="3e462-134">GetPreviousDocDefaultDim</span></span>  

 <span data-ttu-id="3e462-135">GetPreviousProdDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="3e462-135">GetPreviousProdDocDefaultDim</span></span>  

 <span data-ttu-id="3e462-136">InsertDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-136">InsertDocDim</span></span>  

 <span data-ttu-id="3e462-137">UpdateDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="3e462-137">UpdateDocDefaultDim</span></span>  

 <span data-ttu-id="3e462-138">ExtractDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="3e462-138">ExtractDocDefaultDim</span></span>  

 <span data-ttu-id="3e462-139">InsertProdDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-139">InsertProdDocDim</span></span>  

 <span data-ttu-id="3e462-140">UpdateProdDocDefaultDim</span><span class="sxs-lookup"><span data-stu-id="3e462-140">UpdateProdDocDefaultDim</span></span>  

 <span data-ttu-id="3e462-141">InsertServContractDim</span><span class="sxs-lookup"><span data-stu-id="3e462-141">InsertServContractDim</span></span>  

 <span data-ttu-id="3e462-142">UpdateServcontractDim</span><span class="sxs-lookup"><span data-stu-id="3e462-142">UpdateServcontractDim</span></span>  

 <span data-ttu-id="3e462-143">UpdateDefaultDimNewDimValue</span><span class="sxs-lookup"><span data-stu-id="3e462-143">UpdateDefaultDimNewDimValue</span></span>  

 <span data-ttu-id="3e462-144">GetDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-144">GetDocDim</span></span>  

 <span data-ttu-id="3e462-145">GetProdDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-145">GetProdDocDim</span></span>  

 <span data-ttu-id="3e462-146">TypeToTableID1</span><span class="sxs-lookup"><span data-stu-id="3e462-146">TypeToTableID1</span></span>  

 <span data-ttu-id="3e462-147">TypeToTableID2</span><span class="sxs-lookup"><span data-stu-id="3e462-147">TypeToTableID2</span></span>  

 <span data-ttu-id="3e462-148">TypeToTableID3</span><span class="sxs-lookup"><span data-stu-id="3e462-148">TypeToTableID3</span></span>  

 <span data-ttu-id="3e462-149">TypeToTableID4</span><span class="sxs-lookup"><span data-stu-id="3e462-149">TypeToTableID4</span></span>  

 <span data-ttu-id="3e462-150">TypeToTableID5</span><span class="sxs-lookup"><span data-stu-id="3e462-150">TypeToTableID5</span></span>  

 <span data-ttu-id="3e462-151">DeleteJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="3e462-151">DeleteJnlLineDim</span></span>  

 <span data-ttu-id="3e462-152">DeleteDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-152">DeleteDocDim</span></span>  

 <span data-ttu-id="3e462-153">DeletePostedDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-153">DeletePostedDocDim</span></span>  

 <span data-ttu-id="3e462-154">DeleteProdDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-154">DeleteProdDocDim</span></span>  

 <span data-ttu-id="3e462-155">DeleteServContractDim</span><span class="sxs-lookup"><span data-stu-id="3e462-155">DeleteServContractDim</span></span>  

 <span data-ttu-id="3e462-156">ShowJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="3e462-156">ShowJnlLineDim</span></span>  

 <span data-ttu-id="3e462-157">SaveJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="3e462-157">SaveJnlLineDim</span></span>  

 <span data-ttu-id="3e462-158">ShowJnlLineNewDim</span><span class="sxs-lookup"><span data-stu-id="3e462-158">ShowJnlLineNewDim</span></span>  

 <span data-ttu-id="3e462-159">SaveJnlLineNewDim</span><span class="sxs-lookup"><span data-stu-id="3e462-159">SaveJnlLineNewDim</span></span>  

 <span data-ttu-id="3e462-160">ShowDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-160">ShowDocDim</span></span>  

 <span data-ttu-id="3e462-161">SaveDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-161">SaveDocDim</span></span>  

 <span data-ttu-id="3e462-162">ShowProdDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-162">ShowProdDocDim</span></span>  

 <span data-ttu-id="3e462-163">SaveProdDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-163">SaveProdDocDim</span></span>  

 <span data-ttu-id="3e462-164">ShowTempDim</span><span class="sxs-lookup"><span data-stu-id="3e462-164">ShowTempDim</span></span>  

 <span data-ttu-id="3e462-165">SaveTempDim</span><span class="sxs-lookup"><span data-stu-id="3e462-165">SaveTempDim</span></span>  

 <span data-ttu-id="3e462-166">ShowTempNewDim</span><span class="sxs-lookup"><span data-stu-id="3e462-166">ShowTempNewDim</span></span>  

 <span data-ttu-id="3e462-167">SaveTempNewDim</span><span class="sxs-lookup"><span data-stu-id="3e462-167">SaveTempNewDim</span></span>  

 <span data-ttu-id="3e462-168">SaveServContractDim</span><span class="sxs-lookup"><span data-stu-id="3e462-168">SaveServContractDim</span></span>  

 <span data-ttu-id="3e462-169">MoveJnlLineDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="3e462-169">MoveJnlLineDimToLedgEntryDim</span></span>  

 <span data-ttu-id="3e462-170">MoveDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-170">MoveDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="3e462-171">MoveOneDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-171">MoveOneDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="3e462-172">MoveLedgEntryDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="3e462-172">MoveLedgEntryDimToJnlLineDim</span></span>  

 <span data-ttu-id="3e462-173">MoveDimBufToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="3e462-173">MoveDimBufToJnlLineDim</span></span>  

 <span data-ttu-id="3e462-174">MoveDimBufToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="3e462-174">MoveDimBufToLedgEntryDim</span></span>  

 <span data-ttu-id="3e462-175">MoveDimBufToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-175">MoveDimBufToPostedDocDim</span></span>  

 <span data-ttu-id="3e462-176">MoveDimBufToGLBudgetDim</span><span class="sxs-lookup"><span data-stu-id="3e462-176">MoveDimBufToGLBudgetDim</span></span>  

 <span data-ttu-id="3e462-177">CopyJnlLineDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="3e462-177">CopyJnlLineDimToJnlLineDim</span></span>  

 <span data-ttu-id="3e462-178">CopyLedgEntryDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="3e462-178">CopyLedgEntryDimToJnlLineDim</span></span>  

 <span data-ttu-id="3e462-179">CopyDocDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-179">CopyDocDimToDocDim</span></span>  

 <span data-ttu-id="3e462-180">CopyPostedDocDimToPostedDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-180">CopyPostedDocDimToPostedDocDim</span></span>  

 <span data-ttu-id="3e462-181">CopyDocDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="3e462-181">CopyDocDimToJnlLineDim</span></span>  

 <span data-ttu-id="3e462-182">CopyDimBufToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="3e462-182">CopyDimBufToJnlLineDim</span></span>  

 <span data-ttu-id="3e462-183">CopyDimBufToDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-183">CopyDimBufToDocDim</span></span>  

 <span data-ttu-id="3e462-184">CopySCDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-184">CopySCDimToDocDim</span></span>  

 <span data-ttu-id="3e462-185">MoveDocDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="3e462-185">MoveDocDimToLedgEntryDim</span></span>  

 <span data-ttu-id="3e462-186">MoveDocDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-186">MoveDocDimToDocDim</span></span>  

 <span data-ttu-id="3e462-187">MoveDocDimArchvToDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-187">MoveDocDimArchvToDocDim</span></span>  

 <span data-ttu-id="3e462-188">MoveLedgEntryDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-188">MoveLedgEntryDimToDocDim</span></span>  

 <span data-ttu-id="3e462-189">MoveProdDocDimToProdDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-189">MoveProdDocDimToProdDocDim</span></span>  

 <span data-ttu-id="3e462-190">MoveJnlLineDimToProdDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-190">MoveJnlLineDimToProdDocDim</span></span>  

 <span data-ttu-id="3e462-191">MoveJnlLineDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-191">MoveJnlLineDimToDocDim</span></span>  

 <span data-ttu-id="3e462-192">MoveJnlLineDimToJnlLineDim</span><span class="sxs-lookup"><span data-stu-id="3e462-192">MoveJnlLineDimToJnlLineDim</span></span>  

 <span data-ttu-id="3e462-193">CopyLedgEntryDimToLedgEntryDim</span><span class="sxs-lookup"><span data-stu-id="3e462-193">CopyLedgEntryDimToLedgEntryDim</span></span>  

 <span data-ttu-id="3e462-194">MoveTempFromDimToTempToDim</span><span class="sxs-lookup"><span data-stu-id="3e462-194">MoveTempFromDimToTempToDim</span></span>  

 <span data-ttu-id="3e462-195">TransferTempToDimToDocDim</span><span class="sxs-lookup"><span data-stu-id="3e462-195">TransferTempToDimToDocDim</span></span>  

 <span data-ttu-id="3e462-196">MoveJnlLineDimToBuf</span><span class="sxs-lookup"><span data-stu-id="3e462-196">MoveJnlLineDimToBuf</span></span>  

 <span data-ttu-id="3e462-197">CopyICJnlDimToICJnlDim</span><span class="sxs-lookup"><span data-stu-id="3e462-197">CopyICJnlDimToICJnlDim</span></span>  

 <span data-ttu-id="3e462-198">TestDimValue</span><span class="sxs-lookup"><span data-stu-id="3e462-198">TestDimValue</span></span>  

 <span data-ttu-id="3e462-199">TestNewDimValue</span><span class="sxs-lookup"><span data-stu-id="3e462-199">TestNewDimValue</span></span>  

 <span data-ttu-id="3e462-200">MoveDimBufToItemBudgetDim.</span><span class="sxs-lookup"><span data-stu-id="3e462-200">MoveDimBufToItemBudgetDim.</span></span> <span data-ttu-id="3e462-201">(Verwijderen omdat de tabel ItemBudgetDim wordt verwijderd.)</span><span class="sxs-lookup"><span data-stu-id="3e462-201">(Delete because the ItemBudgetDim Table is deleted.)</span></span>  

 <span data-ttu-id="3e462-202">GetServContractDim</span><span class="sxs-lookup"><span data-stu-id="3e462-202">GetServContractDim</span></span>  

 <span data-ttu-id="3e462-203">MoveTempDimToBuf</span><span class="sxs-lookup"><span data-stu-id="3e462-203">MoveTempDimToBuf</span></span>  

 <span data-ttu-id="3e462-204">UpdateSCInvLineDim</span><span class="sxs-lookup"><span data-stu-id="3e462-204">UpdateSCInvLineDim</span></span>  

 <span data-ttu-id="3e462-205">CopyJnlLineDimToBuffer</span><span class="sxs-lookup"><span data-stu-id="3e462-205">CopyJnlLineDimToBuffer</span></span>  

 <span data-ttu-id="3e462-206">UpdateDocDefaultDim2</span><span class="sxs-lookup"><span data-stu-id="3e462-206">UpdateDocDefaultDim2</span></span>  

## <a name="see-also"></a><span data-ttu-id="3e462-207">Zie ook</span><span class="sxs-lookup"><span data-stu-id="3e462-207">See Also</span></span>
 <span data-ttu-id="3e462-208">[Ontwerpdetails: Dimensiesetposten](design-details-dimension-set-entries.md) </span><span class="sxs-lookup"><span data-stu-id="3e462-208">[Design Details: Dimension Set Entries](design-details-dimension-set-entries.md) </span></span>  
 <span data-ttu-id="3e462-209">[Ontwerpdetails: Dimensiesetposten - overzicht](design-details-dimension-set-entries-overview.md) </span><span class="sxs-lookup"><span data-stu-id="3e462-209">[Design Details: Dimension Set Entries Overview](design-details-dimension-set-entries-overview.md) </span></span>  
 <span data-ttu-id="3e462-210">[Ontwerpdetails: Dimensiecombinaties zoeken](design-details-searching-for-dimension-combinations.md) </span><span class="sxs-lookup"><span data-stu-id="3e462-210">[Design Details: Searching for Dimension Combinations](design-details-searching-for-dimension-combinations.md) </span></span>  
 <span data-ttu-id="3e462-211">[Ontwerpdetails: Tabelstructuur](design-details-table-structure.md) </span><span class="sxs-lookup"><span data-stu-id="3e462-211">[Design Details: Table Structure](design-details-table-structure.md) </span></span>  
 [<span data-ttu-id="3e462-212">Ontwerpdetails: Codevoorbeelden van gewijzigde patronen in wijzigingen</span><span class="sxs-lookup"><span data-stu-id="3e462-212">Design Details: Code Examples of Changed Patterns in Modifications</span></span>](design-details-code-examples-of-changed-patterns-in-modifications.md)


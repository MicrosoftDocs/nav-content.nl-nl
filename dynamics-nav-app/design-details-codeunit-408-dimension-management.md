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
# <a name="design-details-codeunit-408-dimension-management"></a>Ontwerpdetails: Codeunit 408 Dimensiebeheer
Codeunit 408 Dimensiebeheer is een functiebibliotheek die veel voorkomende taken afhandelt die verband houden met dimensies, zoals kopiëren van de ene tabel naar de andere of van het ene document naar het andere. In dit onderwerp worden de functies genoemd die in Microsoft Dynamics NAV 2013 R2 zijn gewijzigd en er wordt aangegeven wat er met de functies moet gebeuren. Veel functies zijn verwijderd omdat er geen reden is om te kopiëren tussen dimensietabellen.  

## <a name="modified-functions"></a>Gewijzigde functies  

|Functienaam|Beschrijving wijziging|  
|-------------------|------------------------------|  
|CheckDimSetIDComb|Nieuwe functie die de overige controlefuncties vervangt en die een dimensieset-id als argument gebruikt in plaats van een dimensietabel.|  
|CheckDimSetIDComb<br /><br /> CheckDocDimComb<br /><br /> CheckServContractDimComb<br /><br /> CheckDimBuffer<br /><br /> CheckDimComb<br /><br /> CheckDimValueComb|Wissen. Al het gebruik moet worden gewijzigd in CheckDimSetIDComb.|  
|GetDefaultDim|Wijzigen om een geheel-getal dimensieset-id te retourneren in plaats van een set records.|  
|CopyJnlLineDimToICJnlDim<br /><br /> CopyICJnlDimToJnlLineDim<br /><br /> CopyDocDimtoICDocDim<br /><br /> CopyICDocDimtoICDocDim|Wijzigen voor gebruik met DimSetID > ICJnlLineDim|  

## <a name="deleted-functions"></a>Verwijderde functies  
 De functies die uit codeunit 408 met de Dimensiesetpostenfunctie zijn verwijderd worden hieronder weergegeven.  

> [!CAUTION]  
>  Tijdens de upgrade van de vereffeningcode van Microsoft Dynamics NAV 2009 of eerdere versies naar Microsoft Dynamics NAV 2016 zijn de volgende functies niet beschikbaar in Microsoft Dynamics NAV 2016. Als u aanpassingen hebt die een of meer van de functies gebruiken, moet u die code upgraden.

 InsertJnlLineDim  

 UpdateJnlLineDefaultDim  

 GetJnlLineDefaultDim  

 GetPreviousDocDefaultDim  

 GetPreviousProdDocDefaultDim  

 InsertDocDim  

 UpdateDocDefaultDim  

 ExtractDocDefaultDim  

 InsertProdDocDim  

 UpdateProdDocDefaultDim  

 InsertServContractDim  

 UpdateServcontractDim  

 UpdateDefaultDimNewDimValue  

 GetDocDim  

 GetProdDocDim  

 TypeToTableID1  

 TypeToTableID2  

 TypeToTableID3  

 TypeToTableID4  

 TypeToTableID5  

 DeleteJnlLineDim  

 DeleteDocDim  

 DeletePostedDocDim  

 DeleteProdDocDim  

 DeleteServContractDim  

 ShowJnlLineDim  

 SaveJnlLineDim  

 ShowJnlLineNewDim  

 SaveJnlLineNewDim  

 ShowDocDim  

 SaveDocDim  

 ShowProdDocDim  

 SaveProdDocDim  

 ShowTempDim  

 SaveTempDim  

 ShowTempNewDim  

 SaveTempNewDim  

 SaveServContractDim  

 MoveJnlLineDimToLedgEntryDim  

 MoveDocDimToPostedDocDim  

 MoveOneDocDimToPostedDocDim  

 MoveLedgEntryDimToJnlLineDim  

 MoveDimBufToJnlLineDim  

 MoveDimBufToLedgEntryDim  

 MoveDimBufToPostedDocDim  

 MoveDimBufToGLBudgetDim  

 CopyJnlLineDimToJnlLineDim  

 CopyLedgEntryDimToJnlLineDim  

 CopyDocDimToDocDim  

 CopyPostedDocDimToPostedDocDim  

 CopyDocDimToJnlLineDim  

 CopyDimBufToJnlLineDim  

 CopyDimBufToDocDim  

 CopySCDimToDocDim  

 MoveDocDimToLedgEntryDim  

 MoveDocDimToDocDim  

 MoveDocDimArchvToDocDim  

 MoveLedgEntryDimToDocDim  

 MoveProdDocDimToProdDocDim  

 MoveJnlLineDimToProdDocDim  

 MoveJnlLineDimToDocDim  

 MoveJnlLineDimToJnlLineDim  

 CopyLedgEntryDimToLedgEntryDim  

 MoveTempFromDimToTempToDim  

 TransferTempToDimToDocDim  

 MoveJnlLineDimToBuf  

 CopyICJnlDimToICJnlDim  

 TestDimValue  

 TestNewDimValue  

 MoveDimBufToItemBudgetDim. (Verwijderen omdat de tabel ItemBudgetDim wordt verwijderd.)  

 GetServContractDim  

 MoveTempDimToBuf  

 UpdateSCInvLineDim  

 CopyJnlLineDimToBuffer  

 UpdateDocDefaultDim2  

## <a name="see-also"></a>Zie ook
 [Ontwerpdetails: Dimensiesetposten](design-details-dimension-set-entries.md)   
 [Ontwerpdetails: Dimensiesetposten - overzicht](design-details-dimension-set-entries-overview.md)   
 [Ontwerpdetails: Dimensiecombinaties zoeken](design-details-searching-for-dimension-combinations.md)   
 [Ontwerpdetails: Tabelstructuur](design-details-table-structure.md)   
 [Ontwerpdetails: Codevoorbeelden van gewijzigde patronen in wijzigingen](design-details-code-examples-of-changed-patterns-in-modifications.md)


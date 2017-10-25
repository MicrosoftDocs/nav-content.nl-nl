---
title: 'Ontwerpdetails: boekingsenginestructuur'
description: Boekingsinterface en enkele andere functies in codeunit 12 gebruiken boekingsenginefuncties om grootboekposten en btw-postrecords voor te bereiden en in te voegen. De boekingsengine is ook verantwoordelijk voor het maken van het grootboekjournaal.
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
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 2a0c90fde23b708c3de8365f7211e66bee615cb1
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-posting-engine-structure"></a>Ontwerpdetails: boekingsenginestructuur
Boekingsinterface en enkele andere functies in codeunit 12 gebruiken boekingsenginefuncties om grootboekposten en btw-postrecords voor te bereiden en in te voegen. De boekingsengine is ook verantwoordelijk voor het maken van het grootboekjournaal.  
  
 De functies in de volgende tabel bieden een standaardkader voor het ontwerp van boekingsprocedures (zoals Code, CustPostApplyCustledgEntry, VendPostApplyVendLedgEntry, UnapplyCustLedgEntry, UnapplyVendLedgEntry en Reverse) en exclusieve toegang tot tabel 17, Grootboekpost.  
  
|Routine|Description|  
|-------------|---------------------------------------|  
|StartPosting|Initialiseert boekingsbuffer TempGLEntryBuf, vergrendelt grootboekpost- en btw-posttabellen, en initialiseert Boekingsperiode, Grootboekjournaal en Wisselkoers. Moet slechts eenmaal worden aangeroepen, zodat NextEntryNo 0 is.|  
|ContinuePosting|Hiermee wordt ongerealiseerde btw voor de vorige transactietoename NextTransactionNo gecontroleerd en geboekt, en wordt het boeken van de volgende regel voorbereid.|  
|FinishPosting|Hiermee worden boekingen voltooid door grootboekposten uit de tijdelijke buffer in te voegen in de databasetabel. Altijd gebruikt in combinatie met StartPosting. Controleert op inconsistenties.|  
|InitGLEntry|Gebruikt om nieuwe grootboekpost te initialiseren voor dagboekregel. Retourneert GLEntry als parameter.|  
|InitGLEntryVAT|Hetzelfde als InitGLEntry, maar Tegenrekeningnr. en SummarizeVAT worden ook toegewezen.|  
|InitGLEntryVATCopy|Vergelijkbaar met InitGLEntryVAT, maar er worden ook boekingsgroepgegevens van btw-posten vóór SummarizeVAT gekopieerd.|  
|InsertGLEntry|De enige functie waarmee grootboekposten in de algemene tabel TempGLEntryBuf wordt ingevoegd. Deze functie altijd gebruiken voor invoegen.|  
|CreateGLEntry|Voert een InitGLEntry uit, wijst Bedrag (Rapp.-val.) toe en voert vervolgens InsertGLEntry uit. Vervangt verschillende regels code door een enkele functieaanroep.|  
|CreateGLEntryBalAcc|Hetzelfde als CreateGLEntry, maar Tegenrekeningsoort en Tegenrekeningnr. worden ook toegewezen.|  
|CreateGLEntryVAT|Hetzelfde als CreateGLEntry, maar met extra verwerking voor boekingsgroepen en opslag in tijdelijke btw-buffer:<br /><br /> `GLEntry.CopyPostingGroupsFromDtldCVBuf(DtldCVLedgEntryBuf,GenJnlLine."Gen. Posting Type");`<br /><br /> `InsertVATEntriesFromTemp(DtldCVLedgEntryBuf,GLEntry);`|  
|CreateGLEntryVATCollectAdj|Hetzelfde als CreateGLEntry, maar met extra verzameling van aanpassingen en opslag in tijdelijke btw-buffer:<br /><br /> `CollectAdjustment(AdjAmount,GLEntry.Amount,GLEntry."Additional-Currency Amount",OriginalDateSet);`<br /><br /> `InsertVATEntriesFromTemp(DtldCVLedgEntryBuf,GLEntry);`|  
|CreateGLEntryFromVATEntry|Hetzelfde als CreateGLEntry, maar er worden ook boekingsgroepen uit Btw-post gekopieerd.|  
  
## <a name="see-also"></a>Zie ook  
 [Ontwerpdetails: boekingsinterfacestructuur](design-details-posting-interface-structure.md)

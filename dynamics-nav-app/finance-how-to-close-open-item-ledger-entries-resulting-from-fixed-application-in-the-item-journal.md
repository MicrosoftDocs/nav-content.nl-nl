---
title: Open artikelposten sluiten die uit een vaste vereffening in het artikeldagboek voortkomen
description: U kunt het veld **Vereffenen van post** in het venster **Artikeldagboek** gebruiken om een vaste vereffening tussen een inkomende transactie en de oorspronkelijke uitgaande transactie te maken. Bijvoorbeeld om de uitgaande transactie te corrigeren of de retourzending te verwerken.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/09/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b0b0daad01f8108d035739e387b38af4f0311ff9
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-close-open-item-ledger-entries-resulting-from-fixed-application-in-the-item-journal"></a>Procedure: open artikelposten die uit een vaste vereffening in het artikeldagboek voortkomen sluiten
U kunt het veld **Vereffenen van post** in het venster **Artikeldagboek** gebruiken om een vaste vereffening tussen een inkomende transactie en de oorspronkelijke uitgaande transactie te maken. Bijvoorbeeld om de uitgaande transactie te corrigeren of de retourzending te verwerken. Zie voor meer informatie Vereffenen van post.  

> [!IMPORTANT]  
>  Vaste vereffeningen die op deze manier worden uitgevoerd, worden alleen toegepast op de kosten, niet op de hoeveelheid. Bijgevolg sluit de geboekte positieve artikelpost niet de toegepaste uitgaande post en blijft deze zelf ook geopend. Dit geldt ook wanneer u een vaste vereffening voor een positieve post toepast op een negatieve post die niet is afgesloten door een gewone positieve post. In dat geval blijven de negatieve en de positieve posten geopend.  
>   
>  Dit betekent dat u een voorraadperiode waarin een dergelijke vermelding bestaat, niet kunt sluiten.  

De volgende procedure laat zien hoe u dergelijke posten kunt sluiten door het uitvoeren van twee corrigerende boekingen in het artikeldagboek.  

## <a name="to-close-open-item-ledger-entries-that-result-from-a-fixed-application-in-the-item-journal"></a>Openstaande artikelposten die uit een vaste vereffening in het artikeldagboek voortkomen sluiten  

1.  Gebruik het veld **Vereffenen van post** om een positieve aanpassing met de overeenkomstige hoeveelheid te boeken. De oorspronkelijke negatieve post met een vaste vereffening wordt gesloten.  
2.  Gebruik het veld **Vereffenen van post** om een negatieve vereffening te boeken. De oorspronkelijke positieve correctiepost met een vaste vereffening wordt gesloten.  

## <a name="see-also"></a>Zie ook  
[Procedure: artikelposten verwijderen en opnieuw toepassen](finance-how-to-remove-and-reapply-item-entries.md)  
 [Procedure: Verkoopretouren of annuleringen verwerken](sales-how-process-sales-returns-cancellations.md)   
 [Voorraadwaardering en kostprijsberekening instellen](finance-set-up-inventory-valuation-and-costing.md)   
 [Voorraadkosten beheren](finance-manage-inventory-costs.md)   
 [Ontwerpdetails: Waarderingsmethoden](design-details-costing-methods.md)


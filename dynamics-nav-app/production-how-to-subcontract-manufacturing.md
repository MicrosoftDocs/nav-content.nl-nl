---
title: Productie uitbesteden
description: Zodra de inkooporder is gemaakt vanuit het uitbestedingsvoorstel, kan deze worden geboekt.
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/04/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: fa1d42f623ba3d13f60d49b502c15fcc3f48bde7
ms.contentlocale: nl-nl
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-subcontract-manufacturing"></a>Procedure: Productie uitbesteden
Veel productiebedrijven besteden bepaalde bewerkingen uit aan leveranciers. Uitbesteden kan een eenmalig gebeuren zijn of een integraal onderdeel uitmaken van alle productieprocessen.

Het programma biedt verscheidene tools voor het beheren van uitbesteed werk:  

- Afdelingen met toegewezen leveranciers: met behulp van deze functie kunt u een afdeling instellen die is gekoppeld aan een leverancier (toeleverancier). Dit wordt een uitbestedingsafdeling genoemd. U kunt een uitbestedingsafdeling specificeren bij een bewerking in een bewerkingsplan, waarmee u op eenvoudige wijze de uitbestede activiteit kunt verwerken. Daarnaast kunnen de kosten van de bewerking worden toegewezen op het niveau van het bewerkingsplan of van de afdeling.  
- Afdelingskosten gebaseerd op eenheden of tijd: met behulp van deze functie kunt u opgeven of kosten die samenhangen met de afdeling worden gebaseerd op de productietijd of een vaste toeslag per eenheid. Hoewel toeleveranciers gewoonlijk werken met een vaste toeslag per eenheid die in rekening wordt gebracht voor hun diensten, kan het programma overweg met beide opties (productietijd en vaste toeslag per eenheid).  
- Uitbestedingsvoorstel: met behulp van deze functie kunt u de productieorders vinden met materiaal dat gereed is om naar een toeleverancier te worden gezonden en automatisch inkooporders opstellen voor uitbestedingsbewerkingen op basis van productieorderbewerkingsplannen. Het programma boekt vervolgens automatisch de inkoopordertoeslagen naar de productieorder tijdens het boeken van de inkooporder. Alleen productieorders met de status Vrijgegeven zijn toegankelijk en kunnen worden gebruikt vanuit een uitbestedingsvoorstel.  

## <a name="subcontract-work-centers"></a>Uitbestedingsafdelingen  
Uitbestedingsafdelingen worden op dezelfde manier ingesteld as normale afdelingen met aanvullende informatie. Deze worden op dezelfde manier toegewezen aan bewerkingsplannen als andere afdelingen.  

### <a name="subcontract-work-center-fields"></a>Velden voor uitbestedingsafdelingen  
Dit veld **Toeleveranciersnr.** geeft aan dat de afdeling een uitbestedingsafdeling is. U kunt het nummer invoeren van de toeleverancier die de afdeling levert. Dit veld kan worden gebruikt om afdelingen te beheren die zich niet binnenshuis bevinden, maar werkzaamheden verrichten op contractbasis.  

Als u elk proces uitbesteedt voor een ander tarief bij de leverancier, schakelt u het selectievakje **Specifieke kostprijs** in. Op die manier kunt u kosten instellen op elke bewerkingsplanregel en spaart u de tijd van het opnieuw invoeren van elke inkooporder. De kosten op de bewerkingsplanregel worden gebruikt bij de verwerking in plaats van de kosten in de kostenvelden van de afdeling. Als u **Specifieke kostprijs** inschakelt, worden kosten voor de leverancier berekend per bewerkingsplanbewerking.  

Als u tegen één tarief per leverancier uitbesteedt, laat u het veld **Specifieke kostprijs** leeg. De kosten worden ingesteld door het invullen van de velden **Directe kostprijs**, **Indirecte kosten %** en **Overheadtarief**.  

### <a name="routings-that-use-subcontract-work-centers"></a>Bewerkingsplannen die gebruikmaken van uitbestedingsafdelingen  
Uitbestedingsafdelingen kunnen op dezelfde manier als reguliere afdelingen worden gebruikt voor bewerkingen in bewerkingsplannen.  

U kunt een bewerkingsplan instellen dat gebruikmaakt van een externe afdeling als standaard bewerkingsstap. Aan de andere kant kunt u ook het bewerkingsplan voor een bepaalde productieorder wijzigen zodat deze een externe bewerking bevat. Dit kan nodig zijn in een noodsituatie, zoals het niet correct werken van een server, of wanneer er tijdelijk sprake is van een grotere vraag, waarbij werk dat gewoonlijk binnenshuis wordt uitgevoerd naar een toeleverancier moet worden gestuurd.  

Zie [Procedure: Bewerkingsplannen maken](production-how-to-create-routings.md) voor meer informatie.  

## <a name="subcontracting-worksheet"></a>Uitbestedingsvoorstel  
Zodra u het uitbestedingsvoorstel hebt berekend, wordt het relevante document (in dit geval een inkooporder) opgesteld.  

# <a name="how-to-calculate-subcontracting-worksheets-and-create-subcontract-purchase-orders"></a>Procedure: uitbestedingsvoorstel berekenen en uitbestedingsinkooporders maken
Het venster **Uitbestedingsvoorstel** werkt als het **Planningsvoorstel** door de benodigde voorziening te berekenen van, in dit geval inkooporders, die u in het voorstel bekijkt en vervolgens met de functie **Planningsboodschap uitvoeren** maakt.  

> [!NOTE]  
>  Alleen productieorders met de status **Vrijgegeven** zijn toegankelijk en kunnen worden gebruikt vanuit een uitbestedingsvoorstel.  

### <a name="to-calculate-the-subcontracting-worksheet"></a>Het uitbestedingsvoorstel berekenen  
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Uitbestedingsvoorstel** in en klik vervolgens op de gerelateerde koppeling.  
2.  Als u het voorstel wilt berekenen, klikt u op de actie **Uitbestedingen berekenen**.  
3.  Stel in het venster **Uitbestedingen berekenen** filters in voor de uitbestede bewerkingen of de werkplaatsen waar ze worden uitgevoerd, om zo alleen de relevante productieorders te berekenen.  
4.  Kies de knop **Ok**.  

    Bekijk de regels in het venster **Uitbestedingsvoorstel**. De informatie in dit voorstel is afkomstig van de productieorder en de productieorderbewerkingsplanregels en gaat naar de inkooporder op het moment dat dit document wordt aangemaakt. U kunt een rij uit het voorstel verwijderen zonder dat dit gevolgen heeft voor de oorspronkelijke informatie, net zoals u met andere voorstellen kunt. De informatie verschijnt opnieuw de volgende keer dat u de functie **Uitbestedingen berekenen** uitvoert.  

### <a name="to-create-the-subcontract-purchase-order"></a>De uitbestedingsinkooporder genereren  
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Uitbestedingsvoorstel** in en klik vervolgens op de gerelateerde koppeling.  
2.  Kies op het tabblad **Acties** in de groep **Verwerken** de optie **Planningsboodschap uitvoeren**.  
3.  Plaats een vinkje in het veld **Orders afdrukken** om de inkooporder af te drukken wanneer deze wordt gemaakt.  
4.  Kies de knop **OK**.  

Als alle uitbestede bewerkingen naar dezelfde leveranciersvestiging worden gestuurd, wordt slechts één inkooporder opgesteld.  

De voorstelregel waarvan een inkooporder is gemaakt, wordt verwijderd uit het voorstel. Zodra een inkooporder is gemaakt, wordt het niet meer weergegeven in het voorstel.  

## <a name="posting-subcontract-purchase-orders"></a>Uitbestedingsinkooporders boeken  
Zodra de inkooporders voor toeleveranciers zijn opgesteld, kunnen deze worden geboekt. Bij ontvangst van de order wordt een capaciteitspost geboekt op de productieorder en bij het factureren van de order worden de directe kosten van de inkooporder geboekt op de productieorder.  

Wanneer de inkooporder wordt geboekt als ontvangen, wordt automatisch een output-dagboekpost voor de productieorder geboekt. Dit is alleen van toepassing als de uitbestedingsbewerking de laatste bewerking in het productieorderbewerkingsplan is.  

> [!CAUTION]  
>  De output automatisch boeken voor een voortdurende productieorder wanneer uitbestede artikelen worden ontvangen, is mogelijk niet wenselijk. De redenen voor dit zouden kunnen zijn dat het verwachte outputaantal dat wordt geboekt verschilt van het werkelijke aantal en dat de boekdatum van de automatische output misleidend is.  
>   
>  Om te voorkomen dat de verwachte uitvoer van een productieorder wordt geboekt wanneer de uitbestedingsinkopen worden ontvangen, moet u ervoor zorgen dat de uitbestede bewerking niet de laatste is. Of voeg een nieuwe laatste bewerking voor het laatste outputaantal in.

## <a name="to-post-a-subcontract-purchase-order"></a>Een uitbestedingsinkooporder boeken  
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Inkooporders** in en klik vervolgens op de gerelateerde koppeling.  
2.  Open een inkooporder die op basis van het uitbestedingsvoorstel is gemaakt.  

    Op de inkooporderregels kunt u dezelfde gegevens zien als die in het voorstel stonden. De velden **Prod.-ordernr.**, **Prod.-orderregelnr.**, **Bewerkingsnr.** en **Afdelingsnr.** worden ingevuld met de informatie van de bronproductieorder.  

3.  Kies de actie **Boeken**.  

Wanneer de inkooporder wordt geboekt als ontvangen, wordt automatisch een output-dagboekpost voor de productieorder geboekt. Dit is alleen van toepassing als de uitbestedingsbewerking de laatste bewerking in het productieorderbewerkingsplan is.  

> [!CAUTION]  
>  De output automatisch boeken voor een voortdurende productieorder wanneer uitbestede artikelen worden ontvangen, is mogelijk niet wenselijk. De redenen voor dit zouden kunnen zijn dat het verwachte outputaantal dat wordt geboekt verschilt van het werkelijke aantal en dat de boekdatum van de automatische output misleidend is.  
>   
>  Om te voorkomen dat de verwachte uitvoer van een productieorder wordt geboekt wanneer de uitbestedingsinkopen worden ontvangen, moet u ervoor zorgen dat de uitbestede bewerking niet de laatste is. Of voeg een nieuwe laatste bewerking voor het laatste outputaantal in.  

Wanneer de inkooporder wordt geboekt als gefactureerd, worden de directe kosten van de inkooporder naar de productieorder geboekt.  

## <a name="see-also"></a>Zie ook  
[Productie](production-manage-manufacturing.md)    
[Productie instellen](production-configure-production-processes.md)  
[Gepland](production-planning.md)      
[Voorraad](inventory-manage-inventory.md)  
[Inkoop](purchasing-manage-purchasing.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


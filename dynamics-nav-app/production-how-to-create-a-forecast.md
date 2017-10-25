---
title: Een productieprognose maken
description: U kunt verkoop- en productieprognoses maken in het venster **Productieprognose**.
documentationcenter: 
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
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 106e75dbe6f1fca00ba09a19eeafb965fa83f4ea
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-a-production-forecast"></a>Procedure: Een productieprognose maken
U kunt verkoop- en productieprognoses maken in het venster **Productieprognose**.  

De prognosefunctionaliteit wordt gebruikt om een verwachte vraag aan te maken; de werkelijke vraag komt voort uit verkoop- en productieorders. Tijdens het opstellen van het MPS (Master Production Schedule) wordt de prognose tot een nettowaarde teruggebracht tegen de verkoop- en productieorders. De optie *Onderdeel* op de prognose bepaalt met welke soort vraag rekening wordt gehouden in het proces van het berekenen van de nettowaarde. Als de prognose wordt uitgevoerd voor een verkoopartikel, worden alleen verkooporders gebruikt tegen de prognose. Als het materialen betreft, wordt alleen afhankelijke vraag van productieordermaterialen gebruikt tegen de prognose.  

Met behulp van prognoses kan uw bedrijf "wat als"-scenario's opstellen en efficiënt en kosteneffectief plannen voor en voorzien in de vraag. Nauwkeurige prognoses kunnen een doorslaggevend verschil maken voor de klanttevredenheid met betrekking tot ordertoezeggingsdatums en tijdige levering.  

## <a name="sales-forecasts-and-production-forecasts"></a>Verkoopprognoses en productieprognoses  
De prognosefunctionaliteit in het programma kan worden gebruikt voor het maken van verkoop- of productieprognoses, in combinatie of onafhankelijk van elkaar. De meeste bedrijven die op order produceren, houden bijvoorbeeld geen voorraad eindproducten aan, omdat elk artikel op bestelling wordt geproduceerd. Het vooruitlopen op orders (verkoopprognoses) is van essentieel belang voor een redelijke doorlooptijd van eindproducten (productieprognoses). Zo kunnen bijvoorbeeld onderdelen met een lange levertijd de productie vertragen als deze niet besteld of in voorraad zijn.  

-   De verkoopprognose is de beste schatting die de verkoopafdeling kan maken over toekomstige verkopen, en deze wordt gespecificeerd per artikel en per periode. De verkoopprognose is echter niet altijd voldoende voor de productie.  
-   De productieprognose is de inschatting van de productieplanner van het aantal eindartikelen en afgeleide subassemblageartikelen in specifieke perioden moeten worden geproduceerd om te voldoen aan de voorspelde verkopen.  

In de meeste gevallen wijzigt dus de productieplanner de verkoopprognose zodat deze past bij de productieomstandigheden, terwijl toch aan de verkoopprognose wordt voldaan.  

U kunt handmatig prognoses maken in het venster **Productieprognose**. Er kunnen in het systeem meerdere prognoses bestaan, die aan de hand van de naam en de soort van elkaar worden onderscheiden. Prognoses kunnen desgewenst worden gekopieerd en bewerkt. Het is wel zo dat op elk moment slechts één prognose geldig kan zijn voor planningsdoeleinden.  

De prognose bestaat uit een aantal records, die elk het artikelnummer, de prognosedatum en het prognoseaantal bevatten. De prognose van een artikel bestrijkt een periode, die wordt bepaald door de prognosedatum en de prognosedatum van de volgende (latere) prognoserecord. Vanuit het oogpunt van planning moet het prognoseaantal beschikbaar zijn bij aanvang van de vraagperiode.  

Een prognose moet worden aangeduid als *Verkoopartikel*, *Materiaal* of *Beide*. De prognosesoort *Verkoopartikel* wordt gebruikt voor verkoopprognoses. De productieprognose wordt gemaakt met behulp van de soort *Onderdeel*. De prognosesoort *Beide* wordt alleen gebruikt om de planner een overzicht te geven van zowel de verkoopprognose als de productieprognose. Bij deze optie kunnen de prognoseposten niet worden bewerkt. Door deze prognosesoorten hier aan te duiden kunt u hetzelfde werkblad gebruiken voor het invoeren van een verkoopprognose als u doet bij een productieprognose, en kunt u hetzelfde blad gebruiken om beide prognoses tegelijkertijd te bekijken. Het is wel zo dat het systeem de verschillende inputs (verkoop en productie) verschillend gebruikt bij het berekenen van de planning, gebaseerd op artikel, productie en productie-instellingen.  

## <a name="component-forecast"></a>Materiaalprognose  
De materiaalprognose kan worden beschouwd als een optieprognose in relatie tot een hoofdartikel. Dit kan bijvoorbeeld nuttig zijn als de planner de vraag naar het materiaal kan schatten.  

Omdat de materiaalprognose is ontworpen om opties te definiëren voor een hoofdartikel, moet de materiaalprognose gelijk aan of kleiner zijn dan het prognoseaantal van het verkoopartikel. Als de materiaalprognose hoger is dan de verkoopartikelprognose, beschouwt het systeem het verschil tussen deze twee soorten prognoses als onafhankelijke vraag.  

## <a name="forecasting-periods"></a>Prognoseperioden  
 De prognoseperiode is geldig vanaf de begindatum tot de datum waarop de volgende prognose begint. Het tijdsintervalvenster biedt u meerdere keuzemogelijkheden om de vraag op en bepaalde datum in een periode in te voegen. Het is daarom raadzaam om het bereik van de prognoseperiode niet te wijzigen, tenzij u alle prognoseposten naar de begindatum van deze periode wilt verplaatsen.  

## <a name="forecast-by-locations"></a>Prognose per locatie  
Dit kan worden geconfigureerd in de productie-instellingen. Het is wel zo dat indien op locatie gebaseerde prognoses los van elkaar worden bekeken, de totale prognose mogelijk niet representatief is.

## <a name="to-create-a-production-forecast"></a>Een productieprognose maken

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Productieprognose** in en klik op de gerelateerde koppeling.  
2.  Selecteer op het sneltabblad **Algemeen** een prognose in het veld **Prod.-prognose**. Meerdere prognoses zijn mogelijk: deze zijn van elkaar te onderscheiden door de naam en het prognosetype.  
3.  Selecteer in het veld **Vestigingsfilter** de vestiging waarop deze prognose van toepassing is.  
4.  Selecteer in het veld **Prognosesoort** **Verkoopartikel**, **Component** of **Beide**. Als u **Verkoopartikel** of **Component** selecteert, kunt u het aantal per periode bewerken. Als u **Beide** selecteert, kunt u het aantal niet bewerken, maar wel de knop met de pijl omlaag kiezen om de posten voor de productieprognose weer te geven.  
5.  Geef een **datumfilter** op als u de hoeveelheid gegevens die wordt weergegeven wilt beperken.  
6.  Op het sneltabblad **Matrix voor productieprognose** kunt u de voorspelde aantallen **Verkoopartikelen** of de **Materiaalprognose** voor de verschillende perioden opgeven.  
7.  Op het sneltabblad **Matrixopties** stelt u het tijdsinterval in het veld **Weergeven per** in, waarmee u de weergegeven periode per kolom kunt wijzigen. U kunt kiezen uit de volgende intervallen: **Dag**, **Week**, **Maand**, **Kwartaal**, **Jaar** of de **Boekingsperiode**, zoals ingesteld in Financieel beheer.  

    > [!NOTE]  
    >  Bedenk goed welk tijdsinterval u wilt gebruiken voor toekomstige prognoses, zodat u steeds dezelfde tijdsinterval gebruikt. Wanneer u een voorspeld aantal invoert, is dast geldig vanaf de eerste dag van het door u geselecteerde tijdsinterval. Als u bijvoorbeeld een maand selecteert, voert u het voorspelde aantal op de eerste dag van de maand in. Als u een kwartaal selecteert, voert u het voorspelde aantal op de eerste dag van de eerste maand van het kwartaal in.  

8.  Selecteer in het veld **Weergeven als** hoe de voorspelde aantallen voor het tijdsinterval moeten worden weergegeven. Als u **Mutatie** selecteert, wordt de mutatie in het saldo weergegeven voor het tijdsinterval. Als u **Saldo t/m datum** selecteert, wordt in het venster het saldo van de laatste dag van het tijdsinterval weergegeven.  

> [!NOTE]  
>  U kunt ook een bestaande prognose bewerken. Kies in het venster **Matrix voor productieprognose** de actie **Prod.-prognose kopiëren** en vul het venster **Prod.-prognose** met een bestaande prognose. U kunt de aantallen waar nodig wijzigen.  

## <a name="see-also"></a>Zie ook  
[Productie instellen](production-configure-production-processes.md)  
[Productie](production-manage-manufacturing.md)    
[Voorraad](inventory-manage-inventory.md)  
[Inkoop](purchasing-manage-purchasing.md)  
[Ontwerpdetails: Voorzieningsplanning](design-details-supply-planning.md)   
[Aanbevolen procedures instellen: voorraadplanning](setup-best-practices-supply-planning.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


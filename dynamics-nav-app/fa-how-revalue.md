---
title: Vaste activa herwaarderen
description: Leren hoe u de waarde van vaste activa aanpast, nieuwe bedragen vastlegt als waardevermindering of waardevermeerdering en extra aanschafkosten boekt.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 09c3babe38e1ec20f5d695f97df37104a9cc4d35
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-revalue-fixed-assets"></a>Procedure: Vaste activa herwaarderen
De herwaardering van vaste activa kan bestaan uit waardevermeerderingen, waardeverminderingen of algemene waardecorrecties.

Als de waarde van een vast activum is gestegen, boekt u een dagboekregel met een hoger bedrag, een waardevermeerdering, naar het afschrijvingsboek. Het nieuwe bedrag wordt als een waardevermeerdering vastgelegd op basis van de instelling van de boeking van het vaste activum.

Als de waarde van een vast activum is gedaald, boekt u een dagboekregel met een lager bedrag, een waardevermindering naar het afschrijvingsboek. Het nieuwe bedrag wordt als een waardevermindering vastgelegd op basis van de instelling van de boeking van het vaste activum.

Indexering wordt gebruikt om meerdere waarden voor vaste activa aan te passen op basis van algemene prijswijzigingen. Met de batchverwerking **Vaste activa indexeren** kunt u diverse bedragen wijzigen, zoals waardeverminderingsbedragen en waardevermeerderingsbedragen.

## <a name="to-post-an-appreciation-from-the-fixed-asset-gl-journal"></a>Een waardevermeerdering boeken vanuit het financieel dagboek voor vaste activa
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **VA-fin. dagboeken** in en klik vervolgens op de gerelateerde koppeling.  
2. Maak een eerste dagboekregel en vul de velden indien nodig in.
3. In het veld **VA-boekingssoort** selecteert u **Herwaardering**.
4. Kies de actie **VA-tegenrekening invoegen**. Er wordt een tweede dagboekregel gemaakt voor de tegenrekening die voor de boeking van de waardevermeerdering is ingesteld.

    > [!NOTE]  
>   Stap 4 werkt alleen als u het volgende hebt ingesteld: in het venster **VA-boekingsgroep** voor de boekingsgroep van het vaste activum bevat het veld **Waardevermeerderingsrekening** de gootboekdebetrekening en het veld **Tegenrekening waardevermeerdering** bevat de grootboekrekening waarnaar u tegenrekeningsposten voor waardevermeerdering wilt boeken. Zie het gedeelte "Boekingsgroepen voor vaste activa instellen" in de [Procedure: Algemene gegevens voor vaste activa instellen](fa-how-setup-general.md) voor meer informatie.  
5. Kies de actie **Boeken**.

## <a name="to-post-a-write-down-from-the-fixed-asset-gl-journal"></a>Een waardevermindering boeken vanuit het financieel dagboek voor vaste activa
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **VA-fin. dagboeken** in en klik vervolgens op de gerelateerde koppeling.  
2. Maak een eerste dagboekregel en vul de velden indien nodig in.
3. In het veld **VA-boekingssoort** selecteert u **Waardevermindering**.
4. Kies de actie **VA-tegenrekening invoegen**. Er wordt een tweede dagboekregel gemaakt voor de tegenrekening die voor de boeking van de waardevermindering is ingesteld.

    > [!NOTE]  
>   Stap 4 werkt alleen als u het volgende hebt ingesteld: in het venster **VA-boekingsgroep** voor de boekingsgroep van het vaste activum bevat het veld **Waardeverminderingsrekening** de grootboekrekening en het veld **Waardeverminderingskostenrekening** bevat de grootboekdebetrekening waarnaar u tegenrekeningsposten voor waardeverminderingen wilt boeken. Zie het gedeelte "Boekingsgroepen voor vaste activa instellen" in de [Procedure: Algemene gegevens voor vaste activa instellen](fa-how-setup-general.md) voor meer informatie.
5. Kies de actie **Boeken**.

## <a name="to-perform-general-revaluation-of-fixed-assets"></a>Algemene herwaardering van vaste activa uitvoeren
Indexering wordt gebruikt om meerdere waarden voor vaste activa aan te passen op basis van algemene prijswijzigingen. Met de batchverwerking **Vaste activa indexeren** kunt u diverse bedragen wijzigen, zoals waardeverminderingsbedragen en waardevermeerderingsbedragen. Het selectievakje **Indexering toegestaan** in het venster **Afschrijvingsboek** moet zijn ingeschakeld.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Vast activum indexeren** in en klik vervolgens op de gerelateerde koppeling.  
2. Vul indien nodig de velden in.
3. Kies de knop **Ok**.

    De herwaardering regels worden gemaakt op basis van uw instellingen in stap 2. De regels worden gemaakt in het dagboek voor vaste activa of het financieel dagboek voor vaste activa, afhankelijk van uw sjabloon en batchinstellingen in het venster **VA-dagboekinstellingen**. Zie [Procedure: Algemene gegevens voor vaste activa instellen](fa-how-setup-general.md) voor meer informatie.
4. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **VA-fin. dagboeken** in en klik vervolgens op de gerelateerde koppeling.  
5. Selecteer het dagboek met de vaste activa die u wilt herwaarderen en kies vervolgens de actie **Posten**.  
6. Controleer de gemaakte posten en kies vervolgens de actie **Boeken** om het dagboek te boeken.

    > [!TIP]  
>   Als de indexcijfers alleen voor simulaties worden gebruikt, kunt u een speciaal afschrijvingsboek maken om ze in op te slaan. Deze posten zijn dan niet van invloed op de andere afschrijvingsboeken.

   ## <a name="to-post-additional-acquisition-costs"></a>Aanvullende aanschafkosten boeken
   U boekt extra aanschafkosten voor een vast activum op dezelfde manier als u de oorspronkelijke aanschafkosten boekt: vanaf een inkoopfactuur of vanuit een dagboek voor vaste activa. Zie [Procedure: Vaste activa aanschaffen](fa-how-acquire.md) voor meer informatie.  

Als de afschrijving al is berekend voor het vaste activum, schakelt u het selectievakje **Afschrijving aanschafkosten** in om de extra aanschafkosten af te schrijven, verminderd met de restwaarde. Dit bedrag is evenredig aan het bedrag dat al op het eerder aangeschafte vaste activum is afgeschreven. Hiermee wordt ervoor gezorgd dat de afschrijvingsperiode niet wordt gewijzigd.  

Het afschrijvingspercentage wordt als volgt berekend:  

*P = (totale afschrijving x 100) / afschrijvingsbasis*

*Afschrijvingsbedrag = (P/100) x (extra aanschafkosten - restwaarde)*  

Vergeet niet om het selectievakje **Afschrijving tot VA-boekingsdatum** in te schakelen op de factuur en het financieel dagboek voor vaste activa of de dagboekregels voor vaste activa te selecteren om ervoor te zorgen dat de afschrijving wordt berekend vanaf de laatste boekingsdatum voor vaste activa tot de boekingsdatum van de aanvullende aanschafkosten.

### <a name="example---posting-additional-acquisition-costs"></a>Voorbeeld - aanvullende aanschafkosten boeken
Een machine is aangeschaft op 1 augustus 2000. De aanschafkosten bedragen LV 4.800. De afschrijvingsmethode is lineair over vier jaar.

Op 31 augustus 2000 wordt de batchverwerking **Afschrijving berekenen** uitgevoerd. De afschrijving wordt berekend als:

*boekwaarde x aantal afschrijvingsdagen/totaal aantal afschrijvingsdagen = 4800 x 30 / 1440 = 100*  

Op 15 september 2000 wordt een factuur geboekt voor het schilderen van de machine. Het factuurbedrag is LV 480.

Als u het selectievakje **Afschrijving tot VA-boekingsdatum** op de factuur hebt ingeschakeld voordat u deze boekt, wordt de volgende berekening gemaakt:  

15 afschrijvingsdagen (09-01-00 t/m 09-15-00) worden berekend als:

*boekwaarde x aantal afschrijvingsdagen/resterend aantal afschrijvingsdagen = (4800 - 100) x 15 / 1410 = 50*

Als u het selectievakje **Afschrijving aanschafkosten** op de factuur hebt ingeschakeld voordat u deze boekt, wordt de volgende berekening gemaakt:  

*De extra aanschafkosten worden afgeschreven met ((150 x 100) / 4800) / 100 x 480 = 15*

De afschrijvingsbasis is nu *5280 = (4800 + 480)* en de gecumuleerde afschrijving is *165 = (100 + 50 + 15)*, wat overeenkomt met 45 afschrijvingsdagen van de totale aanschafkosten. Dit betekent dat het activum volledig wordt afgeschreven binnen de verwachte levensduur van vier jaar.  

Als de batchverwerking **Afschrijving berekenen** wordt uitgevoerd op 30-09-0, wordt de volgende berekening gemaakt:  

*Resterende afschrijfbare levensduur is 3 jaar, 10 maanden en 15 dagen = 1395 dagen*  

*Boekwaarde is (5.280 - 165) = LV 5115*  

*Afschrijvingsbedrag voor september 2000: 5115 x 15 / 1395 = 55,00*  

*Totale afschrijving = 165 + 55 = 220*  

Als u het selectievakje **Afschrijving tot VA-boekingsdatum** niet hebt ingeschakeld, verliest het activum 15 afschrijvingsdagen omdat de batchverwerking **Afschrijving berekenen** die op 30-09-00 is uitgevoerd, de afschrijving berekent vanaf 15-09-00 t/m 30-09-00. Als de batchverwerking **Afschrijving berekenen** op 30-09-00 wordt uitgevoerd, is de berekening dus als volgt:  

*Resterende levensduur is 3 jaar, 10 maanden en 15 dagen = 1395 dagen*  

*Boekwaarde is (4.800 + 480 - 100 - 15) = LV 5165*

*Afschrijvingsbedrag voor september 2000: 5165 x 15 / 1395 = 55,54*  

*Totale afschrijving = 100 +15 + 55,54 = 170,54*

## <a name="see-also"></a>Zie ook
[Vaste activa](fa-manage.md)  
[Vaste activa instellen](fa-setup.md)  
[Financiën](finance.md)  
[Welkom bij [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


---
title: Artikelkosten handmatig herwaarderen
description: U kunt de voorraadwaarde van een artikel herwaarderen met de waarderingsmethoden FIFO of Gemiddeld, bijvoorbeeld als de kosten van een artikel veranderen om andere redenen dan transacties.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cost adjustment, cost forwarding, costing method, inventory valuation, costing
ms.date: 08/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 40647e0263b7c21c1f085cd6dde449f8210ede10
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-adjust-item-costs"></a>Procedure: Artikelkosten herwaarderen
De kostprijs van een artikel (voorraadwaarde) dat u inkoopt en later verkoopt, kan tijdens de levensduur veranderen, bijvoorbeeld omdat vrachtkosten worden toegevoegd aan aanschafkosten nadat u het artikel hebt verkocht. Kostenherwaardering is met name belangrijk als u goederen verkoopt voordat u de inkoop van deze goederen factureert. Als u altijd de juiste voorraadwaarde wilt weten, moeten artikelkosten daarom regelmatig worden geherwaardeerd. Hierdoor worden verkoop- en winststatistieken bijgewerkt en gezorgd dat de financiële KPI's kloppen. Zie [Ontwerpdetails: kostenwaardering](design-details-cost-adjustment.md) voor meer informatie.

Voor artikelen met de waarderingsmethode Vast wordt de waarde in het veld **Kostprijs** op de artikelkaart doorgaans gebaseerd op de vaste verrekenprijs. Voor artikelen met alle andere waarderingsmethoden is de waarde gebaseerd op de berekening van de beschikbare voorraad (gefactureerde kosten en verwachte kosten) gedeeld door het aantal in voorraad. Zie het gedeelte "Kostprijsberekening" voor meer informatie.

In [!INCLUDE[d365fin](includes/d365fin_md.md)] worden artikelkosten automatisch aangepast steeds wanneer een voorraadtransactie plaatsvindt, zoals bij het boeken van een inkoopfactuur voor een artikel.

U kunt een functie ook gebruiken om de kosten van een of meer artikelen handmatig aan te passen. Dit is bijvoorbeeld handig als u weet dat artikelkosten om andere redenen dan artikeltransacties zijn gewijzigd.

Artikelkosten worden geherwaardeerd met de waarderingsmethode FIFO of Gemiddeld, afhankelijk van uw keuze in de begeleide instelling **Mijn bedrijf instellen** of in het veld **Waarderingsmethode** op de artikelkaart. Zie [Procedure: Nieuwe artikelen registreren](inventory-how-register-new-items.md) voor meer informatie.  

Als u de waarderingsmethode FIFO gebruikt, zijn de eenheidskosten van een artikel de werkelijke waarde van een ontvangst van het artikel. Voorraad wordt gewaardeerd met de aanname dat de eerste in voorraad geplaatste artikelen het eerst worden verkocht.

Als u de waarderingsmethode Gemiddeld gebruikt, worden de eenheidskosten van een artikel berekend als de gemiddelde eenheidskosten op een bepaald moment na een aanschaf. Voorraad wordt gewaardeerd met de aanname dat alle voorraad tegelijkertijd wordt verkocht. Voor artikelen die gebruik maken van deze waarderingsmethode kunt u op de artikelkaart het veld **Kostprijs** kiezen en zo de historie bekijken van de transacties waaruit de gemiddelde kostprijs wordt berekend.

De kostenherwaardering verwerkt alleen posten die nog niet zijn geherwaardeerd. Als de functie een post aantreft waarbij gewijzigde inkomende kosten moeten worden doorgeschoven naar de bijbehorende uitgaande posten, worden nieuwe waardeposten gemaakt. Deze posten zijn op de gegevens van de oorspronkelijke waardeposten gebaseerd, maar bevatten het geherwaardeerde bedrag. De kostenherwaarderingsfunctie gebruikt de boekingsdatum van de oorspronkelijke waardepost in de herwaarderingspost, tenzij die datum in een afgesloten voorraadperiode valt. In dat geval wordt de begindatum van de volgende open voorraadperiode gehanteerd. Als de voorraadperioden niet worden gebruikt, bepaalt de datum in het veld **Boeken toegest. vanaf** in het venster **Boekhoudinstellingen** wanneer de herwaarderingspost wordt geboekt.

## <a name="to-adjust-item-costs-manually"></a>Artikelkosten handmatig herwaarderen
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Kostprijs herwaarderen - Artikelposten** in en klik vervolgens op de gerelateerde koppeling.
2. Geef in het venster **Kostprijs herwaarderen - Artikelposten** op voor welke artikelen kosten moeten worden aangepast.
3. Kies de knop **OK**.

## <a name="to-make-general-changes-in-the-direct-unit-cost"></a>Ga als volgt te werk om algemene wijzigingen aan te brengen in de directe kostprijs:
Als u de directe kostprijs voor een aantal artikelen moet wijzigen, kunt u de batchverwerking **Artikelprijzen herwaarderen** gebruiken.  

 De batchverwerking past de inhoud aan van het veld **Eenheidsprijs** op de artikelkaart. Dit veld wordt gewijzigd voor alle artikelen of voor geselecteerde artikelen. De batchverwerking vermenigvuldigt de waarde in het veld met een aanpassingsfactor die u opgeeft.  

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Artikelprijzen herwaarderen** in en klik vervolgens op de gerelateerde koppeling.  
2. Geef in het veld **Aan te passen prijs** op welk artikel- of SKU-kaartveld u wilt aanpassen.  
3. Geef in het veld **Herwaarderingsfactor** de factor op waarmee de waarde wordt aangepast. Voer bijvoorbeeld **1.5** in om de waarde met 50% te verhogen.  
4. Stel op het sneltabblad **Artikel** filters in om, bijvoorbeeld, op te geven welke artikelen moeten worden verwerkt met de batchverwerking.  
5. Kies de knop **OK**.  

## <a name="understanding-unit-cost-calculation"></a>Kostprijsberekening
Voor artikelen met de waarderingsmethode Vast wordt de waarde in het veld **Kostprijs** op de artikelkaart doorgaans gebaseerd op de vaste verrekenprijs. Voor artikelen met alle andere waarderingsmethoden is de waarde gebaseerd op de berekening van de beschikbare voorraad (gefactureerde kosten en verwachte kosten) gedeeld door het aantal in voorraad.  

 In de volgende gedeelten wordt beschreven hoe de inhoud van het veld **Waarderingsmethode** van invloed is op de kostprijsberekening voor in- en verkoop.  

## <a name="unit-cost-calculation-for-purchases"></a>Kostprijsberekening voor inkoop  
 Wanneer u artikelen inkoopt, wordt de waarde in het veld **Laatste directe kosten** op de artikelkaart naar het veld **Directe kostprijs** op een inkoopregel of het veld Eenheidsprijs op een artikeldagboekregel gekopieerd.  

 Wat u in het veld **Waarderingsmethode** invult, beïnvloedt hoe [!INCLUDE[d365fin](includes/d365fin_md.md)] de inhoud van het veld **Kostprijs** berekent op de regels.  

### <a name="costing-method-fifo-lifo-specific-or-average"></a>Waarderingsmethode FIFO, LIFO, Specifiek of Gemiddeld  
 De inhoud van het veld **Kostprijs (LV)** op de inkoopregel of het veld **Kostprijs** op de artikeldagboekregel wordt door [!INCLUDE[d365fin](includes/d365fin_md.md)] berekend volgens deze formule:  

 Kostprijs (LV) = (Directe kostprijs - (Totale korting/ Aantal)) * (1 + Indirecte kosten % / 100) + Overheadtarief  

### <a name="costing-method-standard"></a>Waarderingsmethode Vast  
 De waarde in het veld **Kostprijs** op de artikelkaart wordt naar het veld **Kostprijs (LV)** op de inkoopregel of het veld **Kostprijs** op de artikeldagboekregel gekopieerd. Wanneer de waarderingsmethode Vast is ingesteld, is deze altijd gebaseerd op de vaste verrekenprijs.  

 Wanneer u de inkoop boekt, wordt de kostprijs uit de inkoopregel of de artikeldagboekregel gekopieerd naar de inkoopfactuurpost en weergegeven in het overzicht met de posten voor het artikel.  

### <a name="all-costing-methods"></a>Alle waarderingsmethoden  
 De inhoud van het veld **Tot. werk. kosten** of, indien van toepassing, het veld **Tot. verw. kosten** voor deze artikelpost wordt altijd berekend op basis van de kostprijs van de brondocumentregel, ongeacht de waarderingsmethode van het artikel.  

## <a name="unit-cost-calculation-for-sales"></a>Kostprijsberekening voor verkoop  
 Wanneer u artikelen verkoopt, wordt de kostprijs altijd uit het veld Kostprijs op de artikelkaart naar de verkoopregel of de artikeldagboekregel gekopieerd.  

 Tijdens het boeken wordt de kostprijs naar de verkoopfactuurpost gekopieerd en weergegeven in het overzicht met artikelposten. De inhoud van het veld **Tot. werk. kosten** of indien van toepassing het veld **Tot. verw. kosten** in de waardepost voor deze artikelpost wordt door [!INCLUDE[d365fin](includes/d365fin_md.md)] berekend op basis van de kostprijs van de brondocumentregel.  

## <a name="see-also"></a>Zie ook
[Voorraadkosten beheren](finance-manage-inventory-costs.md)  
[Voorraad](inventory-manage-inventory.md)  
[Verkoop](sales-manage-sales.md)  
[Inkoop](purchasing-manage-purchasing.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


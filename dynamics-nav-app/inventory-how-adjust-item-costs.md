---
title: 'Procedure: Artikelkosten herwaarderen'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 59db38c159dd2810656edc668ee431c6414b9d90
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-adjust-item-costs"></a>Procedure: Artikelkosten herwaarderen   
De kostprijs van een artikel (voorraadwaarde) dat u inkoopt en later verkoopt, kan tijdens de levensduur veranderen, bijvoorbeeld omdat vrachtkosten worden toegevoegd aan aanschafkosten nadat u het artikel hebt verkocht. Als u altijd de juiste voorraadwaarde wilt weten, moeten artikelkosten daarom regelmatig worden geherwaardeerd.
Hierdoor worden verkoop- en winststatistieken bijgewerkt en gezorgd dat de financiële KPI's kloppen.

**Opmerking**: artikelkosten worden alleen aangepast door de waarderingsmethode FIFO. Dit betekent dat de kostprijs van een artikel de werkelijke waarden van de ontvangst van het artikel is, en dat de voorraad wordt gewaardeerd op basis van de aanname dat artikelen die het eerst in voorraad zijn geplaatst, het eerst worden verkocht.

De kostenherwaardering verwerkt alleen posten die nog niet zijn geherwaardeerd. Als de functie een post aantreft waarbij gewijzigde inkomende kosten moeten worden doorgeschoven naar de bijbehorende uitgaande posten, worden nieuwe waardeposten gemaakt. Deze posten zijn op de gegevens van de oorspronkelijke waardeposten gebaseerd, maar bevatten het geherwaardeerde bedrag. De kostenherwaarderingsfunctie gebruikt de boekingsdatum van de oorspronkelijke waardepost in de herwaarderingspost, tenzij die datum in een afgesloten voorraadperiode valt. In dat geval wordt de begindatum van de volgende open voorraadperiode gehanteerd. Als de voorraadperioden niet worden gebruikt, bepaalt de datum in het veld **Boeken toegest. vanaf** in het venster **Boekhoudinstellingen** wanneer de herwaarderingspost wordt geboekt.

**Opmerking**: nadat artikelkosten zijn geherwaardeerd, moet de voorraadwaarde worden geboekt naar het grootboek, automatisch of handmatig. Zie voor meer informatie [Procedure: Voorraadkosten naar het grootboek boeken](inventory-how-post-inventory-cost-gl.md).

U kunt artikelkosten op twee manieren herwaarderen:
 - Automatisch, door het systeem kostenwijzigingen steeds te laten herwaarderen wanneer voorraadtransacties optreden.
 - Handmatig, door de batchverwerking **Kostprijs herwaarderen - Artikelposten** voor een of meer artikelen uit te voeren wanneer u weet dat de kosten ervan zijn gewijzigd.  

## <a name="to-adjust-item-costs-automatically"></a>Artikelkosten automatisch herwaarderen
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Voorraadinstellingen** in en kies vervolgens de gerelateerde koppeling.
2. Selecteer in het venster **Voorraadinstellingen** in het veld **Automatische kostenwaardering** een van de volgende waarden.

|Optie |Effect |
|-------|---------|
|Nooit|De kostprijs wordt niet geherwaardeerd tijdens het boeken.|
|Dag|De kostprijs wordt geherwaardeerd als de boeking binnen één dag vóór de werkdatum plaatsvindt.|
|Week|De kostprijs wordt geherwaardeerd als de boeking binnen een week vóór de werkdatum plaatsvindt.|
|Maand|De kostprijs wordt geherwaardeerd als de boeking binnen een maand vóór de werkdatum plaatsvindt.|
|Kwartaal|De kostprijs wordt geherwaardeerd als de boeking binnen een kwartaal vóór de werkdatum plaatsvindt.|
|Jaar|De kostprijs wordt geherwaardeerd als de boeking binnen een jaar vóór de werkdatum plaatsvindt.|
|Altijd|De kostprijs wordt altijd geherwaardeerd tijdens het boeken, ongeacht de boekingsdatum.|

## <a name="to-adjust-item-costs-manually"></a>Artikelkosten handmatig herwaarderen
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Kostprijs herwaarderen - Artikelposten** in en kies vervolgens de gerelateerde koppeling.
2. Geef in het venster **Kostprijs herwaarderen - Artikelposten** op voor welke artikelen kosten moeten worden geherwaardeerd en of de geherwaardeerde tegelijkertijd naar het grootboek worden geboekt.

## <a name="see-also"></a>Zie ook
[Voorraad beheren](inventory-manage-inventory.md)  
[Procedure: voorraadkosten naar het grootboek boeken](inventory-how-post-inventory-cost-gl.md)  
[Verkoop beheren](sales-manage-sales.md)  
[Inkoop beheren](purchasing-manage-purchasing.md)


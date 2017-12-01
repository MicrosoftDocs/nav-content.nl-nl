---
title: 'Procedure: voorraadkosten naar het grootboek boeken'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 34eec596392e9316e807d3c073c3b8e59dbc12e9
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---

# <a name="how-to-post-inventory-costs-to-the-general-ledger"></a>Procedure: voorraadkosten naar het grootboek boeken   
Als u voorraadtransacties (bijvoorbeeld verkoopverzendingen, inkoopfacturen of voorraadherwaarderingen) boekt, worden de gewijzigde aantallen en kosten vastgelegd in respectievelijk de artikel- en waardeposten. Als u deze wijziging van voorraadwaarde wilt doorvoeren in uw financiële boeken, moet u voorraadkosten boeken naar de gerelateerde voorraadrekeningen in het grootboek.

U kunt voorraadkosten op twee manieren boeken naar het grootboek:

- Automatisch, zodat voorraadkosten worden geboekt naar het grootboek, elke keer dat u een voorraadtransactie boekt.
- Handmatig, zodat voorraadkosten alleen naar het grootboek worden geboekt wanneer u een batchverwerking uitvoert.


## <a name="to-post-inventory-costs-automatically"></a>Voorraadkosten automatisch boeken
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Voorraadinstellingen** in en kies vervolgens de gerelateerde koppeling.
2. Schakel in het venster **Voorraadinstellingen** het selectievakje **Autom. voorraadwaarde boeken** in.

Voor iedere voorraadtransactie die u boekt, worden overeenkomende waarden naar de voorraadrekening geboekt, de correctierekening en de KPV-rekening in het grootboek.

Ook als u automatisch kosten boekt, dient u regelmatig de batchverwerking Kostprijs herwaarderen - Artikelposten uit te voeren, om er zeker van te zijn dat de kosten van goederen worden doorgestuurd naar de juiste uitgaande transacties, zoals verkopen of transfers. Dit is vooral belangrijk als u goederen verkoopt voordat u de inkoop van deze goederen factureert.

Als zich tijdens het boeken van de voorraadkosten naar het grootboek een fout voordoet in de dimensie-instellingen, eindigt de boeking met een fout.

## <a name="to-post-inventory-costs-manually"></a>Voorraadkosten handmatig boeken
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Voorraadwaarde boeken** in en kies vervolgens de gerelateerde koppeling.
2. Voorraadkosten handmatig naar het grootboek boeken door de batchverwerking. Als u deze batchverwerking uitvoert, worden grootboekposten op basis van de waardeposten gemaakt. U kunt de posten boeken, zodat deze per boekingsgroep worden samengevat.

**Opmerking**: wanneer u deze batchverwerking uitvoert, is het mogelijk dat er fouten worden aangetroffen met betrekking tot ontbrekende instellingen of incompatibele dimensie-instellingen. Als de batchverwerking fouten aantreft in de dimensie-instellingen, worden deze fouten overschreven en worden de dimensies van de waardepost gebruikt. De batchverwerking slaat de waardeposten van alle andere fouten over en vermeldt deze aan het einde van de lijst in een aparte sectie genaamd “Overgeslagen posten”. U dient de fouten te corrigeren om deze posten te kunnen boeken.

Als u een lijst met de fouten wilt weergeven voordat u de boekingsbatchverwerking uitvoert, kunt u het rapport **Voorraadkosten naar GB boeken - Controle** uitvoeren. In de controlelijst worden alle fouten vermeld die tijdens een controleboeking zijn gevonden. U kunt deze fouten dan corrigeren en de batchverwerking voor het boeken van voorraadkosten uitvoeren zonder posten over te slaan.

Als u een overzicht wilt zien van de waarden die naar het grootboek kunnen worden geboekt zonder de boeking daadwerkelijk uit te voeren, voert u de batchverwerking Voorraadwaarde boeken uit. U doet dit door het selectievakje Boeken in het aanvraagvenster uit te schakelen. Wanneer u de batchverwerking dan uitvoert, wordt alleen een lijst gemaakt met de waarden die klaar zijn om naar het grootboek te worden geboekt. Deze worden echter niet geboekt.

## <a name="see-also"></a>Zie ook
[Voorraad beheren](inventory-manage-inventory.md)    
[Procedure: Artikelkosten herwaarderen](inventory-how-adjust-item-costs.md)  
[Verkoop beheren](sales-manage-sales.md)  
[Inkoop beheren](purchasing-manage-purchasing.md)


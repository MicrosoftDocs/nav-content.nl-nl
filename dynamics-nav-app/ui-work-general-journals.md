---
title: Werken met diversendagboeken
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 2dc2b22fbc0ff70addd16ca14e8c5416c49915e7
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="work-with-general-journals"></a>Werken met diversendagboeken
Met diversendagboeken kunt u financiële transacties naar grootboekrekeningen en andere rekeningen boeken, zoals bank-, klant- en leveranciersrekeningen. Door te boeken met een dagboek worden er altijd posten gemaakt in grootboekrekeningen. Dit geldt zelfs ook als u bijvoorbeeld een dagboekregel naar een klantrekening boekt, omdat een post via een boekingsgroep is geboekt naar een rekening met vorderingen in het grootboek.

De informatie die u invoert in een dagboek is tijdelijk en kan in het dagboek worden gewijzigd. Wanneer u het dagboek boekt, wordt de informatie overgedragen naar de posten van afzonderlijke rekeningen, waar de informatie niet meer kan worden gewijzigd. U kunt echter de vereffening van geboekte posten ongedaan maken en u kunt tegenboekingen of corrigerende boekingen maken.

## <a name="journal-templates-and-batches"></a>Dagboeksjablonen en -batches
Er zijn verschillende sjablonen voor diversendagboeken. Elk dagboeksjabloon wordt vertegenwoordigd door een speciaal venster met specifieke functies en de velden die nodig zijn om die functies te ondersteunen, zoals het venster **Dagboek betalingsreconciliatie**, om bankbetalingen te verwerken en het venster **Betalingsdagboek** om uw leveranciers te betalen.

Voor elke dagboeksjabloon kunt u uw eigen persoonlijke dagboek instellen als een dagboekbatch. U kunt bijvoorbeeld uw eigen dagboekbatch definiëren voor het betalingsdagboek dat uw persoonlijke lay-out en instellingen heeft.

**Opmerking**: een voorbeeld van een persoonlijke instelling die u in uw diversendagboekbatch kunt definiëren, is dat u het systeem kunt laten helpen om bedragvelden in te vullen. Als u het selectievakje **Salderingsbedrag voorstellen** inschakelt op de regel voor uw batch in het venster **Fin. dagboekbatches**, wordt het veld **Bedrag** op bijvoorbeeld diversendagboekregels voor hetzelfde documentnummer automatisch vooraf ingevuld met de waarde die is vereist om het document sluitend te maken. Zie [Dynamics NAV waarden laten voorstellen](ui-let-system-suggest-values.md) voor meer informatie.

## <a name="main-accounts-and-balancing-accounts"></a>Hoofdrekeningen en tegenrekeningen
Als u standaardtegenrekeningen hebt ingesteld voor de dagboekbatches, wordt de tegenrekening automatisch ingevuld wanneer u **Rekeningnr.** invult. in. Vul anders zowel het veld **Rekeningnr.** als het veld **Tegenrekeningnr.** handmatig in. Een positief bedrag in het veld **Bedrag** wordt gedebiteerd van de hoofdrekening en gecrediteerd naar de tegenrekening. Een negatief bedrag wordt gecrediteerd naar de hoofdrekening en gedebiteerd van de tegenrekening.

**Opmerking**: btw wordt afzonderlijk berekend voor de hoofdrekening en de tegenrekening, zodat er gebruik kan worden gemaakt van verschillende percentages.

## <a name="recurring-journals"></a>Periodieke dagboeken
Een periodiek dagboek is een dagboek met specifieke velden voor het beheer van transacties die u regelmatig boekt met weinig of geen wijzigingen. Met de speciale velden voor periodieke transacties kunt u zowel vaste als variabele bedragen boeken. U kunt ook automatische tegenboekingsposten specificeren op de dag na de boekingsdatum en toewijzingssleutels gebruiken voor de periodieke transacties.

## <a name="see-also"></a>Zie ook
[Procedure: verdeelsleutels in dagboeken gebruiken](ui-how-use-allocation-keys-general-journals.md)  
[Financiën](finance-setup.md)  
[Werken met Dynamics NAV](ui-work-product.md)


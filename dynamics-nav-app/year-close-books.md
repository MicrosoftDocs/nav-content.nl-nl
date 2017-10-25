---
title: Overzicht van de taken voor het sluiten van de boeken
description: Meer informatie over het sluiten van de boeken voor een boekjaar of -periode, en wat er gebeurt nadat u het jaareinde hebt afgesloten.
documentationcenter: 
author: jswymer
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: year closing, close accounting period, close fiscal year, bank account detailed trial balance
ms.date: 03/29/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: d709f8bfb5da3a0ebf5b44f3246fa3ccaa69c77f
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="closing-the-books"></a>De boeken sluiten
Nadat gezorgd hebt dat alle rekeningen actueel zijn, en u kosten en inkomsten hebt verdeeld, kunt u de boeken van een boekhoudperiode of boekjaar sluiten.

U bent niet verplicht een jaar af te sluiten, maar maakt het werken in het systeem gemakkelijker omdat u dan kunt profiteren van de handige filteropties. U hoeft zich bovendien geen zorgen te maken over het verlies van transactiedetails wanneer u het jaar afsluit, omdat alle details behouden blijven, zelfs nadat u het jaar hebt afgesloten.

## <a name="closing-book-process"></a>Proces voor het afsluiten van boeken
Bij het proces voor het afsluiten van boeken zijn drie hoofdtaken betrokken:

1. De boekingsperiode afsluiten.

    Een boekjaar wordt gedefinieerd als één of meer open perioden die zijn gedefinieerd in het venster **Boekhoudperioden**. Een boekjaar bestaat over het algemeen uit 12 perioden van een maand, maar u kunt een jaar ook anders definiëren.

    Zie [Procedure: Boekingsperioden afsluiten](year-close-account-periods.md) voor meer informatie.
2. Naboekingen registreren.

    Wanneer u een boekjaar sluit, moet u een aantal administratieve transacties invoeren (zoals vooraf betaalde en te betalen artikelen). De transacties worden herwaarderingsposten genoemd. Er zijn geen speciale regels voor het boeken van deze posten, en het veld **Naboeking** is (zoals bij de overige posten) geselecteerd als ze worden geboekt op een datum in een gesloten boekjaar. Zelfs als een boekjaar is afgesloten, kunt u er nog steeds grootboekposten voor boeken.
3. Saldi van de WenV-rekeningen overboeken naar de balans.

    Nadat een boekjaar is gesloten en alle naboekingen zijn geboekt, moeten de resultatenrekeningen worden gesloten en het netto inkomen van het jaar moet worden overgedragen naar een rekening onder de vermogensrekening van de eigenaren op de balans. Gebruik hiervoor de batchverwerking Afsluiten WenV-rekening. De batchverwerking verwerkt alle grootboekrekeningen van het soort Resultaten en maakt tegenboekingen voor de bijbehorende saldo's. Deze posten worden geplaatst in een dagboek van waar ze kunnen worden geboekt. De batchverwerking boekt ze niet automatisch, behalve wanneer een extra rapportagevaluta wordt gebruikt. Wanneer een extra rapportagevaluta wordt gebruikt, boekt de batchverwerking direct naar het grootboek.

    Zie [Afsluiten WenV-rekening](year-close-income-statement.md) voor meer informatie.
4. Het boeken van de jaareinde-ultimopost samen met de uitstellende vermogensrekeningposten.

    Wanneer de batchverwerking Afsluiten WenV-rekening is voltooid, boekt u de posten die zijn gegenereerd door de batchverwerking. Als u geen rekening Resultaat Lopend Boekjaar heeft gespecificeerd in de batchverwerking, voert u een regel in met een tegenboeking waarmee het netto inkomen wordt geboekt naar de juiste grootboekrekening onder de vermogensrekening van de eigenaren op de balans. Boek ten slotte het dagboek.

    Zie [Procedure: Jaareinde-ultimopost boeken](year-how-post-year-end-close-entry.md) voor meer informatie.

## <a name="what-happens-when-you-close"></a>Wat er gebeurt wanneer u afsluit
Wanneer u het boekjaar aan het einde van het jaar afsluit, verplaatst het systeem uw resultaten van de berekende resultaten. Het systeem markeert tevens het boekjaar als "afgesloten," en markeert alle volgende posten voor het afgesloten jaar als "posten van het vorige jaar."

Het systeem genereert vervolgens een ultimopost, maar boekt de post niet automatisch. U krijgt de gelegenheid de uitstellende vermogensrekeningpost of -posten te maken, zodat u kunt beslissen hoe u uw ultimopost wilt toewijzen. Als een bedrijf bijvoorbeeld verschillende divisies heeft, kunt u in het systeem één ultimopost laten genereren voor alle divisies en kunt u vervolgens een uitstellende post voor de vermogensrekening van elke divisie maken.

U kunt in een eerder boekjaar boeken, zelfs nadat de resultatenrekeningen zijn gesloten, als u nadien nogmaals de batchverwerking Afsluiten WenV-rekening uitvoert.

## <a name="see-also"></a>Zie ook
[Procedure: Nieuw boekjaar openen](finance-how-open-new-fiscal-year.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


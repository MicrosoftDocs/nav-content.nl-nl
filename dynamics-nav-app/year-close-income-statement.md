---
title: Afsluiten WenV-rekening
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 83dfa0db1345aa18d6900470c93ccdc00bd1b403
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---
# <a name="close-income-statement"></a>Afsluiten WenV-rekening
Wanneer een boekjaar is afgelopen, moet u de hierin opgenomen perioden afsluiten. Voer hiervoor de batchverwerking **Afsluiten WenV-rekening** uit. Met deze taak wordt het jaarresultaat overgeboekt naar een rekening op de balans en worden de resultatenrekeningen afgesloten. In een dagboek worden regels gemaakt die u vervolgens kunt boeken.

## <a name="to-run-the-close-income-statement-batch-job"></a>De batchverwerking Afsluiten WenV-rekening uitvoeren
1. Sluit het boekjaar. Het boekjaar moet zijn afgesloten voordat u de batchverwerking kunt uitvoeren. Zie [Procedure: Boekingsperioden afsluiten](year-close-account-periods.md) voor meer informatie.
2. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Afsluiten WenV-rekening** in en kies vervolgens de gerelateerde koppeling.
3. Kies **OK** om de batchverwerking te starten.

## <a name="about-the-close-income-statement-batch-job"></a>Informatie over de batchverwerking Afsluiten WenV-rekening
De batchverwerking verwerkt alle grootboekrekeningen van het soort Resultaten en maakt tegenboekingen voor de bijbehorende saldo's. Dat wil zeggen, dat elke post de som is van alle grootboekposten op de rekening van het boekjaar. Deze nieuwe posten worden geplaatst in een dagboek waarin u een tegenrekening en resultatenrekening in de balans moet opgeven voordat u boekt. Wanneer u het dagboek boekt, wordt een post geboekt in elke resultatenrekening zodat het saldo nul wordt en het jaarresultaat tegelijkertijd wordt overgebracht naar de balans.

U moet het dagboek zelf boeken. De batchverwerking boekt de posten niet automatisch, behalve wanneer een extra rapportagevaluta wordt gebruikt. Wanneer een extra rapportagevaluta wordt gebruikt, boekt de batchverwerking posten direct naar het grootboek.

De datum op de regels die tijdens de batchverwerking in het dagboek worden opgenomen, is altijd een ultimodatum voor het boekjaar. De ultimodatum is een fictieve datum tussen de laatste dag van het oude boekjaar en de eerste dag van het nieuwe jaar. Het voordeel van boeken op een ultimodatum is dat u de juiste saldo's behoudt voor de gewone datums van het boekjaar.

U kunt de batchverwerking **Afsluiten WenV-rekening** meerdere keren gebruiken. Als u de batchverwerking opnieuw uitvoert, kunt ook naar vorige boekjaren boeken, zelfs nadat de WenV-rekeningen zijn afgesloten.

## <a name="see-also"></a>Zie ook
[Boeken sluiten](year-close-books.md)  
[Procedure: de jaareinde-ultimopost boeken](year-how-post-year-end-close-entry.md)  
[Procedure: nieuw boekjaar openen](finance-setup-how-open-new-fiscal-year.md)


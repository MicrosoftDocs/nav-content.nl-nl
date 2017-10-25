---
title: Valutawisselkoersen bijwerken
description: Als u meerdere valuta's in uw bedrijf wilt gebruiken, kunt u een code voor elke gebruikte valuta instellen en een externe wisselkoersservice gebruiken, bijvoorbeeld Yahoo.
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: multiple currencies, Yahoo
ms.date: 07/02/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 50603747629eee61f9bdaed900dcfc0dfc96ab3b
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-update-currency-exchange-rates"></a>Procedure: Valutawisselkoersen bijwerken
U moet een code instellen voor elke gebruikte valuta als u in andere valuta's dan uw lokale valuta inkoopt of verkoopt, in een andere valuta tegoeden of schulden hebt of grootboektransacties in verschillende valuta's vastlegt.  

Aangezien bedrijven steeds vaker in andere landen/regio's opereren, is het belangrijk dat zij de financiën in meer dan één valuta kunnen controleren of rapporteren. In het programma wordt het gebruik van meerdere valuta;s ondersteund. Binnen het programma wordt uw grootboek ingesteld met uw lokale valuta (LV) en wordt een andere valuta ingesteld als een extra valuta, waaraan een huidige wisselkoers wordt toegewezen.  

 Door een tweede valuta in te stellen als een aanvullende rapportagevaluta, slaat [!INCLUDE[d365fin](includes/d365fin_md.md)] automatisch bedragen op in de LV en in deze extra rapportagevaluta bij elke boeking in het grootboek en andere boekingen, zoals btw-boekingen. Wanneer het programma grootboekpostenbedragen berekent in een extra rapportagevaluta, wordt de informatie gebruikt van het venster **Valutawisselkoersen** om de relevante wisselkoers te vinden.  

> [!WARNING]  
>  De functie Extra rapportagevaluta mag NIET worden gebruikt als basis voor de vertaling van een financieel overzicht. Het is geen programma dat een vertaling kan uitvoeren van financiële overzichten van buitenlandse dochterondernemingen als onderdeel van een bedrijfsconsolidatie. De extra rapportagevalutafunctie biedt alleen de optie om rapporten in een andere valuta voor te bereiden, alsof die valuta de lokale valuta van het bedrijf was.

## <a name="adjusting-exchange-rates"></a>Wisselkoersen corrigeren  
Aangezien valutakoersen constant wisselen, moeten de extra valuta-equivalenten in uw systeem periodiek worden gecorrigeerd. Als deze correcties niet worden uitgevoerd, kunnen de bedragen die omgerekend zijn van vreemde (of extra) valuta's en geboekt zijn in het grootboek in LV misleidend zijn. Bovendien moeten dagelijkse posten die geboekt zijn doordat een dagwisselkoers is ingevoerd in het programma worden bijgewerkt nadat de dagwisselkoersgegevens zijn ingevoerd. De batchverwerking Wisselkoers herwaarderen wordt gebruikt om de wisselkoersen van de geboekte klant, leverancier en bankrekeningposten te corrigeren. U kunt er tevens extra rapportagevalutabedragen in grootboekposten mee bijwerken.  

## <a name="displaying-reports-and-amounts-in-the-additional-reporting-currency"></a>Rapporten en bedragen weergeven in de extra rapportagevaluta  
Het gebruik van een extra rapportagevaluta kan in de volgende gevallen hulp bieden bij het rapportageproces voor een bedrijf:  

- Bedrijven in landen/regio's die niet bij de EU horen en die grote hoeveelheden transacties aangaan met bedrijven in EU-landen/regio's. In dit geval wil het bedrijf buiten de EU mogelijk tevens in euro rapporteren om de financiële rapporten beter bruikbaar te maken voor haar handelspartners in de EU.  

- Bedrijven die tevens rapporten in een internationale handelsvaluta in plaats van hun eigen lokale valuta willen weergeven.  

Verschillende rapporten in de module Financieel zijn gebaseerd op grootboekposten. Als u de financiële gegevens in de lijst in de extra rapportagevaluta wilt weergeven, plaatst u eenvoudigweg een vinkje in het veld **Bedragen in rapp.-valuta weergeven** in het betreffende grootboeklijstvenster.  

## <a name="to-set-up-a-currency-exchange-rate-service"></a>Een wisselkoersservice instellen
U kunt een externe service gebruiken om valutawisselkoersen actueel te houden. De Yahoo Currency Exchange Rates-service is vooraf geïnstalleerd en kan worden ingeschakeld.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Valutawisselkoersservices** in en klik vervolgens op de gerelateerde koppeling.
2. Kies de actie **Nieuw**.
3. Vul in het venster **Valutawisselkoersservice** indien nodig de velden in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Kies het selectievakje **Ingeschakeld** om de service in te schakelen.

## <a name="to-update-currency-exchange-rates-through-a-service"></a>Valutawisselkoersen bijwerken met een service
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Valuta's** in en klik vervolgens op de gerelateerde koppeling.
2. Kies de actie **Wisselkoersen bijwerken**.

De waarde in het veld **Wisselkoers** in het venster **Valuta´s** wordt bijgewerkt met de laatste wisselkoers.

## <a name="see-also"></a>Zie ook
[Afsluitingsjaren en -perioden](year-close-years-periods.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


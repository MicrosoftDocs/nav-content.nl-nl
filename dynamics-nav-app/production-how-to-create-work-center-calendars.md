---
title: Vakantieagenda's instellen
description: "Op een afdelingsagenda staan de werkdagen en -tijden, de diensten, vakanties en afwezigheid genoteerd die bepalend zijn voor de brutocapaciteit. gemeten in tijd, van de afdeling op basis van de gedefinieerde efficiëntie en capaciteitswaarden. Voordat er een afdelingsagenda kan worden gemaakt, moet diverse voorbereidingen worden getroffen:"
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/14/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 59131cdded4bf854aed02a7d835e8160342adb36
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-shop-calendars"></a>Procedure: vakantieagenda's instellen
Een afdelings- of bewerkingsplaatsagenda bevat de werkdagen en -tijden, de diensten, vakanties en afwezigheid die bepalend zijn voor de brutocapaciteit, gemeten in tijd, van de afdeling op basis van de gedefinieerde efficiëntie- en capaciteitswaarden.

Voordat een bepaalde afdelings- of bewerkingsplaatsagenda kan worden berekend, moeten er eerst een of meer algemene productieagenda's worden ingesteld. In een productieagenda wordt een standaardwerkweek gedefinieerd in termen van begin- en eindtijden van een werkdag en de ploegen die er werkzaam zijn. Bovendien zijn in een productieagenda de vastgestelde vakantiedagen gedurende het jaar opgenomen.  

Hier wordt beschreven hoe u afdelingsagenda's instelt. Voor het instellen van bewerkingsplaatsagenda's zijn de stappen vergelijkbaar.  

## <a name="to-create-work-shifts"></a>Ploegen maken  
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Ploegen** in en klik op de gerelateerde koppeling.  
2.  Geef op een lege regel in het veld **Code** een nummer op om de ploeg aan te duiden, bijvoorbeeld **1**.  
3.  Geef een omschrijving voor de ploeg in het veld **Omschrijving**, bijvoorbeeld **Vroege ploeg**.  
4.  Vul eventueel regels voor een tweede of derde ploeg in.  

Ook als de afdeling niet met ploegen werkt, moet er toch minstens één ploegcode worden opgegeven.  

## <a name="to-set-up-a-shop-calendar"></a>Een productieagenda instellen  
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Productieagenda's** in en klik op de gerelateerde koppeling.  
2.  Geef op een lege regel in het veld **Code** een nummer op ter aanduiding van de productieagenda.  
3.  Beschrijf de productieagenda in het veld **Omschrijving**.  
4.  Kies de actie **Werkdagen**.
5.  Geef in het venster **Productieagendawerkdagen** een volledige werkweek, met de begin- en eindtijden voor elke dag, op.  

    Selecteer in het veld **Ploeg** een van de ploegen die u eerder hebt gedefinieerd. Voeg een regel toe voor elke werkdag en elke ploeg. Voorbeeld:  

    maandag 07:00 15:00 1   
    dinsdag 07:00 15:00 1  

    Als u een productieagenda met twee ploegen nodig hebt, gaat u op de volgende manier te werk:  

    maandag 07:00 15:00 1   
    maandag 15:00 23:00 2  
    dinsdag 07:00 15:00 1  
    dinsdag 15:00 23:00 2  

    Weekdagen die u niet in de productieagenda definieert, zoals zaterdag en zondag, worden beschouwd als niet-werkdagen en hebben in een afdelingsagenda een beschikbare capaciteit van nul.  

    Wanneer alle werkdagen van een week zijn gedefinieerd, kunt u het venster **Productieagendawerkdagen** sluiten en doorgaan met het invoeren van vakanties en vrije dagen.  

6.  Selecteer in het venster **Productieagenda's** de productieagenda en kies de actie **Vakantiedagen**.
7. Definieer in het venster **Productieagendavakantiedagen** de vakantiedagen van het jaar door voor elke vakantiedag op afzonderlijke regels de begindatum en -tijd, de eindtijd en een omschrijving op te geven. Voorbeeld:  

    04 juli 2014 0:00:00 23:59:00 Zomervakantie  
    05 juli 2014 0:00:00 23:59:00 Zomervakantie  
    06 juli 2014 0:00:00 23:59:00 Zomervakantie  

De gedefinieerde vakantiedagen hebben in een afdelingsagenda een beschikbare capaciteit van nul.  

Nu kan de productieagenda worden toegewezen aan een afdeling om de afdelingsagenda te berekenen waarop de volledige tijdsplanning van alle bewerkingen op die afdeling wordt gebaseerd.  

## <a name="to-calculate-a-work-center-calendar"></a>Een afdelingsagenda berekenen  

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Afdelingen** in en klik op de gerelateerde koppeling.
2. Open de afdeling die u wilt bijwerken.  
3. Geef in het veld **Productieagendacode** op welke productieagenda moet worden gebruikt als basis voor de agenda van de afdeling.  
4. Kies de actie **Agenda**.  
5. Kies in het venster **Afdelingsagenda** de actie **Matrix weergeven**.  

    In het linkerdeel van het matrixvenster worden alle afdelingen weergegeven die zijn ingesteld. In het rechterdeel ziet u een agenda met daarop de beschikbare capaciteitswaarden voor elke werkdag in de gedefinieerde eenheid, bijvoorbeeld **480** minuten. Elke regel geeft de agenda van één afdeling weer.  

    > [!NOTE]  
    >  U kunt de capaciteitswaarden voor elke week of maand ook bekijken door te schakelen tussen opties in het veld **Weergeven per** in het venster **Afdelingsagenda**.  

    Als u de nieuwe productieagenda wilt weergeven als een lijn op de geselecteerde afdeling, moet deze productieagenda eerst worden berekend.  

6.  Kies de actie **Berekenen**.  
7.  Op het sneltabblad **Afdeling** kunt u een filter instellen, zodat er maar voor één afdeling een berekening wordt gemaakt. Stelt u geen filter in, dan worden alle bestaande afdelingsagenda's berekend.  
8.  Definieer de begin- en einddatum van de agendaperiode die moet worden berekend, bijvoorbeeld één jaar, van 1 jan. 2004 tot 31 dec. 2004.
9. Kies de knop **OK** om de capaciteit te berekenen.  

Er zijn nu agendaposten gemaakt (of bijgewerkt) waarin de beschikbare capaciteit per dag (of per andere periode) wordt weergegeven op basis van de volgende drie sets stamgegevens:  

- de in de productieagenda gedefinieerde werkdagen en ploeg  
- de waarde in het veld **Capaciteit** op de afdelingskaart  
- de waarde in het veld **Efficiëntie** op de afdelingskaart.  

De berekende afdelingsagenda bepaalt nu wanneer en hoe veel capaciteit beschikbaar is op deze afdeling. Hiermee bepaalt u de gedetailleerde planning van bewerkingen die worden uitgevoerd op de afdeling.  

## <a name="to-record-work-center-absence"></a>Afwezigheid op de afdeling registreren  
1.  Kies in het venster **Afdelingsagenda** de actie **Matrix weergeven**.
2. Selecteer in het venster **Afdelingsagendamatrix** de afdeling en de agendadag waarop de afwezigheid moet worden geregistreerd en kies vervolgens de actie **Afwezigheid**.  
3.  Definieer in het venster **Afwezigheid** de begintijd, de eindtijd en de omschrijving van de afwezigheid van die dag, bijvoorbeeld: Voorbeeld:  

    25 jan. 2001 08:00 10:00 Onderhoud  

4.  Kies de actie **Bijwerken** en sluit vervolgens het venster **Afwezigheid**.  

De geregistreerde afwezigheid is nu in mindering gebracht op de capaciteit van de geselecteerde dag.  

## <a name="see-also"></a>Zie ook  
[Procedure: basisagenda's instellen](across-how-to-assign-base-calendars.md)  
[Procedure: Afdelingen en bewerkingsplaatsen instellen](production-how-to-set-up-work-and-machine-centers.md)  
[Productie instellen](production-configure-production-processes.md)  
[Productie](production-manage-manufacturing.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  


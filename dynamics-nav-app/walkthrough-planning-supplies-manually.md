---
title: 'Procedure: leveringen handmatig plannen'
description: In het volgende overzicht ziet u het proces voor het plannen van voorraadorders om aan nieuwe vraag te voldoen. U kunt voorraadplanning starten met vaste tussenpozen, bijvoorbeeld elke ochtend of elke maandag, of wanneer u bericht krijgt van verkoop of productie, afhankelijk van het type vraag.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 488b5515d861b89da398094e3fa4634d31b432d1
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="walkthrough-planning-supplies-manually"></a>Procedure: Leveringen handmatig plannen
In het volgende overzicht ziet u het proces voor het plannen van voorraadorders om aan nieuwe vraag te voldoen. U kunt voorraadplanning starten met vaste tussenpozen, bijvoorbeeld elke ochtend of elke maandag, of wanneer u bericht krijgt van verkoop of productie, afhankelijk van het type vraag. In dit scenario gebruikt u het venster **Orderplanning**, een eenvoudig voorraadplanningshulpmiddel op basis van handmatige besluitvorming in plaats van automatische planning op basis van parameters.  

## <a name="about-this-walkthrough"></a>Informatie over deze procedure  
 In deze procedure worden de volgende taken beschreven:  

-   Een inkooporder plannen voor het fabriceren van onderdelen.  
-   Een transferorder plannen om aan de verkoopvraag te voldoen.  
-   Een productieorder plannen voor een artikel met meerdere niveaus.  

## <a name="roles"></a>Rollen  
 In deze procedure worden taken gedemonstreerd voor de volgende gebruikersrollen:  

-   Productieplanner  
-   Inkoper  
-   Verkooporderverwerker  

## <a name="prerequisites"></a>Vereisten  
 Voordat u met dit scenario begint, moet u de [!INCLUDE[d365fin](includes/d365fin_md.md)] installeren. Breng de volgende wijzigingen aan in de database:  

-   Verwijder alle bestaande verkooporders voor fietsen.  
-   Maak één verkooporder voor 10 fietsen op de locatie BLAUW.  
-   Verwijder alle geplande en vast geplande productieorders. Verwijder geen gestarte orders met posten die al zijn geboekt.  

 Gebruik als algemene regel de voorgestelde gegevens uit deze procedure aangezien deze gegevens de benodigde records bevatten.  

## <a name="story"></a>Scenario  
 Eduardo, de productieplanner van een klein productiebedrijf is bezig met het plannen van de productie en inkooporders om te voldoen aan de nieuwe verkoopvraag.  

 Aangezien de producten uit slechts enkele stuklijstniveaus bestaan en de orderstroom tamelijk gering is, gebruikt Eduardo het venster **Orderplanning** om de orders voor voorzieningen handmatig te maken, met één productniveau tegelijk.  

 In een meer complexe productieomgeving wordt het planningsvoorstel gebruikt om de voorraad te plannen op basis van artikelparameters als herplanningsperiode, veiligheidstijd, bestelpunt en batchberekeningen van de geconsolideerde aanvraag van alle productniveaus.  

## <a name="setting-up-the-sample-data"></a>Voorbeeldgegevens instellen  
 In het standaarddemobedrijf CRONUS is momenteel sprake van een grote hoeveelheid niet-geplande vraag. Tijdens de verschillende planningstaken in deze procedure moet u afwijken van de realistische bedrijfswerkstroom door de vraag met vervaldatums in de nabije toekomst te negeren en in plaats daarvan de vraag te gebruiken met latere vervaldatums.  

## <a name="using-the-order-planning-window"></a>Het venster Orderplanning gebruiken  
 U kunt het venster **Orderplanning** openen van verschillende locaties in het menu **Afdelingen** in het navigatiedeelvenster:  

-   Productie, Planning  
-   Verkoop &amp; Marketing, Orderverwerking  
-   Inkoop, Planning  
-   Bovendien kunt u dit venster openen voor een specifieke productieorder door **Planning** te kiezen op het tabblad **Navigeren** in de groep **Order**.  

### <a name="to-use-the-order-planning-window"></a>Het venster Orderplanning gebruiken  

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Orderplanning** in en klik op de gerelateerde koppeling.  

     Als het venster **Orderplanning** voor het eerst wordt geopend, moet er een planning worden berekend om de nieuwe vraag weer te geven sinds deze voor het laatst is berekend.  

2.  Kies de actie **Plan berekenen**.  

     Het planningssysteem analyseert de nieuwe vraag die is geïntroduceerd, zoals nieuwe of gewijzigde verkoop- of productieorders.  

     Op basis van de totale beschikbaarheid wordt de benodigde hoeveelheid voor elke vraagregel berekend. Deze berekening wordt per order uitgevoerd. Dit betekent dat de order met de vraagregel met de vroegste verval- of verzenddatum eerst wordt berekend. Vervolgens worden aanvullende vraagregels in dezelfde volgorde berekend, ongeacht de vervaldatum of de verzenddatum.  

3.  Het venster **Orderplanning** moet zijn gemaximaliseerd en de afmetingen van de kolomvelden moeten zo zijn ingesteld dat alle standaardveldnamen zichtbaar zijn.  

     Wanneer de berekening is voltooid, worden in het venster alle niet-afgehandelde vraagregels weergegeven als samengevouwen orderkopregels gesorteerd op de vroegste vraagdatum.  

     U ziet dat CRONUS diverse orders heeft met niet-afgehandelde vraag. Elke vette planningsregel geeft een order weer, verkoop of productie, met inbegrip van ten minste één orderregel met onvoldoende beschikbaarheid.  

4.  Selecteer in het veld **Vraag weergeven als** het filter **Alle vraag**.  

     In het veld **Soort vraag** kunt u kiezen welke soorten orders u wilt weergeven.  

     Orders zonder beschikbaarheidsproblemen worden niet weergegeven. Als er geen orders bestaan wanneer een planning wordt berekend, verschijnt een bericht en worden er geen planningsregels weergegeven.  

## <a name="planning-a-purchase-order-to-fulfill-component-demand"></a>Een inkooporder plannen om te voldoen aan de vraag naar onderdelen  
 In deze procedure maakt u een inkooporder voor de benodigde productieonderdelen.  

### <a name="to-plan-a-purchase-order-to-fulfill-component-need-in-production"></a>Een inkooporder plannen om te voldoen aan de onderdelenbehoefte voor de productie  

1.  Vouw de eerste regel uit (klik op het symbool +).  
2.  Kies de eerste vraagregel met, artikel, **LSU-15** en kies de actie **Document weergeven**.  
3.  Sluit de geopende productieorder om terug te keren naar het venster **Orderplanning**.  
4.  Selecteer **Inkoop** in het veld **Aanvullingsmethode**.  

     De standaardwaarde komt van de artikelkaart (of SKU-kaart), maar u kunt dit wijzigen in een van de volgende opties:  

    -   **Inkoop** – een inkooporder maken.  
    -   **Transfer** – een transferorder maken.  
    -   **Prod.-order** – een productieorder maken.  

5.  Selecteer in het veld **Aanleveren van** een van de volgende opties op basis van de geselecteerde aanvullingsmethode:  

    -   **Leverancier** – Voor inkoop  
    -   **Locatie** – voor transfers  

     Als het veld niet is ingevuld, verschijnt er een foutbericht wanneer u voorraadorders probeert te maken.  

    > [!NOTE]  
    >  Als voor de onderdelen een standaardleveranciernummer is ingesteld op de artikelkaarten, zijn de regels vooraf ingevuld.  

6.  Kies het veld **Aanleveren van**.  
7.  Kies in het venster **Artikelleveranciers** de actie **Nieuw** en selecteer leverancier **30000**.  
8.  Kies de knop **OK** om terug te gaan naar het venster **Orderplanning**.  
9. Kopieer leveranciernummer **30000** naar de overige regels voor luidsprekeronderdelen in deze productieorder.  

     U kunt nu een inkooporder gaan maken.  

10. Kies de actie **Orders maken**. Het venster **Orders voor voorzieningen maken** wordt geopend.  
11. Kies op het sneltabblad **Orderplanning** in het veld **Orders maken voor** de optie **Actieve order**.  
12. Kies op het sneltabblad **Opties** in het veld **Inkooporder maken** de optie **Inkooporders maken**.  
13. Klik op **OK** om inkooporders te maken voor alle onderdelen van de order.  

     De inkooporders worden gemaakt en opgeslagen als de laatste orders in de lijst met inkooporders.  

## <a name="planning-a-transfer-order-to-fulfill-sales-demand"></a>Een transferorder plannen om aan de verkoopvraag te voldoen  
 In deze procedure gaat u plannen voor de vraag van een verkooporder. Vraagregels geven de verkoopregels aan en niet de onderdeelregels, zoals bij de productievraag.  

### <a name="to-plan-a-transfer-order-to-fulfill-sales-demand"></a>Een transferorder plannen om aan de verkoopvraag te voldoen  

1.  Verplaats de aanwijzer naar de planningsregel voor ordernummer **2008**.  
2.  Vouw de regel uit en verplaats de aanwijzer naar de vraagregel.  

     Verkooporder **2008 betreft** tien luidsprekers van het type **LS-120** die zijn besteld door John Haddock Insurance Co.  

     Voor het artikel is het aanvulsysteem geselecteerd en de standaardleverancier wordt weergegeven.  

    > [!NOTE]  
    >  Onder aan het venster staan vier informatievelden. In het veld **Vroegste beschikbaarheidsdatum** zijn de tien stuks die nodig zijn, beschikbaar via een inkomende voorraadorder, maar pas negen dagen na de huidige vervaldatum. Als dat te laat is voor de klant, bevat het veld **Beschikbaar voor transfer** 13 stuks van het artikel op een andere locatie. U gaat voor deze voorraad een planning maken.  

3.  Kies het veld **Beschikbaar voor transfer** om het venster **Alternatieve voorziening ophalen** te openen.  
4.  Klik op **OK** om de tien beschikbare artikelen te boeken.  

    > [!NOTE]  
    >  Op de vraagregel wordt de voorgestelde inkoop vervangen door een transfer van de locatie GROEN. Met de functie **Orders maken** maakt u een transferorder van GROEN naar de gewenste locatie. Het veld **Vervangingsartikel** werkt op dezelfde manier.  

5.  Kies de actie **Orders maken**. Het venster **Aanvulorders maken** wordt geopend.  
6.  Kies op het sneltabblad **Orderplanning** in het veld **Orders maken voor** de optie **Actieve order**.  
7.  Selecteer op het sneltabblad **Opties** in het veld **Transferorder maken** de optie **Transferorders maken**.  
8.  Klik op **OK** om de transferorder te maken om te voldoen aan de verkooporder.  

     De transferorder is nu gemaakt en in de lijst opgeslagen als de laatste order in de lijst met open transferorders.  

## <a name="planning-a-multilevel-production-order-to-fulfill-sales-demand"></a>Een productieorder met meerdere niveaus plannen om aan de verkoopvraag te voldoen  
 In deze procedure gaat u plannen om aan de verkoopvraag te voldoen voor een geproduceerd artikel met meerdere productniveaus, waarbij de productievraag voor alle niveaus samenhangt.  

### <a name="to-plan-multilevel-production-to-fulfill-sales-demand"></a>Een productie met meerdere niveaus plannen om aan de verkoopvraag te voldoen  

1.  Selecteer de planningsregel met de verkoopvraag voor ordernummer **1001** (gemaakt bij de vereiste gegevens).  

     Deze vraag is een verkoopregel maar voor het artikel is het aanvulsysteem **Prod.-order** gedefinieerd. Voeg een tweede bel toe aan de onderdelenlijst voor elke fiets.  

2.  Kies de actie **Materialen** om het venster **Planningsmaterialen** te openen.  
3.  Wijzig in de regel voor de fietsbel het veld **Aantal per** van **1** in **2**.  
4.  Bekijk in het venster **Orderplanning** de planningsalternatieven. In dit geval zijn er geen alternatieve leveringsmethoden, geen transfer, geen vervangend artikel en geen latere levering. U moet de voorgestelde voorzieningsorder, een productieorder, maken.  
5.  Kies de actie **Orders maken** om de productieorder te maken.  

     U ziet dat in het venster **Orderplanning** de planningregel voor verkooporder **1001** niet meer bestaat en dat aan de eerste verkoopvraag is voldaan.  

6.  Sluit het venster **Orderplanning**.  

     U zou nu in deze weergave kunnen blijven om alle planningstaken te voltooien. In plaats daarvan neemt u nu de rol van de productieplanner op en gaat u naar de zojuist gemaakte productieorder om het venster **Orderplanning** te openen.  

 Als productieplanner moet u nu een specifieke productieorder plannen.  

### <a name="to-plan-a-specific-production-order"></a>Een specifieke productieorder plannen  

1.  Open de productieorder **101001** (voor tien fietsen) die u hebt gemaakt met de functie **Orders maken**.  
2.  Open het venster **Prod.-ordermaterialen** om te controleren of de extra bel wordt weergegeven op de productieorder.  
3.  Kies de actie **Planning**.  

     Het venster **Orderplanning** wordt geopend in een weergave die altijd wordt gefilterd op de specifieke productievraag. De verkoopvraag wordt niet weergegeven. U moet eerst een planning berekenen voordat een nieuwe vraag wordt weergegeven.  

4.  Kies de actie **Plan berekenen**.  

     U ziet dat er vier nieuwe productieorders verschijnen voor de niet-geplande productievraag op basis van order **101001.** De nieuwe regels geven de nieuwe productievraag weer voor de subassemblages die moeten worden gemaakt om de order te produceren.  

5.  Kies de actie **Alles uitvouwen** om een overzicht te krijgen van de volledige productievraag voor de productieorders.  

     Als u aanvullende informatie over de vraagregels wilt verstrekken, kunt u de velden **Aantal vraag** en **Beschikbaar aantal vraag** toevoegen aan uw weergave.  

     U moet nu tien stuks van elk onderdeel leveren.  

     Houd er rekening mee dat vier van de vraagregels aanvullingsmethode Prod.-order hebben. Deze vier halffabrikaten vertegenwoordigen het tweede productniveau van de fiets.  

     De standaardinstellingen voor aanvulling zijn al ingevuld en u kunt de orders gaan maken.  

6.  Kies de actie **Orders maken**.  

     Lees, voordat u de knop **OK** kiest, de tekst op het sneltabblad **Orderplanning**. Deze tekst is belangrijk omdat u weet dat de productstructuur van de fiets een aantal geproduceerde onderdelen (subassemblages) bevat die in de vraag worden opgenomen wanneer u deze productieorder maakt.  

7.  Kies in het venster **Orders voor voorzieningen maken** in het veld **Orders maken voor** de optie **Alle regels** en kies vervolgens de knop **OK** om productieorders te maken voor het tweede productniveau van de order.  

     U ziet dat de hoogste productievraag voor productieorder 101001 niet meer bestaat. Dat betekent dat de aanvankelijke productievraag voor subassemblages nu is ingepland.  

     Bereken in het venster **Orderplanning** nogmaals de planning om de fietsstructuur te plannen.  

8.  Kies de actie **Planning berekenen** om de planning opnieuw te berekenen volgens de instructies uit de Help-tekst.  

     De twee nieuwe regels geven de aanvullende productievraag aan die is afgeleid van de subassemblages die in de vorige stappen zijn gepland. Er wordt aangegeven dat u twee productieorders maakt voor de wielnaven, een voor 10 voornaven en een voor 10 achternaven.  

9. Kies de actie **Alles uitvouwen** om een overzicht te krijgen van de twee productieorders.  

     Het voorgestelde voorzieningsplan geeft aan dat er in totaal vier inkooporders worden gemaakt voor de onderdelen. U besluit de voorgestelde orders te maken.  

10. Kies de actie **Orders maken**.  
11. Selecteer in het veld **Orders maken voor** de optie **Alle regels** en kies vervolgens de knop **OK**. Controleer of er een aanvullende vraag bestaat voor de productie van het hoofdartikel, de fiets (verkocht op verkooporder 1001).  
12. Kies de actie **Plan berekenen**.  

     Het bericht geeft aan dat nu in alle vereiste artikelen is voorzien. Controleer de vast gepland productieorders die worden gemaakt.  

13. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Vast geplande productieorders** in en klik op de gerelateerde koppeling.  

     Bekijk in het venster **Vast geplande productieorders** hoe de begin- en eindtijden van afzonderlijke orders nu zijn gepland volgens de productstructuur. De onderdelen op het laagste niveau worden het eerst geproduceerd. Daarom moet u orders met meerdere niveaus plannen zoals is gedemonstreerd in deze planningswerkstroom.  

## <a name="see-also"></a>Zie ook  
 [Procedures voor bedrijfsprocessen](walkthrough-business-process-walkthroughs.md)   
 [Procedure: Goederen automatisch plannen](walkthrough-planning-supplies-automatically.md)


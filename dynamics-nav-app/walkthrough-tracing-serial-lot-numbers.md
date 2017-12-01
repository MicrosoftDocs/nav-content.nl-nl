---
title: 'Procedure: Serie-/lotnummers traceren'
description: Als er productdefecten optreden, moeten de fouten worden opgespoord en de betreffende artikelen mogen het bedrijf niet verlaten. Als er al defecte artikelen zijn geleverd, is het belangrijk om bij te houden wie ze heeft ontvangen, zodat ze zo nodig kunnen worden teruggehaald.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/22/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 34d488ed98293935d8a2ddf1b042879fb943ad29
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="walkthrough-tracing-serial-lot-numbers"></a>Procedure: Serie-/lotnummers traceren
Als er productdefecten optreden, moeten de fouten worden opgespoord en de betreffende artikelen mogen het bedrijf niet verlaten. Als er al defecte artikelen zijn geleverd, is het belangrijk om bij te houden wie ze heeft ontvangen, zodat ze zo nodig kunnen worden teruggehaald.  

De eerste taak van defectenbeheer is om te onderzoeken waar de defecte artikelen vandaan zijn gekomen en waar ze zijn gebruikt. Dit onderzoek is gebaseerd op historische gegevens en het wordt vergemakkelijkt als er kan worden gezocht via vermeldingen voor het traceren van artikelen in het venster **Artikeltracering**.  

De tweede taak van defectenbeheer is vaststellen of de getraceerde artikelen zijn gepland in open documenten zoals niet-geboekte verkooporders of verbruiksdagboeken. Dit werk wordt uitgevoerd in het venster **Navigeren**. Met de functie Navigeren kunt u naar alle soorten databaserecords zoeken.  

## <a name="about-this-walkthrough"></a>Informatie over deze procedure  
In dit overzicht wordt uitgelegd hoe u kunt achterhalen welke artikelen defect zijn, welke leverancier ze heeft geleverd en waar ze worden gebruikt, zodat deze orders kunnen worden stopgezet of teruggehaald.  

In deze procedure worden de volgende taken beschreven:  

-   Traceren van gebruik naar oorsprong.  
-   Traceren van oorsprong naar gebruik.  
-   Zoeken naar alle huidige records waarin het getraceerde serie-/lotnummer voorkomt.  

## <a name="roles"></a>Rollen  
In dit overzicht worden taken gedemonstreerd voor de volgende gebruikersrollen:  

-   Kwaliteitscontroleur  
-   Magazijnbeheerder  
-   Orderverwerker  
-   Inkoper  

## <a name="prerequisites"></a>Vereisten  
U moet het volgende doen om deze procedure uit te voeren:  

-   Het bedrijf [!INCLUDE[d365fin](includes/d365fin_md.md)].  
-   Als u nieuwe artikelen en een aantal zakelijke transacties wilt maken via de stappen in het gedeelte 'Voorbeeldgegevens voorbereiden', verderop in dit overzicht.  

## <a name="story"></a>Scenario  
Ricardo, de kwaliteitscontroleur, is bezig met het teruggegeven artikel 1002, een racefiets. De klant, Selangorian Ltd., heeft geklaagd dat het frame gescheurde lasnaden heeft. Kwaliteitscontroletechnici hebben bevestigd dat het frame van de teruggegeven fiets gebreken vertoont. De kwaliteitscontroleur moet nu de volgende dingen vaststellen:  

-   Welke partij raceframes vertoont gebreken?  
-   Op welke inkooporder is de defecte partij ontvangen?  

Van de verkoopafdeling weet de kwaliteitscontroleur dat de teruggegeven racefiets, artikel 1002, het serienummer SN1 heeft. Met deze basisinformatie moet hij bepalen waar de voltooide racefiets voor het laatst is gebruikt en dan moet hij deze traceren naar het eerste begin om vast te stellen van welk partijnummer het defecte onderdeel, het frame, afkomstig is.  

Met de resultaten van deze eerste artikeltraceringstaak wordt vastgesteld welke raceframes defect waren en welke leverancier ze heeft geleverd. Daarna, maar binnen hetzelfde algemene traceringsproces, moet de kwaliteitscontroleur alle verkochte racefietsen opzoeken met raceframes uit de defecte partij, zodat deze orders kunnen worden stopgezet of teruggehaald. Ten slotte moet de kwaliteitscontroleur eventuele open documenten opzoeken waarin de defecte partij wordt gebruikt, zodat er geen verdere transacties worden verricht.  

De twee eerste defectenbeheertaken worden uitgevoerd in het venster **Artikeltracering**. De laatste taak wordt uitgevoerd in het venster **Navigeren** in integratie met het venster **Artikeltracering**.  

## <a name="prepare-sample-data"></a>Voorbeeldgegevens voorbereiden  
U moet de volgende nieuwe artikelen maken:  

-   2000, raceframe: partijspecifieke tracering, onderdeel van 1002  
-   1002, racefiets: serienummerspecifieke tracering  

Vervolgens moet u diverse inkoop-, productie- en verkooptransacties met beide artikelen maken.  

### <a name="to-create-the-items"></a>De artikelen maken  

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Artikelen** in en klik vervolgens op de gerelateerde koppeling.  
2.  Kies de actie **Nieuw**.  
3.  Selecteer in het veld **Nr.** Voer in het veld **2000** in en vul de volgende velden in.  

    |Omschrijving|Basiseenheid|Prod.-boekingsgroep|Btw-productboekingsgroep|Voorraadboekingsgroep|Artikeltraceringscode|  
    |-----------------|--------------------------|------------------------------|-----------------------------|-----------------------------|------------------------|  
    |Raceframe|Per stuk|GRONDSTOF|BTW19|GRONDSTOF|LOTALL|  

    > [!NOTE]  
    >  U kunt de basiseenheid invoeren door de knop **Nieuw** te kiezen en vervolgens **PSC** te selecteren in het venster **Artikeleenheden**.  

4.  Alle andere velden hebben acceptabele standaardgegevens of hoeven niet te worden ingevuld.  
5.  Kies de knop **OK** om de eerste nieuwe artikelkaart te maken, 2000.  
6.  Kies **Nieuwe**.  
7.  Selecteer in het veld **Nr.** Voer in het veld **1002** in en vul de volgende velden in.  

    |Omschrijving|Basiseenheid|Prod.-boekingsgroep|Btw-productboekingsgroep|Voorraadboekingsgroep|Aanvullingsmethode|Artikeltraceringscode|  
    |-----------------|--------------------------|------------------------------|-----------------------------|-----------------------------|--------------------------|------------------------|  
    |Racefiets|Per stuk|DET.HANDEL|BTW19|GEREED|Prod.-order|SNALLE|  

    > [!NOTE]  
    >  U kunt de basiseenheid invoeren door de knop **Nieuw** te kiezen en vervolgens **PSC** te selecteren in het venster **Artikeleenheden**.  

    Vervolgens moet u de productie-instelling van het artikel definiëren.

9. Voer op het sneltabblad **Aanvulling** de waarde **1000** in het veld **Bew.-plannr.** in.  
10. Kies het veld **Prod.-stuklijstnr.** en kies vervolgens **Geavanceerd**.  
11. Kies in het venster **Productiestuklijst** de eerste regel **1000** en kies vervolgens de actie **Bewerken**.  
12. Wijzig in het venster **Productiestuklijst** de waarde in het veld **Status** in **In ontwikkeling**.  
13. Ga naar een lege regel, voer **2000** in het veld **Nr.** in en voer vervolgens **1** in het veld **Aantal per** in.  
14. Wijzig de waarde in het veld **Status** terug naar **Gecertificeerd**.  
15. Kies de knop **OK** om de productiestuklijst in te voegen op de artikelkaart en het venster **Productiestuklijst** te sluiten.  

    Vervolgens schaft u raceframes van Custom Metals Incorporated aan.  

### <a name="to-purchase-components"></a>Materialen kopen  
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Inkooporders** in en klik vervolgens op de gerelateerde koppeling.  
2.  Kies de actie **Nieuw**.  
3.  Maak een inkooporder voor de leverancier Custom Metals Incorporated door de volgende regelvelden in te vullen.  

    |Artikel|Aantal|Lotnr.|  
    |----------|--------------|-------------|  
    |2000|10|LOT1|  

4.  Als u het lotnummer wilt invoeren, kiest u de actie **Artikeltraceringsregels**.  
5.  Vul in het venster **Artikeltraceringsregels** de velden **Lotnr.** en **Aantal (Basis)** in en sluit het venster.  
6.  Voer in het veld **Factuurnr. leverancier** een waarde in.  
7.  Kies de actie **Boeken**, selecteer de optie **Ontvangen en factureren** en kies vervolgens de knop **OK**.  

    Als volgende, koopt u racingframes van Coolwood Technologies.  
8.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Inkooporders** in en klik vervolgens op de gerelateerde koppeling.  
9. Kies de actie **Nieuw**.
10. Maak een inkooporder voor de leverancier Coolwood Technologies door de volgende regelvelden in te vullen.  

    |Artikel|Aantal|Lotnr.|  
    |----------|--------------|-------------|  
    |2000|11|LOT2|  

11. Voer het lotnummer in door op het sneltabblad **Regels** in de groep **Regel** de actie **Artikeltraceringsregels** te kiezen.  
12. Vul in het venster **Artikeltraceringsregels** de velden **Lotnr.** en **Aantal (Basis)** in en sluit het venster.  
13. Voer in het veld **Factuurnr. leverancier** een waarde in.  
14. Kies de actie **Boeken**, selecteer de optie **Ontvangen en factureren** en kies vervolgens de knop **OK**.  

    Vervolgens maakt u twee racefietsen, SN1 en SN2.  

### <a name="to-produce-end-items"></a>Eindproducten produceren  
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Vrijgegeven prod.-orders** in en klik op de gerelateerde koppeling.  
2.  Kies de groep **Nieuw**.  
3.  Maak een nieuwe vrijgegeven productieorder door de volgende velden in te vullen.  

    ||||  
    |-|-|-|  
    |Bronnr.|Aantal|Serienr.|  
    |1002|2|SN1|  
    |1002|2|SN2|  

4.  Kies de actie **Productieorder vernieuwen** en kies de knop **OK** om de regel in te vullen.  
5.  Als u de serienummers wilt invoeren, kiest u de actie **Artikeltraceringsregels**.  
6.  Vul in het venster **Artikeltraceringsregels** de velden **Serienr.** en **Aantal (Basis)** in en sluit het venster.  

    Vervolgens moet u het verbruik aan racingframes van LOT1 boeken.  
7.  In het venster **Vrijgegeven productieorder** kiest u de actie **Productiedagboek**.  
8.  In het venster **Productiedagboek** selecteert u de verbruiksregel voor artikel 2000 en kiest u de actie **Artikeltraceringsregels**.
9. Kies in het venster **Artikeltraceringsregels** het veld **Lotnr.**, kies **LOT1** en klik vervolgens op de knop **OK**.  
10. Laat alle andere standaardwaarden in het venster **Productiedagboek** ongewijzigd en kies de actie **Boeken**.  

    Maak als volgende nog twee racefietsen, SN3 en SN4.  

11. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Vrijgegeven prod.-orders** in en klik op de gerelateerde koppeling.  
12. Kies de actie **Nieuw**.  
13. Maak een nieuwe vrijgegeven productieorder door de volgende velden in de kop in te vullen.  

    |Bronnr.|Aantal|Serienr.|  
    |----------------|--------------|----------------|  
    |1002|2|SN3|  
    |1002|2|SN4|  

14. Kies de actie **Productieorder vernieuwen** om de regel in te vullen.  
15. Om de serienummers in te voeren, kiest u de actie **Artikeltraceringsregels** en vult u vervolgens de nummers in op twee regels in het veld **Serienr.** in het venster **Artikeltraceringsregels**.  

    Vervolgens moet u het verbruik aan racingframes van LOT1 boeken.  
16. In het venster **Vrijgegeven productieorder** kiest u de actie **Productiedagboek**.  
17. In het venster **Productiedagboek** selecteert u de verbruiksregel voor artikel 2000 en kiest u de actie **Artikeltraceringsregels**.
18. Kies in het venster **Artikeltraceringsregels** het veld **Lotnr.**, kies **LOT1** en klik vervolgens op de knop **OK**.  
19. Laat alle andere standaardwaarden in het venster **Productiedagboek** ongewijzigd en kies de actie **Boeken**.  

    U hebt nu vier racefietsen gemaakt, SN1 tot en met SN4, en vier van de tien raceframes van LOT1 gebruikt, twee frames per productieorder.  

20. Sluit het productiedagboek en de productieorders.  

    Vervolgens gaat u racefietsen verkopen. Eest verkoopt u de racefiets met SN1 aan Selangorian Ltd.  

### <a name="to-sell-the-end-items"></a>De eindpoducten verkopen  
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Verkooporders** in en klik vervolgens op de gerelateerde koppeling.  
2.  Kies de actie **Nieuw** en maak vervolgens een verkooporder door de volgende velden in te vullen.  

    |Klant|Artikel|Aantal|Serienr.|  
    |--------------|----------|----------|----------------|  
    |Anton Geestig Adviezen|1002|0|SN1|  

3.  Om het serienummer in te voeren, kiest u de actie **Artikeltraceringsregels** en vult u vervolgens het nummer in het veld **Serienr.** in het venster **Artikeltraceringsregels** in.  
4.  Kies de actie **Boeken**, selecteer de optie **Verzenden en factureren** en kies vervolgens de knop **OK**.  

    Vervolgens gaat u de racefiets met SN2 aan Cannon Group PLC verkopen.  

5.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Verkooporders** in en klik vervolgens op de gerelateerde koppeling.  
6.  Kies de actie **Nieuw** en maak vervolgens een verkooporder door de volgende velden in te vullen.  

    |Klant|Artikel|Aantal|Serienr.|  
    |--------------|----------|----------|----------------|  
    |Van Terp Kantoorinrichting|1002|0|SN2|  

7.  Om het serienummer in te voeren, kiest u de actie **Artikeltraceringsregels** en vult u vervolgens het nummer in het veld **Serienr.** in het venster **Artikeltraceringsregels** in.  
8.  Kies de actie **Boeken**, selecteer de optie **Verzenden en factureren** en kies vervolgens de knop **OK**.  

    Ten slotte moet u een paar raceframes afzonderlijk verkopen. Van Terp Kantoorinrichting bestelt ook vier afzonderlijke raceframes voor hun eigen assemblagelijn.  

9. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Verkooporders** in en klik vervolgens op de gerelateerde koppeling.  
10. Kies de actie **Nieuw** en maak vervolgens een verkooporder door de volgende velden in te vullen.  

    |Klant|Artikel|Aantal|Serienummer|  
    |--------------|----------|----------|----------------|  
    |Van Terp Kantoorinrichting|2000|5|LOT1|  

11. Om het serienummer op het sneltabblad **Regels** in de groep **Regel** in te voeren, kiest u de actie **Artikeltraceringsregels** en typt u vervolgens het nummer in het veld **Serienr.** in het venster **Artikeltraceringsregels**.  

    > [!NOTE]  
    >  Boek de laatste verkooporder niet (voor vijf raceframes).  

    Hiermee is de voorbereiding van gegevens voltooid voor het demonstreren van de functies voor het traceren van en navigeren door artikelen.  

## <a name="tracing-from-usage-to-origin"></a>Traceren van gebruik naar oorsprong  
 Van de verkoopafdeling weet de kwaliteitscontroleur dat de teruggegeven racefiets, artikel 1002, het serienummer SN1 heeft. Met deze basisinformatie kan hij bepalen waar de voltooide racefiets voor het laatst is gebruikt, in dit geval bij de verkoopverzending aan Selangorian Ltd. Vervolgens moet de kwaliteitscontroleur deze traceren naar het eerste begin om vast te stellen van welk partijnummer het defecte frame afkomstig is en welke leverancier deze heeft geleverd.  

### <a name="to-determine-which-lot-included-the-faulty-frame-and-who-supplied-it"></a>Vaststellen uit welke partij het defecte frame afkomstig is en wie deze heeft geleverd  
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Artikeltracering** in en klik vervolgens op de gerelateerde koppeling.  
2.  Voer in het veld **Artikeltracering** de tekst **SN1** in het veld **Serienr.-filter** in en voer vervolgens **1002** in het veld **Artikelfilter** in.  
3.  Laat de standaardinstelling **Met artikeltracering** staan in het veld **Onderdelen weergeven** en houd de standaardtraceringsmethode **Gebruik - oorsprong** bij **Traceringsmethode**.  
4.  Kies de actie **Traceren**.  

    U ziet dat een van de verkoopverzendkoppen overeenkomt met de zoekcriteria. Voordat u doorgaat met de tracering, controleert u of dit de verzending met de defecte racefiets aan Selangorian Ltd is.  

5.  Selecteer de traceringsregel en kies de actie **Document weergeven**.  

    Ga nu verder met het traceren van de oorsprong van de verkoopverzending van de racefiets met nummer SN1.  
6.  Klik op het pictogram + op de traceringsregels om geleidelijk de keten van transacties waaruit de verkoopverzending afkomstig is, uit te vouwen en achterwaarts te traceren.  

    U kunt de volgende transactiegeschiedenis traceren:  

    -   Het eerste geboekte document terug in de transactieketen is de uitvoerboeking van SN1 van de eerste vrijgegeven productieorder.  
    -   Het volgende geboekte document terug in de keten is de verbruiksboeking van de eerste vrijgegeven productieorder. Hier ziet de kwaliteitscontroleur dat er een raceframe van LOT1 is gebruikt.  
    -   Het laagste geboekte document in deze keten is de geboekte inkoopontvangst waarop raceframes met LOT1 in de voorraad zijn gekomen.  

    De kwaliteitscontroleur heeft nu vastgesteld welke partij raceframes defect was en hij kan zoeken op de laatste traceringsregel om te zien welke leverancier deze heeft geleverd, namelijk Custom Metals Incorporated.  

    > [!NOTE]  
    >  Breng geen verdere wijzigingen aan in het traceringsresultaat, want dit gaat u gebruiken in het volgende gedeelte.  

     Hiermee is de eerste taak voor defectenbeheer met het venster **Artikeltracering** voltooid. De kwaliteitscontroleur moet nu bepalen of er andere documenten zijn geboekt waarop raceframes uit LOT1 zijn verwerkt.  

## <a name="tracing-from-origin-to-usage"></a>Traceren van oorsprong naar gebruik  
 De kwaliteitscontroleur heeft vastgesteld dat de defecte raceframes afkomstig waren uit LOT1. Hij moet nu achterhalen welke andere racefietsen eventueel een raceframe uit de defecte partij hebben, zodat deze fietsen kunnen worden stopgezet of teruggehaald.  

 Een manier om deze traceringstaak voor te bereiden in het venster **Artikeltracering** is om handmatig LOT1 in te voeren in het veld **Lotnr.-filter** en 2000 in het veld **Artikelfilter**. In dit overzicht wordt echter gebruikgemaakt van de functie **Tegengesteld traceren - Van regel**.  

### <a name="to-find-all-usage-of-the-faulty-lot"></a>Al het gebruik van de defecte partij opsporen  

1.  Selecteer in het venster **Artikeltracering** de regel van de inkoopontvangst, de laatste traceringsregel, en kies vervolgens **Tegengesteld traceren - Van regel**.  

    Het traceringsresultaat is nu gebaseerd op de filters van de traceringsregel voor de inkoopontvangst, LOT1 en artikel 2000, en het resultaat is gebaseerd op de traceringsmethode **Oorsprong - gebruik**.  

    Voor een overzicht van al het gebruik van artikel 2000 met LOT1 blijft u alle traceringsregels uitvouwen.  

2.  Kies de actie **Alles uitvouwen**.  

    De eerste vier traceringsregels verwijzen naar de verkoopverzending aan Selangorian Ltd., die al is opgelost. De laatste regel geeft aan dat er nog een racefiets, SN2, is geproduceerd in dezelfde vrijgegeven productieorder en vervolgens verkocht en verzonden in een andere verkoopverzending.  

    De kwaliteitscontroleur licht direct de verkoopafdeling in, zodat ze kunnen beginnen met het terughalen van de defecte racefiets bij de klant, Cannon Group PLC.  

    Tegelijkertijd kan hij aan de laatste drie traceringsregels zien dat er nog twee artikelen, SN3 en SN4, zijn geproduceerd op basis van raceframes uit LOT1. Hij onderneemt actie om deze eindartikelen in de voorraad te blokkeren.  

    Hiermee is de tweede taak voor defectenbeheer met het venster **Artikeltracering** voltooid. Aangezien het venster **Artikeltracering** uitsluitend is gebaseerd op geboekte posten, moet de kwaliteitscontroleur naar het venster **Navigeren** gaan om te controleren of LOT1 niet is gebruikt in niet-geboekte documenten.  

## <a name="finding-all-records-of-a-seriallot-number"></a>Alle records van een serie/lotnummer zoeken  
 In het venster **Artikeltracering** heeft de kwaliteitscontroleur gezien dat LOT1 de defecte raceframes bevatte, van welke leverancier ze afkomstig zijn en in welke geboekte transactie ze zijn gebruikt. Hij moet nu bepalen of LOT1 in open documenten voorkomt door te integreren van het traceringsresultaat naar het venster **Navigeren**, waar hij een zoekactie op alle databaserecords kan uitvoeren.  

### <a name="to-find-all-occurrences-of-lot1-in-non-posted-records-such-as-open-orders"></a>Alle gevallen van LOT1 in niet-geboekte records zoeken zoals open orders  

1.  Selecteer in het venster **Artikeltracering** de aanwijzer in de eerste traceringsregel, de inkoopontvangst van LOT1.  
2.  Kies de actie **Navigeren**.  

    Het venster **Navigeren** is vooraf ingesteld met zoekfilters op basis van het traceringsresultaat voor LOT1. De kwaliteitscontroleur ziet dat de meeste records te maken hebben met documenten die al zijn geïdentificeerd in het venster **Artikeltracering**. Zo verwijst bijvoorbeeld de laatste navigatieregel van het type Productieorder naar de twee vrijgegeven productieorders waarvoor raceframes van LOT1 zijn gebruikt.  

    De tweede navigatieregel van het type **Verkoopregel** is een niet-geboekte documentregel, dus de kwaliteitscontroleur gaat verder met onderzoeken.  

3.  Als u de verkoopregelrecord wilt openen, selecteert u de tweede navigatieregel en kiest u de actie **Weergeven**. U kunt ook klikken op het getal in het veld **Aantal records**.  

    Hier ziet de kwaliteitscontroleur één open verkoopregel voor de defecte raceframes. Hij stelt onmiddellijk aan de verkoopafdeling voor dat ze deze order annuleren en een nieuwe productieorder starten op basis van goede raceframes.  

 Hiermee is het overzicht van het gebruik van het venster **Navigeren** voor defectenbeheer in integratie met het venster **Artikeltracering** voltooid.  

## <a name="see-also"></a>Zie ook
[Procedure: Werken met serie- en lotnummers](inventory-how-work-item-tracking.md)  
[Procedure: artikelen met artikeltracering traceren](inventory-how-to-trace-item-tracked-items.md)  
[Procedures voor bedrijfsprocessen](walkthrough-business-process-walkthroughs.md)  


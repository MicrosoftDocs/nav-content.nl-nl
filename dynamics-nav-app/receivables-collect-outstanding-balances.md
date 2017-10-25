---
title: Klanten herinneren aan of beboeten voor achterstallige betalingen
description: Beschrijft hoe u een aanmaning aan een klant verzendt over een betaling die achterstallig is, en kosten aan de betaling toevoegt voor de vertraging.
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: payment due, debt, overdue, fee, charge, reminder
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: e7543ab169a1a6ab16c9fdf0afdec88b7749d717
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-collect-outstanding-balances"></a>Procedure: Openstaande saldi innen
Tijdens het beheer van tegoeden moet u ook controleren of openstaande bedragen op tijd worden betaald. Als klanten betalingen hebben openstaan, kunt u beginnen met het rekeningoverzicht van de klant als een herinnering te sturen. U kunt ook aanmaningen sturen.

U kunt aanmaningen gebruiken om klanten te herinneren aan openstaande bedragen. U kunt aanmaningen ook gebruiken om rentefacturen zoals rente en boetes te berekenen en deze op te nemen op de aanmaning. Gebruik rentefacturen als u klanten rente en aanmaningskosten wilt laten betalen zonder ze te herinneren aan openstaande bedragen.  

## <a name="reminders"></a>Aanmaningen
Voor u aanmaningen kunt maken, moet u aanmaningscondities instellen en deze toewijzen aan uw klanten. Elke aanmaningsconditie heeft vooraf gedefinieerde aanmaningsniveaus. Elk aanmaningsniveau bevat regels over wanneer de aanmaning wordt verstuurd, bijvoorbeeld hoeveel dagen na de vervaldatum van de factuur of na het versturen van de vorige herinnering. De inhoud van het venster **Rentefactuurcondities** bepaalt of er rente in rekening wordt gebracht op de aanmaning.  

U kunt de batchverwerking **Aanmaningen maken** periodiek uitvoeren om aanmaningen te maken voor alle klanten met achterstallige saldo's, of u kunt handmatig een aanmaning maken voor een specifieke klant en de regels automatisch laten uitrekenen en invullen.  

Nadat u de aanmaningen hebt gemaakt, kunt u ze aanpassen. De tekst die wordt afgedrukt aan het begin of eind van een aanmaning wordt bepaald door de aanmaningscondities en kan worden bekeken in de kolom **Omschrijving**. Als een berekend bedrag automatisch is ingevoegd in de begin-, of eindtekst, wordt de tekst niet aangepast wanneer u regels verwijdert. In dat geval moet u de functie **Aanmaningstekst bijwerken** gebruiken.  

Voor een klantpost waarbij het veld **Afwachten** is ingevuld wordt geen aanmaning gemaakt. Als er echter een aanmaning wordt gemaakt op basis van een andere post, wordt een wachtende post ook opgenomen op de aanmaning. Er wordt geen rente berekend op regels met deze posten.

Nadat u aanmaningen hebt gemaakt en eventuele aanpassingen hebt gedaan, kunt u testrapporten afdrukken of de aanmaningen versturen, meestal als e-mail.

## <a name="finance-charges"></a>Financiële kosten
Wanneer een klant niet op de vervaldatum betaalt, kunt u automatisch aanmaningskosten laten berekenen en die optellen bij de openstaande bedragen op de rekening van de klant. U kunt klanten op de hoogte stellen van de toeslagen door rentefacturen te versturen.  

> [!NOTE]  
> U gebruikt rentefacturen om rente en aanmaningskosten te berekenen en om uw klanten hiervan op de hoogte te stellen zonder ze te herinneren aan achterstallige betalingen. U kunt ook rente berekenen op achterstallige betalingen wanneer u aanmaningen maakt.  

U kunt handmatig rentefacturen maken voor een afzonderlijke klant en de regels automatisch in laten vullen. U kunt ook de functietaak **Rentefacturen maken** gebruiken om rentefacturen te maken voor alle of geselecteerde klanten met achterstallige saldo's.  

Nadat u de rentefacturen hebt gemaakt, kunt u ze aanpassen. De tekst die wordt afgedrukt aan het begin of eind van de rentefactuur wordt bepaald door de rentefactuurtermijnen en kan worden bekeken in de kolom **Omschrijving** in de regels. Als een berekend bedrag automatisch is ingevoegd in de begin-, of eindtekst, wordt de tekst niet aangepast wanneer u regels verwijdert. In dat geval moet u de functie **Rentefactuurtekst bijwerken** gebruiken.  

Nadat u de rentefacturen hebt gemaakt en eventuele aanpassingen hebt gedaan, kunt u testrapporten afdrukken of de rentefacturen versturen, meestal via e-mail.  

## <a name="to-send-the-customer-statement-report"></a>Het rekeningoverzichten van de klant verzenden
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "Pictogram Zoeken naar pagina of rapport"), voer **Klant - Rekeningoverzicht** in en klik vervolgens op de gerelateerde koppeling.
2. Vul indien nodig de velden in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Geef onder **Uitvoeropties** aan hoe de lijst aan het rapport aan de klant moet worden verzonden.

> [!NOTE]  
>   Als u meerdere valuta's gebruikt, wordt het rekeningoverzicht van de klant altijd afgedrukt in de valuta van de klant. De laatste datum in een dagafschriftperiode wordt ook gebruikt als de datum en de vervaldatum van het overzicht, indien verval is opgenomen.

## <a name="to-set-up-reminder-terms"></a>U kunt aanmaningscondities als volgt instellen
Als klanten betalingen hebben openstaan, moet u bepalen wanneer en hoe u hen wilt aanmanen. Daarnaast kunt u hun rekening eventueel debiteren met rente of kosten. U kunt zoveel aanmaningscondities instellen als u wilt. Voor elke aanmaningsconditiecode kunt u een onbeperkt aantal aanmaningsniveaus definiëren.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "Pictogram Zoeken naar pagina of rapport"), voer **Aanmaningscondities** in en klik vervolgens op de gerelateerde koppeling.  
2. Vul indien nodig de velden in.  
3. Als u meer dan één combinatie van aanmaningscondities wilt gebruiken, stelt u een code in voor elke.

## <a name="to-set-up-reminder-levels"></a>Aanmaningsniveaus volgt instellen
De instelling van niveau 1 wordt gebruikt als er voor het eerst een aanmaning wordt gemaakt voor een klant. Wanneer de aanmaning wordt verstuurd, wordt het niveau geregistreerd in de aanmaningsposten die worden gemaakt en gekoppeld aan de individuele klantposten. Als het nodig is om de klant nog eens aan te manen, worden alle aanmaningposten die zijn gekoppeld aan open klantposten gecontroleerd op wat het hoogst gebruikte niveau is. De voorwaarden van het volgende niveau worden dan gebruikt voor de nieuwe aanmaning.

Als u meer aanmaningen maakt dan waar u niveaus voor hebt gedefinieerd, worden de voorwaarden van het hoogste niveau gebruikt. U kunt zoveel aanmaning maken als ingesteld in het veld **Max. aantal aanmaningen** in de aanmaningscondities.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "Pictogram Zoeken naar pagina of rapport"), voer **Aanmaningscondities** in en klik vervolgens op de gerelateerde koppeling.  
2. Selecteer in het venster **Aanmaningscondities** de regel met de condities waarvoor u niveaus wilt instellen en kies vervolgens de actie **Niveaus**.  
3. Vul indien nodig de velden in.  

    Voor elk aanmaningsniveau kunt u afzonderlijke voorwaarden specificeren, waaronder extra kosten in zowel de lokale valuta als in vreemde valuta. U kunt allerlei toeslagen in vreemde valuta's definiëren voor elke code in het venster **Aanmaningsniveaus**.
4. Kies de actie **Valuta's**.
5. Definieer in het venster **Valuta's voor aanmaningsniveau** voor elke aanmaningsniveaucode en corresponderend aanmaningsniveaunummer een valutacode en een toeslag.

    > [!NOTE]  
    > De valutacondities die u hier hebt ingesteld, worden gebruikt wanneer u aanmaningen maakt in een vreemde valuta. Als u geen condities voor aanmaningen in vreemde valuta's hebt ingesteld, worden de condities die in de tabel **Aanmaningsniveau** zijn ingesteld, gebruikt en vervolgens omgerekend naar de betreffende valuta.

    Voor elk aanmaningsniveau kunt u tekst specificeren die wordt afgedrukt vóór (**Begintekst**) of na (**Eindtekst**) in de posten op de aanmaning.

6. Kies respectievelijk de acties **Begintekst** of **Eindtekst** en vul het venster **Aanmaningstekst** in.
7. Als u automatisch gerelateerde waarden in de resulterende aanmaningstekst wilt invoegen, voert u de volgende tijdelijke aanduidingen in het veld **Tekst** in.  

|Tijdelijke aanduiding|Waarde|  
|-----------------|-----------|  
|%1|Inhoud van het veld **Documentdatum** in de aanmaningskop|  
|%2|Inhoud van het veld **Vervaldatum** in de aanmaningskop|  
|%3|Inhoud van het veld **Rente** in de relateerde rentefactuurcondities|  
|%4|Inhoud van het veld **Restbedrag** in de aanmaningskop|  
|%5|Inhoud van het veld **Rentebedrag** in de aanmaningskop|  
|%6|Inhoud van het veld **Toeslag** in de aanmaningskop|  
|%7|Het totaalbedrag van de aanmaning|  
|%8|Inhoud van het veld **Aanmaningsniveau** in de aanmaningskop|  
|%9|Inhoud van het veld **Valutacode** in de aanmaningskop|  
|%10|Inhoud van het veld **Boekingsdatum** in de aanmaningskop|  
|%11|De bedrijfsnaam|  
|%12|Inhoud van het veld **Toeslag per regel** in de aanmaningskop|  

Als u schrijft **U bent %9 %7 verschuldigd op %2**, bevat de resulterende aanmaning bijvoorbeeld de volgende tekst: U bent **USD 1200,50 verschuldigd op 02-02-2014.**

Nadat u de aanmaningscondities hebt ingesteld (met aanvullende niveaus en tekst), voert u een van de codes in op elke klantenkaart. Zie [Procedure: Nieuwe klanten registreren](sales-how-register-new-customers.md) voor meer informatie.

## <a name="to-create-a-reminder-automatically"></a>Automatisch een aanmaningen maken
Een herinnering is te vergelijken met een factuur. Wanneer u een aanmaning maakt, moeten een aanmaningskop, evenals een of meer aanmaningsregels, worden ingevuld. U kunt een functie gebruiken om automatisch aanmaningen te maken voor alle klanten.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "Pictogram Zoeken naar pagina of rapport"), voer **Aanmaningen** in en klik vervolgens op de gerelateerde koppeling.
2. Kies in het venster **Aanmaning** de actie **Aanmaningen maken**.
3. Vul in het venster **Aanmaningen maken** de velden in om te definiëren hoe en naar wie de aanmaningen worden gemaakt.
4. Kies de knop **OK**.

## <a name="to-create-a-reminder-manually"></a>Handmatig aanmaningen maken
In het venster **Aanmaning** kunt u het sneltabblad **Algemeen** handmatig invullen en de regels vervolgens automatisch laten invullen.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "Pictogram Zoeken naar pagina of rapport"), voer **Aanmaningen** in en klik vervolgens op de gerelateerde koppeling.
2. Kies de actie **Nieuw**.
3. Vul indien nodig de velden op het sneltabblad **Algemeen** in.
4. Kies de actie **Aanmaningsregels voorstellen**.
5. Vul in de batchverwerking **Aanmaningsregels voorstellen** de velden in om te definiëren hoe en naar wie de aanmaningen worden gemaakt.
6. Schakel het selectievakje **Wachtende posten opnemen** in als ook u wachtende, openstaande posten wilt opnemen in de aanmaningen.

    > [!Important]
    > De openstaande die wachtend zijn, worden ingevoegd, ongeacht de instelling van het selectievakje Alleen vervallen posten.

7. Kies de knop **OK**.

## <a name="to-replace-reminder-texts"></a>Aanmaningsteksten vervangen  
U kunt op verschillende manieren bepalen hoe u tekst wilt weergegeven op de afgedrukte aanmaning. In sommige gevallen kunt u de begin- en eindtekst die u hebt gedefinieerd voor het huidige niveau vervangen door de tekst van een ander niveau.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "Pictogram Zoeken naar pagina of rapport"), voer **Aanmaningen** in en klik vervolgens op de gerelateerde koppeling.
2. Open de relevante aanmaning en kies de actie **Aanmaningstekst bijwerken**.
3. Voer in het venster **Aanmaningstekst bijwerken** het vereiste niveau in het veld **Aanmaningsniveau** in.
3. Klik op **OK** om de begin- en eindtekst bij te werken.

## <a name="to-issue-a-reminder"></a>Een aanmaning verzenden
Nadat u aanmaningen hebt gemaakt en eventuele aanpassingen hebt gedaan, kunt u testrapporten afdrukken of de aanmaningen versturen.

Wanneer u een aanmaning verstuurt, worden de gegevens overgebracht naar een afzonderlijk venster voor verstuurde aanmaningen. Tegelijkertijd worden aanmaningsposten geboekt. Als er rente of aanmaningskosten in rekening zijn gebracht worden posten zowel geboekt als klantpost als in het grootboek.

Wanneer een aanmaning is verzonden, worden de posten geboekt volgens uw specificaties in het venster **Aanmaningscondities**. Op basis van deze specificatie wordt bepaald welke rente en/of toeslagen worden geboekt naar de klantenrekening en het grootboek. De instelling in het venster **Klantboekingsgroepen** bepaalt naar welke rekening de boekingen worden uitgevoerd.

Voor elke klantenpost op de rentefactuur wordt een post gemaakt in het venster **Aanmanings-/rentefactuurposten**.

Als de selectievakjes **Rente boeken** of **Toeslag boeken** in het venster **Aanmaningscondities** zijn ingeschakeld, worden ook de volgende posten gemaakt:

- Eén post in de tabel **Klantenposten**
- Eén debiteurenpost in de desbetreffende grootboekrekening
- Eén rentepost en/of één toeslagpost in de desbetreffende grootboekrekening

Daarnaast kunnen btw-posten worden gemaakt als u de aanmaning verzendt.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "Pictogram Zoeken naar pagina of rapport"), voer **Aanmaningen** in en klik vervolgens op de gerelateerde koppeling.
2. Selecteer de desbetreffende aanmaning en kies vervolgens de actie **Verzenden**.
3. Vul in het venster **Aanmaningen verzenden** de benodigde velden in.
4. Kies de knop **Ok**.

Een aanmaning wordt afgedrukt of verzonden naar een opgegeven e-mailadres als PDF-bijlage.

## <a name="to-set-up-finance-charge-terms"></a>Rentefactuurcondities instellen
U moet een code instellen waarmee elke renteberekening wordt aangeduid. Vervolgens kunt u deze code opgeven in het veld **Rentefactuurconditie** op de leverancierskaarten.

U berekent rentefacturen via de rentedagenmethode of de methode voor openstaande saldi.

Bij de methode Openstaand bedrag is de rente een percentage van het openstaande bedrag:  

    Balance Due method - Finance Charge = Overdue Amount x (Interest Rate / 100)

Bij de methode Rentedagen wordt rekening gehouden met het aantal dagen dat de betalingstermijn is overschreden:  

    Average Daily Balance method - Finance Charge = Overdue Amount x (Days Overdue / Interest Period) x (Interest Rate/100)

Elke code in de tabel Rentefactuurconditie is bovendien gekoppeld aan de subtabel Rentefactuurtekst. Voor elke set rentefactuurcondities kunt u een begin- en/of eindtekst definiëren die op de rentefactuur wordt opgenomen.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "Pictogram Zoeken naar pagina of rapport"), voer **Rentefactuurcondities** in en klik vervolgens op de gerelateerde koppeling.  
2. Vul indien nodig de velden in.  
3. Als u meer dan één combinatie van rentefactuurcondities wilt gebruiken, stelt u een code in voor elke.

    Voor elk rentefactuurconditie kunt u afzonderlijke voorwaarden specificeren, waaronder extra kosten in zowel de lokale valuta als in vreemde valuta. U kunt allerlei toeslagen in vreemde valuta's definiëren voor elke code in het venster **Rentefactuurcondities**.
4. Kies de actie **Valuta's**.
5. In het venster **Valuta's voor rentefactuurcondities** definieert u voor elke conditie een valutacode en een toeslag.

    > [!NOTE]  
    > Wanneer u aanmaningskosten in een vreemde valuta maakt, worden de vreemdevalutacondities die u instelt, gebruikt om rentefacturen te maken. Als u geen condities voor rentefactuurcondities in vreemde valuta's hebt ingesteld, worden de condities in de lokale valuta uit het venster **Rentefactuurcondities** gebruikt en omgerekend naar de betreffende valuta.

    Voor elke rentefactuurconditie kunt u tekst opgeven die wordt afgedrukt vóór (**Begintekst**) of na (**Eindtekst**) in de posten op de rentefactuur.  
6. Kies respectievelijk de acties **Begintekst** of **Eindtekst** en vul het venster **Rentefactuurtekst** in.
7. Als u automatisch gerelateerde waarden in de resulterende rentefactuurtekst wilt invoegen, voert u de volgende tijdelijke aanduidingen in het veld **Tekst** in.

|Tijdelijke aanduiding|Waarde|  
|-----------------|-----------|  
|%1|Inhoud van het veld **Documentdatum** in de rentefactuurkoptekst|  
|%2|Inhoud van het veld **Vervaldatum** in de rentefactuurkoptekst|  
|%3|Inhoud van het veld **Rente** in de relateerde rentefactuurcondities|  
|%4|Inhoud van het veld **Restbedrag** in de rentefactuurkoptekst|  
|%5|Inhoud van het veld **Rentebedrag** in de rentefactuurkoptekst|  
|%6|Inhoud van het veld **Toeslag** in de rentefactuurkoptekst|  
|%7|Het totaalbedrag van de aanmaning|  
|%8|Inhoud van het veld **Valutacode** in de rentefactuurkoptekst|  
|%9|Inhoud van het veld **Boekingsdatum** in de rentefactuurkoptekst|  

## <a name="to-create-a-finance-charge-memo-manually"></a>Handmatig rentefacturen maken  
Een rentefactuur is te vergelijken met een factuur. U kunt een kop handmatig en de regels automatisch invullen of u kunt automatisch rentefacturen voor alle klanten maken.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "Pictogram Zoeken naar pagina of rapport"), voer **Rentefacturen** in en klik vervolgens op de gerelateerde koppeling.  
2. Kies de actie **Nieuw** en vul indien nodig de velden in.  
3. Kies de actie **Rentefactuurregels voorstellen**.
4. Stel in het venster **Rentefactuur** een filter in op het sneltabblad **Klantenpost** als u alleen rentefacturen voor specifieke posten wilt maken.  
5.  Kies **OK** om de batchverwerking te starten.  

## <a name="to-update-finance-charge-memo-texts"></a>De rentefactuurteksten bijwerken  
Het kan zijn dat u de begin- en eindtekst die u voor de rentefactuurcondities hebt ingesteld, wilt bijwerken. Als u dat doet op een moment waarop u de rentefacturen hebt gemaakt, maar nog niet hebt verzonden, kunt u de facturen bijwerken met de gewijzigde tekst.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "Pictogram Zoeken naar pagina of rapport"), voer **Rentefactuur** in en klik vervolgens op de gerelateerde koppeling.  
2. open de rentefactuur waarvoor u tekst wilt wijzigen en kies vervolgens de actie **Rentefactuurtekst bijwerken**.
3. Op het sneltabblad **Rentefactuurtekst bijwerken** kunt u een filter instellen als u verschillende facturen wilt bijwerken.
4. Klik op **OK** om de begin- en eindtekst bij te werken.  

## <a name="to-issue-finance-charge-memos"></a>Rentefacturen verzenden
Nadat u de rentefacturen hebt gemaakt en eventuele aanpassingen hebt gedaan, kunt u testrapporten afdrukken of de rentefacturen versturen.

Wanneer een aanmaning is verzonden, worden de posten geboekt volgens uw specificaties in het venster **Rentefactuurcondities**. Op basis van deze specificatie wordt bepaald welke rente en/of toeslagen worden geboekt naar de klantenrekening en het grootboek. De instelling in het venster **Klantboekingsgroepen** bepaalt naar welke rekening de boekingen worden uitgevoerd.

Voor elke klantenpost op de rentefactuur wordt een post gemaakt in het venster **Aanmanings-/rentefactuurposten**.

Als de selectievakjes **Rente boeken** of **Toeslag boeken** in het venster **Rentefactuurcondities** zijn ingeschakeld, worden ook de volgende posten gemaakt:

- Eén post in de tabel **Klantenposten**
- Eén debiteurenpost in de desbetreffende grootboekrekening
- Eén rentepost en/of één toeslagpost in de desbetreffende grootboekrekening

Daarnaast kunnen btw-posten worden gemaakt als u de rentefactuur verzendt.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "Pictogram Zoeken naar pagina of rapport"), voer **Rentefacturen** in en klik vervolgens op de gerelateerde koppeling.
2. Selecteer de desbetreffende rentefactuur en kies vervolgens de actie **Verzenden**.
3. Vul in het venster **Rentefacturen verzenden** de benodigde velden in.
4. Kies de knop **Ok**.

Een rentefactuur wordt afgedrukt of verzonden naar een opgegeven e-mailadres als PDF-bijlage.

## <a name="to-view-reminder-and-finance-charge-entries"></a>Aanmanings- en renteposten weergeven  
Zodra u een aanmaning verzendt, wordt in het venster **Aanmanings-/renteposten** een aanmaningspost gemaakt voor elke aanmaningsregel met een klantenpost. U kunt vervolgens in een overzicht weergeven welke aanmaningsposten u voor een bepaalde klant hebt gemaakt.    
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "Pictogram Zoeken naar pagina of rapport"), voer **Klanten** in en klik vervolgens op de gerelateerde koppeling.  
2. Open de desbetreffende klantenkaart en kies vervolgens de actie **Posten**.
3. Selecteer in het venster **Klantenposten** de regel met de post waarvan u de aanmaningsposten wilt weergeven, en kies de actie **Aanmanings-/rentefactuurposten**.

## <a name="see-also"></a>Zie ook
[Tegoeden beheren](receivables-manage-receivables.md)  
[Verkoop](sales-manage-sales.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


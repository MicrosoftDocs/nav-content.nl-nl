---
title: Betalingstolerantie en contantkortingstolerantie.
description: U kunt de betalingstolerantie instellen om een factuur te sluiten wanneer de betaling het bedrag op de factuur niet volledig dekt.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/10/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 1cd3d0ea7e1543707dbc197eec02d0691dd8e42c
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-work-with-payment-tolerances-and-payment-discount-tolerances"></a>Procedure: Werken met betalingstolerantie en contantkortingstolerantie
U kunt een betalingstolerantie instellen om een factuur te sluiten wanneer de betaling het bedrag op de factuur niet volledig dekt. U kunt een contantkortingstolerantie instellen om een contantkorting te verlenen nadat de datum van de betalingskorting is verstreken.  

U kunt betalingstoleranties gebruiken, zodat elk openstaand bedrag een vastgestelde maximumbetalingstolerantie heeft. Als aan de betalingstolerantie wordt voldaan, wordt het betalingsbedrag geanalyseerd. Als het betalingsbedrag ontoereikend is, wordt het openstaande bedrag volledig afgesloten door de ontoereikende betaling. Er wordt een gedetailleerde post op de betalingspost geboekt, zodat er geen restbedrag overblijft op de vereffende factuurpost. Als het betalingsbedrag te hoog is, wordt een nieuwe gedetailleerde post geboekt op de betalingspost, zodat er geen restbedrag overblijft op de betalingspost.

U kunt contantkortingstoleranties gebruiken, zodat als u een betalingskorting accepteert nadat de betalingskortingsdatum is verstreken, deze altijd wordt geboekt naar de contantkortingsrekening of een betalingstolerantierekening.

## <a name="applying-payment-tolerance-to-multiple-documents"></a>Betalingstolerantie voor meerdere documenten toepassen  
Documenten hebben altijd dezelfde betalingstolerantie, ongeacht of ze afzonderlijk of samen met andere documenten worden vereffend. Acceptatie van een late contantkorting wanneer u betalingstolerantie op meerdere documenten toepast, vindt automatisch plaats voor elk document waarin de volgende regel is ingesteld op true:  

*contantkortingsdatum < betaaldatum in geselecteerde post <= betalingstolerantiedatum*  

Deze regel wordt ook gebruikt om te bepalen of er waarschuwingen moeten worden weergegeven wanneer u betalingstolerantie op meerdere documenten toepast. De waarschuwing voor contantkortingstolerantie wordt voor elke post weergegeven die voldoet aan de datumcriteria. Zie 'Voorbeeld 2 - Tolerantieberekeningen voor meervoudige documenten' voor meer informatie. 

U kunt kiezen om een waarschuwing weer te geven die is gebaseerd op tolerantie in verschillende situaties.  

- De eerste waarschuwing heeft betrekking op de contantkortingstolerantie. U krijgt de mogelijkheid een late contantkorting goed te keuren. U kunt vervolgens kiezen of de tolerantie op de kortingsvervaldatum moet worden geaccepteerd.  
- De tweede waarschuwing heeft betrekking op de betalingstolerantie. U krijgt een melding dat alle posten kunnen worden afgesloten, aangezien het verschil minder is dan het totaal van de maximumbetalingstolerantie voor de vereffende posten. U kunt vervolgens kiezen of de tolerantie op het betalingsbedrag moet worden geaccepteerd.

Zie voor meer informatie de sectie 'Betalingstolerantiewaarschuwingen in- of uitschakelen'.     

## <a name="to-set-up-tolerances"></a>Toleranties instellen  
Met toleranties voor dagen en bedragen kunt u een factuur ook afsluiten als het betalingsbedrag niet gelijk is aan het volledige factuurbedrag. De reden hiervoor kan zijn dat de vervaldatum voor de betalingskorting is overschreden, dat er goederen zijn afgetrokken of dat er een kleine fout is gemaakt. Dit geldt ook voor restituties en creditnota's.  

U kunt pas toleranties instellen als u verschillende tolerantierekeningen hebt ingesteld, boekingsmethoden voor zowel contantkortingstolerantie als betalingstolerantie hebt opgegeven en vervolgens de batchverwerking **Betalingstolerantie wijzigen** hebt uitgevoerd.  
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Boekingsgroepinstellingen** in en klik vervolgens op de gerelateerde koppeling.  
2. Stel in het venster **Boekingsgroepinstellingen** een debet- en een creditrekening voor verkoopbetalingstolerantie in en een debet- en creditrekening voor inkoopbetalingstolerantie.  
3. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Klantboekingsgroepen** in en klik vervolgens op de gerelateerde koppeling.    
4. Stel in het venster **Klantboekingsgroepen** een debet- en een creditrekening voor betalingstolerantie in. Zie [Boekingsgroepen instellen](finance-posting-groups.md) voor meer informatie.  
5. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Boekingsgroepinstellingen** in en klik vervolgens op de gerelateerde koppeling.  
6. Stel in het venster **Leveranciersboekingsgroepen** een debet- en een creditrekening voor betalingstolerantie in.  
7. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Grootboekinstellingen** in en klik vervolgens op de gerelateerde koppeling.  
8. Open het venster **Boekhoudinstellingen**.  
9. Vul op het sneltabblad **Vereffening** de velden **Betalingstolerantieboeking**, **Respijtperiode contantkorting** en **Betalingstolerantieboeking** in.   
10. Kies de actie **Betalingstolerantie wijzigen**.
11. Vul in het venster **Betalingstolerantie wijzigen** de velden **Betalingstolerantie %** en **Max. betalingstolerantiebedrag** in en kies vervolgens de knop **OK**.

> [!IMPORTANT]  
>  U hebt nu alleen voor de lokale valuta een tolerantie ingesteld. Als u wilt dat tolerantie voor betalingen, creditnota's en terugbetalingen in een vreemde valuta worden afgehandeld door [!INCLUDE[d365fin](includes/d365fin_md.md)], moet u de batchverwerking **Betalingstolerantie wijzigen** uitvoeren met een waarde in het veld **Valutacode**.  

> [!NOTE]  
>  Als u telkens wanneer u een vereffening toepast in de tolerantie een betalingstolerantiewaarschuwing wilt krijgen, moet u de betalingstolerantiewaarschuwing inschakelen. Zie voor meer informatie de sectie 'Betalingstolerantiewaarschuwingen in- of uitschakelen'.  
>   
>  Als u tolerantie wilt uitschakelen voor een klant of leverancier, moet u toleranties blokkeren op de relevante klanten- of leverancierskaart. Zie voor meer informatie de sectie 'Betalingstolerantie voor klanten blokkeren'.  
>   
>  Wanneer u toleranties instelt, controleert [!INCLUDE[d365fin](includes/d365fin_md.md)] ook of er openstaande posten zijn en wordt de tolerantie ook voor deze posten berekend.

## <a name="to-enable-or-disable-payment-tolerance-warnings"></a>Betalingstolerantiewaarschuwingen in- of uitschakelen
De betalingstolerantiewaarschuwing verschijnt wanneer u een vereffening boekt die een saldo heeft binnen de toegestane tolerantie. Vervolgens kiest u hoe u het saldo wilt boeken en vastleggen.    
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Grootboekinstellingen** in en klik vervolgens op de gerelateerde koppeling.  
2. Schakel in het venster **Grootboekinstellingen** op het sneltabblad **Vereffening** het selectievakje **Betalingstolerantiewaarschuwing** in om de waarschuwing te activeren. Schakel het selectievakje uit als u de waarschuwing wilt deactiveren.  

> [!NOTE]  
>  De standaardoptie voor het venster **Betalingstolerantiewaarschuwing** is **Saldo behouden als restbedrag**. De standaardoptie voor het venster **Cont.-kortingstolerantiewaarschuwing** is **Late contantkorting niet aanvaarden**.

## <a name="to-block-payment-tolerance-for-customers"></a>Betalingstolerantie voor klanten blokkeren  
Betalingstolerantie wordt standaard toegestaan. Als u geen betalingstolerantie wilt toestaan voor een bepaalde klant of leverancier, moet u de tolerantie op de desbetreffende klanten- of leverancierskaart blokkeren. Hierna wordt beschreven hoe u dit doet voor een klant. De stappen zijn vergelijkbaar voor een leverancier.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Klant** of **Leverancier** in en klik vervolgens op de gerelateerde koppeling.  
2. Schakel op de het sneltabblad **Betalingen** het selectievakje **Betalingstolerantie blokkeren** in .  

> [!NOTE]  
>  Als de klant of leverancier openstaande posten heeft, moet u eerst de betalingstolerantie verwijderen voor posten die momenteel openstaan.

## <a name="example-1---tolerance-calculations-for-a-single-document"></a>Voorbeeld 1 - tolerantieberekeningen voor één document
Hieronder vindt u enkele voorbeeldscenario's waarin de verwachte tolerantieberekeningen en -boekingen in verschillende situaties worden behandeld.  

Het venster **Grootboekinstellingen** bevat de volgende instellingen:
- Respijtperiode contantkorting: 5 dagen  
- Max. betalingstolerantie: 5  

Scenario's met alternatief A of B vertegenwoordigen het volgende:  

- **A** In dit geval is de waarschuwing voor contantkortingstolerantie uitgeschakeld OF heeft de gebruiker de waarschuwing aan staan en geselecteerd om de late contantkorting toe te staan (het saldo boeken als betalingstolerantie).  
- **B** In dit geval heeft de gebruiker de waarschuwing ingeschakeld en geselecteerd de late contantkorting niet toe te staan (Saldo laten als Restbedrag).  

|—|Factuur|Contantk.|Max.<br /><br /> Bet.-tol.|Datum contantk.|Contantk.-tol. Datum|Betaaldatum|Bet.|Tolerantiesoort|Alle posten gesloten|Contantk.-tol. <br /> GB/vlottende passiva|Bet.<br /><br /> Tol.<br /><br /> GB|  
|-------|----------|----------------|-----------------------|---------------------|--------------------------|------------------|----------|--------------------|------------------------|------------------------------|----------------------------|  
|1|1.000|20|5|15-01-03|20-01-03|<=15.01.03|985|Bet.-tol.|Ja|0|-5|  
|2|**1,000**|**20**|**5**|**15.01.03**|**01/20/03**|**<=15.01.03**|**980**|**Geen**|**Ja**|**0**|**0**|  
|3|1.000|20|5|15-01-03|20.01.03|<=15.01.03|975|Bet.-tol.|Ja|0|5|  
|4A|1.000|20|5|15-01-03|20-01-03|16-01-03 20-01-03|1005|Contantk.-tol.|Nee, 25 op de bet.|20/-20|0|  
|5A|1.000|20|5|15-01-03|20-01-03|16-01-03 20-01-03|1000|Contantk.-tol.|Nee, 20 op de bet.|20/-20|0|  
|6A|1.000|20|5|15-01-03|20-01-03|16-01-03 20-01-03|995|Contantk.-tol.|Nee, 15 op de bet.|20/-20|0|  
|4B|1.000|20|5|15-01-03|20-01-03|16-01-03 20-01-03|1005|Bet.-tol.|Ja|0|-5|  
|**5B**|**1,000**|**20**|**5**|**15.01.03**|**01/20/03**|**16-01-03 20-01-03**|**1000**|**Geen**|**Ja**|**0**|**0**|  
|6B|1.000|20|5|15-01-03|20-01-03|16-01-03 20-01-03|995|Bet.-tol.|Ja|0|5|  
|7|1.000|20|5|15-01-03|20-01-03|16-01-03 20-01-03|985|Contantk.-tol. & Bet.-tol.|Ja|20/-20|-5|  
|8|1.000|20|5|15-01-03|20-01-03|16-01-03 20-01-03|980|Contantk.-tol.|Ja|20/-20|0|  
|9|1.000|20|5|15-01-03|20-01-03|16-01-03 20-01-03|975|Contantk.-tol. & Bet.-tol.|Ja|20/-20|5|  
|10|1.000|20|5|15-01-03|20-01-03|>20.01.03|1005|Bet.-tol.|Ja|0|-5|  
|**11**|**1,000**|**20**|**5**|**15.01.03**|**01/20/03**|**>20.01.03**|**1000**|**Geen**|**Ja**|**0**|**0**|  
|12|1.000|20|5|15-01-03|20-01-03|>20.01.03|995|Bet.-tol.|Ja|0|5|  
|13|1.000|20|5|15-01-03|20-01-03|>20.01.03|985|Geen|Nee, 15 op de factuur|0|0|  
|14|1.000|20|5|15-01-03|20-01-03|>20.01.03|980|Geen|Nee, 20 op de factuur|0|0|  
|15|1.000|20|5|15-01-03|20-01-03|>20.01.03|975|Geen|Nee, 25 op de factuur|0|0|  

### <a name="payment-range-diagrams"></a>Betalingsbereikdiagrammen  
Het bovenstaande scenario resulteert in de volgende diagrammen met betalingsbereiken:  

#### <a name="1-payment-date-011503-scenarios-1-3"></a>(1) Betaaldatum <=15.01.03 (scenario's 1-3)  
Restbedrag per  

Normale vereffeningsregels  

![Afzonderlijke betalingstolerantieregels &#40;vóór 03&#47;15&#41;](media/singlePmtTolRules(Pre1503).gif "singlePmtTolRules(Pre1503)")  

(1) Als de betaling binnen dit bereik valt, kunnen alle vereffeningsposten, met of zonder tolerantie, worden afgesloten.  

(2) Als de betaling binnen dit bereik valt, kunnen er geen vereffeningsposten worden afgesloten, ook niet met tolerantie.  

#### <a name="2-payment-date-is-between-011603-and-012003-scenarios-4-9"></a>(2) Betaaldatum ligt tussen 16.01.03 en 20.01.03 (scenario's 4-9)  
Restbedrag per  

Normale vereffeningsregels  

![Afzonderlijke betalingstolerantieregels &#40;respijtperiode&#41;](media/singlePmtTolRules(GracePeriod).gif "singlePmtTolRules(GracePeriod)")  

(1) Als de betaling binnen dit bereik valt, kunnen alle vereffeningsposten, met of zonder tolerantie, worden afgesloten.  

(2) Als de betaling binnen dit bereik valt, kunnen er geen vereffeningsposten worden afgesloten, ook niet met tolerantie.  

#### <a name="3-payment-date-is-after-012003-scenarios-10-15"></a>(3) Betaaldatum valt na 20.01.03 (scenario's 10-15)  
Restbedrag per  

Normale vereffeningsregels  

![Afzonderlijke betalingstolerantieregels &#40;vóór 01&#47;20&#41;](media/singlePmtTolRules(Post0120).gif "singlePmtTolRules(Post0120)")  

(1) Als de betaling binnen dit bereik valt, kunnen alle vereffeningsposten, met of zonder tolerantie, worden afgesloten.  

(2) Als de betaling binnen dit bereik valt, kunnen er geen vereffeningsposten worden afgesloten, ook niet met tolerantie.  

## <a name="example-2---tolerance-calculations-for-multiple-documents"></a>Voorbeeld 2 - tolerantieberekeningen voor meerdere documenten
Hieronder vindt u enkele voorbeeldscenario's waarin de verwachte tolerantieberekeningen en -boekingen in verschillende situaties worden behandeld. De voorbeelden zijn beperkt tot de scenario's waarbij alle posten bij de vereffening worden afgesloten.  

Het venster **Grootboekinstellingen** bevat de volgende instellingen:
- Respijtperiode contantkorting 5 dagen  
- Max. betalingstolerantie 5  

Scenario's met alternatief A, B, C of D vertegenwoordigen het volgende:  

- **A** In dit geval is de waarschuwing voor contantkortingstolerantie uitgeschakeld OF de gebruiker heeft de waarschuwing aan staan en heeft geselecteerd de late contantkorting voor elke factuur toe te staan (Boeken als tolerantie).  
- **B** In dit geval heeft de gebruiker de waarschuwing ingeschakeld en geselecteerd de late contantkorting voor geen enkele factuur toe te staan.  
- **C** In dit geval heeft de gebruiker de waarschuwing ingeschakeld en geselecteerd om de late contantkorting toe te staan voor de eerste factuur, maar niet voor de tweede.  
- **D** In dit geval heeft de gebruiker de waarschuwing ingeschakeld en geselecteerd om de late contantkorting niet toe te staan voor de eerste factuur, maar wel voor de tweede.  

|—|Factuur|Contantk.|Max. bet.-tol.|Datum contantk.|Contantk.-tol. Datum|Betaaldatum|Bet.|Tolerantiesoort|Alle posten gesloten|Contantk.-tol. <br /> GB/vlottende passiva|Bet.-tol.<br /><br /> GB|  
|-------|----------|---------------|-------------------|---------------------|--------------------------|------------------|---------|--------------------|------------------------|------------------------------|------------------------|  
|1|1.000 <br />1.000|60 <br />30|5 <br />5|15-01-03 <br />17-01-03|20-01-03 <br />22.01.03|<=15.01.03|1920|Bet.-tol.|Ja|0<br /><br /> 0|-5 <br />-5|  
|**2**|**1,000** <br />**1,000**|**60** <br />**30**|**5** <br />**5**|**15.01.03** <br />**01/17/03**|**01/20/03** <br />**01/22/03**|**<=15.01.03**|**1910**|**Geen**|**Ja**|**0**<br /><br /> **0**|0 <br />0|  
|3|1.000 <br />1.000|60 <br />30|5 <br />5|15-01-03 <br />17-01-03|20-01-03 <br />22.01.03|<=15.01.03|1900|Bet.-tol.|Ja|0<br /><br /> 0|5 <br />5|  
|4B|1.000 <br />1.000|60 <br />30|5 <br />5|15-01-03 <br />17-01-03|20-01-03 <br />22.01.03|16-01-2003 17-01-2003|1980|Bet.-tol.|Ja|0<br /><br /> 0|-5<br /><br /> -5|  
|**5B**|**1,000** <br />**1,000**|**60** <br />**30**|**5** <br />**5**|**15.01.03** <br />**01/17/03**|**01/20/03** <br />**01/22/03**|**16-01-03 17-01-03**|**1970**|**Geen**|**Ja**|**0**<br /><br /> **0**|**0**<br /><br /> **0**|  
|6B|1.000 <br />1.000|60 <br />30|5 <br />5|15-01-03 <br />17-01-03|20-01-03 <br />22.01.03|16-01-2003 17-01-2003|1960|Bet.-tol.|Ja|0<br /><br /> 0|5<br /><br /> 5|  
|7A|1.000 <br />1.000|60 <br />30|5 <br />5|15-01-03 <br />17-01-03|20-01-03 <br />22.01.03|16-01-2003 17-01-2003|1920|Contantk.-tol. & Bet.-tol.|Ja|60/60<br /><br /> 0/0|-5 <br />-5|  
|8A|1.000 <br />1.000|60 <br />30|5 <br />5|15-01-03 <br />17-01-03|20-01-03 <br />22.01.03|16-01-2003 17-01-2003|1910|Contantk.-tol.|Ja|60/60<br /><br /> 0/0|0 <br />0|  
|9A|1.000 <br />1.000|60 <br />30|5 <br />5|15-01-03 <br />17-01-03|20-01-03 <br />22.01.03|16-01-2003 17-01-2003|1900|Contantk.-tol. & Bet.-tol.|Ja|60/60|5 <br />5|  
|10B|1.000 <br />1.000|60 <br />30|5 <br />5|15-01-03 <br />17-01-03|20-01-03 <br />22.01.03|18-1-2003 20-01-2003|2010|Bet.-tol.|Ja|0<br /><br /> 0|-5<br /><br /> -5|  
|**11B**|**1,000** <br />**1,000**|**60** <br />**30**|**5** <br />**5**|**15.01.03** <br />**01/17/03**|**01/20/03** <br />**01/22/03**|**18-01-03 20-01-03**|**2000**|**Geen**|**Ja**|**0**<br /><br /> **0**|**0**<br /><br /> **0**|  
|12B|1.000 <br />1.000|60 <br />30|5 <br />5|15-01-03 <br />17-01-03|20-01-03 <br />22.01.03|18-1-2003 20-01-2003|1990|Bet.-tol.|Ja|0<br /><br /> 0|5<br /><br /> 5|  
|13D|1.000 <br />1.000|60 <br />30|5 <br />5|15-01-03 <br />17-01-03|20-01-03 <br />22.01.03|18-1-2003 20-01-2003|1980|Contantk.-tol. & Bet.-tol.|Ja|0/0<br /><br /> 30/-30|-5 <br />-5|  
|14D|1.000 <br />1.000|60 <br />30|5 <br />5|15-01-03 <br />17-01-03|20-01-03 <br />22.01.03|18-1-2003 20-01-2003|1970|Contantk.-tol.|Ja|0/0<br /><br /> 30/-30|0 <br />0|  
|15D|1.000 <br />1.000|60 <br />30|5 <br />5|15-01-03 <br />17-01-03|20-01-03 <br />22.01.03|18-1-2003 20-01-2003|1960|Contantk.-tol. & Bet.-tol.|Ja|0/0<br /><br /> 30/-30|5 <br />5|  
|16D|1.000 <br />1.000|60 <br />30|5 <br />5|15-01-03 <br />17-01-03|20-01-03 <br />22.01.03|18-1-2003 20-01-2003|1950|Contantk.-tol. & Bet.-tol.|Ja|60/-60<br /><br /> 0/0|-5 <br />-5|  
|17D|1.000 <br />1.000|60 <br />30|5 <br />5|15-01-03 <br />17-01-03|20-01-03 <br />22.01.03|18-1-2003 20-01-2003|1940|Contantk.-tol.|Ja|60/-60<br /><br /> 0/0|0 <br />0|  
|18D|1.000 <br />1.000|60 <br />30|5 <br />5|15-01-03 <br />17-01-03|20-01-03 <br />22.01.03|18-1-2003 20-01-2003|1930|Contantk.-tol. & Bet.-tol.|Ja|60/-60<br /><br /> 0/0|5 <br />5|  
|19A|1.000 <br />1.000|60 <br />30|5 <br />5|15-01-03 <br />17-01-03|20-01-03 <br />22.01.03|18-1-2003 20-01-2003|1920|Contantk.-tol. & Bet.-tol.|Ja|60/-60<br /><br /> 30/-30|-5 <br />-5|  
|20A|1.000 <br />1.000|60 <br />30|5 <br />5|15-01-03 <br />17-01-03|20-01-03 <br />22.01.03|18-1-2003 20-01-2003|1910|Contantk.-tol.|Ja|60/-60<br /><br /> 30/-30|0 <br />0|  
|21A|1.000 <br />1.000|60 <br />30|5 <br />5|15-01-03 <br />17-01-03|20-01-03 <br />22.01.03|18-1-2003 20-01-2003|1900|Contantk.-tol. & Bet.-tol.|Ja|60/-60<br /><br /> 30/-30|5 <br />5|  
|22B|1.000 <br />1.000|60 <br />30|5 <br />5|15-01-03 <br />17-01-03|20-01-03 <br />22.01.03|21-1-2003 22-01-2003|2010|Bet.-tol.|Ja|0<br /><br /> 0|-5<br /><br /> -5|  
|**23B**|**1,000** <br />**1,000**|**60** <br />**30**|**5** <br />**5**|**15.01.03** <br />**01/17/03**|**01/20/03** <br />**01/22/03**|**21-01-03 22-01-03**|**2000**|**Geen**|**Ja**|**0**<br /><br /> **0**|**0**<br /><br /> **0**|  
|24B|1.000 <br />1.000|60 <br />30|5 <br />5|15-01-03 <br />17-01-03|20-01-03 <br />22.01.03|21-1-2003 22-01-2003|1990|Bet.-tol.|Ja|0<br /><br /> 0|5<br /><br /> 5|  
|25A|1.000 <br />1.000|60 <br />30|5 <br />5|15-01-03 <br />17-01-03|20-01-03 <br />22.01.03|21-1-2003 22-01-2003|1980|Contantk.-tol. & Bet.-tol.|Ja|0/0<br /><br /> 30/30|-5 <br />-5|  
|26A|1.000 <br />1.000|60 <br />30|5 <br />5|15-01-03 <br />17-01-03|20-01-03 <br />22.01.03|21-1-2003 22-01-2003|1970|Contantk.-tol.|Ja|0/0<br /><br /> 30/30|0 <br />0|  
|27A|1.000 <br />1.000|60 <br />30|5 <br />5|15-01-03 <br />17-01-03|20-01-03 <br />22.01.03|21-1-2003 22-01-2003|1960|Contantk.-tol. & Bet.-tol.|Ja|0/0<br /><br /> 30/30|5 <br />5|  
|28|1.000 <br />1.000|60 <br />30|5 <br />5|15-01-03 <br />17-01-03|20-01-03 <br />22.01.03|>22.01.03|2010|Bet.-tol.|Ja|0|-5|  
|**29**|**1,000** <br />**1,000**|**60** <br />**30**|**5** <br />**5**|**15.01.03** <br />**01/17/03**|**01/20/03** <br />**01/22/03**|**>22.01.03**|**2000**|**Geen**|**Ja**|**0**|**0**|  
|30|1.000 <br />1.000|60 <br />30|5 <br />5|15-01-03 <br />17-01-03|20-01-03 <br />22.01.03|>22.01.03|1990|Bet.-tol.|Ja|0|5|  

### <a name="payment-range-diagrams"></a>Betalingsbereikdiagrammen  
Het bovenstaande scenario resulteert in de volgende diagrammen met betalingsbereiken:  

#### <a name="1-payment-date-011503-scenarios-1-3"></a>(1) Betaaldatum <=15-01-03 (scenario's 1-3)  
Restbedrag per  

Normale vereffeningsregels  

![Meerdere betalingstolerantieregels &#40;vóór 03&#47;15&#41;](media/multiplePmtTolRules(Pre1503).gif "multiplePmtTolRules(Pre1503)")  

(1) Als de betaling binnen dit bereik valt, kunnen alle vereffeningsposten, met of zonder tolerantie, worden afgesloten.  

(2) Als de betaling binnen dit bereik valt, kunnen er geen vereffeningsposten worden afgesloten, ook niet met tolerantie.  

#### <a name="2-payment-date-is-between-011603-and-011703-scenarios-4-9"></a>(2) Betaaldatum ligt tussen 16.01.03 en 17.01.03 (scenario's 4-9)  
Restbedrag per  

Normale vereffeningsregels  

![Meerdere betalingstolerantieregels &#40;respijtperiode&#41;](media/multiplePmtTolRules(GracePeriodInv1).gif "multiplePmtTolRules(GracePeriodInv1)")  

(1) Als de betaling binnen dit bereik valt, kunnen alle vereffeningsposten, met of zonder tolerantie, worden afgesloten.  

(2) Als de betaling binnen dit bereik valt, kunnen er geen vereffeningsposten worden afgesloten, ook niet met tolerantie.  

#### <a name="3-payment-date-is-between-011803-and-012003-scenarios-10-21"></a>(3) Betaaldatum ligt tussen 18.01.03 en 20.01.03 (scenario's 10-21)  
Restbedrag per  

Normale vereffeningsregels  

![Meerdere betalingstolerantieregels &#40;respijtperiode&#41;](media/multiplePmtTolRules(GracePeriodInv1-2).gif "multiplePmtTolRules(GracePeriodInv1-2)")  

(1) Als de betaling binnen dit bereik valt, kunnen alle vereffeningsposten, met of zonder tolerantie, worden afgesloten.  

(2) Als de betaling binnen dit bereik valt, kunnen er geen vereffeningsposten worden afgesloten, ook niet met tolerantie.  

#### <a name="4-payment-date-is-between-012103-and-012203-scenarios-22-27"></a>(4) Betaaldatum ligt tussen 21-1-2003 en 22.01.03 (scenario's 22-27)  
Restbedrag per  

Normale vereffeningsregels  

![Meerdere betalingstolerantieregels &#40;respijtperiode&#41;](media/multiplePmtTolRules(GracePeriodInv2).gif "multiplePmtTolRules(GracePeriodInv2)")  

(1) Als de betaling binnen dit bereik valt, kunnen alle vereffeningsposten, met of zonder tolerantie, worden afgesloten.  

(2) Als de betaling binnen dit bereik valt, kunnen er geen vereffeningsposten worden afgesloten, ook niet met tolerantie.  

#### <a name="5-payment-date-is-after-012203-scenarios-28-30"></a>(5) Betaaldatum valt na 22.01.03 (scenario's 28-30)  
Restbedrag per  

Normale vereffeningsregels  

![Meerdere betalingstolerantieregels &#40;na 01&#47;22&#41;](media/multiplePmtTolRules(Post0122).gif "multiplePmtTolRules(Post0122)")  

(1) Als de betaling binnen dit bereik valt, kunnen alle vereffeningsposten, met of zonder tolerantie, worden afgesloten.  

(2) Als de betaling binnen dit bereik valt, kunnen er geen vereffeningsposten worden afgesloten, ook niet met tolerantie.

## <a name="see-also"></a>Zie ook  
[Financiën](finance.md)  
[Financiën instellen](finance-setup-finance.md)  
[Tegoeden beheren](receivables-manage-receivables.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


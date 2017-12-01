---
title: 'Procedure: Onderhanden werk voor een project berekenen'
description: Met projecten kunt u het verbruik van de bedrijfsresources plannen en de diverse kosten bijhouden die samenhangen met het resourceverbruik voor een bepaald project. Projecten brengen het verbruik met zich mee van arbeidsuren, machine-uren, voorraadartikelen en andere soorten verbruik die moeten worden bijgehouden terwijl het project voortduurt.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: ea0953192454302a83a9187cd6569905723fd150
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="walkthrough-calculating-work-in-process-for-a-job"></a>Procedure: Onderhanden werk voor een project berekenen
Met projecten kunt u het verbruik van de bedrijfsresources plannen en de diverse kosten bijhouden die samenhangen met het resourceverbruik voor een bepaald project. Projecten brengen het verbruik met zich mee van arbeidsuren, machine-uren, voorraadartikelen en andere soorten verbruik die moeten worden bijgehouden terwijl het project voortduurt. Als een project over langere tijd loopt, moet u deze kosten mogelijk overdragen naar een OHW-rekening (Onderhanden werk) op de balans terwijl het project wordt voltooid. Vervolgens kunt u de kosten en verkopen indien van toepassing verantwoorden in uw resultatenrekeningen.  

## <a name="about-this-walkthrough"></a>Informatie over deze procedure  
 In deze procedure worden de volgende taken beschreven:  

-   OHW berekenen.  
-   Een OHW-berekeningsmethode kiezen.  
-   Een deel van een project uitsluiten van OHW.  
-   OHW boeken naar de grootboekrekening.  
-   Een OHW-boeking terugdraaien.  

 In elke stap van het proces wordt de waarde berekend en worden de projecttransacties naar het grootboek verplaatst. De berekenings- en boekingsstappen zijn van elkaar gescheiden zodat u uw gegevens kunt controleren en wijzigingen kunt aanbrengen voordat de posten naar het grootboek worden geboekt. Daarom moet u controleren of alle gegevens correct zijn nadat u de batchverwerking voor berekening hebt uitgevoerd en voordat u de batchverwerking voor boeking hebt uitgevoerd.  

## <a name="roles"></a>Rollen  
 In deze procedure is projectteamlid Tricia de hoofdpersoon.  

## <a name="prerequisites"></a>Vereisten  
 Voordat u de stappen in dit overzicht kunt uitvoeren, moet [!INCLUDE[d365fin](includes/d365fin_md.md)] op uw computer zijn geïnstalleerd.  

## <a name="story"></a>Scenario  
 In dit scenario gaat het om het bedrijf Cronus International Ltd., een design- en consultancyfirma die nieuwe infrastructuren ontwerpt (conferentiezalen en kantoren) en inricht met meubels, accessoires en opslagruimten. Het werk bij CRONUS is voor het grootste deel projectgericht en projectteamlid Tricia gebruikt projecten om een overzicht te krijgen van de lopende projecten waaraan CRONUS werkt en de projecten die zijn voltooid. De projecten kunnen soms tamelijk lang zijn en meerdere maanden lopen. Tricia gebruikt een OHW-rekening voor het vastleggen van het onderhanden werk en het bijhouden van de kosten gedurende het project.  

## <a name="calculating-wip"></a>OHW berekenen  
 CRONUS heeft een langdurig project aangenomen dat nu is uitgebreid tot over meerdere rapportageperioden. Tricia, een lid van het projectteam berekent het onderhanden werk (OHW) om ervoor te zorgen dat de financiële rapportage van het bedrijf accuraat is.  

 Tijdens deze procedure selecteert Tricia een bepaalde groep taken die wordt opgenomen in de OHW-berekening. In het venster **Projecttaakregels** kan ze deze regels opgeven in de kolom **OHW-totaal**.  

 De volgende tabel beschrijft de volgende drie opties.  

|Veld|Description|  
|-------------------------------------|---------------------------------------|  
|**<blank>**|Leeg laten als de projecttaak deel uitmaakt van een groep taken.|  
|**Totaal**|Definieert de reeks of groep taken die zijn opgenomen in de berekening van OHW en verantwoording. Binnen de groep wordt elke projecttaak waarvoor **Taaksoort project** is ingesteld op **Boeken**, opgenomen in het OHW-totaal tenzij het veld **OHW-totaal** is ingesteld op **Uitgesloten**.|  
|**Uitgesloten**|Geldt alleen voor een taak met **Taaksoortproject** **Boeken**. De taak wordt niet meegenomen wanneer OHW en verantwoording worden berekend.|  

 In het volgende scenario past Tricia de methode Kostprijs toe, die door haar bedrijf standaard wordt gebruikt, om het OHW berekenen. Zij geeft aan welk deel van het project wordt meegenomen in de OHW-berekening door OHW-totaalwaarden toe te wijzen aan verschillende projecttaakregels.  

### <a name="to-calculate-wip"></a>OHW berekenen  

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Projecten** in en klik vervolgens op de gerelateerde koppeling.  
2.  Selecteer in de lijst **Projecten** het project **Deerfield** en kies de actie **Bewerken**. Hiermee opent u de projectkaart in de bewerkmodus.  

     OHW kan worden berekend op basis van Kostprijs, Verkoopprijs, Kostprijs van omzet, Percentage voltooid of Contract voltooid. In dit voorbeeld wordt door CRONUS de methode Kostprijs toegepast.  

3.  Kies op het sneltabblad **Boeking** het veld **OHW-methode** en selecteer **Kostprijs**.  
4.  Kies de actie **Projecttaakregels** en stel de volgende waarden in het veld **OHW-totaal** in.  

     De volgende tabel beschrijft de waarden.  

    |Projecttaaknr.|Veld OHW-totaal|  
    |------------------|----------------------|  
    |1130|Exclusief|  
    |1190|Totaal|  
    |1210|Exclusief|  
    |1310|Exclusief|  

5.  Kies de actie **OHW** en kies vervolgens de actie **OHW berekenen**.  
6.  In het venster **OHW voor project berekenen** kunt u een project selecteren waarvoor u OHW wilt berekenen. Selecteer op het sneltabblad **Project** **Deerfield** in het veld **Nr.**. te kiezen.  
7.  Voer in het veld **Boekingsdatum** een datum in die na de werkdatum ligt.
8.  Typ **1** in het veld **Documentnr.**. Hiermee maakt u een document waar u later, als u het wilt traceren, naar kunt verwijzen.  
9. Kies **OK** om de batchverwerking te starten. Er wordt een bericht weergegeven. Kies de knop **OK** om door te gaan. Sluit het venster **Projecttaakregels**.  

    > [!NOTE]  
    >  Het bericht geeft aan dat er waarschuwingen zijn in verband met de OHW-berekening. U gaat de waarschuwingen bekijken in de volgende procedure.  

10. Vouw op de kaart **Project** het sneltabblad **OHW en verantwoording** uit om de berekende waarden weer te geven. U kunt ook de **Boekingsdatum OHW** bekijken en eventuele waarden die naar het grootboek zijn geboekt.  

 Zoals u ziet, bedraagt de waarde voor **Verantw. totale kosten** 215,60 in de kolom **Te boeken**. Dit reflecteert de totale kostprijs van twee van de artikelen in groep projecttaken 1110 – 1130. Het derde artikel was ingesteld op **Uitgesloten** en dus is niet opgenomen in de OHW-berekening.  

### <a name="to-review-wip-warnings"></a>OHW-waarschuwingen bekijken  

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Cockpit OHW taak** in en klik vervolgens op de gerelateerde koppeling.  
2.  Selecteer het project **Deerfield** en kies vervolgens de actie **Waarschuwingen weergeven**.  
3.  Controleer in het venster **OHW-waarschuwingen project** de waarschuwing waaraan de taak is gekoppeld.  

 Na deze boekingsperiode moet Tricia het OHW opnieuw berekenen om het tot dan toe voltooide werk op te nemen.  

### <a name="to-recalculate-wip"></a>OHW opnieuw berekenen  

1.  Op de kaart **Project** kiest u de actie **OHW-posten** om de OHW-berekening weer te geven.  

     In het venster **OHW-posten project** ziet u de OHW-posten die de laatste keer zijn berekend voor een project ook als het OHW nog niet in het grootboek is geboekt.  

2.  U kunt de stappen volgen in de procedure waarin wordt uitgelegd hoe u OHW kunt herberekenen. Elke keer als het OHW wordt berekend, wordt een post gemaakt in het venster **OHW-posten project**.  
3.  Sluit het venster.  

> [!NOTE]  
>  Onderhanden werk en Verantwoording worden alleen berekend. Het wordt niet geboekt in het grootboek. Als u dat wel wilt doen, moet u de batchverwerking **OHW naar GB boeken** uitvoeren nadat u OHW en verantwoording hebt berekend.

## <a name="posting-wip-to-general-ledger"></a>OHW boeken naar het grootboek  
 Nadat Tricia het OHW voor dit project heeft berekend, kan ze het naar het grootboek boeken.  

### <a name="to-post-wip-to-general-ledger"></a>OHW naar het grootboek boeken  

1.  Selecteer het project **Deerfield** in de lijst **Projecten**.  
2.  Kies de actie **OHW** en kies vervolgens de actie **OHW naar GB boeken**.  
3.  Selecteer in het venster **Project-OHW naar GB boeken** de waarde **Deerfield** in het veld **Nr.** op het sneltabblad **Project**. veld.  
4.  Geef in het sneltabblad **Opties** in het veld **Tegenboekingsdocumentnr.** **1** op.  
5.  Kies de knop **OK** om OHW naar het grootboek te boeken.  
6.  Klik op **OK** om het bevestigingsvenster af te sluiten.  

     Nadat u de boeking hebt voltooid, kunt u de boekingsinformatie bekijken in het venster **GB-posten OHW**.  

7.  Selecteer in de lijst **Projecten** het project **Deerfield** en kies de actie **GB-posten OHW**.  

     In het venster **GB-posten OHW project** ziet u dat het OHW naar het grootboek is geboekt.  

8.  Sluit het venster.  
9. Open de kaart **Project** voor het project **Deerfield**.  
10. Zoals u ziet is nu op het sneltabblad **OHW en verantwoording** in de kolom **Geboekt** het veld **Verantw. totale kosten GB** ingevuld, waarmee wordt aangegeven met het OHW met succes naar het grootboek is geboekt.  
11. Kies de knop **OK** om de kaart te sluiten.  

## <a name="reversing-a-wip-posting"></a>Een OHW-boeking tegenboeken  
 Tricia bepaalt dat de projecttaken die zijn uitgesloten van de berekening van OHW hadden moeten worden berekend in OHW. Gelukkig kan ze de onjuiste boeking terugdraaien zonder dat ze nieuwe OHW-boekingen hoeft te boeken.  

### <a name="to-reverse-a-wip-posting"></a>Een OHW-boeking tegenboeken  

1.  Selecteer het project **Deerfield** in de lijst **Projecten**.  
2.  Kies de actie **OHW** en kies vervolgens de actie **OHW naar GB boeken**.  
3.  Selecteer in het venster **Project-OHW naar GB boeken** de waarde **Deerfield** in het veld **Nr.** op het sneltabblad **Project**. veld.  
4.  Geef in het sneltabblad **Opties** in het veld **Tegenboekingsdocumentnr.** **1** op.  
5.  Geef de oorspronkelijke boekingsdatum op in het veld **Tegenboekingsdatum**. Dit moet dezelfde datum zijn als u hebt gebruikt toen u voor het eerst het OHW berekende.  
6.  Schakel het selectievakje **Alleen tegenboeken** in. Hiermee wordt het eerder geboekte OHW teruggedraaid en het nieuwe OHW naar het grootboek geboekt.  
7.  Kies de knop **OK** om de batchverwerking uit te voeren en kies vervolgens de knop **OK** om het bevestigingsvenster te sluiten.  
8.  Open de kaart **Project** voor **Deerfield**.  
9. Controleer op het sneltabblad **OHW en verantwoording** of er geen geboekte OHW-posten zijn.  
10. Sluit dit venster.  
11. Selecteer in de lijst **Projecten** het project **Deerfield**, kies de actie **OHW** en kies vervolgens de actie **GB-posten OHW**. Bij de OHW-posten is het selectievakje **Omgekeerd** ingeschakeld.  
12. Sluit dit venster.  
13. U kunt teruggaan naar de **Projecttaakregels** voor het project, de vereiste onderdelen van het project in de OHW-berekening opnemen, het OHW opnieuw berekenen en de nieuwe waarde naar het grootboek boeken.  

    > [!NOTE]  
    >  Stel Tricia OHW had berekend en geboekt voor een project met onjuiste datums. Volgens de methode die eerder werd beschreven, kan zij de onjuiste boekingen tegenboeken, de datums corrigeren en de boekingen opnieuw naar het grootboek posten.  

## <a name="next-steps"></a>Volgende stappen  
 In dit scenario heeft u de stappen doorgenomen voor het berekenen van OHW in [!INCLUDE[d365fin](includes/d365fin_md.md)]. Bij grotere projecten kan het handig zijn om de kosten periodiek over te dragen naar een OHW-rekening terwijl het project wordt voltooid. In dit overzicht hebt u gezien hoe u taakregels uitsluit van een berekening. Ook hebt u gezien wanneer u een herberekening moet uitvoeren. En tot slot dit wordt in dit scenario aangegeven hoe u de OHW naar het grootboek boekt. Ook is een voorbeeld opgenomen van hoe u een OHW-post naar het grootboek kunt tegenboeken.  

## <a name="see-also"></a>Zie ook  
 [Procedures voor bedrijfsprocessen](walkthrough-business-process-walkthroughs.md)  
 [Procedure: Projecten plannen](walkthrough-managing-projects-with-jobs.md)   
 [OHW-methoden](projects-understanding-wip.md)   
 [Voortgang en prestaties bewaken](projects-how-monitor-progress-performance.md)  
 [Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


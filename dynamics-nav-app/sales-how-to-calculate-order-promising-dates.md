---
title: Ordertoezeggingsdatums berekenen
description: Met de functie Ordertoezegging wordt de vroegst mogelijke datum berekend waarop een artikel beschikbaar is voor verzending of levering. Met deze functie worden ook behoefteregels gemaakt voor de datums die u accepteert.
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
ms.openlocfilehash: 5c2167397d95d04c937ddf1820e6e9edff906b2f
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-calculate-order-promising-dates"></a>Procedure: ordertoezeggingsdatums berekenen
Een bedrijf moet de klanten op de hoogte kunnen stellen van leverdatums van orders. Met het venster **Ordertoezeggingsregels** kunt u dit doen vanuit een verkooporderregel.  

Op basis van de bekende en verwachte beschikbaarheidsdatums van een item berekent [!INCLUDE[d365fin](includes/d365fin_md.md)] onmiddellijk verzend- en leverdatums, die vervolgens aan de klant kunnen worden toegezegd.  

Als u een aangevraagde leverdatum op een verkooporderregel plaatst, wordt automatisch deze datum gebruikt als uitgangspunt voor de volgende berekeningen:  

- verzochte leverdatum - verzendtijd = geplande verzenddatum  
- geplande verzenddatum - verwerkingstijd uitgaand magazijn = verzenddatum  

Als de artikelen op de verzenddatum kunnen worden gepickt, kan het verkoopproces worden voortgezet. Als de artikelen niet op de verzenddatum kunnen worden gepickt, wordt een voorraadwaarschuwing gegeven.  

Als u geen aangevraagde leverdatum op een verkooporderregel hebt opgegeven of als u niet aan de aangevraagde leverdatum kunt voldoen, wordt gezocht naar de vroegste datum waarop de artikelen beschikbaar zijn. Vervolgens wordt deze datum ingevuld op de regel in het veld **Verzenddatum** waarna de volgende formules worden gebruikt om te bepalen op welke datum de artikelen volgens planning worden verzonden en geleverd aan de klant:  

- verzenddatum + verwerkingstijd uitgaand magazijn = geplande verzenddatum  
- Geplande verzenddatum + Verzendtijd = Geplande leverdatum  

## <a name="about-order-promising"></a>Informatie over ordertoezeggingen
Met de functionaliteit Ordertoezegging kunt u orders toezeggen, die op een bepaalde datum moeten worden verzonden of geleverd. De datum voor ATP (Available To Promise) of CTP (Capable To Promise) van een artikel wordt berekend en er worden orderregels gemaakt voor de datums die u accepteert. Met deze functionaliteit wordt de vroegst mogelijke datum berekend waarop een artikel beschikbaar is voor verzending of levering. De functie maakt ook aanvraagregeles, voor het geval dat de artikelen eerst moeten worden ingekocht, voor de datums die u accepteert.

[!INCLUDE[d365fin](includes/d365fin_md.md)] maakt gebruik van twee fundamentele begrippen:  

- Available to Promise (ATP)  
- Capable to promise (CTP)  

### <a name="available-to-promise"></a>Available to Promise  
Available to promise (ATP, ook wel aangeduid als 'Beschikbare voorraad') berekent datums op basis van het reserveringssysteem. Het voert een beschikbaarheidscontrole uit van de niet-gereserveerde aantallen in voorraad met betrekking tot de geplande productie, inkoop, transfers en verkoopretouren. Op basis van deze informatie berekent [!INCLUDE[d365fin](includes/d365fin_md.md)] automatisch de leverdatum van de order van de klant, omdat de artikelen beschikbaar zijn in voorraad of na geplande ontvangsten.  

### <a name="capable-to-promise"></a>Capable to Promise  
CTP gebruikt een 'wat als' scenario waar het item niet in voorraad is en er geen orders zijn gepland. Op basis van dit scenario berekent [!INCLUDE[d365fin](includes/d365fin_md.md)] de vroegste datum waarop het artikel beschikbaar wordt als het wordt geproduceerd, gekocht of overgebracht.  


### <a name="calculations"></a>Berekeningen  
Wanneer [!INCLUDE[d365fin](includes/d365fin_md.md)] de leverdatum van de klant berekent, worden twee taken uitgevoerd:  

- Berekent de vroegste leverdatum wanneer de klant niet om een specifieke leverdatum heeft verzocht.  
- Controleert of de door de klant gevraagde of toegezegde leverdatum reaistisch is.  

Als de klant niet om een specifieke leverdatum vraagt, wordt de verzenddatum gelijk aan de werkdatum, en wordt de beschikbaarheid vervolgens gebaseerd op deze datum. Als het artikel in voorraad is, berekent [!INCLUDE[d365fin](includes/d365fin_md.md)] vooruit in tijd om te bepalen wanneer de order kan worden afgeleverd. Dit gebeurt aan de hand van de volgende formules:  

- Verzenddatum + Uitgaand magazijn + Geplande verzending + verwerkingstijd = Datum  
- Geplande verzenddatum + Verzendtijd = Geplande leverdatum  

[!INCLUDE[d365fin](includes/d365fin_md.md)] controleert vervolgens of de berekende leverdatum realistisch is door terug in tijd te rekenen om te bepalen wanneer het item beschikbaar moet zijn om te voldoen aan de toegezegde datum. Dit gebeurt aan de hand van de volgende formules:  

- Geplande leverdatum - Verzendtijd = Geplande verzenddatum  
- Geplande verzenddatum - Uitgaande magazijnverwerking = Verzenddatum  

De verzenddatum wordt gebruikt om de beschikbaarheidscontrole uit te voeren. Als het item op deze datum beschikbaar is, bevestigt [!INCLUDE[d365fin](includes/d365fin_md.md)] dat aan de aangevraagde/toegezegde levering kan worden voldaan door de geplande leverdatum gelijk te stellen aan de aangevraagde/toegezegde leverdatum. Als het item niet beschikbaar is, verschijnt er een lege datum en kan de orderverwerker vervolgens de CTP-functionaliteit gebruiken.  

Op basis van de nieuwe datums en tijden, worden alle gerelateerde datums berekend volgens de formules die eerder in deze sectie zijn weergegeven. De CTP-berekening duurt langer, maar geeft een nauwkeurige datum voor wanneer de klant het artikel kan verwachten. De datums die worden berekend vanuit CTP, worden weergegeven in de velden **Geplande leverdatum** en **Eerste verzenddatum** in het venster **Ordertoezeggingsregels**.  

De orderverwerker voltooit het CTP-proces door de datums te accepteren. Dit betekent dat een planningsregel en een reserveringspost voor het artikel worden gemaakt vóór de berekende datum om ervoor te zorgen dat aan de order kan worden voldaan.  

Naast de externe ordertoezegging die u kunt uitvoeren in het venster **Ordertoezeggingsregels**, kunt u ook interne of externe leverdatums voor stuklijstartikelen beloven. Zie voor meer informatie [Procedure: beschikbaarheid van artikelen weergeven](inventory-how-availability-overview.md).

## <a name="to-set-up-order-promising"></a>Ordertoezegging instellen  
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Ordertoezeggingsinstellingen** in en klik op de gerelateerde koppeling.  
2. Voer in het veld **Uitsteltijd** een nummer en tijdseenheidscode in. Selecteer een van de volgende codes.  

    |Code|Omschrijving|  
    |----------|-----------------|  
    |**d**|Agendadag|  
    |**w**|Week|  
    |**m**|Maand|  
    |**k**|Kwartaal|  
    |**j**|jaar|  

    "3w" geeft bijvoorbeeld aan dat de uitsteltijd drie weken is. Gebruik voor alle codes "h" als voorvoegsel om de huidige tijdseenheid aan te geven. Voer bijvoorbeeld **hm** in als de uitsteltijd de huidige maand moet zijn.  
3. Voer in het veld **Ordertoezeggingsnrs.** een nummerreeks in door een regel te selecteren in het overzicht in het venster **Nr.-reeks**.  
4. Voer in het veld **Ordertoezeggingssjabloon** een ordertoezeggingsjabloon in door een regel te selecteren in het overzicht in het venster **Overzicht ink.-voorstelsjabl.**  
5. Voer in het veld **Ordertoezeggingsvoorstel** een inkoopvoorstel in door een regel te selecteren in het overzicht in het venster **Inkoopvoorstelbatches**.

### <a name="to-enter-inbound-warehouse-handling-time-in-the-inventory-setup-window"></a>Inslagtijd invoeren in het venster met de voorraadinstellingen  
Als u een inslagtijd wilt instellen voor de berekening van de ordertoezegging op de inkoopregel, kunt u deze instellen als standaardwaarde voor de voorraad en de vestiging.    
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Voorraadinstellingen** in en klik vervolgens op de gerelateerde koppeling.  
2. Voer in het veld **Inslagtijd** op het sneltabblad **Algemeen** het aantal dagen in dat u wilt opnemen in de berekening van de ordertoezegging.  

> [!NOTE]  
>  Als u het veld **Inslagtijd** op de **vestigingskaart** hebt ingevuld voor de vestiging, wordt de inhoud van het veld gebruikt als standaardinslagtijd.  

### <a name="to-enter-inbound-warehouse-handling-time-on-location-cards"></a>Inslagtijd invoeren op vestigingskaarten  
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Vestiging** in en klik vervolgens op de gerelateerde koppeling.  
2.  Open de relevante vestigingskaart.  
3.  Voer in het veld **Inslagtijd** op het sneltabblad **Algemeen** het aantal dagen in dat u wilt opnemen in de berekening van de ordertoezegging.  

> [!NOTE]  
>  Als u het veld **Inslagtijd** leeg laat, wordt voor de berekening de waarde in het venster **Voorraadinstellingen** gebruikt.

### <a name="to-enter-outbound-warehouse-handling-time-in-the-inventory-setup-window"></a>Uitslagtijd invoeren in het venster met de voorraadinstellingen  
Als u een uitslagtijd wilt instellen voor de berekening van de ordertoezegging op de verkoopregel, kunt u deze instellen als standaardwaarde voor de voorraad.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Voorraadinstellingen** in en klik vervolgens op de gerelateerde koppeling.  
2. Voer in het veld **Uitslagtijd** op het sneltabblad **Algemeen** het aantal dagen in dat u wilt opnemen in de berekening van de ordertoezegging.  

> [!NOTE]  
>  Als u het veld **Uitslagtijd** op de vestigingskaart hebt ingevuld voor de vestiging, wordt de inhoud van het veld gebruikt als standaarduitslagtijd.  

### <a name="to-enter-outbound-warehouse-handling-time-on-location-cards"></a>Uitslagtijd invoeren op vestigingskaarten  
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Vestigingen** in en klik vervolgens op de gerelateerde koppeling.  
2.  Open de relevante vestigingskaart.  
3.  Voer in het veld **Uitslagtijd** op het sneltabblad **Magazijn** het aantal dagen in dat u wilt opnemen in de berekening van de ordertoezegging.  

> [!NOTE]  
>  Als u het veld **Uitslagtijd** leeg laat, wordt voor de berekening de waarde in het venster **Voorraadinstellingen** gebruikt.

## <a name="to-make-an-item-critical"></a>Artikelen als kritiek aanmerken  
Voordat u een artikel in de ordertoezeggingsberekening kunt opnemen, moet het zijn gemarkeerd als kritiek. Deze instellingen zorgen dat de niet-kritieke artikelen niet leiden tot irrelevante ordertoezeggingsberekeningen   
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Artikelen** in en klik vervolgens op de gerelateerde koppeling.  
2.  Open de relevante artikelkaart.  
3.  Selecteer op het sneltabblad **Planning** het veld **Kritisch**.  

## <a name="to-calculate-an-order-promising-date"></a>Een ordertoezeggingsdatum berekenen  
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Verkooporder** in en klik vervolgens op de gerelateerde koppeling.  
2.  Open de betreffende verkooporder en selecteer de verkooporderregels die moeten worden berekend.  
3.  Kies de actie **Ordertoezegging** en kies daarna de actie **Ordertoezeggingsregels**.  
4.  Selecteer een regel en selecteer vervolgens een van de volgende opties:  

    - Selecteer **ATP** als de vroegste datum moet worden berekend waarop het artikel beschikbaar is met betrekking tot de voorraad, de geplande ontvangsten en de brutobehoeften.  
    - Selecteer **CTP** als u weet dat het artikel momenteel niet in voorraad is en de vroegste datum moet worden berekend waarop het artikel beschikbaar wordt door nieuwe aanvullende behoefteregels te maken.  
5.  Kies de knop **Accepteren** om de vroegst beschikbare verzenddatum te accepteren.  

## <a name="see-also"></a>Zie ook  
[Verkoop](sales-manage-sales.md)  
[Datumberekening voor inkoop](purchasing-date-calculation-for-purchases.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


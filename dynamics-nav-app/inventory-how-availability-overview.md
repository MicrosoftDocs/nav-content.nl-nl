---
title: Een beschikbaarheidsoverzicht verkrijgen
description: U kunt informatie verkrijgen over de beschikbaarheid van artikelen of voorraad in verschillende vestigingen, per verkoop- of inkoopgebeurtenis, per periode of per positie van het artikel in een assemblage- of productiestuklijst.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: stock
ms.date: 08/15/2017
ms.author: SorenGP
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 81872839df11a13489bbc192ad97dae04976ebb0
ms.contentlocale: nl-nl
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-view-the-availability-of-items"></a>Procedure: beschikbaarheid van artikelen weergeven
Vanuit de context van een zakelijke taak kunt u geavanceerde informatie krijgen over waar en wanneer een artikel beschikbaar is, zoals wanneer u met een klant praat over een leverdatum.

U kunt de beschikbaarheid van alle artikelen per vestiging bekijken en u kunt de beschikbaarheid van elk artikel per gebeurtenis, per periode, of per vestiging weergegeven. Een gebeurtenis is elke geplande artikeltransactie, bijvoorbeeld een verkoopverzending of een inkomende transferontvangst.

> [!NOTE]  
>   Beschikbaarheidsweergaven per vestiging vereisen dat u voorraad onderhoudt op meerdere vestigingen. Zie voor meer informatie [Procedure: Vestigingen instellen](inventory-how-setup-locations.md).

In [!INCLUDE[d365fin](includes/d365fin_md.md)] worden de beschikbaarheidscijfers weergegeven in twee verschillende velden, elk met een andere definitie:

* Het veld **In voorraad** bevat het werkelijke aantal van vandaag op basis van geboekte artikelposten.
* Het veld **Geplande voorraad** wordt berekend en toont de beschikbare hoeveelheid plus geplande ontvangsten minus brutobehoeften. (In [!INCLUDE[d365fin](includes/d365fin_md.md)] gebruiken omvatten geplande ontvangsten hoeveelheden op inkooporders en inkomende transferorders. Brutobehoeften omvatten aantallen op verkooporders en uitgaande transferorders.)

> [!TIP]  
>   Het geplande beschikbare saldo is met name van belang voor weergave in de vensters **Beschikbaarheid per periode** en **Artikelbeschikbaarheid per gebeurtenis**, aangezien deze de datumdimensie bevatten.  

> [!NOTE]  
>   In de volgende procedures wordt beschreven hoe geavanceerde beschikbaarheidsgegevens worden weergegeven vanuit het artikeloverzicht en de artikelkaart. U kunt ook toegang tot de informatie krijgen vanuit verkoopdocumentregels, voor het artikel op de regel. Zie [Procedure: Producten verkopen](sales-how-sell-products.md) voor meer informatie.

## <a name="to-view-the-availability-of-an-item-according-to-when-it-will-be-received-or-shipped"></a>U kunt de beschikbaarheid van een artikel weergeven op basis van wanneer het wordt verzonden of ontvangen
U geeft de beschikbaarheid van een artikel weer op basis van geplande artikeltransacties in het venster **Artikelbeschikbaarheid per gebeurtenis**.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Artikelen** in en klik vervolgens op de gerelateerde koppeling.
2. Open de kaart van het artikel waarvoor u beschikbaarheid wilt weergeven.
3. Kies de actie **Artikelbeschikbaarheid per** en kies vervolgens de actie **Gebeurtenis**.

    In het venster **Artikelbeschikbaarheid per gebeurtenis** ziet u hoe het voorraadaantal van het artikel zich in de loop van de tijd ontwikkelt volgens geplande verzend- en ontvangstgebeurtenissen. Het venster biedt een verkorte weergave met één regel verzamelde informatie per tijdsinterval, waarin voorraadaantallen veranderen. Tijdsintervallen waarin geen gebeurtenissen hebben plaatsgevonden, worden niet weergegeven. U kunt elke regel gegevens over de gebeurtenis of gebeurtenissen die de gecumuleerde hoeveelheid op de regel veroorzaken, uitvouwen.
4. Kies de waarde in het veld **Geplande voorraad** om alleen de artikelposten te bekijken of documenten te openen die de waarde vormen.

## <a name="to-view-the-availability-of-an-item-in-different-periods"></a>De beschikbaarheid van een artikel in verschillende perioden weergeven
U geeft de beschikbaarheid van een artikel in de loop van de tijd voor bepaalde perioden weer in het venster **Beschikbaarheid per periode**.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Artikelen** in en klik vervolgens op de gerelateerde koppeling.
2. Open de kaart van het artikel waarvoor u beschikbaarheid wilt weergeven.
3. Kies de actie **Artikelbeschikbaarheid per** en kies vervolgens de actie **Periode**.

    In het venster **Beschikbaarheid per periode** ziet u hoe het voorraadaantal van het artikel zich in de loop van de tijd ontwikkelt, weergegeven voor een periode die u selecteert, zoals Dag, Week of Kwartaal.
4. Kies de waarde in het veld **Geplande voorraad** om alleen de artikelposten te bekijken of documenten te openen die de waarde vormen.

## <a name="to-view-the-availability-of-an-item-at-the-locations-where-it-is-stored"></a>De beschikbaarheid weergeven van een artikel op de vestigingen waar het is opgeslagen
U geeft de beschikbaarheid van een artikel op de verschillende vestigingen waar het is opgeslagen, weer in het venster **Artikelbeschikbaarheid per vestiging**.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Artikelen** in en klik vervolgens op de gerelateerde koppeling.
2. Open de kaart van het artikel waarvoor u beschikbaarheid wilt weergeven.
3. Kies de actie **Artikelbeschikbaarheid per** en kies vervolgens de actie **Vestiging**.

    In het venster **Artikelbeschikbaarheid per vestiging** ziet u hoe het voorraadaantal van het artikel zich in de toekomst zal ontwikkelen voor elke vestiging waar het is opgeslagen.
4. Kies de waarde in het veld **In voorraad (Beschikb.)** om alleen de artikelposten te bekijken die de waarde vormen.
5. Kies de waarde in het veld **Geplande voorraad** om alleen de artikelposten te bekijken of documenten te openen die de waarde vormen.

## <a name="to-view-the-availability-of-all-items-by-the-location-where-they-are-stored"></a>De beschikbaarheid weergeven van alle artikelen op de vestiging waar ze zijn opgeslagen
U geeft de beschikbaarheid van al uw artikelen in al uw vestigingen weer in het venster **Artikelen per vestiging**.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Artikelen** in en klik vervolgens op de gerelateerde koppeling.
2. Kies de actie **Artikelen per vestiging**.

    Het venster **Artikelen per vestiging** toont voor al uw artikelen hoeveel er in elke vestiging beschikbaar zijn.
3. Kies de waarde in het veld **In voorraad (Beschikb.)** om alleen de artikelposten te bekijken die de waarde vormen.

## <a name="to-view-the-availability-of-an-item-by-its-use-in-assembly-or-production-boms"></a>De beschikbaarheid van een artikel weergeven op basis van het gebruik ervan in assemblage- of productiestuklijsten
Als een artikel in assemblage- of productiestuklijsten bestaat, ofwel als het bovenliggende artikel ofwel als onderdeel, kunt u zien hoeveel eenheden ervan vereist zijn in het venster **Artikelbeschikbaarheid per stuklijstniveau**. In het venster wordt weergegeven hoeveel eenheden van een bovenliggend artikel u kunt maken op basis van de beschikbaarheid van onderliggende artikelen op onderliggende regels. Een artikel dat een assemblage- of productiestuklijst heeft, wordt weergegeven in het venster als een opvouwbare regel. U kunt deze regel uitvouwen om de onderliggende onderdelen en subassemblages op lagere niveaus met hun eigen stuklijsten te bekijken.

U kunt het venster gebruiken om te bepalen of u een verkooporder voor een artikel op een bepaalde datum kunt afhandelen door te kijken naar de huidige beschikbaarheid en de hoeveelheden die door de onderdelen ervan kunnen worden geleverd. U kunt ook het venster om knelpunten in verwante stuklijsten te identificeren.

Op elke regel in het venster voor zowel hoofdartikelen als onderliggende artikelen kunnen de beschikbaarheidscijfers worden opgegeven in de volgende sleutelvelden. U kunt deze cijfers gebruiken om toe te zeggen hoeveel eenheden van een bovenliggend hoofdartikel u kunt leveren als u het gerelateerde assemblageproces start.

|Veld|Omschrijving|
|------|-----------|
|**Bovenliggende kan worden gemaakt**|Hiermee wordt weergegeven hoeveel eenheden van een willekeurige subassemblage in het topartikel u kunt maken. In het veld wordt opgegeven hoeveel directe bovenliggende eenheden u kunt assembleren. De waarde is gebaseerd op de beschikbaarheid van het artikel op de regel.|
|**Topartikel kan worden gemaakt**|Hiermee wordt weergegeven hoeveel eenheden van het topartikel u kunt maken. In het veld wordt opgegeven hoeveel eenheden van het stuklijstartikel op de bovenste regel u kunt assembleren. De waarde is gebaseerd op de beschikbaarheid van het artikel op de regel.|

### <a name="item-availability-by-bom-level-window"></a>Venster Artikelbeschikbaarheid per stuklijstniveau
Het venster **Artikelbeschikbaarheid per stuklijstniveau** bevat gegevens voor het artikel op de kaart of de documentregel waarvoor het venster wordt geopend. Het artikel wordt altijd weergegeven op de bovenste regel. U kunt informatie voor andere artikelen of voor alle items weergeven door de waarde te wijzigen in het veld **Artikelfilter**.

> [!NOTE]  
>   Standaard geven beschikbaarheidscijfers op de regels de totale beschikbaarheid van alle artikelen onder het topartikel aan. Deze cijfers worden weergegeven in het veld **Beschikbaar aantal** en de focus ligt op het topartikel. Informatie over hoeveel subassemblages u kunt maken is echter mogelijk vervormd. Als u een ware indicatie wilt krijgen van het aantal weergegeven subassemblages dat u kunt maken, moet u het selectievakje **Totale beschikbaarheid weergeven** uitschakelen en vervolgens het cijfer in het veld **Bovenliggende kan worden gemaakt** bekijken.

Met het veld **Knelpunt** wordt opgegeven welk artikel in de stuklijststructuur ervoor zorgt dat u geen grotere hoeveelheid kunt maken dan wordt weergegeven in het veld **Topartikel kan worden gemaakt**. Het knelpuntartikel kan bijvoorbeeld een aangeschaft onderdeel zijn met een verwachte ontvangstdatum die te laat is om extra eenheden van het topartikel te maken voor de datum in het veld **Vereist per datum**.

## <a name="assembly-availability-window"></a>Venster Beschikbaarheid assemblage
In het venster **Beschikbaarheid assemblage** vindt u gedetailleerde beschikbaarheidsinformatie voor de component. Het venster wordt geopend:

- Automatisch vanuit een verkooporderregel bij assembleren op order wanneer u een aantal invoert dat zorgt voor een beschikbaarheidsprobleem van een onderdeel.
- Automatisch vanuit een assemblage-orderkop wanneer u in het veld Aantal een waarde invoert die zorgt voor een beschikbaarheidsprobleem van een onderdeel.
- Handmatig wanneer u het opent vanuit een assemblageorder. Kies op het tabblad Acties, in de groep Functies, Beschikbaarheid tonen.

Het sneltabblad **Details** toont gedetailleerde beschikbaarheidsinformatie voor de component, inclusief het aantal assemblageorders dat op de vervaldatum samengesteld kan zijn op basis van de beschikbaarheid van de vereiste onderdelen. Dit wordt weergegeven in het veld Kan assembleren op het sneltabbald Details.

De waarde in het veld **Kan assembleren** wordt in een rood lettertype weergegeven als het aantal lager is dan het aantal in het veld **Resterend aantal**, wat betekent dat er niet voldoende onderdelen beschikbaar zijn voor het samenstellen van het volledige aantal.

In het sneltabblad **Regels** vindt u gedetailleerde beschikbaarheidsinformatie over de componenten.

Als een of meer assemblageonderdelen niet beschikbaar zijn, wordt dit weerspiegeld in het veld **Kan assembleren** op de betreffende regel als een aantal lager is dan het aantal in het veld **Resterend aantal** op het sneltabbald **Details**.

## <a name="see-also"></a>Zie ook
[Voorraad beheren](inventory-manage-inventory.md)  
[Assemblagebeheer](assembly-assemble-items.md)  
[Procedure: Werken met stuklijsten](inventory-how-work-BOMs.md)    
[Procedure: Vestigingen instellen](inventory-how-setup-locations.md)  
[Procedure: Voorraad overbrengen tussen vestigingen](inventory-how-transfer-between-locations.md)  
[Procedure: Producten verkopen](sales-how-sell-products.md)      
[Werken met Dynamics NAV](ui-work-product.md)  
[Algemene bedrijfsfunctionaliteit](ui-across-business-areas.md)


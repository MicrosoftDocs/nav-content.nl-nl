---
title: Artikelen samenstellen
description: Als het veld **Aanvullingsmethode** op de artikelkaart **Assemblage** bevat, is de standaardbevoorradingsmethode van het artikel het assembleren van gedefinieerde onderdelen en mogelijk door een gedefinieerde bron.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b7f371c48aa70d2b99ce7b7333b92a63d7764f28
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-assemble-items"></a>Procedure: artikelen samenstellen
Als het veld **Aanvullingsmethode** op de artikelkaart **Assemblage** bevat, is de standaardbevoorradingsmethode van het artikel het assembleren van gedefinieerde onderdelen en mogelijk door een gedefinieerde bron.  

De onderdelen en bronnen die voor dit soort assemblageartikel worden gebruikt, moeten worden gedefinieerd in een assemblagestuklijst. Zie [Procedure: Werken met stuklijsten](inventory-how-work-BOMs.md) voor meer informatie.  

Assemblageartikelen kunnen voor twee verschillende assemblageprocessen ingesteld worden:  

-   Op voorraad assembleren.  
-   Op order assembleren.  

Meestal gebruikt u **Op voorraad assembleren** voor artikelen die u voorafgaand aan de verkoop wilt assembleren, zoals het voorbereiden op een kit-campagne, en in voorraad wilt houden totdat ze worden besteld. Deze artikelen betreffen meestal standaardartikelen, zoals verpakte kits die u niet aanbiedt voor het aanpassen van aanvragen van klanten.  

U gebruikt meestal **Op order assembleren** voor artikelen die u niet op voorraad wilt hebben, omdat u verwacht deze op speciale klantverzoeken af te kunnen stemmen of omdat u de voorraadkosten wilt minimaliseren door deze net op tijd te leveren. Zie voor meer informatie [Procedure: op order geassembleerde artikelen verkopen](assembly-how-to-sell-items-assembled-to-order.md).  

Zie voor meer informatie over hoe u een component instelt [Op voorraad assembleren of Op order assembleren begrijpen](assembly-assemble-to-order-or-assemble-to-stock.md).  

Deze instellingen zijn standaardinstellingen die beheren hoe de verkoop en regels voor assemblageorders aanvankelijk worden verwerkt. U kunt van deze standaardinstellingen afwijken en het assemblageartikel op de meest optimale manier leveren bij de verwerking van een verkoop. Zie voor meer informatie [Procedure: voorraadartikelen in assembleren-op-order-stromen verkopen](assembly-how-to-sell-assemble-to-order-items-and-inventory-items-together.md) en [Procedure: op-order-assembleren-artikelen en voorraadartikelen samen verkopen](assembly-how-to-sell-assemble-to-order-items-and-inventory-items-together.md).

> [!NOTE]  
> Assemblycomponenten worden op een speciale manier verwerkt in standaardmagazijnconfiguraties. Zie voor meer informatie de sectie Op-order-assembleren-artikelen in voorraadpicks afhandelen in [Procedure: artikelen picken met een voorraadpick](warehouse-how-to-pick-items-with-inventory-picks.md).   

In deze procedure maakt en verwerkt u een assemblageorder voor artikelen die op voorraad geassembleerd worden, wat betekent dat er geen gekoppelde verkooporder is. De stappen zijn het starten van de assemblageorder, afhandelen van eventuele problemen met de beschikbaarheid van onderdelen en gedeeltelijk boeken van output van het assemblageartikel .

## <a name="to-assemble-an-item"></a>Een item assembleren  
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Assemblageorders** in en klik vervolgens op de gerelateerde koppeling.  
2.  Kies de actie **Nieuw**. Het venster **Nieuwe assemblageorder** wordt geopend.  
3.  Vul indien nodig de velden in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4.  Selecteer in het veld **Artikelnr.** het assemblageartikel dat u wilt verwerken. Het veld is gefilterd, zodat alleen de artikelen die zijn ingesteld voor assemblage weergegeven worden, wat betekent dat ze een assemblagestuklijst toegewezen hebben gekregen.  
5.  Voer in het veld **Aantal** het aantal eenheden in dat u van het artikel wilt assembleren.  

    > [!NOTE]  
    >  Indien een of meer onderdelen niet beschikbaar zijn om op de opgegeven vervaldatum aan het opgegeven aantal assemblageartikelen te voldoen, wordt het venster **Beschikbaarheid assemblage** automatisch geopend met gedetailleerde informatie over het aantal assemblageartikelen dat kan worden geassembleerd op basis van de beschikbare onderdelen. Zie voor meer informatie [Procedure: beschikbaarheid van artikelen weergeven](inventory-how-availability-overview.md).  Wanneer u het venster sluit, wordt de assemblageorder met waarschuwingen omtrent de beschikbaarheid op de regels van het betrokken onderdeel gemaakt.  

    De regels van de assemblageorder worden automatisch gevuld met de inhoud van de assemblagestuklijst en aantallen volgens de orderkop van de assemblageorder.  

    > [!NOTE]  
    >  Indien het venster **Beschikbaarheid assemblage** werd geopend toen u de assemblage-orderkop invulde, staat bij iedere betrokken orderregel van de assemblage **Ja** in het veld **Waarschuwing beschikbaarheid** met een koppeling naar gedetailleerde beschikbaarheidsinformatie. Zie voor meer informatie Beschikbaarheid controleren. U kunt een beschikbaarheidsprobleem van een onderdeel oplossen door de begindatum uit te stellen, het onderdeel te vervangen door een ander item of een beschikbare vervanging te selecteren indien deze is gedefinieerd.  

6.  Geef in het veld **Te assembleren aantal** op hoeveel eenheden van het assemblageartikel u als uitvoer wilt boeken, de volgende keer dat u de assemblageorder boekt. Dit aantal mag lager zijn dan de waarde in het veld **Aantal** om het gedeeltelijk boeken van uitvoer aan te geven.  

    > [!NOTE]  
    >  Om ervoor te zorgen dat het boeken van het verbruik van onderdelen overeenkomt met het boeken van de output van het assemblageartikel, worden de velden met aantallen in de orderregels van de assemblageorder automatisch aangepast aan de waarde die u in het veld **Te assembleren aantal** invoert.  
7.  Geef op orderregels van assemblageorders van het type **Item** of **Bron**, in het veld **Te verbruiken aantal**, het aantal eenheden op dat u als verbruikt wilt boeken, de volgende keer dat u de assemblageorder boekt. Standaard wordt het verwachte te verbruiken aantal volgens de assemblagestuklijst en het aantal van de assemblage-orderkop ingevoegd, maar u kunt dit vergroten of verkleinen, om bijvoorbeeld een overmatig verbruik van onderdelen aan te geven of het feit dat extra bronnen gebruikt zijn.  
8.  Wanneer u gereed bent om gedeeltelijk of volledig te boeken, kiest u de actie **Boeken**.  

    > [!NOTE]  
    >  Indien er in de regels van de assemblageorder nog steeds waarschuwingen aanwezig zijn, wordt de boeking geblokkeerd. Een bericht over welke onderdelen niet in voorraad zijn wordt weergegeven.  

Nadat het boeken is voltooid, wordt het assemblageartikel als uitvoer geboekt naar de vestigingscode en mogelijke opslaglocatiecode die op de assemblageorder zijn gedefinieerd. De locatie voor handmatig gemaakte assemblageorders kan worden gekopieerd van de instelling **Standaard locatie voor Orders**. Voor assembleren-op-order kan de vestigingscode van de verkooporderregel worden gekopieerd.  

## <a name="see-also"></a>Zie ook
[Assemblagebeheer](assembly-assemble-items.md)  
[Procedure: Werken met stuklijsten](inventory-how-work-BOMs.md)  
[Voorraad](inventory-manage-inventory.md)  
[Ontwerpdetails: Magazijnbeheer](design-details-warehouse-management.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


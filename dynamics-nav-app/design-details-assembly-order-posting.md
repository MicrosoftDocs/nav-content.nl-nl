---
title: 'Ontwerpdetails: Assemblageorderboeking'
description: Assemblageorderboeking wordt gebaseerd op dezelfde principes als wanneer de soortgelijke activiteiten van verkooporders en productieverbruik/-output worden geboekt. De principes worden echter gecombineerd in de zin dat assemblageorders hun eigen boeking-UI hebben, zoals die voor verkooporders, terwijl de feitelijke postboeking op de achtergrond wordt uitgevoerd als directe artikel- en resourcedagboekboekingen, zoals die voor productieverbruik, output en capaciteit.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 8a8cd33e4ec0a044565fbce821de4034c7da74a5
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-assembly-order-posting"></a>Ontwerpdetails: Assemblageorderboeking
Assemblageorderboeking wordt gebaseerd op dezelfde principes als wanneer de soortgelijke activiteiten van verkooporders en productieverbruik/-output worden geboekt. De principes worden echter gecombineerd in de zin dat assemblageorders hun eigen boeking-UI hebben, zoals die voor verkooporders, terwijl de feitelijke postboeking op de achtergrond wordt uitgevoerd als directe artikel- en resourcedagboekboekingen, zoals die voor productieverbruik, output en capaciteit.  

Net als bij productieorderboeking worden de verbruikte materialen en de gebruikte resources omgezet en uitgevoerd als de component wanneer de productieorder is voltooid. Zie [Ontwerpdetails: Productieorderboeking](design-details-production-order-posting.md) voor meer informatie. De kostenstroom voor assemblageorders is echter minder complex, met name omdat de assemblagekostenboeking slechts eenmaal plaatsvindt en daarom geen OHW-voorraad genereert.  

De volgende dagboekboekingen treden op tijdens assemblageorderboekingen:  

-   Het artikeldagboek boekt positieve artikelposten, die output van het assemblageartikel vertegenwoordigen, uit de assemblageorderkop.  
-   Het artikeldagboek boekt negatieve artikelposten, die verbruik van assemblagecomponenten vertegenwoordigen, uit de assemblageorderregels.  
-   Het resourcedagboek boekt gebruik van assemblageresources (tijdseenheden) vanaf de assemblageorderregels.  
-   Het capaciteitsdagboek boekt waardeposten die betrekking hebben op het resourceverbruik, vanaf de assemblageorderregels.  

Het volgende diagram bevat de structuur van artikel- en resourceposten die het gevolg zijn van assemblageorderboeking.  

![Resource- en capaciteitskosten](media/design_details_assembly_posting_1.png "design_details_assembly_posting_1")  

> [!NOTE]  
>  Bewerkingsplaatsen en afdelingen zijn opgenomen om te illustreren dat capaciteitsposten zowel worden gemaakt vanuit productie als vanuit assemblage.  

In het volgende diagram wordt aangegeven hoe assemblagegegevens in posten stromen tijdens het boeken:  

![Gegevensstroom tijdens het boeken](media/design_details_assembly_posting_2.png "design_details_assembly_posting_2")  

## <a name="posting-sequence"></a>Boekingsvolgorde  
De boeking van een assemblageorder vindt plaats in de volgende volgorde:  

1.  De assemblageorderregels zijn geboekt.  
2.  De assemblageorderkop is geboekt.  

De volgende tabel toont de volgorde van de acties.  

|Actie|Description|  
|------------|-----------------|  
|Boeking initialiseren|1. Voer voorlopige controles uit.<br />2. Voeg een boekingsnummer toe en wijzig de assemblageorderkop.<br />3. Geef de assemblageorder vrij.|  
|Post|<ol><li>Maak de geboekte assemblageorderkop.</li><li>Kopieer opmerkingsregels.</li><li>Boek assemblageorderregels (verbruik):<br /><br /> <ol><li>Maak een statusvenster om assemblageverbruik te berekenen.</li><li>Haal het resterende aantal op waarop de artikeldagboekregel wordt gebaseerd.</li><li>Stel de verbruikte en resterende aantallen opnieuw in.</li><li>Voor assemblageorderregels van de soort Artikel:<br /><br /> <ol><li>Vul velden op de artikeldagboekregel in.</li><li>Breng reserveringen over naar de artikeldagboekregel.</li><li>Boek de artikeldagboekregel om de artikelposten te maken.</li><li>Maak magazijndagboekregels en boek ze.</li></ol></li><li>Voor assemblageorderregels van de soort Resource:<br /><br /> <ol><li>Vul velden op de artikeldagboekregel in.</li><li>Boek de artikeldagboekregel. Hierdoor ontstaan capaciteitsposten.</li><li>Maak en boek een resourcedagboekregel.</li></ol></li><li>Breng veldwaarden van de assemblageorderregel over naar een zojuist gemaakte, geboekte assemblageorderregel.</li></ol></li><li>Boek de assemblageorderkop (output):<br /><br /> <ol><li>Vul velden op de artikeldagboekregel in.</li><li>Breng reserveringen over naar de artikeldagboekregel.</li><li>Boek de artikeldagboekregel om de artikelposten te maken.</li><li>Maak magazijndagboekregels en boek ze.</li><li>Stel de assemblageaantallen en de resterende aantallen opnieuw in.</li></ol></li></ol>|  

> [!IMPORTANT]  
>  In tegenstelling tot productieoutput, die wordt geboekt tegen verwachte kosten, wordt assemblyuitvoer tegen de feitelijke prijs geboekt.  

## <a name="cost-adjustment"></a>Kostenherwaardering  
 Zodra een assemblageorder is geboekt, wat inhoudt dat materiaal (onderdelen) en resources in een nieuw artikel worden geassembleerd, moet het mogelijk zijn om de werkelijke kosten van dat assemblageartikel en de werkelijke voorraadkosten van de betrokken onderdelen te bepalen. Hiervoor worden kosten van de geboekte posten van de bron (de onderdelen en resources) naar de geboekte posten van het doel (de component) doorgestuurd. Het doorsturen van kosten wordt uitgevoerd door het berekenen en genereren van nieuwe posten, zogenaamde herwaarderingsposten, die aan de doelposten worden gekoppeld.  

 De door te sturen assemblagekosten worden gedetecteerd met het detectiemechanisme op orderniveau. Zie voor informatie over andere mechanismen voor herwaarderingsdetectie [Ontwerpdetails: Kostenwaardering](design-details-cost-adjustment.md)  

### <a name="detecting-the-adjustment"></a>De correctie detecteren  
De detectiefunctie op orderniveau wordt gebruikt voor conversiescenario's, productie en assemblage. De functie werkt als volgt:  

-   Kostenherwaardering wordt gedetecteerd door de order te markeren telkens wanneer een materiaal/resource wordt geboekt als verbruikt/gebruikt voor de order.  
-   Kosten wordt doorgestuurd door de kosten voor het materiaal/de resource toe te passen op de uitvoerposten die aan dezelfde order zijn gekoppeld.  

De volgende afbeelding toont de structuur van de herwaarderingspost en hoe assemblagekosten worden aangepast.  

![Structuur van herwaarderingspost](media/design_details_assembly_posting_3.png "design_details_assembly_posting_3")  

### <a name="performing-the-adjustment"></a>De aanpassing doorvoeren  
De spreiding van gedetecteerde correcties van materiaal en resourcekosten op de assemblyuitvoerposten wordt uitgevoerd door de batchverwerking **Kostprijs herwaarderen - Artikelposten**. Deze bevat de functie Aanpassing op meerdere niveaus aanbrengen, die bestaat uit de volgende twee elementen:  

-   Assemblageordercorrectie aanbrengen - hiermee worden kosten van materiaal en resourcegebruik doorgestuurd naar de assemblage-uitvoerpost. Regel 5 en 6 in het algoritme hieronder zijn hiervoor verantwoordelijk.  
-   Correcties op één niveau aanbrengen - hiermee worden kosten voor afzonderlijke artikelen doorgestuurd met behulp van de waarderingsmethode ervan. Regels 9 en 10 in het algoritme hieronder zijn hiervoor verantwoordelijk.  

![Algoritme van assemblageherwaardering](media/design_details_assembly_posting_4.jpg "design_details_assembly_posting_4")  

> [!NOTE]  
>  Het element voor het maken van OHW- herwaarderingen op regel 7 en 8 is verantwoordelijk voor het doorsturen van productiemateriaal en capaciteitsverbruik naar de output van onvoltooide productieorders. Dit wordt niet gebruikt bij het aanpassen van assemblageorderkosten aangezien het concept OHW niet van toepassing is op assemblage.  

Voor informatie over hoe kosten van assemblage en productie worden geboekt naar het grootboek raadpleegt u [Ontwerpdetails: voorraadboeking](design-details-inventory-posting.md).  

## <a name="assembly-costs-are-always-actual"></a>Assemblagekosten zijn altijd werkelijk  
 Het concept van onderhanden werk (OHW) geldt niet voor assemblageorderboeking. Assemblagekosten worden alleen geboekt als werkelijke kosten, nooit als verwachte kosten. Zie [Ontwerpdetails: verwachte-kostenboeking](design-details-expected-cost-posting.md) voor meer informatie.  

Dit wordt ingeschakeld door de volgende gegevensstructuur.  

-   In het veld **Soort** op artikeldagboekregels in de tabellen **Capaciteitspost** en **Waardepost** wordt *Resource* gebruikt om posten van assemblageresources te identificeren.  
-   In het veld **Artikelboekingssoort** op artikeldagboekregels in de tabellen **Capaciteitspost** en **Waardepost** worden *Assemblage-uitvoer* en *Assemblageverbruik* gebruikt om respectievelijk de artikelposten van assemblage-uitvoer en de posten van verbruikte assemblagecomponenten te identificeren.  

Daarnaast worden boekingsgroepsvelden in de assemblageorderkop en de assemblageorderregels standaard als volgt ingevuld.  

|Entiteit|Soort|Boekingsgroep|Prod.-boekingsgroep|  
|------------|----------|-------------------|------------------------------|  
|Assemblageorderkop|Artikel|Voorraadboekingsgroep|Prod.-boekingsgroep|  
|Assemblageorderregel|Artikel|Voorraadboekingsgroep|Prod.-boekingsgroep|  
|Assemblageorderregel|Resource||Prod.-boekingsgroep|  

Alleen werkelijke kosten worden geboekt naar het grootboek en er worden geen interimrekeningen gevuld vanuit assemblageorderboeking. Zie voor meer informatie [Ontwerpdetails: rekeningen in het grootboek](design-details-accounts-in-the-general-ledger.md).  

## <a name="assemble-to-order"></a>Op order assembleren  
De artikelpost die het resultaat is van het boeken van een op-order-assembleren-verkoop wordt vast toegepast op de bijbehorende artikelpost voor de assemblageuitvoer. Dienovereenkomstig, worden de kosten van een op-order-assembleren-verkoop afgeleid van de assemblageorder waaraan deze verkoop is gekoppeld.  

Artikelposten van de soort Verkoop die het gevolg zijn van het boeken van op-order-assembleren aantallen, worden gemarkeerd met **Ja** in het veld **Op order assembleren**.  

Bij het boeken van verkooporderregels waarbij een gedeelte afkomstig is uit voorraad en een ander gedeelte een op-order-assembleren aantal is, worden afzonderlijke artikelposten gemaakt, één voor het voorraadaantal en één voor het op-order-assembleren aantal.  

## <a name="see-also"></a>Zie ook  
 [Ontwerpdetails: Voorraadwaardering](design-details-inventory-costing.md)   
 [Ontwerpdetails: Productieorderboeking](design-details-production-order-posting.md)   
 [Ontwerpdetails: Waarderingsmethoden](design-details-costing-methods.md)  
 [Voorraadkosten beheren](finance-manage-inventory-costs.md)  
 [Financiën](finance.md)  
 [Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  


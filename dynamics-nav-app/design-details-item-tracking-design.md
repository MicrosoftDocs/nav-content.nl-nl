---
title: 'Ontwerpdetails: Ontwerp artikeltracering'
description: In dit onderwerp wordt het ontwerp achter artikeltracering in [!INCLUDE[d365fin](includes/d365fin_md.md)] beschreven.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, item, tracking, tracing
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: acbb706d154f164c4e33e0bebaf84cd5a47862cc
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-item-tracking-design"></a>Ontwerpdetails: Ontwerp artikeltracering
In de eerste versie van Artikeltracering in [!INCLUDE[d365fin](includes/d365fin_md.md)] 2.60 werden serienummers of lotnummers direct geregistreerd in artikelposten. Dit ontwerp bood volledige beschikbaarheidsgegevens en eenvoudige tracering van historische posten, maar het miste flexibiliteit en functionaliteit.  

Vanaf [!INCLUDE[d365fin](includes/d365fin_md.md)] 3.00 bevond de artikeltraceringfunctionaliteit zich in een afzonderlijke objectstructuur met complexe koppelingen naar geboekte documenten en artikelposten. Dit ontwerp was flexibel en bood uitgebreide functionaliteit, maar artikeltraceringsposten werden niet volledig betrokken bij beschikbaarheidsberekeningen.  

Vanaf [!INCLUDE[d365fin](includes/d365fin_md.md)] 3.60 is de artikeltraceringfunctionaliteit geïntegreerd in het reserveringsysteem, waarmee reserveringen, ordertracering en planningsboodschappen worden verwerkt. Zie voor meer informatie "Ontwerpdetails: Reservering, ordertracering en planningsboodschappen" in "Ontwerpdetails: Voorraadplanning".  

Dit laatste ontwerp integreert artikeltraceringsposten in berekeningen van de totale beschikbaarheid in het hele systeem, inclusief planning, productie en magazijnactiviteiten. Het klassieke concept van het overzetten van serie- en lotnummers in de artikelposten, wordt opnieuw gebruikt om te zorgen voor eenvoudige toegang tot historische gegevens voor artikeltracering. In verband met verbeteringen in de artikeltracering in [!INCLUDE[d365fin](includes/d365fin_md.md)] 3.60 is het reserveringsysteem uitgebreid tot niet-order netwerkentiteiten, zoals dagboeken, facturen en creditnota's.  

Met het toevoegen van serie- of lotnummers verwerkt het reserveringssysteem permanente artikelkenmerken terwijl ook cyclische koppelingen tussen voorziening en vraag in de vorm van ordertraceringsposten en reserveringsposten worden verwerkt. Een ander kenmerk van serie- of lotnummers in vergelijking met de conventionele reserveringsgegevens is het feit dat deze gedeeltelijk of volledig kunnen worden geboekt. De tabel **Reserveringspost** (T337) werkt daarom nu met een gekoppelde tabel, de tabel **Traceringsspecificatie** (T336), waarmee optellingen tussen traceringsaantallen actieve en geboekte artikelen worden beheerd en weergegeven. Zie voor meer informatie [Ontwerpdetails: Actieve tegenover historische artikeltraceringsposten](design-details-active-versus-historic-item-tracking-entries.md).  

In het volgende diagram wordt het ontwerp van artikeltraceringfunctionaliteit in [!INCLUDE[d365fin](includes/d365fin_md.md)] aangegeven.  

![Artikeltraceringontwerp](media/design_details_item_tracking_design.png "design_details_item_tracking_design")  

Het centrale boekingsobject is opnieuw ontworpen om de unieke subclassificatie van een documentregel te verwerken in de vorm van serie- of lotnummers. Er zijn speciale relatietabellen toegevoegd om de één-op-veel relaties tussen geboekte documenten en de gesplitste artikelposten en waardeposten te maken.  

Codeunit 22, **Artikeldagboek. - Regel boeken** splitst nu de boeking volgens de artikeltraceringsnummers die zijn opgegeven op de documentregel. Voor ieder uniek artikeltraceringsnummer op de regel wordt een eigen artikelpost voor het artikel gemaakt. Dit betekent dat de koppeling van de geboekte documentregel naar de bijbehorende artikelposten nu een één-op-veel relatie is. Deze relatie wordt uitgevoerd door de volgende tabellen met artikeltraceringrelaties.  

|Veld|Description|  
|---------------|---------------------------------------|  
|**Artikelpostrelatie** (T6507)|Relateert verzonden of ontvangen regels aan artikelposten|  
|**Waardepostrelatie** (T6508)|Relateert gefactureerde regels aan waardeposten|  

Zie voor meer informatie [Ontwerpdetails: Boekingsstructuur artikeltracering](design-details-item-tracking-posting-structure.md).  

## <a name="see-also"></a>Zie ook  
[Ontwerpdetails: Artikeltracering](design-details-item-tracking.md)


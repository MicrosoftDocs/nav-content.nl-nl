---
title: 'Ontwerpdetails: Vraag en aanbod afsluiten'
description: Wanneer de vereffeningsprocedures voor voorzieningen zijn uitgevoerd, zijn er drie mogelijke eindsituaties.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 337fdb4c625e17e72f4adb692cbf0f2729ae96b7
ms.contentlocale: nl-nl
ms.lasthandoff: 10/26/2017

---
# <a name="design-details-closing-demand-and-supply"></a>Ontwerpdetails: Vraag en aanbod afsluiten
Wanneer de vereffeningsprocedures voor voorzieningen zijn uitgevoerd, zijn er drie mogelijke eindsituaties:  

-   Er is voldaan aan het benodigde aantal en de datum van de vraaggebeurtenissen en de planning hiervoor kan worden afgesloten. De voorzieningsgebeurtenis is nog open en kan de volgende vraag verwerken, zodat de vereffeningsprocedure overnieuw kan starten met de huidige voorzieningsgebeurtenis en de volgende vraag.  

-   De voorzieningenorder kan niet worden aangepast om alle vraag te verwerken. De vraaggebeurtenis is nog open, met een niet-gedekt aantal dat mogelijk kan worden gedekt door de volgende voorzieningsgebeurtenis. De huidige voorzieningsgebeurtenis wordt dus afgesloten, zodat de vereffeningsprocedure opnieuw kan starten met de huidige vraag en de volgende voorzieningsgebeurtenis.  

-   Alle vraag is gedekt; er is geen verdere vraag (of er is helemaal geen vraag geweest). Als er eventuele surplusvoorziening is, kan deze worden verlaagd (of geannuleerd) en vervolgens gesloten. Het is mogelijk dat er verder in de keten aanvullende voorzieninggebeurtenissen zijn en die moeten ook worden geannuleerd.  

 Als laatste maakt het planningssysteem een ordertraceringskoppeling tussen de voorziening en de vraag.  

## <a name="creating-the-planning-line-suggested-action"></a>De planningsregel (voorgestelde actie) maken  
 Als een actie - Nieuw, Aantal wijzigen, Herplannen, Herplannen en aantal wijzigen of Annuleren- wordt voorgesteld om de voorzieningenorder te herzien, maakt het planningssysteem een planningsregel in het planningsvoorstel. Vanwege ordertracering wordt de planningsregel niet alleen gemaakt wanneer de voorzieningsgebeurtenis wordt afgesloten, maar ook als de vraaggebeurtenis wordt afgesloten, zelfs als de voorzieningsgebeurtenis nog openstaat en nog kan veranderen als de volgende vraaggebeurtenis wordt verwerkt. Dit betekent dat nadat de planningsregel is gemaakt, deze weer kan worden gewijzigd.  

 Om databasetoegang te beperken bij het verwerken van productieorders, kan de planningsregel worden onderhouden op drie niveaus terwijl wordt geprobeerd het minst veeleisende onderhoudsniveau uit te voeren:  

-   Maak alleen de planningsregel met de huidige vervaldatum en aantal maar zonder het bewerkingsplan en materialen.  

-   Bewerkingsplan opnemen: het geplande bewerkingsplan wordt opgesteld inclusief de berekening van begin- en einddatums en -tijden. Dit is vereist voor wat betreft de databasetoegang. Voor het bepalen van de eind- en vervaldatums kan het noodzakelijk zijn om dit te berekenen, zelfs als de voorzieningsgebeurtenis niet is afgesloten (in het geval van voorwaartse planning).  

-   Ontwikkeling stuklijst opnemen: dit kan wachten tot vlak voordat de voorzieningsgebeurtenis wordt gesloten.  

 Hiermee worden de omschrijvingen afgerond van hoe vraag en voorzieningen worden geladen, prioriteit krijgen en worden vereffend door het planningssysteem. Bij integratie met deze voorraadplanningactiviteit moet het systeem ervoor zorgen dat het vereiste voorraadniveau van elk gepland artikel wordt onderhouden op basis van het bestelbeleid.  

## <a name="see-also"></a>Zie ook  
 [Ontwerpdetails: Vraag en aanbod afstemmen](design-details-balancing-demand-and-supply.md)   
 [Ontwerpdetails: Centrale begrippen van het planningssysteem](design-details-central-concepts-of-the-planning-system.md)   
 [Ontwerpdetails: Voorraadplanning](design-details-supply-planning.md)


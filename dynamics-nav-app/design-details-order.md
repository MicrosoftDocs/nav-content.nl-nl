---
title: 'Ontwerpdetails: Order'
description: In dit onderwerp vindt u informatie over order-naar-order-koppelingen in een omgeving waarin op order wordt geproduceerd.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, order
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7e8105795f4b2a45510fc50cfed4a8fadad8f1eb
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-order"></a>Ontwerpdetails: Order
In een op-order-produceren omgeving wordt een artikel ingekocht of geproduceerd om uitsluitend aan een specifieke vraag te voldoen. Meestal heeft dit betrekking op A-producten en de motivatie om het bestelbeleid Order te kiezen, kan zijn dat de vraag niet frequent is, dat de doorlooptijd onbeduidend is of dat de vereiste kenmerken verschillen.  
  
Het programma maakt een order-naar-order-koppeling die fungeert als voorlopige verbinding tussen de voorziening, een voorzieningenorder of voorraad, en de vraag waaraan het zal voldoen.  
  
Afgezien van het gebruik van het bestelbeleid kan de order-aan-order koppeling tijdens planning op de volgende manieren worden toegepast:  
  
* Wanneer het productiebeleid Op order produceren wordt gebruikt om productieorders met meerdere niveaus of projecttype te maken (waarbij benodigde onderdelen op dezelfde productieorder worden geproduceerd).  
* Wanneer de functie Verkooporderplanning wordt gebruikt om een productieorder te maken van een verkooporder.  
  
Zelfs als een productiebedrijf zichzelf beschouwt als een op-order-produceren omgeving, kan het het best zijn een lot-voor-lot bestelbeleid te gebruiken als de artikelen standaard zijn, zonder variatie in kenmerken. Hierdoor gebruikt het systeem niet-geplande voorraad en worden verkooporders alleen gecumuleerd met dezelfde verzenddatum of binnen een bepaalde periode.  
  
## <a name="order-to-order-links-and-past-due-dates"></a>Order-naar-order koppelingen en overschreden vervaldatums  
In tegenstelling tot de meeste combinaties van voorziening en vraag, worden gekoppelde orders met vervaldatums voor de begindatum van de planning, volledig door het systeem gepland. De bedrijfsreden voor deze uitzondering is dat specifieke vraag-voorzieningcombinaties moeten worden gesynchroniseerd tot aan uitvoering. Zie voor meer informatie over de bevroren zone die de meeste vraag/voorziening toepast [Ontwerpdetails: Werken met orders voor de geplande begindatum](design-details-dealing-with-orders-before-the-planning-starting-date.md).  
  
## <a name="see-also"></a>Zie ook  
[Ontwerpdetails: Bestelbeleid](design-details-reordering-policies.md)   
[Ontwerpdetails: Planningsparameters](design-details-planning-parameters.md)   
[Ontwerpdetails: Bestelbeleid verwerken](design-details-handling-reordering-policies.md)   
[Ontwerpdetails: Voorraadplanning](design-details-supply-planning.md)

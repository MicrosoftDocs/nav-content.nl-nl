---
title: 'Aanbevolen procedures instellen: Bestelbeleid'
description: Het veld **Bestelbeleid** op artikelkaarten biedt vier verschillende planningmethodes die de interactie tussen de afzonderlijke planningsparameters aansturen.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b96fc662f741bd705e673f7d17b2467b4e6dc846
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="setup-best-practices-reordering-policies"></a>Aanbevolen procedures instellen: Bestelbeleid
Het veld **Bestelbeleid** op artikelkaarten biedt vier verschillende planningmethodes die de interactie tussen de afzonderlijke planningsparameters aansturen.  

De aanbevolen procedure voor het selecteren van een bestelbeleid is de ABC-classificatie van het product. Wanneer u ABC-classificatie voor voorraadbeheer en -planning gebruikt, worden items volgens drie verschillende klassen beheerd, afhankelijk van de waarde en het volume ten opzichte van de totale voorraad. De waarde/volume-verhouding van de drie klassen wordt in de volgende tabel weergegeven.

|Klasse|Percentage van de totale omvang in voorraad|Percentage van de totale waarde in voorraad|
|-----|-----------------------------|----------------------------|
|A|10-20|50-70|
|B|20|20|
|L|60-70|10-30|

De ABC-classificatie stelt dat inspanningen en geld bespaard kunnen worden door minder controle toe te passen op items met een lage waarde/volume-verhouding dan op items met een hoge waarde/volume-verhouding. De volgende illustratie toont welk bestelbeleid in [!INCLUDE[d365fin](includes/d365fin_md.md)] het geschiktst is voor respectievelijk items van het type A, B of C.

![ABC-classificatie](media/abc_classification.png "abc_classification")

De volgende tabel bevat de aanbevolen procedures voor het selecteren van de vier beleidsterreinen.  

|Insteloptie|Aanbevolen procedure|Opmerking|  
|------------------|-------------------|-------------|  
|**Order**|Gebruiken voor A-producten.<br /><br /> Gebruiken voor op maat gemaakte producten.<br /><br /> Gebruik in de productie voor items op het hoogste niveau en voor dure onderdelen en halffabrikaten.<br /><br /> Gebruiken voor artikelen die als doorverzendingen en speciale orders worden aangekocht.<br /><br /> Niet gebruiken als u geen automatische reservering accepteert.|A-artikelen, zoals lederen banken in een meubelwinkel, zijn dure artikelen met lage en onregelmatige bestelsnelheden waarbij voorraad onaanvaardbaar is of de vereiste kenmerken variëren. Het beste bestelbeleid is daarom een beleid dat specifiek voor elke vraag een planning maakt.|  
|**Lot-for-Lot**|Gebruiken voor B-producten.<br /><br /> Gebruiken in de productie voor onderdelen die op meerdere stuklijsten voorkomen. Dit zorgt ervoor dat inkooporders voor dezelfde leverancier worden gecombineerd zodat betere prijzen kunnen worden onderhandeld.<br /><br /> Gebruiken als u niet zeker weet welk bestelbeleid u moet selecteren.|B-artikelen, zoals eetkamerstoelen, hebben een regelmatige en redelijk hoge bestelsnelheid maar ook hoge opslagkosten. Het beste bestelbeleid voor B-artikelen is daarom een voordelig beleid dat de vraag bij de bestelcyclus bundelt.<br /><br /> 80 procent van de artikelen kan dit beleid gebruiken.<br /><br /> Kan worden gebruikt zonder planningparameters.|  
|**Vast bestelaantal**|Gebruiken voor C-producten.<br /><br /> Combineren met bestelpuntparameters.<br /><br /> Gebruiken in de productie voor onderdelen van het laagste niveau.<br /><br /> Niet gebruiken als het artikel vaak wordt gereserveerd.|C-artikelen, zoals theekopjes, zijn artikelen met een lage waarde en een hoge en regelmatige bestelsnelheid. Het beste bestelbeleid voor C-artikelen is daarom een beleid dat constante beschikbaarheid garandeert door altijd boven het bestelpunt te blijven.<br /><br /> Als de gebruiker een hoeveelheid reserveert voor een onzekere vraag, raakt de planning verstoord. Zelfs als de geplande voorraad met betrekking tot het bestelpunt aanvaardbaar is, zijn de hoeveelheden mogelijk niet beschikbaar vanwege de reservering.|  
|**Maximum aantal**|Gebruiken voor C-artikelen met hoge transportkosten of opslagbeperkingen.<br /><br /> Combineren met een of meer orderwijzigingen (Minimum/Maximum bestelaantal of lotgrootte).|C-artikelen, zoals theekopjes, zijn artikelen met een lage waarde en een hoge en regelmatige bestelsnelheid. Het beste bestelbeleid voor C-artikelen is daarom een beleid dat constante beschikbaarheid garandeert door altijd boven het bestelpunt te blijven, maar onder een maximum voorraadhoeveelheid.<br /><br /> Om het voorgestelde order te wijzigen, kunt u het bestelaantal verlagen tot een opgegeven maximum bestelaantal, verhoogd tot een opgegeven minimum bestelaantal of afgerond tot het voldoet aan een opgegeven lotgrootte. **Opmerking:** als dit in combinatie met een bestelpunt wordt gebruikt, blijft de voorraad tussen bestelpunt en het maximum aantal.|  

## <a name="see-also"></a>Zie ook  
 [Aanbevolen procedures instellen: Voorraadplanning](setup-best-practices-supply-planning.md)   
 [Ontwerpdetails: Bestelbeleid](design-details-reordering-policies.md)   
 [Ontwerpdetails: Order](design-details-order.md)   
 [Ontwerpdetails: Lot-voor-lot](design-details-lot-for-lot.md)   
 [Ontwerpdetails: Vast bestelaantal](design-details-fixed-reorder-qty.md)   
 [Ontwerpdetails: Maximaal aantal](design-details-maximum-qty.md)   
 [Complexe toepassingsgebieden instellen met aanbevolen procedures](set-up-complex-application-areas-using-best-practices.md)  
 [Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


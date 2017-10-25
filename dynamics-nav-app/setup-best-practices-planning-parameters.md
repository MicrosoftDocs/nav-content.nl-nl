---
title: 'Aanbevolen procedures instellen: Planningparameters'
description: "Het sneltabblad **Planning** op de artikelkaart is het hart van de toeleveringsketen van een bedrijf. De juiste planningsparameters instellen is zeer belangrijk voor efficiënt voorraadbeheer en sterke klantenservice."
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 8ea9ceaffa7a82405c43783d2a22f0b81ec4600d
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="setup-best-practices-planning-parameters"></a>Aanbevolen procedures instellen: Planningparameters
Het sneltabblad **Planning** op de artikelkaart is het hart van de toeleveringsketen van een bedrijf. De juiste planningsparameters instellen is zeer belangrijk voor efficiënt voorraadbeheer en sterke klantenservice.  

 De volgende tabel bevat de aanbevolen procedures voor het instellen van de geselecteerde planningparametervelden. Voor meer informatie over een veld, kiest u de koppeling in de kolom **Veld instellen**.  

|Veld instellen|Aanbevolen procedure|Opmerking|  
|-----------------|-------------------|-------------|  
|Bestelbeleid||Zie voor meer informatie [Aanbevolen procedures instellen: Bestelbeleid](setup-best-practices-reordering-policies.md).|  
|Reserveren|Selecteer **nooit** wanneer het artikel is gepland met behulp van een bestelpunt.<br /><br /> Selecteer in de productie **nooit** om het planningssysteem alle aanvragen te laten dekken.<br /><br /> Selecteer **optioneel** voor artikelen die u wilt reserveren voor de belangrijkste klanten.<br /><br /> Selecteer **altijd** voor niet-unieke artikelen, zoals artikelen van het type divers die op specifieke aanvraag binnenkomen.|Reserveringen neutraliseren algemeen het doel van de planning, die bestemd is om vraag en aanbod op elkaar af te stemmen. Daarom mogen items die zijn ingesteld voor planning over het algemeen niet worden gereserveerd.<br /><br /> Als de gebruiker een voorraadaantal voor toekomstige vraag reserveert, wordt de planning verstoord en is bestelpunt mogelijk niet correct. Zelfs als de geplande voorraad met betrekking tot het bestelpunt aanvaardbaar is, zijn de hoeveelheden mogelijk niet beschikbaar vanwege de reservering.|  
|Dempingsperiode|Instellen met het oog op de flexibiliteit van de leverancier.|Als de leverancier wijzigingen in de laatste orders accepteert, kunt u een langere periode gebruiken. Als de leverancier een vaste planning vereist, moet u uw periode zo veel mogelijk inkorten.<br /><br /> Zie [Ontwerpdetails: Planningsparameters](design-details-planning-parameters.md) voor informatie over de algemene instellingen.|  
|Dempingsaantal||Zie [Ontwerpdetails: Planningsparameters](design-details-planning-parameters.md) voor informatie over de algemene instellingen.|  
|Inclusief voorraad|Altijd selecteren wanneer u het Lot-per-Lot bestelbeleid gebruikt.|Niet alleen selecteren in speciale situaties, zoals wanneer voorraadartikelen niet verkoopbaar zijn.|  
|Veiligheidstijd|Ingesteld tussen 1D en 6D<br /><br /> Stel een veiligheidstijd in van ten minste één dag om ervoor te zorgen dat de goederen beschikbaar zijn op de dag voordat ze nodig zijn.<br /><br /> Als u een nieuwe leverancier gebruikt, stel dan een langere tijd in totdat hun leveringsprestaties bekend zijn.<br /><br /> Definieer langere levertijden voor kritieke onderdelen in de productie.|Leveringen die door het systeem gepland zijn om voorraaduitputting te voorkomen, worden geleverd op de dag dat de uitputting zich voordoet. Dit kan verscheidene uren te laat zijn indien, bijvoorbeeld de vraag 's ochtends nodig is en de levering in de namiddag gebeurt. **Opmerking:** het veld **Veiligheidstijd** gebruikt de basisagenda. 14D is dus niet noodzakelijkerwijs twee weken.|  
|Veiligheidsvoorraad|Gebruiken voor artikelen met grote schommelingen in de vraag.<br /><br /> Gebruiken in de productie voor kritieke onderdelen.<br /><br /> Gebruiken voor artikelen die onder serviceovereenkomsten vallen.|Als het veld **Bestelpunt** niet is ingevuld, werkt de veiligheidsvoorraad ook als bestelpunt.|  
|Lotaccumulatieperiode|Als u alleen enkele grote orders wilt en u wilt een voorraad aanhouden, stel dan een lang lotaccumulatieperiode in.<br /><br /> Als u meerdere kleine orders en minimale voorraad wilt, stel dan een korte lotaccumulatieperiode in.|De lotaccumulatieperiode is doorgaans de langste periode waarin u voorraad bijhoudt.|  
|Bestelpunt|Baseer het bestelpunt op het vraagprofiel van het artikel.|Als historische gegevens aantonen dat de gemiddelde artikelvraag 100 eenheden is met een doorlooptijd van zeven dagen, kan het bestelpunt worden ingesteld op een minimum van 100.<br /><br /> Dit betekent dat wanneer het voorraadniveau minder dan 100 bedraagt, het planningssysteem zal voorstellen om aan te vullen omdat het zeven dagen duurt om het artikel te leveren en omdat er voldoende moet zijn om de vraag gedurende zeven dagen te dekken.|  
|Tijdsinterval|Leeg laten, wat betekent dat het voorraadniveau elke dag wordt gecontroleerd.|Het voorraadniveau dagelijks controleren zorgt voor optimale bestelpuntplanning. **Opmerking:** een tijdsinterval van 1W betekent dat het voorraadniveau gedurende één week onder het bestelpunt mag liggen voordat een voorzieningsorder wordt voorgesteld.|  
|Afrondingsprecisie|Instellen op 0,00001 bij dure productie.|Grote hoeveelheden afval of materiaalverbruik kunnen leiden tot zeer grote voorraadkosten. Daarom kan het relevant zijn om de kleinste afrondingsprecisie in te stellen om deze potentiële kost te minimaliseren.|  

> [!NOTE]  
>  Aanbevolen procedures voor de planningsparameters op artikelkaarten zijn ook van toepassing op dezelfde velden op de SKU-kaarten.  
>   
>  Als bedrijven de vraag voor verschillende vestigingen plannen, dan is het ten zeerste aanbevolen om SKU's te definiëren voor elke locatie en om alle vraag te maken met een waarde in het veld **vestigingscode**. Zie [Ontwerpdetails: Vraag op lege vestiging](design-details-demand-at-blank-location.md) voor meer informatie.  

## <a name="see-also"></a>Zie ook  
 [Aanbevolen procedures instellen: Voorraadplanning](setup-best-practices-supply-planning.md)   
 [Ontwerpdetails: Voorzieningsplanning](design-details-supply-planning.md)   
 [Complexe toepassingsgebieden instellen met aanbevolen procedures](set-up-complex-application-areas-using-best-practices.md)  
 [Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


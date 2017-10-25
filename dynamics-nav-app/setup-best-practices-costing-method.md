---
title: 'Best Practices voor instellen: Waarderingsmethode'
description: De **Waarderingsmethode** op de artikelkaart definieert hoe de kostenstroom van het artikel wordt geregistreerd en of een werkelijke of gebudgetteerde waarde wordt gekapitaliseerd en gebruikt in de kostenberekening.
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
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: a2c25ffc6c2012bac4e86ebbce0f3c33ecaf68fc
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="setup-best-practices-costing-method"></a>Best Practices voor instellen: Waarderingsmethode
De **Waarderingsmethode** op de artikelkaart definieert hoe de kostenstroom van het artikel wordt geregistreerd en of een werkelijke of gebudgetteerde waarde wordt gekapitaliseerd en gebruikt in de kostenberekening.  

 Het instellen van de juiste waarderingsmethode overeenkomstig het artikelsoort en de bedrijfsomgeving is belangrijk om economische voorraden te garanderen.  

 De volgende tabel bevat de aanbevolen procedures voor het instellen van het veld **Waarderingsmethode**. Zie [Ontwerpdetails: Waarderingsmethoden](design-details-costing-methods.md) voor meer informatie.  

|Insteloptie|Aanbevolen procedure|Opmerking|  
|------------------|-------------------|-------------|  
|FIFO|Gebruik waar de productkosten stabiel zijn.<br /><br /> Gebruik voor artikelen met een beperkte houdbaarheid, omdat de oudste goederen moeten worden verkocht voordat ze hun uiterste houdbaarheidsdatum overschrijden.|De kostprijs van een artikel is de werkelijke waarde van de ontvangst van het artikel dat met de FIFO-regel is geselecteerd.<br /><br /> In voorraadwaardering wordt verondersteld dat de artikelen die als eerste in voorraad worden geplaatst, als eerst worden verkocht. **Opmerking:** wanneer de prijzen stijgen, wordt in de balans een grotere waarde weergegeven. Dit betekent dat de belastingschulden vermeerderen, maar de creditscores en de mogelijkheid om contanten te lenen verbeteren.|  
|LIFO|Gebruik waar voorraadniveaus voortdurend worden onderhouden of na verloop van tijd worden verhoogd.|De kostprijs van een artikel is de werkelijke waarde van de ontvangst van het artikel dat met de LIFO-regel is geselecteerd.<br /><br /> In voorraadwaardering wordt verondersteld dat de artikelen die als laatste in voorraad worden geplaatst, als eerst worden verkocht. **Opmerking:** wanneer de prijzen stijgen, vermindert de waarde op de resultatenrekening. Dit betekent dat de belastingschulden verminderen, maar de mogelijkheid om contanten te lenen verslechterd. **Belangrijk**: Verboden in veel landen of regio's, aangezien het kan worden gebruikt voor het drukken van winst.|  
|Gemiddelde|Gebruik waar de productkosten instabiel zijn.<br /><br /> Gebruik waar de voorraden worden gestapeld of samengevoegd en niet kunnen worden onderscheiden, zoals chemische producten.|De kostprijs van een artikel bestaat uit de exacte kosten waarmee de betreffende eenheid is ontvangen.|  
|Specifiek|Gebruik in productie of handel van gemakkelijk identificeerbare artikelen met tamelijk hoge kostprijs.<br /><br /> Gebruiken voor artikelen die onder wetgeving vallen.<br /><br /> Gebruik voor artikelen met met serienummers.|De kostprijs van een artikel wordt berekend als de gemiddelde kostprijs op elk tijdstip na de inkoop.<br /><br /> Voor voorraadwaardering wordt aangenomen dat alle voorraden tegelijkertijd zijn verkocht.|  
|Vast|Gebruik waar kostenbeheersing essentieel is.<br /><br /> Gebruik in herhaalde productie, om de directe materiaal-, arbeids- en productieoverheadkosten te waarderen.<br /><br /> Gebruik waar er discipline en personeel zijn om normen na te volgen.|De kostprijs van een artikel is vooraf ingesteld op basis van de geschatte prijs.<br /><br /> Wanneer de werkelijke kosten later gerealiseerd zijn, moet de vaste verrekenprijs aan de werkelijke aangepast worden door verschilwaarden.|  

## <a name="see-also"></a>Zie ook  
 [Ontwerpdetails: Waarderingsmethoden](design-details-costing-methods.md)   
 [Ontwerpdetails: Voorraadwaardering](design-details-inventory-costing.md)   
 [Complexe toepassingsgebieden instellen met aanbevolen procedures](set-up-complex-application-areas-using-best-practices.md)  
 [Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


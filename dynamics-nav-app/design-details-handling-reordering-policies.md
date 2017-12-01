---
title: 'Ontwerpdetails: Bestelbeleid verwerken'
description: "Overzicht van taken voor het definiëren van een bestelbeleid in voorraadplanning."
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
ms.openlocfilehash: 2cd1d0e770e5fd7daa92e98486038aefdb678c5a
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-handling-reordering-policies"></a>Ontwerpdetails: Bestelbeleid verwerken
Om een artikel deel te laten nemen aan voorraadplanning, moet een bestelbeleid worden gedefinieerd. Er zijn vier soorten bestelbeleid:  
  
* Vast bestelaantal  
* Maximum aantal  
* Order  
* Lot-for-Lot  
  
Beleid voor vast bestelaantal en maximum aantal heeft betrekking op voorraadplanning. Hoewel voorraadplanning technisch eenvoudiger is dan de vereffeningsprocedure, moet dit beleid naast elkaar bestaan met stapsgewijze vereffening van voorziening en ordertracering. Er gelden strikte regels voor de verwerking van het bestelbeleid om de integratie tussen deze twee te beheren en om zichtbaarheid te bieden in de betrokken planningslogica.  
  
## <a name="in-this-section"></a>In dit gedeelte  
[Ontwerpdetails: De rol van het bestelpunt](design-details-the-role-of-the-reorder-point.md)  
[Ontwerpdetails: Het verwachte voorraadniveau en het bestelpunt controleren](design-details-monitoring-the-projected-inventory-level-and-the-reorder-point.md)  
[Ontwerpdetails: De rol van het tijdsinterval](design-details-the-role-of-the-time-bucket.md)  
[Ontwerpdetails: Onder het overflowniveau blijven](design-details-staying-under-the-overflow-level.md)  
[Ontwerpdetails: Verwachte negatieve voorraad verwerken](design-details-handling-projected-negative-inventory.md)  
[Ontwerpdetails: Bestelbeleid](design-details-reordering-policies.md)  
  
## <a name="see-also"></a>Zie ook  
[Ontwerpdetails: Planningsparameters](design-details-planning-parameters.md)   
[Ontwerpdetails: Tabel Planningstoewijzing](design-details-planning-assignment-table.md)   
[Ontwerpdetails: Centrale begrippen van het planningssysteem](design-details-central-concepts-of-the-planning-system.md)   
[Ontwerpdetails: Vraag en aanbod afstemmen](design-details-balancing-demand-and-supply.md)   
[Ontwerpdetails: Voorraadplanning](design-details-supply-planning.md)

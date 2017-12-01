---
title: 'Ontwerpdetails: Verschil'
description: Verschil wordt gedefinieerd als het verschil tussen de werkelijke kosten en de vaste verrekenprijs, zoals in de volgende formule wordt beschreven.
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
ms.openlocfilehash: 63032d592b5fe9e58c52e64ed0a30ceeda2532fe
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-variance"></a>Ontwerpdetails: Verschil
Verschil wordt gedefinieerd als het verschil tussen de werkelijke kosten en de vaste verrekenprijs, zoals in de volgende formule wordt beschreven.  

 werkelijke kosten – standaardkosten = verschil  

 Als de werkelijke kosten veranderen, bijvoorbeeld omdat u een artikeltoeslag boekt op een latere datum, wordt het verschil overeenkomstig bijgewerkt.  

> [!NOTE]  
>  Herwaardering heeft geen invloed op de verschilberekening, omdat herwaardering alleen de voorraadwaarde wijzigt.  

## <a name="example"></a>Opmerking  
 In het volgende voorbeeld ziet u hoe het verschil wordt berekend voor aangeschafte artikelen. Het is gebaseerd op het volgende scenario:  

1.  De gebruiker koopt een artikel tegen LV 90,00, maar de vaste verrekenprijs is LV 100,00. Het inkoopverschil is dus LV -10,00.  
2.  LV 10,00 wordt gecrediteerd naar de inkoopverschillenrekening.  
3.  De gebruiker boekt een artikeltoeslag van LV 20,00. De werkelijke kosten worden verhoogd tot LV 110,00 en de waarde van het inkoopverschil wordt LV 10,00.  
4.  LV 20,00 wordt gedebiteerd naar de inkoopverschillenrekening. Het netto-inkoopverschil wordt LV 10,00.  
5.  De gebruiker herwaardeert het artikel van LV 100,00 naar LV 70,00. Dit heeft geen invloed op de verschilberekening, alleen op de voorraadwaarde.  

 De volgende tabel toont de twee soorten resulterende waardeposten.  

 ![Berekening van het inkoopverschil](media/design_details_inventory_costing_11_purchase_variance.png "design_details_inventory_costing_11_purchase_variance")  

## <a name="determining-the-standard-cost"></a>De standaardkosten bepalen  
 De vaste verrekenprijs wordt gebruikt bij het berekenen van het te kapitaliseren verschil en aantal. Aangezien de vaste verrekenprijs na verloop van tijd kan worden gewijzigd als gevolg van handmatige updateberekeningen, hebt u een tijdstip nodig waarop de vaste verrekenprijs wordt vastgesteld voor verschilberekening. Dit punt is wanneer de voorraadtoename wordt gefactureerd. Voor geproduceerde of geassembleerde artikelen worden standaardkosten bepaald wanneer de kosten worden gewaardeerd.  

 De volgende tabel toont hoe verschillende kostenaandelen worden gegenereerd voor geproduceerde en geassembleerde artikelen als u de functie Vaste verrekenprijs berekenen gebruikt.  

|Aandeel kosten|Ingekocht artikel|Geproduceerd/geassembleerd artikel|  
|----------------|--------------------|------------------------------|  
|**Vaste verrekenprijs**||Materiaalkosten (één niveau) + Capaciteitskosten (één niveau) + Uitbestedingskosten (één niveau) + Cap.-overheadkosten (één niveau) + Prod.-overheadkosten (één niveau)|  
|**Materiaalkosten (Eén niv.)**|Kostprijs|![Vergelijking 1](media/design_details_inventory_costing_11_equation_1.png "design_details_inventory_costing_11_equation_1")|  
|**Capaciteitskosten (Eén niv.)**|Niet van toepassing|![Vergelijking 2](media/design_details_inventory_costing_11_equation_2.png "design_details_inventory_costing_11_equation_2")|  
|**Uitbestedingskosten (Eén niv.)**|Niet van toepassing|![Vergelijking 3](media/design_details_inventory_costing_11_equation_3.png "design_details_inventory_costing_11_equation_3")|  
|**Cap.-overheadkosten (Eén niv.)**|Niet van toepassing|![Vergelijking 4](media/design_details_inventory_costing_11_equation_4.png "design_details_inventory_costing_11_equation_4")|  
|**Prod.-overheadkosten. (Eén niv.)**|Niet van toepassing|(Materiaalkosten (één niveau) + Capaciteitskosten (één niveau) + Uitbestedingskosten (één niveau)) * Indirecte kosten % / 100 + Overheadtarief|  
|**Materiaalkosten (Alle niv.)**|Kostprijs|![Vergelijking 5](media/design_details_inventory_costing_11_equation_5.png "design_details_inventory_costing_11_equation_5")|  
|**Capaciteitskosten (Alle niv.)**|Niet van toepassing|![Vergelijking 6](media/design_details_inventory_costing_11_equation_6.png "design_details_inventory_costing_11_equation_6")|  
|**Uitbestedingskosten (Alle niv.)**|Niet van toepassing|![Vergelijking 7](media/design_details_inventory_costing_11_equation_7.png "design_details_inventory_costing_11_equation_7")|  
|**Samengevouwen capaciteitsoverheadkosten**|Niet van toepassing|![Vergelijking 8](media/design_details_inventory_costing_11_equation_8.png "design_details_inventory_costing_11_equation_8")|  
|**Prod.-overheadkosten (Alle niv.)**|Niet van toepassing|![Vergelijking 9](media/design_details_inventory_costing_11_equation_9.png "design_details_inventory_costing_11_equation_9")|  

## <a name="see-also"></a>Zie ook  
 [Ontwerpdetails: Voorraadwaardering](design-details-inventory-costing.md)   
 [Ontwerpdetails: Waarderingsmethoden](design-details-costing-methods.md) [Voorraadkosten beheren](finance-manage-inventory-costs.md)  
 [Financiën](finance.md)  
 [Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


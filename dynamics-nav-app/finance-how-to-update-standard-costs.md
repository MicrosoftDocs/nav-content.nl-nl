---
title: Vaste verrekenprijzen aanpassen
description: U moet regelmatig de vaste verrekenprijzen van onderdelen bijwerken en de nieuwe kosten tot aan het hoofdartikel berekenen.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/09/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: dd2bb16af611be7f7720fdf07eb65fd268aba039
ms.contentlocale: nl-nl
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-update-standard-costs"></a>Procedure: vaste verrekenprijzen aanpassen
U moet regelmatig de vaste verrekenprijzen van onderdelen bijwerken en de nieuwe kosten tot aan het hoofdartikel berekenen. Het proces bestaat meestal uit de volgende vier stappen:  

1.  Kosten bijwerken op het niveau van onderdeel en capaciteit. Zie voor meer informatie de batchverwerking **Vaste verrekenprijs artikel voorstellen**.  
2.  Het consolideren en berekenen van de materiaal- en capaciteitskosten om de totale productiekosten van de artikelen te berekenen.  
3.  De vaste verrekenprijzen implementeren die worden ingevoerd wanneer u de vorige batchverwerkingen uitvoert. De vaste verrekenprijzen worden pas van kracht nadat ze zijn geïmplementeerd. Zie voor meer informatie Vaste verrekenprijswijzigingen doorvoeren.  
4.  De wijzigingen implementeren om het veld **Kostprijs** op de artikelkaart bij te werken en voorraadherwaardering uit te voeren. Zie [Procedure: Voorraad herwaarderen](inventory-how-revalue-inventory.md) voor meer informatie.  

Zie [Vaste verrekenprijs berekenen](finance-about-calculating-standard-cost.md) voor nadere informatie.  
## <a name="to-update-standard-costs"></a>Vaste verrekenprijs aanpassen  
1.  Voer de batchverwerking **Kostprijs herwaarderen - Artikelposten** uit.  
2.  Voer de batchverwerking **Voorraadwaarde boeken** uit.  
3.  Open het **Vaste-verrekenprijsvoorstel** en gebruik een of meer van de volgende functies:  

    1.  Voer de batchverwerking **Vaste verrekenprijs artikel voorstellen** uit.  
    2.  Bekijk de resultaten en breng desgewenst wijzigingen aan.  
    3.  Voer de batchverwerking **Vaste verrekenprijs capaciteit voorstellen** uit.  
    4.  Bekijk de resultaten en breng desgewenst wijzigingen aan.
    5. Voer de batchverwerking **Vaste verrekenprijs berekenen** uit.
    6.  Bekijk de resultaten en breng desgewenst wijzigingen aan.
    7.  Voer de batchverwerking **Vaste verrekenprijswijzigingen doorvoeren** uit.  
4.  Bekijk en boek het venster **Herwaarderingsdagboek**, waarin de posten uit de vorige stappen in dit proces zijn ingevuld.  

## <a name="see-also"></a>Zie ook  
 [Informatie over het berekenen van vaste verrekenprijzen](finance-about-calculating-standard-cost.md)   
 [Voorraadkosten beheren](finance-manage-inventory-costs.md)   
 [Ontwerpdetails: Waarderingsmethoden](design-details-costing-methods.md) [[Financiën](finance.md)  
 [Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  


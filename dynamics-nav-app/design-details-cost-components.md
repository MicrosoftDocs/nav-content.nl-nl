---
title: 'Ontwerpdetails: Kostenonderdelen'
description: Kostenonderdelen zijn verschillende soorten kosten die de waarde vormen van een artikeltoename of -afname.
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
ms.openlocfilehash: 2971e080c0acd47bff6d7ba6f21e1a366a6de5e8
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-cost-components"></a>Ontwerpdetails: Kostenonderdelen
Kostenonderdelen zijn verschillende soorten kosten die de waarde vormen van een artikeltoename of -afname.  

 De volgende tabel toont de verschillende kostenonderdelen en eventuele onderliggende kostenonderdelen waaruit ze bestaan.  

|Kostenonderdeel|Ondergeschikt kostenonderdeel|Description|  
|--------------------|--------------------------------|---------------------------------------|  
|Directe kosten|Kostprijs (directe inkoopprijs)|Kosten die kunnen worden herleid tot een kostenobject.|  
|Directe kosten|Vrachtkosten (artikeltoeslag)|Kosten die kunnen worden herleid tot een kostenobject.|  
|Directe kosten|Verzekeringskosten (artikeltoeslag)|Kosten die kunnen worden herleid tot een kostenobject.|  
|Indirecte kosten||Kosten die niet kunnen worden herleid tot een kostenobject.|  
|Verschil|Inkoopverschil|Het verschil tussen werkelijke kosten en de vaste verrekenprijs. Wordt uitsluitend geboekt voor artikelen met de waarderingsmethode **Standaard**.|  
|Verschil|Materiaalverschil|Het verschil tussen werkelijke kosten en de vaste verrekenprijs. Wordt uitsluitend geboekt voor artikelen met de waarderingsmethode **Standaard**.|  
|Verschil|Capaciteitsverschil|Het verschil tussen werkelijke kosten en de vaste verrekenprijs. Wordt uitsluitend geboekt voor artikelen met de waarderingsmethode **Standaard**.|  
|Verschil|Uitbestedingsverschil|Het verschil tussen werkelijke kosten en de vaste verrekenprijs. Wordt uitsluitend geboekt voor artikelen met de waarderingsmethode **Standaard**.|  
|Verschil|Verschillen cap.-overhead|Het verschil tussen werkelijke kosten en de vaste verrekenprijs. Wordt uitsluitend geboekt voor artikelen met de waarderingsmethode **Standaard**.|  
|Verschil|Productieoverheadverschil|Het verschil tussen werkelijke kosten en de vaste verrekenprijs. Wordt uitsluitend geboekt voor artikelen met de waarderingsmethode **Standaard**.|  
|Herwaardering||Waardevermindering of -vermeerdering van de huidige voorraadwaarde.|  
|Afronding||Restwaarden die ontstaan door de manier waarop de waardering van negatieve voorraadmutaties wordt berekend.|  

> [!NOTE]  
>  Vracht- en verzekeringskosten zijn artikeltoeslagen die op elk moment aan de kosten van een artikel kunnen worden toegevoegd. Wanneer u de batchverwerking **Kostprijs herwaarderen - Artikelposten** uitvoert, wordt de waarde van gerelateerde negatieve voorraadmutaties overeenkomstig bijgewerkt.  

## <a name="see-also"></a>Zie ook  
 [Ontwerpdetails: Voorraadwaardering](design-details-inventory-costing.md)   
 [Ontwerpdetails: Verschil](design-details-variance.md) [Voorraadkosten beheren](finance-manage-inventory-costs.md)  
 [Financiën](finance.md)  
 [Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  


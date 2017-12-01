---
title: 'Ontwerpdetails: Verwachte kostenboeking'
description: Verwachte kosten zijn de schatting van, bijvoorbeeld de kosten van een ingekocht artikel, die u vastlegt voordat u de factuur voor het artikel ontvangt.
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
ms.openlocfilehash: 0b14943e1bb214c26dfbae765a2467df1d06e50b
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-expected-cost-posting"></a>Ontwerpdetails: Verwachte kostenboeking
Verwachte kosten zijn de schatting van, bijvoorbeeld de kosten van een ingekocht artikel, die u vastlegt voordat u de factuur voor het artikel ontvangt.  

 U kunt verwachte kosten boeken naar de voorraad en het grootboek. Wanneer u een aantal boekt dat alleen wordt ontvangen of verzonden, maar niet gefactureerd, wordt een waardepost gemaakt met de verwachte kosten. Deze verwachte kosten zijn van invloed op de voorraadwaarde, maar worden niet geboekt naar het grootboek, tenzij u het systeem hebt ingesteld om dit te doen.  

> [!NOTE]  
>  Verwachte kosten worden alleen beheerd voor artikeltransacties. Verwachte kosten zijn niet voor immateriële transactiesoorten zoals capaciteit en artikelkosten.  

 Als slechts het aantaldeel van een voorraadtoename is geboekt, verandert de voorraadwaarde in het grootboek niet, tenzij u het selectievakje **Verw. kostprijs naar GB boeken** hebt geselecteerd in het venster **Voorraadinstelling**. In dat geval worden de verwachte kosten geboekt naar interimrekeningen op het moment van ontvangst. Nadat de ontvangst volledig is gefactureerd, worden de interimrekeningen vereffend en worden de werkelijke kosten geboekt naar de voorraadrekening.  

 Ter ondersteuning van reconciliatie en traceerbaarheid bevat de gefactureerde waardepost het verwachte kostenbedrag dat is geboekt om de interimrekeningen te vereffenen.  

## <a name="example"></a>Opmerking  
 Het volgende voorbeeld toont verwachte kosten als het selectievakje **Autom. voorraadwaarde boeken** en **Verw. kostprijs naar GB boeken** zijn ingeschakeld in het venster **Voorraadinstelling**.  

 U boekt een inkooporder als ontvangen. De verwachte kosten zijn LV 95,00.  

 **Waardeposten**  

|Boekingsdatum|Boekingssoort|Tot. verw. kosten|Verw. kostn geboekt nr grootbk|Verwachte kosten|Artikelpostnr.|Volgnummer|  
|------------------|----------------|------------------------------|----------------------------------|-------------------|---------------------------|---------------|  
|01-01-20|Directe kosten|95,00|95,00|Ja|1|1|  

 **Relatieposten in het grootboek - Relatietabel artikelposten**  

|Grootboekpostnr.|Waardepostnr.|Grootboekjournaalnr.|  
|--------------------|---------------------|-----------------------|  
|1|1|1|  
|2|1|1|  

 **Grootboekposten**  

|Boekingsdatum|Grootboekrekening|Rekeningnr. (En-US demo)|Bedrag|Volgnummer|  
|------------------|------------------|---------------------------------|------------|---------------|  
|01-01-20|Voorraadtussenrekening (tussenrek.)|5530|-95,00|2|  
|01-01-20|Voorraadrekening (tussenrek.)|2131|95,00|1|  

 U kunt de inkooporder op een later moment boeken als gefactureerd. De gefactureerde kosten zijn LV 100,00.  

 **Waardeposten**  

|Boekingsdatum|Tot. werk. kosten|Tot. verw. kosten|Vrd.-waarde geboekt|Verwachte kosten|Artikelpostnr.|Volgnummer|  
|------------------|----------------------------|------------------------------|-------------------------|-------------------|---------------------------|---------------|  
|15-01-20|100.00|-95,00|100.00|Nee|1|2|  

 **Relatieposten in het grootboek - Relatietabel artikelposten**  

|Grootboekpostnr.|Waardepostnr.|Grootboekjournaalnr.|  
|--------------------|---------------------|-----------------------|  
|3|2|2|  
|4|2|2|  
|5|2|2|  
|6|2|2|  

 **Grootboekposten**  

|Boekingsdatum|Grootboekrekening|Rekeningnr. (En-US demo)|Bedrag|Volgnummer|  
|------------------|------------------|---------------------------------|------------|---------------|  
|15-01-20|Voorraadtussenrekening (tussenrek.)|5530|95,00|4|  
|15-01-20|Voorraadrekening (tussenrek.)|2131|-95,00|3|  
|15-01-20|Vereffeningsrekening directe kosten|7291|-100|6|  
|15-01-20|Voorraadrekening|2130|100|5|  

## <a name="see-also"></a>Zie ook
 [Ontwerpdetails: Voorraadwaardering](design-details-inventory-costing.md)   
 [Ontwerpdetails: Kostenwaardering](design-details-cost-adjustment.md)   
 [Ontwerpdetails: Reconciliatie met het grootboek](design-details-reconciliation-with-the-general-ledger.md)   
 [Ontwerpdetails: Voorraadboeking](design-details-inventory-posting.md)   
 [Ontwerpdetails: Verschil](design-details-variance.md)  
 [Voorraadkosten beheren](finance-manage-inventory-costs.md)  
 [Financiën](finance.md)  
 [Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


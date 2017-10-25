---
title: 'Ontwerpdetails: Tabelstructuur'
description: Om te begrijpen hoe de functie voor opslag en boekingen van dimensieposten opnieuw wordt ontworpen, is het belangrijk om de tabelstructuur te begrijpen.
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
ms.openlocfilehash: f39360c3890a521cc921e49dd038c18a4a51f805
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-table-structure"></a>Ontwerpdetails: Tabelstructuur
Om te begrijpen hoe de functie voor opslag en boekingen van dimensieposten opnieuw wordt ontworpen, is het belangrijk om de tabelstructuur te begrijpen.  

## <a name="new-tables"></a>Nieuwe tabellen  
 Er zijn drie nieuwe tabellen ontworpen om dimensiesetposten te beheren.  

### <a name="table-480-dimension-set-entry"></a>Tabel 480 Dimensiesetpost  
 Tabel 480 **Dimensiesetpost** is een nieuwe tabel. U kunt deze tabel niet wijzigen. Nadat gegevens naar de tabel zijn geschreven, kunt u ze niet meer verwijderen of wijzigen. Het verwijderen van gegevens vereist dat u alle gevallen controleert van de dimensieset-id in de hele database, inclusief partneroplossingen.  

|Veldnr.|Veldnaam|Gegevenssoort|Opmerking|  
|---------------|----------------|---------------|-------------|  
|1|**Id**|Geheel getal|>0,0 is gereserveerd voor de lege dimensieset. Verwijst naar veld 3 in tabel 481.|  
|2|**Dimensiecode**|Code 20|Tabelrelatie met tabel 348.|  
|3|**Dimensiewaardecode**|Code 20|Tabelrelatie met tabel 349.|  
|4|**Dimensiewaarde-id**|Geheel getal|Verwijst naar veld 12 in tabel 349. Het is de secundaire sleutel die wordt gebruikt wanneer tabel 481 wordt doorlopen.|  
|5|**Dimensienaam**|Tekst 30|CalcField. Opzoeken in tabel 348.|  
|6|**Dimensiewaardenaam**|Tekst 30|CalcField. Opzoeken in tabel 349.|  

#### <a name="table-481-dimension-set-tree-node"></a>Tabel 481 Boomstructuurpunt dimensieset  
 Tabel 481 **Boomstructuurpunt dimensieset** is een nieuwe tabel. U kunt deze tabel niet wijzigen. De tabel wordt gebruikt om te zoeken naar een dimensieset. Als de dimensieset niet wordt gevonden, wordt een nieuwe set gemaakt.  

|Veldnr.|Veldnaam|Gegevenssoort|Opmerking|  
|---------------|----------------|---------------|-------------|  
|1|**Bovenliggende dimensieset-id**|Geheel getal|0 voor knooppunt bovenste niveau.|  
|2|**Dimensiewaarde-id**|Geheel getal|Tabelrelatie met veld 12 in tabel 349.|  
|3|**Dimensieset-id**|Geheel getal|AutoIncrement. Gebruikt in veld 1 in tabel 480.|  
|4|**In gebruik**|Boolean|Onwaar indien niet in gebruik.|  

##### <a name="table-482-reclas-dimension-set-buffer"></a>Tabel 482 Herklass. dimensiesetbuffer  
 Tabel 482 **Herklass. dimensiesetbuffer** is een nieuwe tabel. De tabel wordt gebruikt om een dimensieset-id te wijzigen. Het is vereist wanneer u een dimensiewaardecode en een nieuwe dimensiewaardecode bewerkt, bijvoorbeeld in de tabel **Art.-herindelingsdagboek**.  

|Veldnr.|Veldnaam|Gegevenssoort|Opmerking|  
|---------------|----------------|---------------|-------------|  
|1|**Dimensiecode**|Code 20|Tabelrelatie met tabel 348.|  
|2|**Dimensiewaardecode**|Code 20|Tabelrelatie met tabel 349.|  
|3|**Dimensiewaarde-id**|Geheel getal|Verwijst naar veld 12 in tabel 349.|  
|4|**Nieuwe dimensiewaardecode**|Code 20|Tabelrelatie met tabel 349.|  
|5|**Nieuwe dimensiewaarde-id**|Geheel getal|Verwijst naar veld 12 in tabel 349.|  
|6|**Dimensienaam**|Tekst 30|CalcField. Opzoeken in tabel 348.|  
|7|**Dimensiewaardenaam**|Tekst 30|CalcField. Opzoeken in tabel 349.|  
|8|**Nieuwe dimensiewaardenaam**|Tekst 30|CalcField. Opzoeken in tabel 349.|  

## <a name="modified-tables"></a>Gewijzigde tabellen  
 Alle transactie- en budgettabellen zijn gewijzigd om dimensiesetposten te beheren.  

### <a name="changes-to-transaction-and-budget-tables"></a>Wijzigingen in transactie- en budgettabellen  
 Er is een nieuw veld toegevoegd aan alle transactie- en budgettabellen.  

|Veldnr.|Veldnaam|Gegevenssoort|Opmerking|  
|---------------|----------------|---------------|-------------|  
|480|**Dimensieset-id**|Geheel getal|Verwijst naar veld 1 in tabel 480.|  

#### <a name="changes-to-table-83-item-journal-line"></a>Wijzigingen in tabel 83 Artikeldagboekregel  
 Twee nieuwe velden zijn toegevoegd aan tabel 83 **Artikeldagboekregel**.  

|Veldnr.|Veldnaam|Gegevenssoort|Opmerking|  
|---------------|----------------|---------------|-------------|  
|480|**Dimensieset-id**|Geheel getal|Verwijst naar veld 1 in tabel 480.|  
|481|**Nieuwe dimensieset-id**|Geheel getal|Verwijst naar veld 1 in tabel 480.|  

##### <a name="changes-to-table-349-dimension-value"></a>Wijzigingen in tabel 349 Dimensiewaarde  
 Er is een nieuw veld toegevoegd aan tabel 349 **Dimensiewaarde**.  

|Veldnr.|Veldnaam|Gegevenssoort|Opmerking|  
|---------------|----------------|---------------|-------------|  
|12|**Dimensiewaarde-id**|Geheel getal|AutoIncrement. Gebruikt voor referenties in tabel 480 en tabel 481.|  

###### <a name="tables-that-get-new-field-480-dimension-set-id"></a>Tabellen met het nieuwe veld 480 Dimensieset-id  
 Er is een nieuw veld, 480 **Dimensieset-id**, toegevoegd aan de volgende tabellen. Voor de tabellen waarin de geboekte gegevens worden opgeslagen, levert het veld alleen een niet-bewerkbare weergave van dimensies, die wordt gemarkeerd als Meer details. Voor de tabellen waarin werkdocumenten worden opgeslagen, is het veld bewerkbaar. Voor de buffertabellen die intern worden gebruikt, zijn geen bewerkbare of niet-bewerkbare voorzieningen nodig.  

 Veld 480 kan niet worden bewerkt in de volgende tabellen.  

|Tabelnr.|Tabelnaam|  
|---------------|----------------|  
|17|**Grootboekpost**|  
|21|**Klantenpost**|  
|25|**Leverancierspost**|  
|32|**Artikelpost**|  
|110|**Verkoopverzendkop**|  
|111|**Verkoopverzendregel**|  
|112|**Verkoopfactuur**|  
|113|**Verkoopfactuurregel**|  
|114|**Verkoopcreditnota**|  
|115|**Verkoopcreditnotaregel**|  
|120|**Inkoopontvangst**|  
|121|**Inkoopontvangstregel**|  
|122|**Inkoopfactuur**|  
|123|**Inkoopfactuurregel**|  
|124|**Inkoopcreditnota**|  
|125|**Inkoopcreditnotaregel**|  
|169|**Projectpost**|  
|203|**Resourcepost**|  
|271|**Bankpost**|  
|281|**Inventarisatiepost**|  
|297|**Verzonden aanmaning**|  
|304|**Verzonden rentefactuur**|  
|5107|**Verkoopkoparchief**|  
|5108|**Verkoopregelarchief**|  
|5109|**Inkoopkoparchief**|  
|5110|**Inkoopregelarchief**|  
|5601|**VA-post**|  
|5625|**Onderhoudspost**|  
|5629|**Verzekeringsdekkingspost**|  
|5744|**Transferverzendkop**|  
|5745|**Transferverzendregel**|  
|5746|**Transferontvangstkop**|  
|5747|**Transferontvangstregel**|  
|5802|**Waardepost**|  
|5832|**Capaciteitspost**|  
|5907|**Servicepost**|  
|5908|**Servicekop**|  
|5933|**Serviceorderboekingsbuffer**|  
|5970|**Gearch. servicecontractkop**|  
|5990|**Serviceverzendingskop**|  
|5991|**Serviceverzendingsregel**|  
|5992|**Servicefactuurkop**|  
|5993|**Servicefactuurregel**|  
|5994|**Servicecreditnotakop**|  
|5995|**Servicecreditnotaregel**|  
|6650|**Retourverzending**|  
|6651|**Retourverzendregel**|  
|6660|**Retourontvangstkop**|  
|6661|**Retourontvangstregel**|  

 Veld 480 kan worden bewerkt in de volgende tabellen.  

|Tabelnr.|Tabelnaam|  
|---------------|----------------|  
|36|**Verkoopkop**|  
|37|**Verkoopregel**|  
|38|**Inkoopkop**|  
|39|**Inkoopregel**|  
|81|**Fin. dagboekregel**|  
|83|**Artikeldagboekregel**|  
|89|**Stuklijstdagboekregel**|  
|96|**Budgetpost**|  
|207|**Resourcedagboekregel**|  
|210|**Projectdagboekregel**|  
|221|**Dagboekverdeelsleutel**|  
|246|**Behoefteregel**|  
|295|**Aanmaning**|  
|302|**Rentefactuur**|  
|5405|**Productieorder**|  
|5406|**Prod.-orderregel**|  
|5407|**Materiaalregel**|  
|5615|**VA-verdeelsleutel**|  
|5621|**VA-dagboekregel**|  
|5635|**Verzekeringsdagboekregel**|  
|5740|**Transferkop**|  
|5741|**Transferregel**|  
|5900|**Servicekop**|  
|5901|**Serviceartikelregel**|  
|5902|**Serviceregel**|  
|5965|**Servicecontractkop**|  
|5997|**Standaardserviceregel**|  
|7134|**Artikelbudgetpost**|  
|99000829|**Planningsmateriaal**|  

 Veld 480 is toegevoegd aan de volgende buffertabellen.  

|Tabelnr.|Tabelnaam|  
|---------------|----------------|  
|49|**Factuurboekingsbuffer**|  
|212|**Projectboekingsbuffer**|  
|372|**Betalingsbuffer**|  
|382|**K/L-postbuffer**|  
|461|**Regelbuffer vooruitbetalingsfactuur**|  
|5637|**VA-fin. boekingsbuffer**|  
|7136|**Buffer artikelbudget**|  

## <a name="see-also"></a>Zie ook  
 [Ontwerpdetails: Dimensiesetposten](design-details-dimension-set-entries.md)   
 [Dimensiesetposten - overzicht](design-details-dimension-set-entries-overview.md)   
 [Ontwerpdetails: Dimensiecombinaties zoeken](design-details-searching-for-dimension-combinations.md)   
 [Ontwerpdetails: Codeunit 408 Dimensiebeheer](design-details-codeunit-408-dimension-management.md)   
 [Ontwerpdetails: Codevoorbeelden van gewijzigde patronen in wijzigingen](design-details-code-examples-of-changed-patterns-in-modifications.md)


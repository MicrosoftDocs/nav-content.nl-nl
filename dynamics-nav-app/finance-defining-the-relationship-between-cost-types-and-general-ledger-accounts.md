---
title: "De relatie tussen de kostensoorten en grootboekrekeningen definiëren"
description: Leer hoe u de relatie tussen de kostensoort en de grootboekrekening definieert.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cost types, general ledger
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 6bedd251aad7f15f40a255e5b44c6080bbb73bdb
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="defining-the-relationship-between-cost-types-and-general-ledger-accounts"></a>De relatie tussen de kostensoorten en grootboekrekeningen definiëren
De relatie tussen het kostensoort en de grootboekrekening wordt gemaakt in het kostensoort en in de grootboekrekening.  

* Het veld **Grootboekrekeningbereik** in de tabel **Kostensoort** bepaalt welke grootboekrekeningen tot een kostensoort behoren.  
* Het veld **Nr. saldokostensoort** in het rekeningschema bepaalt tot welk kostensoort een grootboekrekening behoort.  

Deze twee velden worden automatisch ingevuld wanneer u de functie **Kostensoorten ophalen uit rekeningschema** gebruikt.  

## <a name="relationship-between-general-ledger-accounts-and-cost-types"></a>Relatie tussen de grootboekrekeningen en kostensoorten  
Er bestaat een n:1-relatie tussen de grootboekrekeningen en kostensoorten Verschillende grootboekrekeningen kunnen tot één kostensoort behoren, maar elke afzonderlijke grootboekrekening behoort maar tot één kostensoort. De volgende tabel beschrijft de detail in de relatie.  

|Relatie|**Grootboekrekeningbereik**|**Nr. kostensoort**|  
|------------------|------------------------------------------------|-------------------------------------------|  
|Één grootboekrekening voor elk kostensoort|Eén grootboekrekening|Eén kostensoort|  
|Verschillende grootboekrekeningen voor één kostensoort|Bijvoorbeeld rekeningenbereik grootboek 7110..7193 voor elke grootboekrekening|Voor elke grootboekrekening in het bereik is slechts één kostensoort|  
|Kostensoorten zonder overeenkomende grootboekrekeningen|<Empty>||  
|Grootboekrekeningen waarvan de posten niet overgebracht worden||<Empty>|  

## <a name="cost-types-without-a-relationship-to-the-general-ledger"></a>Kostensoorten zonder relatie met het grootboek  
Er bestaat mogelijk geen relatie tussen een kostensoort en grootboekrekeningen als aan een van de volgende voorwaarden wordt voldaan:  

* Rekeningen voor operationeel boekhouden zoals voor het de berekenen van rente en afschrijvingen, nemen alleen de kosten mee van de operationele boekhouding.  
* Ondersteunende kostensoorten, zoals kostensoorten 9901, 9902 en 9903 in de [!INCLUDE[d365fin](includes/d365fin_md.md)]-database , worden gebruikt als credit- of debet-rekeningen voor toewijzingen.  
* De ondersteunende rekening, 9920 in de [!INCLUDE[d365fin](includes/d365fin_md.md)]-database, bevat de werkelijke overlopende transitoria die het verschil laten zien tussen de kosten en de onkosten uit het grootboek.  

## <a name="see-also"></a>Zie ook  
[Kosten verantwoorden](finance-manage-cost-accounting.md)  
[Kostenboekhouding instellen](finance-set-up-cost-accounting.md)   
[Kostprijsboekhouding](finance-about-cost-accounting.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


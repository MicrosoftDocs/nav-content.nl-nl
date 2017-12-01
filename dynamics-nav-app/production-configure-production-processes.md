---
title: Productieprocessen configureren
description: Als u materiaal wilt omzetten in geproduceerde eindartikelen, moeten productieresources, zoals stuklijsten, bewerkingsplannen, machinebedienden en machines worden ingesteld in het systeem.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/04/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b22fe53cc9a9ce6bb357f9eaf54fc37c4e1242b9
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="setting-up-manufacturing"></a>Productie instellen
Als u materiaal wilt omzetten in geproduceerde eindartikelen, moeten productieresources, zoals stuklijsten, bewerkingsplannen, machinebedienden en machines worden ingesteld in het systeem.

Machinebedienden en machines worden in het systeem weergegeven als bewerkingsplaatsen die in afdelingen en afdelingsgroepen kunnen worden ingedeeld. Wanneer deze resources zijn ingesteld, kunnen hieraan bewerkingen worden toegewezen aan de hand van de gedefinieerde materiaal- (stuklijst) en processtructuur (bewerkingsplan) voor het artikel en volgens de capaciteit van de bewerkingsplaats of afdeling. U kunt ook de productiecapaciteit van elke afzonderlijke resource instellen. De capaciteit wordt gedefinieerd aan de hand van de beschikbare werktijd voor de machine en afdelingen en wordt bepaald door agenda's voor elk niveau. In een agenda voor een afdeling worden de gegevens voor het aantal werkdagen of -uren, de diensten, de vakantiedagen en de afwezigheid aangegeven die de bruto beschikbare capaciteit van de afdeling bepalen (gewoonlijk uitgedrukt in minuten). Dit alles wordt bepaald door de waarden die zijn gedefinieerd voor de efficiency en capaciteit.  

Wanneer u de productie hebt ingesteld, kunt u productieorders plannen en uitvoeren. Zie [Planning](production-planning.md) en [Productie](production-manage-manufacturing.md) voor meer informatie.  

 In de volgende tabel wordt een reeks taken beschreven, met koppelingen naar de beschrijvende onderwerpen.   

|**Als u dit wilt doen**|**Zie**|  
|------------|-------------|  
|De productiefuncties configureren, zoals het definiëren van shopfloorwerkuren en het selecteren van planningsprincipes.|De pagina **Productie-instellingen**.|  
|Een standaardwerkweek in de productieafdeling definiëren met de begin- en eindtijd van elke werkdag en de bijbehorende dienst.|[Procedure: Productieagenda's maken](production-how-to-create-work-center-calendars.md)|  
|Vaste waarden en vereisten van productieresources indelen als afdelingen of bewerkingsplaatsen om de productie-output te bepalen.|[Procedure: Afdelingen en bewerkingsplaatsen instellen](production-how-to-set-up-work-and-machine-centers.md)|
|Productiebewerkingen in de vereiste volgorde indelen en met de vereiste werktijden toewijzen aan afdelingen of bewerkingsplaatsen.|[Procedure: bewerkingsplannen maken](production-how-to-create-routings.md)|
|Productiematerialen of halffabricaten indelen onder een geproduceerd hoofdartikel en de stuklijst voor uitvoering certificeren in afdelingen.|[Procedure: productiestuklijsten maken](production-how-to-create-production-boms.md)|
|Controleren of het juiste onderdeelaantal beschikbaar is als geproduceerde artikelen in één eenheid in voorraad zijn, maar in een andere eenheid worden geproduceerd.|[Procedure: Werken met productiebatcheenheden](production-how-to-use-the-manufacturing-batch-unit-of-measure.md)|  
|Productfamilies met productieartikelen definiëren met soortgelijke productieprocessen om op verbruik te besparen. Uit één vel kunnen bijvoorbeeld tegelijkertijd vier stuks van het ene artikel en tien stuks van een ander artikel worden geproduceerd.|[Procedure: Werken met productfamilies](production-how-work-family.md)|
|Standaardtaken gebruiken om het maken van bewerkingsplannen te vereenvoudigen door extra informatie bij te voegen voor terugkerende bewerkingen.|[Procedure: Standaard bewerkingsplanregels instellen](production-how-set-up-standard-routing-lines.md)|  
|Afdelingen en bewerkingsplannen voor uitbestede productiebewerkingen voorbereiden.|[Procedure: Productie uitbesteden](production-how-to-subcontract-manufacturing.md)|  

## <a name="see-also"></a>Zie ook
[Productie](production-manage-manufacturing.md)    
[Gepland](production-planning.md)   
[Voorraad](inventory-manage-inventory.md)  
[Inkoop](purchasing-manage-purchasing.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


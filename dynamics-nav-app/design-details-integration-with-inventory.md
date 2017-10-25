---
title: 'Ontwerpdetails: Integratie met voorraad'
description: De module Magazijnbeheer en de module Voorraad kunnen met elkaar communiceren in inventarisatie en in voorraad- of magazijnherwaardering.
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
ms.openlocfilehash: ca9a1b5b1ea20fc125107f3fb5b7a74814a85837
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-integration-with-inventory"></a>Ontwerpdetails: Integratie met voorraad
De module Magazijnbeheer en de module Voorraad kunnen met elkaar communiceren in inventarisatie en in voorraad- of magazijnherwaardering.  
  
## <a name="physical-inventory"></a>Physical Inventory  
 Het venster **Mag.-inventarisatiedagboek** wordt gebruikt met het venster **Inventarisatiedagboek** voor alle geavanceerd magazijnvestigingen. De voorraad op het niveau van opslaglocaties wordt berekend en er wordt een afgedrukte lijst geleverd voor de magazijnmedewerker. Het overzicht toont welke artikelen in welke opslaglocaties moeten worden geteld.  
  
 De magazijnmedewerker voert het getelde aantal in het venster **Mag.-inventarisatiedagboek** in en boekt vervolgens het dagboek.  
  
 Als het getelde aantal groter is dan het aantal op de dagboekregel, wordt een verplaatsing voor dit verschil geboekt van de standaard herwaarderingsopslaglocatie naar de getelde opslaglocatie. Hiermee wordt het aantal in de getelde opslaglocatie verhoogd en het aantal in de standaardherwaarderingsopslaglocatie verlaagd.  
  
 Als het getelde aantal kleiner is dan het aantal op de dagboekregel, wordt een verplaatsing voor dit verschil geboekt van de getelde opslaglocatie naar de standaard herwaarderingsopslaglocatie. Hiermee wordt het aantal in de getelde opslaglocatie verlaagd en het aantal in de standaardherwaarderingsopslaglocatie verhoogd.  
  
 In geavanceerde magazijnconfiguraties wordt de waarde in het veld **Aantal (berekend)** opgehaald uit artikelposten en wordt de waarde in het veld **Aantal (Inventarisatie)** opgehaald uit magazijnposten, met uitzondering van de inhoud van de herwaarderingsopslaglocatie. Het veld **Aantal** geeft het verschil aan tussen de eerste twee velden, en moet gelijk zijn aan de inhoud van de correctieopslaglocatie.  
  
 Wanneer u het inventarisatiedagboek boekt, wordt de voorraad en de standaardherwaarderingsopslaglocatie bijgewerkt.  
  
### <a name="warehouse-adjustments-to-the-item-ledger"></a>Magazijncorrecties in de artikelpost  
 U gebruikt het venster **Artikeldagboek** en de functie **Magazijnherwaardering berekenen** om voorraad op de artikelpost aan te passen in overeenstemming met een aanpassing die is gemaakt in het artikelaantal in een magazijnopslaglocatie. Als u een koppeling tussen de voorraad en het magazijn wilt maken, moet u een standaardherwaarderingsopslaglocatie per vestiging definiëren.  
  
 De standaardcorrectieopslaglocatie registreert artikelen in het magazijn wanneer u een toename voor de voorraad boekt. Als u echter een afname boekt, wordt het aantal op de standaardopslaglocatie ook verlaagd. In beide gevallen worden artikelposten en magazijnposten gemaakt.  
  
> [!NOTE]  
>  De correctieopslaglocatie wordt niet weergegeven in de beschikbaarheidsberekening.  
  
 Wanneer u de opslaglocatie-inhoud wilt aanpassen, kunt u het magazijnartikeldagboek gebruiken, van waaruit u het artikelnummer, de zonecode, de opslaglocatiecode en het aantal kunt invoeren die u wilt aanpassen.  
  
 Als u een positief aantal invoert en de regel boekt, wordt de voorraad die in de opslaglocatie is opgeslagen vergroot en wordt het aantal dat in de standaardherwaarderingsopslaglocatie is opgeslagen, even veel verkleind.  
  
## <a name="see-also"></a>Zie ook  
 [Ontwerpdetails: Magazijnbeheer](design-details-warehouse-management.md)   
 [Ontwerpdetails: Beschikbaarheid in het magazijn](design-details-availability-in-the-warehouse.md)

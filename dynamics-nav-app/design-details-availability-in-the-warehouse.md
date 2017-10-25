---
title: 'Ontwerpdetails: Beschikbaarheid in het magazijn'
description: "Het systeem moet een constante controle op artikelbeschikbaarheid in het magazijn hebben, zodat uitgaande orders efficiënt kunnen stromen en optimale leveringen kunnen worden geboden."
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
ms.openlocfilehash: 875286386168fea79f47dfdf0c78ef202cc21da0
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-availability-in-the-warehouse"></a>Ontwerpdetails: Beschikbaarheid in het magazijn
Het systeem moet een constante controle op artikelbeschikbaarheid in het magazijn hebben, zodat uitgaande orders efficiënt kunnen stromen en optimale leveringen kunnen worden geboden.  

 De beschikbaarheid varieert afhankelijk van toewijzingen op het niveau van de opslaglocatie, wanneer magazijnactiviteiten optreden zoals picks en verplaatsingen en wanneer het voorraadreserveringssysteem beperkingen oplegt. Een tamelijk complex algoritme verifieert of aan alle voorwaarden is voldaan voordat aantallen worden toegewezen aan picks voor uitgaande stromen.  

## <a name="bin-content-and-reservations"></a>Inhoud van opslaglocatie en reserveringen  
 In elke installatie van magazijnbeheer bestaan artikelaantallen als magazijnposten, in het magazijntoepassingsgebied, en als artikelposten, in het voorraadtoepassingsgebied. Deze twee boekingssoorten bevatten verschillende informatie over waar artikelen bestaan en of ze beschikbaar zijn. Met magazijnposten wordt de beschikbaarheid van een artikel per (soort) opslaglocatie gedefinieerd, wat opslaglocatie-inhoud wordt genoemd. Artikelposten definiëren de beschikbaarheid van een artikel op basis van de reservering hiervan voor uitgaande documenten.  

 Er bestaan speciale functies in het algoritme voor picken om het aantal te berekenen dat kan worden gepickt wanneer de opslaglocatie-inhoud wordt gekoppeld met reserveringen.  

## <a name="quantity-available-to-pick"></a>Beschikbaar aantal voor picken  
 Wanneer het pickalgoritme bijvoorbeeld geen rekening houdt met artikelaantallen die zijn gereserveerd voor een wachtende verkooporderverzending, kunnen die artikelen worden gepickt voor een andere verkooporder die eerder wordt verzonden, wat voorkomt dat aan de eerste verkoop wordt voldaan. Om deze situatie te voorkomen, wordt met het algoritme voor picken aantallen afgetrokken die zijn gereserveerd voor andere uitgaande documenten, aantallen op bestaande pickdocumenten, en aantallen die zijn gepickt maar nog niet verzonden of verbruikt.  

 Het resultaat wordt weergegeven in het veld **Beschikb. te picken aantal** in het venster **Pick Worksheet**, waar het veld dynamisch wordt berekend. De waarde wordt ook berekend wanneer gebruikers magazijnpicks direct voor uitgaande documenten maken. Dergelijke uitgaande documenten kunnen verkooporders, productieverbruik of uitgaande transfers zijn, waar het resultaat wordt weergegeven in de bijbehorende velden met aantallen, zoals **Te verwerken aantal**.  

> [!NOTE]  
>  Voor wat betreft de prioriteit van reserveringen wordt het te reserveren aantal afgetrokken van het aantal dat beschikbaar is voor picken. Als het beschikbare aantal in pickopslaglocaties bijvoorbeeld 5 eenheden is, maar 100 eenheden zich in opslaglocaties bevinden en u probeert meer dan 5 eenheden voor een andere order te reserveren, wordt een foutbericht weergegeven omdat het extra aantal in pickopslaglocaties beschikbaar moet zijn.  

### <a name="calculating-the-quantity-available-to-pick"></a>Het aantal berekenen dat beschikbaar is voor picken  
 Het aantal dat beschikbaar is voor picken, wordt als volgt berekend:  

 beschikbaar aantal om te picken = aantal in pickopslaglocaties - aantal in picks en verplaatsingen – (gereserveerd aantal in pickopslaglocaties + gereserveerd aantal in picks en verplaatsingen)  

 Het volgende diagram bevat de verschillende elementen van de berekening.  

 ![Beschikbaar te picken aantal met reserveringsoverlapping](media/design_details_warehouse_management_availability_2.png "design_details_warehouse_management_availability_2")  

## <a name="quantity-available-to-reserve"></a>Beschikbaar aantal voor reserveren  
 Omdat de concepten opslaglocatie en reservering naast elkaar bestaan, moet het aantal artikelen dat beschikbaar is om te reserveren, worden afgestemd met toewijzingen aan uitgaande magazijndocumenten.  

 Het zou mogelijk moeten zijn om alle artikelen in voorraad te reserveren, met uitzondering van artikelen waarvoor uitgaande verwerking is gestart. Het aantal dat kan worden gereserveerd, wordt gedefinieerd als het aantal in alle documenten en alle typen opslaglocaties, behalve de volgende uitgaande aantallen:  

-   Aantal in niet-geregistreerde pickdocumenten  
-   Aantal in verzendopslaglocaties  
-   Aantal in naar-productieopslaglocaties  
-   Aantal in grijpvoorraadlocaties  
-   Aantal in naar-assemblageopslaglocaties  
-   Aantal in correctieopslaglocaties  

 Het resultaat wordt weergegeven in het veld **Totaal beschikbaar aantal** in het venster **Reservation**.  

 Op een reserveringsregel wordt het aantal dat niet kan worden gereserveerd omdat het in het magazijn is toegewezen, weergegeven in het veld **Aant. toegewezen in magazijn** in het venster **Reservering**.  

### <a name="calculating-the-quantity-available-to-reserve"></a>Het aantal berekenen dat beschikbaar is voor reservering  
 Het aantal dat beschikbaar is voor reserveringen, wordt als volgt berekend:  

 beschikbaar aantal om te reserveren = totaal aantal in voorraad - aantal in picks en verplaatsingen voor brondocumenten - gereserveerd aantal - aantal in uitgaande opslaglocaties  

 Het volgende diagram bevat de verschillende elementen van de berekening.  

 ![Beschikbaar voor reserveren, per magazijntoewijzingen](media/design_details_warehouse_management_availability_3.png "design_details_warehouse_management_availability_3")  

## <a name="see-also"></a>Zie ook  
 [Ontwerpdetails: Magazijnbeheer](design-details-warehouse-management.md)


---
title: Artikelen en locaties instellen voor gestuurde opslag en pick
description: "Er is bij het instellen van een magazijnlocatie voor gestuurde opslag en pick nieuwe functionaliteit beschikbaar om u te helpen om het magazijn op de meest efficiënte wijze te beheren."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 6ec7065cb2d633ea18c586c6369487052464a482
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-items-and-locations-for-directed-put-away-and-pick"></a>Procedure: Artikelen en locaties instellen voor gestuurde opslag en pick
Er is bij het instellen van een magazijnlocatie voor gestuurde opslag en pick nieuwe functionaliteit beschikbaar om u te helpen om het magazijn op de meest efficiënte wijze te beheren. Als u deze functionaliteit ten volle wilt benutten, geeft u extra informatie op over de artikelen, zodat het eenvoudiger wordt om de berekeningen uit te voeren die zijn vereist voor het voorstellen van de meest efficiënte en de meest doeltreffende wijzen voor het uitvoeren van magazijnactiviteiten. Zie voor meer informatie [Ontwerpdetails: Magazijninstelling](design-details-warehouse-setup.md).

## <a name="to-set-up-an-item-for-directed-put-away-and-pick"></a>U kunt als volgt een artikelen instellen voor gestuurde opslag en pick  
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Artikelen** in en klik vervolgens op de gerelateerde koppeling.  
2.  Open de kaart voor het artikel dat u wilt instellen voor gestuurde opslag en pick.
3. Door de velden op het sneltabblad **Magazijn** van het artikel in te vullen geeft u aan hoe het artikel in het magazijn wordt verwerkt.  
4.  Kies de actie **Eenheden**.
5. Vul de velden in het venster **Artikeleenheden** in om aan te geven in welke eenheden de artikeltransacties worden uitgevoerd. Voer ook de hoogte, breedte, lengte, kubieke inhoud en het gewicht in voor de verschillende eenheden.
6. Kies de actie **Opslaglocatie-inhoud**.
7. In het venster **Opslaglocatie-inhoud** kunt u de vestiging en opslaglocatie definiëren waaraan u het artikel wilt toewijzen. Het veld **Standaard** wordt niet gebruikt wanneer de vestiging is ingesteld voor gestuurde opslag en pick.  

## <a name="to-activate-directed-put-away-and-pick-functionality"></a>Om gestuurde opslag en pick te activeren  
Met gestuurde opslag en pick beschikt u over geavanceerde magazijnconfiguratiefuncties, waardoor de efficiëntie en de betrouwbaarheid van gegevens sterk kunnen worden verbeterd. Als u deze functionaliteit wilt gebruiken, moet u eerst een aantal parameters instellen in uw magazijn.  

Als u de functionaliteit van gestuurde opslag en pick wilt gebruiken, moet u deze functionaliteit activeren op de vestigingskaart.    
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Vestigingen** in en klik vervolgens op de gerelateerde koppeling.  
2.  Selecteer de vestiging waarin u gestuurde opslag en pick wilt gebruiken en kies de actie **Bewerken**.  
3.  Schakel het selectievakje **Gestuurde opslag en pick** op het sneltabblad **Magazijn** in.  

U hoeft de andere velden op de vestigingskaart pas later in het installatieproces in te vullen.  

> [!NOTE]  
>  U kunt het gebruik van opslaglocaties niet voor het magazijn instellen als voor de vestiging nog artikelposten openstaan.  

De volgende stap bestaat uit het definiëren van het soort opslaglocatie waarmee u wilt werken. Zie [Procedure: Opslaglocatiesoorten instellen](warehouse-how-to-set-up-bin-types.md) voor meer informatie. Hiermee geeft u aan hoe een bepaalde opslaglocatie wordt gebruikt bij de verwerking van de artikelenstroom in het magazijn. U kunt een bepaald soort opslag toewijzen aan zowel een zone als een opslaglocatie.  

Als bepaalde artikelen onder verschillende omstandigheden moeten worden opgeslagen in het magazijn, kunt u ook magazijnklassen definiëren. Magazijnklassen worden gebruikt voor het voorstellen van de plaatsing van artikelen in opslaglocaties. U wijst magazijnklassen toe aan productgroepen, die vervolgens worden toegewezen aan artikelen en SKU's of zones en opslaglocaties die kunnen voldoen aan de opslagvoorwaarden die de magazijnklasse vereist.  

U bent nu gereed om zones instellen als u in uw magazijn wilt werken met zones. Met zones vermindert u het aantal velden dat u moet invullen wanneer u uw opslaglocaties instelt omdat opslaglocaties die in zones zijn gemaakt verschillende eigenschappen van de zone overnemen. Zones kunnen het bovendien voor nieuwe of tijdelijke werknemers eenvoudiger maken om zich in uw magazijn te oriënteren. Houd er rekening mee dat de stroom wordt beheerd door opslaglocaties, waardoor het mogelijk is om met opslaglocaties en slechts één zone te werken.  

## <a name="to-set-up-a-zone-in-your-warehouse"></a>U kunt als volgt een zone instellen in het magazijn  
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Vestigingen** in en klik vervolgens op de gerelateerde koppeling.  
2.  Selecteer de vestiging waarin u een zone wilt instellen, open de vestigingskaart en kies de actie **Zones**.  
3.  Vul de velden in het venster **Zones** naar wens in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

Wanneer u een zoneparameter wijzigt, worden de nieuwe kenmerken toegepast op alle nieuwe opslaglocaties in de zone. De kenmerken van bestaande opslaglocaties blijven echter ongewijzigd.  

> [!NOTE]  
>  Als u zonder zones wilt werken, moet u toch één zonecode maken die alleen voor de code is gedefinieerd.  

De volgende stap bij het instellen van het magazijn bestaat uit het definiëren van opslaglocaties. Zie [Procedure: gebruik van opslaglocaties voor locaties instellen](warehouse-how-to-set-up-locations-to-use-bins.md) voor meer informatie.  

Daarnaast moet u opslagsjablonen en tellingsperioden maken. Zie voor meer informatie [Procedure: Opslagsjablonen instellen](warehouse-how-to-set-up-put-away-templates.md).  

## <a name="see-also"></a>Zie ook  
[Magazijnbeheer](warehouse-manage-warehouse.md)  
[Voorraad](inventory-manage-inventory.md)  
[Magazijnbeheer instellen](warehouse-setup-warehouse.md)     
[Assemblagebeheer](assembly-assemble-items.md)    
[Ontwerpdetails: Magazijnbeheer](design-details-warehouse-management.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  


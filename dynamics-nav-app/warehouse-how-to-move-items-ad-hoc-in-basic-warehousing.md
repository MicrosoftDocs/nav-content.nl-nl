---
title: Artikelen ad hoc verplaatsen in standaardmagazijnconfiguraties
description: Mogelijk moet u soms artikelen verplaatsen tussen interne opslaglocaties, opslaglocaties voor ontvangst of verzending uitgezonderd, zonder een specifieke vraag uit een brondocument. U kunt deze ad hoc verplaatsingen bijvoorbeeld uitvoeren om het magazijn te herstructureren, items naar een inspectiegebied te brengen of extra items naar en van een productiegebied te verplaatsen zonder een relatie in het systeem met het brondocument van de productieorder.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 6178f14d7436e7545eacfbf7462ca1c7cdb3d9ef
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-move-items-ad-hoc-in-basic-warehouse-configurations"></a>Procedure: Artikelen ad hoc verplaatsen in standaardmagazijnconfiguraties
Mogelijk moet u soms artikelen verplaatsen tussen interne opslaglocaties, opslaglocaties voor ontvangst of verzending uitgezonderd, zonder een specifieke vraag uit een brondocument. U kunt deze ad hoc verplaatsingen bijvoorbeeld uitvoeren om het magazijn te herstructureren, artikelen naar een inspectiegebied te brengen of extra artikelen naar en van een productiegebied te verplaatsen zonder een relatie in het systeem met het brondocument van de productieorder.  

Bij standaard magazijnconfiguraties, dat wil zeggen locaties die gebruik maken van de instelling **Opslaglocatie verplicht** en eventueel de instellingen **Pick vereist** en **Opslag vereist**, kunt u zonder brondocumenten ad hoc verplaatsingen registreren op de volgende manieren:  

    - Met het venster **Interne verplaatsing**.  
    - Open het venster **Artikel-herindelingsdagboek**.  

> [!NOTE]  
>  Bij geavanceerde magazijnconfiguraties, dat wil zeggen locaties die gebruik maken van de instelling **Gestuurde opslag en Pick**, gebruikt u het venster **Werkblad Verplaatsing** of het venster **Interne mag. Pick** of **Interne mag. Opslag** voor het ad hoc verplaatsen van artikelen tussen opslaglocaties.  

## <a name="to-move-items-as-an-internal-movement"></a>Items verplaatsen als een interne verplaatsing  
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Interne verplaatsing** in en klik vervolgens op de gerelateerde koppeling.  
2.  Vul het veld **Nr.** op het sneltabblad **Algemeen** in . in door het veld te verlaten of door **AssistEdit** te kiezen om een selectie uit de nummerreeks te maken.  
3.  Voer in het veld **Locatiecode** de locatie in waar de verplaatsing plaatsvindt.  

    Indien de vestiging als magazijnmedewerker als standaardlocatie is ingesteld, wordt de vestigingscode automatisch ingevoegd.  
4.  Voer in het veld **Code naar opslaglocatie** een code in voor de opslaglocatie waarnaar u het item wilt verplaatsen. Voor productiedoeleinden zou dit bijvoorbeeld de code voor de grijpvoorraadlocatie kunnen zijn, zoals gedefinieerd op de vestigingskaart of afdeling.  
5.  Voer in het veld **Vervaldatum** de datum in waarop de verplaatsing moet worden voltooid.  
6.  Kies op het sneltabblad **Regels** het veld **Artikelnr.** om het venster **Opslaglocatie-inhoudsoverzicht** te openen en selecteer het artikel dat moet worden verplaatst, op basis van de beschikbaarheid in opslaglocaties. U kunt ook de actie **Opslaglocatie-inhoud ophalen** kiezen om de interne verplaatsingsregels te vullen op basis van uw filters. Zie de knopinfo voor de actie **Opslaglocatie-inhoud ophalen** voor meer informatie.   

    Wanneer u het item hebt geselecteerd, wordt het veld **Code Van opslaglocatie** automatisch gevuld op basis van de geselecteerde opslaglocatie-inhoud, maar u kunt dit wijzigen in een andere opslaglocatie waar het artikel beschikbaar is.  

    > [!NOTE]  
    >  Aangezien het veld **Artikelnr.** en **Code Van opslaglocatie** verbonden zijn, kunnen hun waarden wijzigen wanneer u een veld bewerkt.  

    Het veld **Code Naar opslaglocatie** wordt gevuld met de waarde die u in de kop hebt ingevoerd, maar u kunt deze op de regel wijzigen in een andere opslaglocatiecode die niet is geblokkeerd of gereserveerd voor speciale doeleinden. Zie voor meer informatie over het toewijzen van speciale opslaglocaties Speciaal.  
7.  Als u bepaald hebt van en naar welke opslaglocatie u het artikel wilt verplaatsen, voert u het te verplaatsen aantal in het veld **Aantal** in.  

    > [!NOTE]  
    >  De hoeveelheid moet beschikbaar zijn in Naar opslaglocatie.  

8.  Als u klaar bent om de interne verplaatsing te verwerken, kiest u de actie **Voorraadverplaatsing maken**.  

    > [!NOTE]  
    >  Wanneer u de voorraadverplaatsing hebt gemaakt, worden de regels van de interne verplaatsing verwijderd.  

    U voert de rest van de ad hoc verplaatsing in het venster **Voorraadverplaatsing** op dezelfde manier uit als bij een verplaatsing op basis van brondocumenten. Zie voor meer informatie bijvoorbeeld [Procedure: onderdelen verplaatsen naar een bewerkingsgebied in standaardmagazijnconfiguraties](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md)  

## <a name="to-move-items-with-the-item-reclassification-journal"></a>Artikelen verplaatsen met het artikelherindelingsdagboek
In plaats van magazijnverplaatsingdocumenten te gebruiken, kunt u de verplaatsing van artikelen ook registreren door hun opslaglocatiecodes opnieuw in te delen. Zie voor meer informatie [Procedure: Voorraad tellen, corrigeren en herindelen](inventory-how-count-adjust-reclassify.md).   
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Art.-herindelingsdagboek** in en klik vervolgens op de gerelateerde koppeling.  
2.  Definieer op elke dagboekregel de opslaglocaties waaruit en waarnaar u items wilt verplaatsen door de velden **Code Opslaglocatie** en **Code Nieuwe opslaglocatie** in te vullen.  

    1.  Als u de gehele inhoud van een opslaglocatie wilt verplaatsen naar een andere opslaglocatie, kiest u de actie **Opslaglocatie-inhoud ophalen**.  
    2.  Vul de filters in voor het zoeken naar de opslaglocatie waarvan u de inhoud wilt verplaatsen en klik op **OK**. De dagboekregels worden gevuld met de inhoud van de opslaglocatie.  
3.  Vul de overige velden op elke dagboekregel in.   
4.  Boek het herindelingsdagboek.  

    > [!NOTE]  
    >  In tegenstelling tot verplaatsingsdocumenten maakt een verplaatsing die is geboekt met het herindelingsdagboek geen magazijnaanvraag om een fysieke taak uit te voeren.  

## <a name="see-also"></a>Zie ook  
[Magazijnbeheer](warehouse-manage-warehouse.md)  
[Voorraad](inventory-manage-inventory.md)  
[Magazijnbeheer instellen](warehouse-setup-warehouse.md)     
[Assemblagebeheer](assembly-assemble-items.md)    
[Ontwerpdetails: Magazijnbeheer](design-details-warehouse-management.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


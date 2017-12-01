---
title: Picken voor interne bewerkingen in geavanceerde magazijnconfiguraties
description: In geavanceerde magazijnconfiguraties waarbij de locatie is ingesteld voor het gebruik van picken en verzending, kunt u componenten voor productie- en assemblageactiviteiten kiezen via het venster **Magazijnpick**.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 08b79f573a9fc013068f7e1f5dd593a596a579a3
ms.contentlocale: nl-nl
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-pick-for-assembly-or-production-in-advanced-warehouse-configurations"></a>Procedure: Picken voor assemblage of productie in geavanceerde magazijnconfiguraties
In geavanceerde magazijnconfiguraties waarbij de locatie is ingesteld voor het gebruik van picken en verzending, kunt u componenten voor productie- en assemblageactiviteiten kiezen via het venster **Magazijnpick**.  

U kunt tevens het venster **Verplaatsingsvoorstel** gebruiken voor ad hoc verplaatsing van artikelen tussen opslaglocaties, dat wil zeggen, zonder verwijzing naar een brondocument. Zie [Procedure: Artikelen verplaatsen in geavanceerde magazijnconfiguraties](warehouse-how-to-move-items-in-advanced-warehousing.md) voor meer informatie.  

Zie [Procedure: Onderdelen verplaatsen naar een bewerkingsgebied in standaardmagazijnconfiguraties](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md) voor informatie over het picken van artikelen voor interne bewerkingen in standaardmagazijnvestigingen die alleen zijn ingesteld voor picken.  

Een magazijn-pickdocument kan niet van het begin af gemaakt worden, omdat een pick-activiteit altijd onderdeel is van een werkstroom, zowel bij een pull- als bij een push-scenario.  

Bij een push-scenario kan een magazijn-pickdocument gemaakt worden door **Mag. Pick maken** in het brondocument te selecteren, zoals een vrijgegeven assemblageorder of een verzending uit het magazijn. Zie voor meer informatie [Procedure: artikelen picken met een magazijnpick](warehouse-how-to-pick-items-for-warehouse-shipment.md).  

Tevens kunt u bij een pull-scenario een magazijnpickdocument maken door het venster **Pickvoorstel** te gebruiken om pickverzoeken, voor zowel verzending als voor interne doeleinden, vast te stellen en vervolgens de benodigde magazijnpickdocumenten te maken.  

De volgende procedure beschrijft een pull-scenario, waarbij u onderdelen voor een vrijgegeven productieorder pickt met behulp van het venster **Werkblad Pick**. De procedure geldt ook voor een assemblageorder.  

Als u een pick-verzoek wilt maken, bij zowel een pull- als een push-scenario, moeten de betreffende brondocumenten vrijgegeven worden. Voor interne doeleinden kunnen brondocumenten op de volgende manieren vrijgegeven worden.  

|Brondocument|Vrijgavemethode|  
|---------------------|--------------------|  
|Productieorder|Wijzig de ordersoort in vrijgegeven productieorder.|  
|Assemblageorder|Wijzig de status in Vrijgegeven.|  

## <a name="to-pick-components-using-the-pick-worksheet"></a>Onderdelen picken op basis van het pickvoorstel  
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Pickvoorstel** in en klik vervolgens op de gerelateerde koppeling.  
2.  Kies de actie **Magazijndocumenten ophalen** en selecteer vervolgens de onderdeelregels van de vrijgegeven productieorder.  
3.  Inspecteer en sorteer de regels om een efficiënte pickronde samen te stellen en combineer ze eventueel met andere voorstelregels zodat de werknemer zo min mogelijk tijd nodig heeft.  
4.  Kies de actie **Pick maken**.  
5.  Bepaal hoe de magazijn-pickdocumenten gemaakt moeten worden en hoe de pickregels gesorteerd moeten worden door de velden in het venster **Pick maken** in te vullen.  
6.  Kies de knop **Ok**. Magazijn-pickdocumenten worden gemaakt met een pickregel voor ieder onderdeel dat voor de interne activiteit benodigd is.  

Indien het gebied voor interne activiteit, zoals een productie-shopfloor, een standaardopslaglocatie heeft voor het plaatsen van onderdelen die voor de activiteit benodigd zijn, wordt de code van deze opslaglocatie ingevoerd in de Plaatsen-regels in het magazijnpickdocument, zodat de magazijnmedewerkers weten waar de artikelen geplaatst moeten worden. Zie voor meer informatie het veld **Code verbruikslocatie** of **Opslaglocatie Naar-assemblage**.

## <a name="filling-the-consumption-bin"></a>De verbruiksopslaglocatie vullen
In dit stroomdiagram wordt weergegeven hoe het veld **Opslaglocatie** op de productieordercomponentregels wordt ingevuld op basis van uw locatie-instellingen.

![Diagram van opslaglocatiestroom](media/binflow.png "Opslaglocatiestroom")  

## <a name="see-also"></a>Zie ook
[Magazijnbeheer](warehouse-manage-warehouse.md)  
[Voorraad](inventory-manage-inventory.md)  
[Magazijnbeheer instellen](warehouse-setup-warehouse.md)     
[Assemblagebeheer](assembly-assemble-items.md)    
[Ontwerpdetails: Magazijnbeheer](design-details-warehouse-management.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


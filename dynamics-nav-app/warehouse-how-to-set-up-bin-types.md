---
title: Opslaglocatiesoorten instellen
description: U kunt de stroom van artikelen beheren via opslaglocaties die door u zijn gedefinieerd voor speciale magazijnactiviteiten. Met het toewijzen van een soort aan een opslaglocatie stelt u een aantal basisactiviteiten voor de locatie in, en daarmee ook de manier waarop de opslaglocatie in wordt gebruikt.
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
ms.openlocfilehash: 406f9e1a325c791fb19558e13db5ace93fdc8e31
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-bin-types"></a>Procedure: Opslaglocatiesoorten instellen
U kunt de stroom van artikelen beheren via opslaglocaties die door u zijn gedefinieerd voor speciale magazijnactiviteiten. Met het toewijzen van een soort aan een opslaglocatie stelt u een aantal basisactiviteiten voor de locatie in, en daarmee ook de manier waarop de opslaglocatie in wordt gebruikt.  

Er zijn acht soorten opslaglocaties. U kunt binnen uw magazijn met alle acht mogelijke opslaglocatiesoorten werken of kunt u werken met alleen de opslaglocatiesoorten ONTVANGEN, OPSLAGPICK, VERZENDEN en QC. Bij deze vier soorten opslaglocaties kunnen suggesties worden aangebracht die de stroom van artikelen ondersteunen en het vastleggen van voorraadafwijkingen mogelijk maken.  

## <a name="to-set-up-the-bin-types-you-want-to-use"></a>U kunt als volgt de gewenste soorten opslaglocatie instellen  
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Opslaglocatiesoorten** in en klik vervolgens op de gerelateerde koppeling.  
2.  In het venster **Opslaglocatiesoorten** geeft u een code op voor het soort opslaglocatie (10 cijfers en/of letters).  
3.  Selecteer de activiteiten die bij elke opslaglocatiesoort kunnen worden uitgevoerd.  

> [!NOTE]  
>  Opslaglocatiesoorten zijn alleen van toepassing als u in de vestiging gestuurde opslag en pick gebruikt.  

Het soort opslaglocatie geeft enkel aan hoe een bepaalde opslaglocatie gebruikt wordt bij de verwerking van de artikelenstroom in het magazijn. U kunt de suggesties voor elk magazijndocument vervangen en u kunt items naar of uit iedere opslaglocatie verplaatsen door een magazijnverplaatsing uit te voeren.  

Hieronder vindt u een overzicht van de soorten opslaglocaties die u kunt maken.  

|Opslaglocatiesoort|Description|  
|------------------|---------------------------------------|  
|ONTVANGST|Artikelen die zijn geregistreerd als geboekte ontvangsten, maar die nog niet zijn opgeslagen.|  
|VERZENDING|Artikelen die zijn gepickt voor magazijnverzendregels, maar die nog niet zijn geboekt als verzonden.|  
|OPSLAG|Meestal items die in grote eenheden worden opgeslagen, maar die u niet wilt picken. Aangezien deze opslaglocaties niet worden gebruikt voor het picken, hetzij voor productieorders of verzendingen, is het gebruik van een opslaglocatie voor opslag mogelijk beperkt, maar deze opslaglocatiesoort kan nuttig zijn indien u een grote hoeveelheid items hebt aangeschaft. Dit soort opslaglocaties moeten altijd een lage rangschikking van opslaglocaties hebben, zodat wanneer ontvangen artikelen opgeslagen zijn, andere opslaglocaties van het type OPSLAGPICK- met een hogere rangschikking- die bij het item horen eerder opgeslagen worden. Indien u dit type opslaglocatie gebruikt, moet u regelmatig een opslaglocatieaanvulling uitvoeren, zodat de items in deze opslaglocaties ook beschikbaar zijn in de opslaglocaties van het type OPSLAGPICK of PICK.|  
|PICK|Artikelen die alleen worden gebruikt voor pickactiviteiten, bijvoorbeeld artikelen met een naderende vervaldatum die u naar dit soort opslaglocatie hebt verplaatst. Deze opslaglocaties behoren een hoge rangschikking te krijgen, zodat altijd eerst wordt voorgesteld om artikelen uit deze locaties te halen.|  
|OPSL-PICK|Artikelen in opslaglocaties die worden voorgesteld voor de opslag- en pickfuncties. Opslaglocaties van dit soort beschikken waarschijnlijk over verschillende zonevolgordes. U kunt locaties voor bulkopslag bijvoorbeeld instellen als een laaggeclassificeerde versie van dit soort, in tegenstelling tot de normale pickopslaglocaties of een pickopslaggebied.|  
|QC|Deze opslaglocatie wordt gebruikt voor voorraadaanpassing indien u deze opslaglocatie opgeeft in het veld **Code aanpassing opslaglocatie** op de locatiekaart. U kunt dit soort locaties ook instellen voor defecte artikelen en artikelen die worden geïnspecteerd. Als u bepaalde artikelen ontoegankelijk wilt maken voor de normale artikelenstroom, kunt u de artikelen eveneens verplaatsen naar dit soort opslaglocatie.<br /><br /> **OPMERKING:** in tegenstelling tot alle andere soorten opslaglocaties is bij de opslaglocatie van het type **QC** geen enkel selectievakje voor de verwerking van artikelen standaard ingeschakeld. Dit geeft aan dat alle inhoud die u in een opslaglocatie van QC plaatst uitgesloten is van de stroom van artikelen.|  

## <a name="see-also"></a>Zie ook
[Magazijnbeheer](warehouse-manage-warehouse.md)  
[Voorraad](inventory-manage-inventory.md)  
[Magazijnbeheer instellen](warehouse-setup-warehouse.md)     
[Assemblagebeheer](assembly-assemble-items.md)    
[Ontwerpdetails: Magazijnbeheer](design-details-warehouse-management.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


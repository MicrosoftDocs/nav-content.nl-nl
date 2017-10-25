---
title: Resourcekosten, prijzen en capaciteit instellen
description: Als u resources wilt gebruiken en projectbeheer wilt mogelijk maken, geeft u kosten en prijzen voor afzonderlijke resources of resourcegroepen op en stelt u de resourcecapaciteit in.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, capacity, staff
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: e1c2f8f41bb493c4ce2efa2156631c6d9d273439
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-resources"></a>Procedure: Resources instellen
Om resourceactiviteiten correct te beheren, moet u resources en de bijbehorende kosten en prijzen instellen. De aan projecten gerelateerde prijzen, kortingen en kostenfactorregels worden ingesteld op de projectkaart. U kunt de kosten en prijzen opgeven voor afzonderlijke resources, resourcegroepen of alle beschikbare resources van het bedrijf.

Wanneer resources worden gebruikt of verkocht voor een project, worden de bijbehorende prijzen en kosten opgehaald uit de informatie die u instelt.

Bij het maken van de resource geeft u het standaardbedrag per uur op. Als u bijvoorbeeld 5 uur lang een specifieke machine gebruikt voor een project, worden de kosten van het project gebaseerd op de kosten per uur.

## <a name="to-set-up-a-resource"></a>Een resource instellen
Maak een kaart per resource die u wilt gebruiken in projecten.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Resources** in en klik vervolgens op de gerelateerde koppeling.
2. Kies de actie **Nieuw**.
3. Vul indien nodig de velden in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-set-up-a-resource-group"></a>Een gebruikersgroep instellen
U kunt meerdere resources in één resourcegroep combineren. De capaciteit en budgetten van individuele resources worden bij elkaar opgeteld en vormen de capaciteit en het budget voor de resourcegroep. Het is ook mogelijk om capaciteit op te geven voor de resourcegroepen die los staat van de opgetelde waarden, of een aanvulling hierop vormt.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Resourcegroepen** in en klik vervolgens op de gerelateerde koppeling.
2. Kies de actie **Nieuw**.
3. Vul indien nodig de velden in.

## <a name="to-set-capacity-for-a-resource"></a>Capaciteit voor een resource instellen
Om te berekenen hoeveel tijd een resource aan projecten kan besteden moet de capaciteit ervan eerst worden ingesteld als beschikbare tijd per periode op de werkagenda. Deze instelling wordt gebruikt als u projectplanningsregels invult die de resource bevatten. Zie [Procedure: Projecten maken](projects-how-create-jobs.md) voor meer informatie.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Resources** in en klik vervolgens op de gerelateerde koppeling.
2. Open de desbetreffende resourcekaart en kies vervolgens de actie **Resourcecapaciteit**.
3. Geef in het venster **Resourcecapaciteit** in het veld **Weergeven per** de lengte van de periode op, zoals **Dag**, die wordt weergegeven in kolommen op het sneltabblad **Resourcecapaciteitsmatrix**.
4. Geef voor elke resource op een regel voor elke periode in de kolommen het aantal uren op dat de resource beschikbaar is.
5. Of, als u de wekelijke capaciteit van de resource wilt detailleren met een begin- en een einddatum, kiest u de actie **Capaciteit instellen**.
6. Vul in het venster **Resourcecapaciteitsinstellingen** indien nodig de velden in.
7. Kies de actie **Capaciteit bijwerken**. Het venster **Resourcecapaciteit** wordt bijgewerkt met de ingevoerde capaciteit.
8. Sluit het venster.

## <a name="to-set-up-alternate-resource-costs"></a>Alternatieve resourcekosten instellen
Naast de kosten die op de resourcekaart worden opgegeven, kunt u alternatieve kosten voor elke resource instellen. Als een werknemer bijvoorbeeld een hoger uurtarief heeft voor overwerk, kunt u een resourcekostprijs voor het overwerktarief instellen. De alternatieve kostprijs die u voor de resource instelt, vervangt de kostprijs op de resourcekaart wanneer u de resource in het resourcedagboek gebruikt.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Resources** in en klik vervolgens op de gerelateerde koppeling.  
2. Selecteer de resource waarvoor u een of meerdere alternatieve kosten wilt instellen en kies vervolgens de actie **Kosten**.  
3. Vul in het venster **Resourcekostprijzen** indien nodig de velden op een regel in.  
4. Herhaal stap 3 voor elke alternatieve resourcekostprijs die u wilt instellen.

**Opmerking**. Als u resourcekostprijzen wilt instellen die gelden voor alle resources en resourcegroepen, opent u het venster **Resourcekostprijzen** en vult u de velden in.

## <a name="to-set-up-alternate-resource-prices"></a>Alternatieve resourceprijzen instellen
Naast de prijs die op de resourcekaart wordt opgegeven, kunt u alternatieve prijzen voor elke resource instellen. Deze alternatieve prijzen kunnen voorwaardelijk zijn. Ze kunnen afhankelijk zijn van of de resource met een bepaald project of werksoort wordt gebruikt.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Resources** in en klik vervolgens op de gerelateerde koppeling.
2. Selecteer de resource waarvoor u een of meerdere alternatieve prijzen wilt instellen, en kies vervolgens de actie **Prijzen**.
3. Vul in het venster **Resourceprijzen** indien nodig de velden op een regel in.
4. Herhaal stap 3 voor elke alternatieve resourceprijs die u wilt instellen.

## <a name="see-also"></a>Zie ook
[Projectbeheer instellen](projects-setup-projects.md)  
[Projectbeheer](projects-manage-projects.md)  
[Financiën](finance.md)  
[Inkoop](purchasing-manage-purchasing.md)         
[Verkoop](sales-manage-sales.md)      
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  


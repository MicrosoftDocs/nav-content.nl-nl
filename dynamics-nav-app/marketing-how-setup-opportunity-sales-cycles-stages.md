---
title: Verkoopcycli instellen voor opportunities en cyclusfasen
description: Beschrijft hoe u verkoopstadia definieert, van eerste contact tot sluiten, om een verkoopcyclus te maken en toe te wijzen aan opportunities in Dynamics NAV.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 06/06/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 547e24b87fcd643406f1aa9cbde9bf85c44cae71
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-opportunity-sales-cycles-and-cycle-stages"></a>Procedure: Verkoopcycli instellen voor opportunities en cyclusfasen
Voordat u verkoopopportunities in gebruik kunt nemen, moet u verkoopcycli en verkoopcyclusfasen instellen. Een verkoopcyclus bestaat uit een reeks fasen vanaf het eerste contact tot aan het sluiten van een verkoop. Elke fase kan bepaalde vereisten hebben waaraan moet worden voldaan, zoals een verkoopofferte, voordat een opportunity naar de volgende fase kan gaan. U kunt ook aangeven of een fase kan worden overgeslagen. U kunt elk gewenst aantal verkoopcycli instellen en u kunt binnen een verkoopcyclus elk gewenst aantal verkoopcyclusfasen instellen.

Het implementeren van opportunityverkoopcycli betreft het instellen van de verkoopcycluscode, het definiëren van de verschillende fasen van de cyclus en het toewijzen van de cyclus aan opportunities. Het toekennen van de relevante activiteit of taken aan de opportunity kan ook deel uitmaken van het instellen van een verkoopcyclus.

In dit onderwerp wordt ook beschreven hoe u taken en activiteiten instelt en hoe u taken toewijst aan activiteiten. Zie voor meer informatie de sectie 'Activiteiten instellen met taken'.

## <a name="to-set-up-opportunity-sales-cycle-codes"></a>Opportunityverkoopcycluscodes instellen
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Verkoopcycli** in en klik vervolgens op de gerelateerde koppeling. Het venster **Verkoopcycli** wordt geopend en be vat alle bestaande verkoopcycli.
2. Kies de actie **Nieuw** en vul indien nodig de velden in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

Herhaal deze stappen om het gewenste aantal verkoopcycli in te stellen. Nadat u de opportunityverkoopcycli hebt ingesteld, kunt u de verschillende fases instellen binnen elke cyclus.

## <a name="to-define-opportunity-sales-cycle-stages"></a>Fasen van opportunityverkoopcycli definiëren
1. Selecteer in het venster **Verkoopcycli** de opportunityverkoopcyclus waarvoor u fases wilt instellen en kies vervolgens de actie **Fasen**. Het venster **Verkoopcyclusfasen** verschijnt.
2. Kies de actie **Nieuw** om een nieuwe fase in de verkoopcyclus in te voeren.

Herhaal deze stappen om het gewenste aantal fasen binnen de verkoopcyclus in te stellen.

## <a name="to-assign-stage-cycles-to-opportunities"></a>Verkoopfasecycli aan opportunities toewijzen
Nadat u de opportunityfasecyclus toevoegt, kunt u beginnen om verkoopopportunities toe te voegen en vervolgens de fasecyclus aan opportunities toewijzen door het veld **Verkoopcycluscode** in te stellen. Zie voor meer informatie [Procedure: Verkoopopportunities maken](marketing-how-create-opportunities.md).

## <a name="to-set-up-activities-with-tasks"></a>Activiteiten instellen met taken
U kunt meerdere taken combineren, bijvoorbeeld taken die elk een stap in activiteiten vertegenwoordigen. Activiteittaken worden gerelateerd aan elkaar met een datumformule. U kunt activiteiten aan opportunities, verkopers of contacten toewijzen.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Activiteiten** in en klik vervolgens op de gerelateerde koppeling.
2. Kies de actie **Nieuw** en vul indien nodig de velden in.
3. Vul op het sneltabblad **Regels** de velden indien nodig in om een of meer taken in de activiteit te definiëren.

## <a name="to-assign-tasks-or-activities-of-tasks-to-opportunities"></a>Taken of activiteiten van taken toewijzen aan opportunities
Wanneer u een taak hebt ingesteld, kunt u deze toewijzen aan een verkoopopportunity en daarmee de activiteit toewijzen waartoe de taak behoort.

> [!NOTE]  
>   In deze procedure wordt beschreven hoe u activiteittaken toekent aan opportunities. de stappen zijn soortgelijk wanneer u taken toewijst aan contacten en verkopers.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Opportunity's** in en klik vervolgens op de gerelateerde koppeling.
2. Selecteer een opportunity en kies vervolgens de actie **Taken**.
3. Kies in het venster **Taakoverzicht** de actie **Taak maken**.
4.  Vul in het venster **Taak maken** de benodigde velden in.

    U ziet in het veld **Opportunity** dat het automatisch is toegewezen aan de betreffende opportunity.
5. Kies de knop **OK**.
6. Selecteer in het venster **Taakoverzicht** de nieuwe taak en kies vervolgens de actie **Activiteiten toewijzen**.
7. Vul in het venster **Activiteit toewijzen** desgewenst de velden in en kies vervolgens de knop **OK**.

## <a name="see-also"></a>Zie ook
[Verkoopopportunities verwerken](marketing-processing-sales-opportunities.md)  
[Verkoop](sales-manage-sales.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


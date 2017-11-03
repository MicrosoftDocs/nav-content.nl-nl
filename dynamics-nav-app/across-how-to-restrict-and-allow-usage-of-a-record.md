---
title: 'Procedure: Het gebruik van een record verhinderen en toestaan'
description: Als u wilt voorkomen dat een record wordt gebruikt bij bepaalde activiteiten, bijvoorbeeld totdat de record is goedgekeurd, kunt u twee werkstroomantwoorden opnemen in een werkstroom die het gebruik van de record bestuurt.
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
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 639d6575de6b9ea29c160ecb5cb55cff5574c77d
ms.contentlocale: nl-nl
ms.lasthandoff: 10/26/2017

---
# <a name="how-to-restrict-and-allow-usage-of-a-record"></a>Procedure: Het gebruik van een record verhinderen en toestaan
Als u wilt voorkomen dat een record wordt gebruikt bij bepaalde activiteiten, bijvoorbeeld totdat de record is goedgekeurd, kunt u twee werkstroomantwoorden opnemen in een werkstroom die het gebruik van de record bestuurt. Eén werkstroomantwoord beperkt het gebruik van de record zoals gedefinieerd door de werkstroomgebeurtenis en -voorwaarden. Een andere werkstroomantwoord staat het gebruik van de record toe zoals gedefinieerd door de werkstroomgebeurtenis en -voorwaarden. Er bestaan twee responsen in de generieke versie van [!INCLUDE[d365fin](includes/d365fin_md.md)] voor dit doel: **Gebruik van een record beperken** en **Gebruik van een record toestaan**.

> [!NOTE]  
>  De algemene versie van [!INCLUDE[d365fin](includes/d365fin_md.md)] helpt verhinderen dat een record wordt geboekt, als betaling wordt geëxporteerd en als cheque wordt afgedrukt. Als een Microsoft-partner andere beperkingen wil ondersteunen, moet deze de toepassingscode aanpassen.  

> [!NOTE]  
>  De werkstroomfunctionaliteit om te verhinderen en toe te staan dat records worden gebruikt houdt geen verband met de functionaliteit om het boeken van artikel-, klant- en leveranciersrecords te blokkeren.

In de volgende procedure wordt beschreven hoe u het boeken van inkooporders kunt verhinderen totdat deze zijn goedgekeurd. De nieuwe werkstroom wordt gebaseerd op de bestaande werkstroomsjabloon Goedkeuringswerkstroom inkoopfactuur.  

## <a name="to-create-a-workflow-step-that-restricts-posting-of-unapproved-purchase-orders"></a>Een werkstroomstap maken die voorkomt dat niet-goedgekeurde inkooporders worden geboekt  
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Werkstromen** in en klik op de gerelateerde koppeling.  
2. Maak in het venster **Werkstromen** een nieuwe werkstroom genaamd Goedkeuringswerkstroom inkooporder. Zie voor meer informatie [Procedure: Werkstromen maken](across-how-to-create-workflows.md).  
3. Kies de actie **Kopiëren van werkstroomsjabloon**.  
4. Kies het veld **Bronwerkstroomcode** en kies vervolgens in het venster **Werkstroomsjablonen** de werkstroomsjabloon Goedkeuringswerkstroom inkooporder.  

     Zoals u ziet, draait het bij de eerste twee werkstroomstappen om het verhinderen en vervolgens het toestaan van het gebruik van inkoopfacturen. Ga door met het wijzigen van de gebeurtenisvoorwaarde in de eerste stap van de werkstroom om op te geven dat deze van toepassing is op inkooporders.  
5. Kies op het sneltabblad **Werkstroomstappen** het veld **Gebeurtenisvoorwaarden** en selecteer vervolgens voor het filter **Documentsoort** de optie **Order**.  
6. Ga door om andere werkstroomstappen te bewerken, te verwijderen of toe te voegen in een bedrijfsproces dat begint door het boeken van niet-goedgekeurde inkooporders te verhinderen.  

## <a name="see-also"></a>Zie ook  
[Procedure: Werkstromen maken](across-how-to-create-workflows.md)   
[Werkstroom](across-workflow.md)   


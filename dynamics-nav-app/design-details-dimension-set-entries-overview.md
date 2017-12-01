---
title: Overzicht dimensiesetposten
description: In dit onderwerp wordt beschreven hoe dimensiesetposten worden opgeslagen en geboekt in [!INCLUDE[d365fin](includes/d365fin_md.md)].
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: dimension
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: ce9459785ee39fa89baf61b2e97be41ddde661f6
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="dimension-set-entries-overview"></a>Overzicht dimensiesetposten
In dit onderwerp wordt beschreven hoe dimensiesetposten worden opgeslagen en geboekt in [!INCLUDE[d365fin](includes/d365fin_md.md)].  
  
## <a name="dimension-sets"></a>Dimensiesets  
Een dimensieset is een unieke combinatie dimensiewaarden. Een dimensieset wordt als dimensiesetposten in de database opgeslagen. Elke dimensiesetpost vertegenwoordigt één dimensiewaarde. De dimensiesetpost wordt geïdentificeerd door een gemeenschappelijke dimensieset-id die is toegewezen aan elke dimensiesetpost die tot de dimensieset behoort.  
  
In het volgende voorbeeld ziet u een dimensieset met drie dimensiesetposten. De dimensieset wordt geïdentificeerd door een dimensieset-id 108.  
  
|Dimensieset-id|Dimensiecode|Dimensiewaardecode|Dimensiewaardenaam|  
|----------------------|--------------------|--------------------------|--------------------------|  
|108|DISTRICT|70|Noord-Amerika|  
|108|BEDRIJFSGROEP|HOME|Home|  
|108|KSTNPLAATS|VERKOOP|Verkoop|  
  
## <a name="dimension-set-entries"></a>Dimensiesetposten  
Dimensiesets worden opgeslagen in de tabel **Dimensiesetpost** als dimensiesetposten met dezelfde dimensieset-id.  
  
![Overzicht van dimensiepost](media/dimensionentrynav7.png "DimensionEntryNAV7")  
  
Wanneer u een nieuwe dagboekregel, documentkop of documentregel maakt, kunt u een combinatie van dimensiewaarden opgeven. In plaats van elke dimensiewaarde expliciet in de database op te slaan, wordt een dimensieset-id toegewezen aan de dagboekregel, documentkop of documentregel om zo de dimensieset op te geven.  
  
Wanneer u het venster **Dimensiesetposten bewerken** bewerkt en sluit, wordt gecontroleerd of de combinatie van dimensiewaarden als een dimensieset in de tabel voorkomt. Als de combinatie in de tabel voorkomt, wordt de overeenkomende dimensieset-id toegewezen aan de dagboekregel, documentkop of documentregel. Anders wordt een nieuwe dimensieset toegevoegd aan de tabel en wordt de nieuwe dimensieset-id toegewezen aan de dagboekregel, documentkop of documentregel.  
  
## <a name="performance-improvement"></a>Prestatieverbetering  
Door dimensiesets eenmalig in de database op te slaan, wordt databaseruimte bespaard en wordt de algehele prestatie verbeterd.  
  
## <a name="see-also"></a>Zie ook  
[Ontwerpdetails: Dimensiecombinaties zoeken](design-details-searching-for-dimension-combinations.md)   
[Ontwerpdetails: Tabelstructuur](design-details-table-structure.md)   
[Ontwerpdetails: Codeunit 408 Dimensiebeheer](design-details-codeunit-408-dimension-management.md)   
[Ontwerpdetails: Codevoorbeelden van gewijzigde patronen in wijzigingen](design-details-code-examples-of-changed-patterns-in-modifications.md)   
[Ontwerpdetails: Dimensiesetposten](design-details-dimension-set-entries.md)   


---
title: Probleemrapportage instellen in servicebeheer
description: Leer hoe u processen voor probleemrapportage instelt.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/22/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: fac280fc2dac2206b1e037656c522bcfef9bc9c7
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---

# <a name="how-to-set-up-fault-reporting"></a>Procedure: Probleemrapportage instellen
Met probleemrapportage kunt u standaarden voor het vastleggen van probleemgegevens voor service-items bepalen. U kunt bijvoorbeeld opgeven wat het probleem is, welke symptomen u ziet, wat de oorzaak van het probleem is en hoe het probleem moet worden verholpen.  

Met probleemcodes worden de veelvoorkomende serviceartikelproblemen of ondernomen acties met betrekking tot serviceartikelen beschreven. Afhankelijk van het niveau van probleemrapportage in het bedrijf, moet u wellicht probleemgebiedcodes en symptoomcodes instellen voordat u probleemcodes instelt. Met probleemgebieden worden gebieden van serviceartikelproblemen beschreven. Met probleemoorzaakcodes kan de oorzaak voor serviceartikelproblemen worden omschreven en kan zo nodig worden aangegeven of garantie- en contractkortingen moeten worden uitgesloten. U kunt bijvoorbeeld garantie- en contractkortingen uitsluiten wanneer de klant op enige manier verantwoordelijk is voor het serviceartikelprobleem. U wijst probleemoorzaakcodes toe aan serviceorders. Zie voor meer informatie [Procedure: Werken aan servicetaken](service-how-to-work-on-service-tasks.md).  

## <a name="to-specify-the-overall-level-of-fault-reporting-to-use"></a>Het algemene probleemrapportageniveau voor gebruik opgeven
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Service-instellingen** in en klik vervolgens op de gerelateerde koppeling. 
2. Kies in het veld **Probleemrapportageniveau** een van de opties die in de volgende tabel worden beschreven.  
  
    |**Probleemniveau**|**Beschrijving**|  
    |------------|-------------|  
    |Geen | Er worden geen rapportagecodes gebruikt.|  
    |Probleem | De codes worden weergegeven in de tabel **Probleemcodes**. Deze codes duiden op problemen met serviceartikelen of acties die moeten worden ondernomen voor de serviceartikelen. U kunt gerelateerde codes groeperen in groepen van het type **Probleemgebiedcode**.|  
    |Probleem + symptoom. | U geeft een combinatie van codes op in de tabellen **Probleemcodes** en **Symptoomcodes**. Veelvoorkomende symptoomcodes kunnen bijvoorbeeld bestaan uit indicaties die een klant kan gebruiken om een probleem te beschrijven, zoals een geluid of kwaliteit.|  
    |Probleem + symptoom + gebied | U gebruikt probleem-, symptoom- en probleemgebiedcodes als een implementatie van IRIS, het internationale systeem voor reparatiecodes.|  
  
Ten slotte kunt u bij het instellen van probleemrapportage ook opgeven welke reparaties of oplossingen aan een probleem of defect zijn gekoppeld. U stelt dit in op de pagina **Relaties probleem-/oplossingscodes**, waar u combinaties van codes instelt voor de serviceartikelgroep van het serviceartikel van waaruit u het venster hebt geopend. Tevens wordt aangegeven hoe vaak elke combinatie voorkomt.

## <a name="to-create-fault-and-resolution-code-relationships"></a>Relaties tussen probleem- en oplossingscodes maken
<!--this needs to go in a working with topic-->
Als u de veelgebruikte herstelmethoden voor bepaalde artikelproblemen wilt bekijken wanneer u service voor de artikelen uitvoert, moet u gegevens over relaties tussen probleem- en oplossingscodes instellen. Met de batchtaak **Rel. probleem-/oplossingscodes invoegen** kunt u alle combinaties van probleem- en oplossingscodes in geboekte serviceorders zoeken en deze vastleggen op de pagina **Rel. probleem-/oplossingscodes**. 
  
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Rel. probleem-/oplossingscodes invoegen** in en klik vervolgens op de gerelateerde koppeling.  
2. Voer datums in om de periode op te geven die u in de batchverwerking wilt opnemen.  
3. Schakel het selectievakje **Relatie op basis van serviceartikelgroep** in als u de relaties wilt rangschikken op serviceartikelgroep.  
4. Schakel het selectievakje **Handmatig ingevoegde records behouden** in als u de records wilt bewaren die u handmatig in het venster **Rel. probleem-/oplossingscodes** hebt ingevoegd.  

## <a name="see-also"></a>Zie ook
[CRM - Service instellen](service-setup-service.md)  
[CRM - Service](service-service.md)  


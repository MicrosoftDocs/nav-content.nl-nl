---
title: Statussen instellen voor serviceorders en reparaties
description: U moet negen herstelstatusopties instellen waarmee u de voortgang van herstel en onderhoud van serviceartikelen in serviceorders kunt aangeven.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: d7dbc4cfc06d4c74476a04512bd368a0ab26f837
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-statuses-for-service-orders-and-repairs"></a>Procedure: Statussen instellen voor serviceorders en reparaties
U moet herstelstatusopties instellen waarmee u de voortgang van herstel en onderhoud van serviceartikelen in serviceorders kunt aangeven. U moet minimaal negen herstelstatusopties instellen om situaties of ondernomen acties met betrekking tot de service voor serviceartikelen aan te duiden.  

U kunt het prioriteitsniveau voor serviceorderstatusopties instellen. De vier prioriteiten zijn Hoog, Relatief hoog, Relatief laag en Laag.  
  
Wanneer u de herstelstatus van een serviceartikel in een serviceorder wijzigt, wordt de serviceorderstatus bijgewerkt. De herstelstatus van elk serviceartikel is gekoppeld aan de serviceorderstatus. Als de serviceartikelen zijn gekoppeld aan twee of meer opties voor serviceorderstatus, wordt de serviceorderstatus met de hoogste prioriteit geselecteerd.  

## <a name="to-set-up-a-repair-status"></a>Herstelstatus instellen  
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Herstelstatus** in en klik vervolgens op de gerelateerde koppeling. 2. Maak een nieuwe herstelstatus.  
3. Vul de velden **Code** en **Omschrijving** in.  
4. In het veld **Serviceorderstatus** kiest u de orderstatus waaraan u de herstelstatus wilt koppelen. In het veld **Prioriteit** wordt de prioriteit weergegeven van de serviceorderstatus die u hebt gekozen.  
5. Kies een herstelstatus. U kunt er slechts één kiezen.  
6. Kies het veld **Boeken toegestaan** als u serviceorders wilt boeken met serviceartikelen met deze herstelstatus.  
7. Schakel het selectievakje **Status Wachtend toegestaan** in als u de optie voor serviceorderstatus handmatig wilt wijzigen in **In behandeling** op serviceorders met serviceartikelen met deze herstelstatus.  
8. Schakel de selectievakjes **Status In verwerking toegestaan**, **Status Gereedgemeld toegestaan** en **Status Afwachten toegestaan** op dezelfde manier in.
  
## <a name="to-set-up-service-status-priorities"></a>Servicestatusprioriteiten instellen  
1. Kies het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Serviceorderstatus** in en kies vervolgens de gerelateerde koppeling.  
2. Selecteer de serviceorderstatus waarvoor u een prioriteit wilt instellen.  
3. Kies de gewenste prioriteit voor deze serviceorderstatus in het veld **Prioriteit**. Herhaal deze stap voor elke status.  
  
## <a name="see-also"></a>Zie ook  
[Serviceorderstatus en herstelstatus begrijpen]()  
[CRM - Service instellen](service-setup-service.md)  


---
title: 'Procedure: Overschrijvingsbericht afdrukken'
description: U kunt leveranciers helpen bij het uitvoeren van reconciliaties door het overschrijvingsbericht af te drukken voordat u een betalingsdagboek boekt en nadat u een betaling hebt geboekt.
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/26/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 71c84b4a7bad83e6008c0fa34f908e133b014a59
ms.contentlocale: nl-nl
ms.lasthandoff: 10/26/2017

---

#<a name="how-to-print-remittance-advice"></a>Procedure: Overschrijvingsbericht afdrukken
U kunt het overschrijvingsbericht afdrukken voordat u een betalingsdagboek boekt en nadat u een betaling hebt geboekt. Op het bericht worden de nummers van de leverancierfactuur weergegeven waarmee leveranciers reconciliaties kunnen uitvoeren.

##<a name="to-print-remittance-advice"></a>Overschrijvingsbericht afdrukken
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Betalingsdagboeken** in en klik vervolgens op de gerelateerde koppeling.  
2. In het venster **Betalingsdagboek** selecteert u de betaling waarvoor het overschrijvingsbericht wilt afdrukken.  
3. Kies de actie **Overschrijvingsbericht afdrukken**.  
4. Kies de gewenste filters in de batchverwerking **Overschrijvingsbericht - dagboek** op het sneltabblad **Fin. dagboekregel**.  
  
    >[!Note]
    > U kunt filteren met het externe documentnummer van de leverancier om betalingen af te stemmen met facturen.

5. Selecteer op het sneltabblad **Leverancier** de gewenste filters.  
6. Kies **Afdrukken** om het rapport af te drukken of kies **Voorbeeld** om het nu weer te geven.  

## <a name="using-remittance-advice-reports"></a>Rapporten met overschrijvingsberichten gebruiken
De volgende tabel beschrijft de rapporten die u met overschrijvingsberichten kunt gebruiken:

|Rapporteren|Description|
|----|----|
|Rapport Overschrijvingsbericht - dagboek|Dit rapport geeft aan welke documenten in de betaling zijn opgenomen. Voor dagboekregels kunt u de dagboeksjabloon en de dagboekbatch opgeven waaruit de overschrijvingsberichten moeten worden afgedrukt, de eerste datum van de activiteit kiezen om af te drukken en filtereren op een documentnummer. Voor leveranciers kunt u de leveranciernummers opgeven die u wilt opnemen in het rapport. |
|Rapport Overschrijvingsbericht - posten| Dit rapport geeft aan welke documenten in de betaling zijn opgenomen. U kunt de rapportinhoud bepalen met behulp van filters. Stel extra velden in op het tabblad door het veld **Veld** te kiezen. Voor leveranciersposten kunt u opgeven welke leveranciers u in het rapport wilt opnemen, de datum van de eerste activiteit om af te drukken, de valuta en het op te nemen volgnummer. |

> [!Note]
> Het rapport Overschrijvingsbericht - dagboek ondersteunt geen scenario's met verschillende valuta's of betalingstoleranties. Zie [Procedure: Vereffening van posten in verschillende valuta's inschakelen](finance-how-enable-application-ledger-entries-different-currencies.md) voor meer informatie.

> [!Tip]
> Voor meer informatie over het werken met rapporten zie [Controlelijsten weergeven vóór boeken](ui-how-view-test-reports-posting.md), [Werken met rapporten](ui-work-report.md) en [Gegevens zoeken, filteren en sorteren](ui-enter-criteria-filters.md).

##<a name="see-also"></a>Zie ook  
[Welkom bij Dynamics NAV](across-get-started.md)

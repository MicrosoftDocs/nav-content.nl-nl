---
title: Validatie van inkoopbedragen instellen
description: In [!INCLUDE[navnow](../../includes/navnow_md.md)] kunt u de functie **Totaalbedragen documenten controleren** activeren om het totaalbedrag van inkoopdocumenten te valideren voordat een inkoopfactuur en inkoopcreditnota worden geboekt.
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
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 8f5b2ef03cd1e0dee5d15a220926f40e9dec239c
ms.contentlocale: nl-nl
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-set-up-validation-of-purchase-amounts"></a>Procedure: Validatie van inkoopbedragen instellen
In [!INCLUDE[navnow](../../includes/navnow_md.md)] kunt u de functie **Totaalbedragen documenten controleren** activeren om het totaalbedrag van inkoopdocumenten te valideren voordat een inkoopfactuur en inkoopcreditnota worden geboekt. Standaard wordt het totale inkoopdocumentbedrag gevalideerd wanneer u boekt. Het totale bedrag van de ingevoegde inkoopregels moet gelijk zijn aan het bedrag inclusief btw en het btw-bedrag. Als u het inkoopdocumentbedrag automatisch wilt valideren, moet u het documentbedrag inclusief btw en de btw van het documentbedrag in het venster **Inkoopfactuur** of **Inkoopcreditnota** invoeren.  

Als u slechts één inkoopregel of meer verkoopregels met hetzelfde btw-percentage hebt, wordt de juiste documentbedrag-btw automatisch berekend wanneer u de inkoopregels en het documentbedrag inclusief btw invoegt. Als u verschillende inkoopregels met verschillende btw-percentages hebt, moet de waarde van de documentbedrag-btw handmatig worden gewijzigd.  

U kunt ook bepalen wanneer de documenttotaalbedragen en de totaalbedragen van de ingevoegde inkoopregels verschillen. U kunt de optie **Totale op inkoopfactuur/CR-nota weergeven** activeren om het volgende weer te geven in de ingevoegde inkoopregels:  

- Totaalbedrag  
- Totaalbasisbedrag  
- Totaal btw-bedrag  
- Totaalbedrag incl. btw  

De berekende bedragen worden weergegeven in de inkoopfactuur of de inkoopcreditnota. Standaard wordt dit totaalbedrag niet weergegeven.  

U kunt deze optie alleen inschakelen als de inkoopfactuur of de inkoopcreditnota het volgende heeft:  

- Een minimum van één inkoopregel.  
- Het aantalveld opgegeven.  

## <a name="to-set-up-validation-of-total-amounts-for-purchase-documents"></a>Validatie van totaalbedragen voor inkoopdocumenten instellen  

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Inkoopinstellingen** in en klik vervolgens op de gerelateerde koppeling.  
2.  Vul in het sneltabblad **Algemeen** de velden in, zoals in de volgende tabel is beschreven.  

    |Veld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Totale op inkoopfactuur/CR-nota weergeven.**|Selecteren om de totalen opnieuw te berekenen van alle inkoopfacturen en creditnota's. Dit kan een tijdrovend proces zijn, afhankelijk van het aantal documenten dat moet worden herberekend.|  
    |**Totaalbedragen documenten controleren**|Selecteren om de velden **Documentbedrag incl. btw** en **Btw documentbedrag** in de vensters **Inkoopfactuur** en **Inkoopcreditnota** te wijzigen.|  

3.  Kies de knop **OK**.  

## <a name="see-also"></a>Zie ook  
[Nederlandse lokale functionaliteit](netherlands-local-functionality.md)  
[Inkopen instellen](../../sales-how-work-standard-lines.md)


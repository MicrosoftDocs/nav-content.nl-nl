---
title: Ontvangsten combineren
description: "Als u meer dan één inkoopontvangst tegelijk wilt factureren, kunt u de functie Ontvangsten combineren gebruiken."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/14/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 10749dc8d8d692d94c5405fbb0a4a965d482f013
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-combine-receipts-on-a-single-invoice"></a>Procedure: Ontvangsten combineren op één factuur
Als u meer dan één inkoopontvangst tegelijk wilt factureren, kunt u de functie **Ontvangsten combineren** gebruiken.  

Een gecombineerde inkoopontvangst kan pas worden gemaakt wanneer meer inkoopontvangsten van dezelfde leverancier in dezelfde valuta zijn geboekt. U moet dus twee of meer inkooporders hebben ingevuld en deze hebben geboekt als ontvangen, maar niet als gefactureerd.  

Wanneer inkoopontvangsten zijn gecombineerd op een factuur en zijn geboekt, wordt een geboekte inkoopfactuur gemaakt voor de gefactureerde regels. Het veld **Gefactureerd aantal** op de oorspronkelijke inkooporder of het oorspronkelijke inkoopraamcontract wordt bijgewerkt op basis van het gefactureerde aantal. Dit oorspronkelijke inkoopdocument wordt echter niet verwijderd, zelfs als dit volledig is ontvangen en gefactureerd en daarom moet u het inkoopdocument zelf verwijderen.  

## <a name="to-combine-receipts"></a>Ontvangsten combineren  
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Inkoopfacturen** in en klik vervolgens op de gerelateerde koppeling.  
2. Kies de actie **Nieuw**. Zie voor meer informatie [Procedure: Inkopen vastleggen](purchasing-how-record-purchases.md).  
3. Op het sneltabblad **Regels** selecteert u de actie **Ontvangstregels ophalen**.  
4. Selecteer meerdere ontvangstregels die u wilt opnemen in de factuur.  

    Als een onjuiste ontvangstregel is geselecteerd of als u opnieuw wilt beginnen, kunt u de regels op de inkoopfactuur gewoon verwijderen en vervolgens de functie **Ontvangstregels ophalen** opnieuw gebruiken.  
5. Kies de actie **Boeken** om de factuur te boeken.  

## <a name="to-remove-open-purchase-orders-after-combined-receipt-posting"></a>Open inkooporders verwijderen na gecombineerde ontvangstboeking  
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Gefact. inkooporders verwijderen** in en klik vervolgens op de gerelateerde koppeling.  
2. Vul indien nodig de velden in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)].
3. Kies de knop **OK**.  

U kunt de afzonderlijke orders ook handmatig verwijderen.

Herhaal stap 1 t/m 3 voor alle andere betrokken documenten, zoals inkoopraamcontracten.

## <a name="see-also"></a>Zie ook  
[Inkoop](purchasing-manage-purchasing.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


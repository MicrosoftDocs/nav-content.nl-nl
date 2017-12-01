---
title: Kosten of inkomsten rechtstreeks in grootboek registreren
description: Voor zakelijke activiteiten die niet door een document worden vertegenwoordigd, zoals kleinere ontvangsten of kasontvangsten, kunt u de gerelateerde transacties maken door dagboekregels te boeken in het venster Diversendagboek.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: direct posting, general ledger
ms.date: 06/28/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: fc87a8111eb1383985816eb5901c714bbe1ccac1
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-post-transactions-directly-to-the-general-ledger"></a>Procedure: Transacties direct naar het grootboek boeken
De meeste financiële transacties worden geboekt naar het grootboek door bepaalde bedrijfsdocumenten, zoals inkoopfacturen en verkooporders. Voor zakelijke activiteiten die niet door een document worden vertegenwoordigd in [!INCLUDE[d365fin](includes/d365fin_md.md)], zoals kleinere ontvangsten of kasontvangsten, kunt u de gerelateerde transacties maken door dagboekregels te boeken in het venster **Diversendagboek**.

Een veelvoorkomend gebruik van het dagboek is uitgaven van werknemers van eigen geld tijdens zakelijke activiteiten te boeken, voor latere terugbetaling. Zie voor meer informatie [Procedure: uitgaven van werknemers vastleggen en terugbetalen](finance-how-record-reimburse-employee-expenses.md).

Dagboeken boeken financiële transacties direct naar grootboekrekeningen en andere rekeningen zoals bank-, klant-, leveranciers- en werknemersrekeningen. Door te boeken met een dagboek worden er altijd posten gemaakt in grootboekrekeningen. Dit geldt zelfs ook als u bijvoorbeeld een dagboekregel naar een klantrekening boekt, omdat een post via een boekingsgroep is geboekt naar een rekening met vorderingen in het grootboek. U kunt uw versie van een dagboek aanpassen door een dagboekbatch of -sjabloon in te stellen. Zie [Werken met diversendagboeken](ui-work-general-journals.md) voor meer informatie.

In tegenstelling tot posten die zijn geboekt met documenten, die een creditnotaproces vereisen, kunt posten correct tegenboeken die met het diversendagboek zijn geboekt. Zie voor meer informatie [Procedure: Boekingen tegenboeken](finance-how-reverse-journal-posting.md).

## <a name="to-post-a-transaction-directly-to-a-general-ledger-account"></a>Een transactie direct naar het grootboek boeken
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Dagboeken** in en klik vervolgens op de gerelateerde koppeling.
2. Open de relevante dagboekbatch. Zie [Werken met diversendagboeken](ui-work-general-journals.md) voor meer informatie.
3. Vul op een nieuwe dagboekregel de velden indien nodig in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]    
4. Herhaal stap 3 voor alle afzonderlijke transacties die u wilt boeken.

    > [!TIP]  
    > Als u meerdere transactieregels boven één tegenrekeningsregel wilt invoeren, bijvoorbeeld, voor één bankrekening, selecteert u het selectievakje **Salderingsbedrag voorstellen** op de regel voor uw batch in het venster **Fin. dagboekbatches**. Vervolgens wordt het veld **Bedrag** op de tegenrekeningsregel automatisch ingevuld met de waarde die nodig is om de transacties in balans te brengen.
5. Kies de actie **Boeken** om de transacties op de betreffende grootboekrekeningen te registreren.

## <a name="see-also"></a>Zie ook
[Werken met diversendagboeken](ui-work-general-journals.md)  
[Procedure: kosten van werknemers registreren en terugbetalen](finance-how-record-reimburse-employee-expenses.md)  
[Procedure: boekingen tegenboeken](finance-how-reverse-journal-posting.md)  
[Financiën](finance.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  


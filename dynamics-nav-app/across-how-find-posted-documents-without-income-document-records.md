---
title: Documenten zonder bijlagen zoeken
Description: "U kunt grootboekposten zoeken voor geboekte inkoop- en verkoopdocumenten die geen elektronische inkomende documenten hebben, zoals geïmporteerde facturen."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 515026b4da842afeda1759f50313dc26bcfd3350
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-find-posted-documents-without-incoming-document-records"></a>Procedure: Geboekte documenten zonder inkomende documentrecords zoeken
Vanuit de vensters **Rekeningschema** en **Grootboekposten** kunt u zoeken naar grootboekposten voor geboekte inkoop- en verkoopdocumenten die geen inkomende documentrecords hebben, en deze centraal koppelen aan bestaande records of nieuwe records maken met gekoppelde documentbestanden.

## <a name="to-find-posted-documents-without-incoming-document-records"></a>Geboekte documenten zonder inkomende documentrecords zoeken
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Rekeningschema** in en klik vervolgens op de gerelateerde koppeling.
2. Selecteer een regel voor een grootboekrekening waarvan de grootboekposten die u wilt zien, geboekte inkoop- en verkoopdocumenten zijn zonder inkomende documentrecords en kies vervolgens de actie **Geboekte documenten zonder inkomend document**.
3. U kunt ook de actie **Posten** kiezen.
4. Kies in het venster **Grootboekposten** de actie **Geboekte documenten zonder inkomend document**.

Het venster **Geboekte documenten zonder inkomend document** wordt geopend en toont geboekte inkoop- en verkoopdocumenten zonder inkomende documentrecords die worden gerepresenteerd door grootboekposten in de Grootboekrekening waarvoor u het venster hebt geopend. Het venster kan maximaal 1000 regels weergeven. Standaard bevat het veld **Datumfilter** daarom een filter dat de regels beperkt tot posten met een boekingsdatum vanaf het begin van de boekhoudperiode tot de werkdatum.

## <a name="to-connect-found-documents-to-existing-incoming-document-records"></a>Gevonden documenten koppelen aan bestaande inkomende documentrecords
1. Selecteer in het venster **Geboekte documenten zonder inkomend document** de regel voor een geboekt document dat u wilt koppelen aan een bestaande inkomende documentrecord en kies vervolgens de actie **Inkomend document selecteren** .
2. Selecteer in het venster **Inkomende documenten** de inkomende documentrecord die u wilt koppelen aan het gevonden geboekte document en kies vervolgens de knop **OK**.
3. Selecteer in het venster **Geboekte documenten zonder inkomend document** de inkomende documentrecord die nu is gekoppeld aan het geboekte document, zoals u kunt zien in het feitenblok **Inkomende documentbestanden**.

Als er geen relevante inkomende documentrecord in het venster **Inkomende documenten** staat, kunt u er een maken. Zie [Procedure: Inkomende documentrecords maken](across-how-create-income-document-records.md) voor meer informatie.

## <a name="see-also"></a>Zie ook
[Inkomende documenten verwerken](across-process-income-documents.md)  
[Inkomende documenten](across-income-documents.md)  
[Inkoop](purchasing-manage-purchasing.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


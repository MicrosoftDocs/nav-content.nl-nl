---
title: 'Procedure: Geboekte documenten zonder inkomende documentrecords zoeken'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: eb65922decc86ca6834cae4cf46c6f2ff492e29c
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-find-posted-documents-without-incoming-document-records"></a>Procedure: Geboekte documenten zonder inkomende documentrecords zoeken
Vanuit de vensters **Rekeningschema** en **Grootboekposten** kunt u zoeken naar grootboekposten voor geboekte inkoop- en verkoopdocumenten die geen inkomende documentrecords hebben, en deze centraal koppelen aan bestaande records of nieuwe records maken met gekoppelde documentbestanden.

## <a name="to-find-posted-documents-without-incoming-document-records"></a>Geboekte documenten zonder inkomende documentrecords zoeken
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Rekeningschema** in en kies vervolgens de gerelateerde koppeling.
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
[Inkoop beheren](purchasing-manage-purchasing.md)  
[Werken met Dynamics NAV](ui-work-product.md)


---
title: 'Procedure: Inkomende documentrecords van documenten en posten maken en verbinden'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: fece4e6e38075db6d394c71418fda82a7aa082e1
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-connect-and-disconnect-incoming-document-records-from-documents-and-entries"></a>Procedure: Inkomende documentrecords van documenten en posten maken en verbinden
U kunt externe bedrijfsdocumenten in Dynamics NAV opslaan door de documentbestanden aan de gerelateerde inkomende documentrecords te koppelen. Als het document, zoals een inkoopfactuur, niet is ontstaan als inkomende documentrecord, kunt u het later nog maken en koppelen aan een inkomende documentrecord. U kunt inkomende documentbestanden ook koppelen aan geboekte inkoop- en verkoopdocumenten en aan leveranciers-, klant- en grootboekposten door het feitenblok **Inkomende documentbestanden** te gebruiken, bijvoorbeeld in het venster **Geboekte inkoopfacturen** en het venster **Leveranciersposten**.

Vanuit de vensters **Rekeningschema** en **Grootboekposten** kunt u zoeken naar grootboekposten voor geboekte inkoop- en verkoopdocumenten die geen inkomende documentrecords hebben, en deze centraal koppelen aan bestaande records of nieuwe records maken met gekoppelde documentbestanden. Zie [Procedure: Geboekte documenten zonder inkomende documentrecords zoeken](across-how-find-posted-documents-without-income-document-records.md) voor meer informatie.

In de volgende procedures wordt beschreven hoe u een bestand koppelt aan een bestaande inkoopfactuur die niet van een inkomende documentrecord is gemaakt, en hoe u een bestand koppelt aan een leverancierspost. Het koppelen van een bestand aan geboekte inkoop- of verkoopdocumenten werkt op dezelfde wijze.

## <a name="to-create-and-connect-an-incoming-document-record-from-a-purchase-invoice"></a>Een inkomende documentrecord maken van een inkoopfactuur en koppelen
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Inkoopfacturen** in en kies vervolgens de gerelateerde koppeling.
2. Selecteer de regel voor een inkoopfactuur waaraan u een bestand wilt koppelen en kies vervolgens de actie **Inkomend document van bestand maken**.
3. U kunt ook de regel voor een inkoopfactuur selecteren waaraan u een bestand wilt koppelen en vervolgens de actie **Bestand koppelen** kiezen.
4. In het venster **Bestand invoegen**, selecteert u het bestand dat het betreffende inkomende document vertegenwoordigt. Kies vervolgens de knop **Openen**.

## <a name="to-create-and-connect-an-incoming-document-record-from-a-vendor-ledger-entry"></a>Een inkomende documentrecord maken van een leverancierspost en koppelen
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Leveranciersposten** in en kies vervolgens de gerelateerde koppeling.
2. Selecteer een regel voor een leverancierspost waaraan u een bestand wilt koppelen en kies vervolgens de actie **Inkomend document van bestand maken**.
3. U kunt ook een regel voor een leverancierspost selecteren waaraan u een bestand wilt koppelen en vervolgens de actie **Bestand koppelen** kiezen.
4. In het venster **Bestand invoegen**, selecteert u het bestand dat het betreffende inkomende document vertegenwoordigt. Kies vervolgens de knop **Openen**.

## <a name="to-remove-a-connection-from-an-incoming-document-record-to-a-posted-document"></a>De relatie van een inkomende documentrecord met een geboekt document verwijderen
U kunt bestandbijlagen van niet-geboekte documenten op elk moment verwijderen door de gerelateerde inkomende documentrecord te verwijderen. Als het document is geboekt, moet u eerst de relatie met de inkomende documentrecord verwijderen.

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Inkomende documenten** in en kies vervolgens de gerelateerde koppeling.
2. Selecteer de regel voor een inkomende documentrecord die is verbonden met een geboekt document dat u wilt verwijderen en kies vervolgens de actie **Referentie naar record verwijderen**.

De verbinding met het geboekte document wordt verwijderd. U kunt nu doorgaan met het verbinden van een andere inkomende documentrecord met het geboekte document, zoals wordt beschreven in dit onderwerp.

## <a name="see-also"></a>Zie ook  
[Inkomende documenten verwerken](across-process-income-documents.md)  
[Inkomende documenten](across-income-documents.md)  
[Inkoop beheren](purchasing-manage-purchasing.md)  
[Werken met Dynamics NAV](ui-work-product.md)


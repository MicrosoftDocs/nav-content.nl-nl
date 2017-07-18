---
title: 'Procedure: Inkomende documenten instellen'
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
ms.openlocfilehash: 2bce97c76876c86a576ec6a281a306a46881027c
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-incoming-documents"></a>Procedure: Inkomende documenten instellen
Als u dagboekregels van inkomende documentrecords maakt, moet u in het venster **Instellingen van inkomende documenten** vastleggen welke dagboeksjabloon en batch moeten worden gebruikt.

Als u niet wilt dat gebruikers facturen of dagboekregels maken van inkomende documentrecords, tenzij de documenten zijn goedgekeurd, moet u fiatteurs instellen in het venster **Fiatteurs inkomende documenten**.

Als u PDF- en afbeeldingsbestanden naar elektronische documenten wilt omzetten waarnaar u kunt converteren, bijvoorbeeld inkoopfacturen in Dynamics NAV, moet u eerst de OCR-functie instellen en de service inschakelen.

Wanneer de functie Inkomende documenten is ingesteld, kunt u verschillende functies gebruiken om onkostenbewijzen te controleren, OCR-taken te beheren en inkomende documentbestanden handmatig of automatisch te converteren naar de relevante documenten of dagboekregels. De externe bestanden kunnen worden gekoppeld in elke procesfase, inclusief naar geboekte documenten en naar de resulterende leverancier, klant en grootboekposten. Zie voor meer informatie [Procedure: Inkomende documenten verwerken](across-process-income-documents.md).

## <a name="to-set-up-the-incoming-documents-feature"></a>De functie Inkomende documenten instellen
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Instellingen van inkomende documenten** in en kies vervolgens de gerelateerde koppeling.
2. Vul indien nodig de velden in. Kies een veld om een korte omschrijving van het veld of een koppeling naar meer informatie te lezen.

## <a name="to-set-up-approvers-of-incoming-document-records"></a>Fiatteurs van inkomende documentrecords instellen
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Instellingen van inkomende documenten** in en kies vervolgens de gerelateerde koppeling.  
2. Kies in het venster **Instellingen van inkomende documenten** de actie **Fiatteurs**.

    Het venster **Fiatteurs inkomende documenten** bevat alle gebruikers die zijn ingesteld in uw Dynamics NAV.  
3. Selecteer een of meer gebruikers die een inkomend document kunnen goedkeuren voordat een verwant document of verwante dagboekregel kan worden gemaakt.

Wanneer fiatteurs zijn ingesteld in het venster **Fiatteurs inkomende documenten**, kunnen alleen die gebruikers een inkomend document goedkeuren als het selectievakje **Goedkeuring vereist voor maken** is ingeschakeld in het venster **Instellingen inkomende documenten**.

**Opmerking**: deze goedkeuringsinstellingen zijn niet gerelateerd aan goedkeuringswerkstromen. Zie voor meer informatie [Procedure: Goedkeuringswerkstromen gebruiken](across-how-use-approval-workflows.md).

## <a name="to-set-up-an-ocr-service"></a>Een OCR-service instellen
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Instellingen van OCR-service** in en kies vervolgens de gerelateerde koppeling.
2. Vul indien nodig de velden in. Kies een veld om een korte omschrijving van het veld of een koppeling naar meer informatie te lezen.


## <a name="to-encrypt-your-login-information"></a>Uw aanmeldgegevens versleutelen
We raden u aan de aanmeldgegevens te beveiligen die u invoert in het venster **Instellingen van OCR-service**. U kunt gegevens op de server versleutelen door nieuwe encryptiesleutels te genereren of bestaande sleutels te importeren die u inschakelt op de serverinstantie die verbinding maakt met de database.

1. Kies in het venster **Instellingen van OCR-service** de actie **Versleutelingsbeheer**.
2. Schakel in het venster **Beheer gegevensversleuteling** versleuteling van uw gegevens in.

## <a name="see-also"></a>Zie ook  
[Inkomende documenten verwerken](across-process-income-documents.md)  
[Inkomende documenten](across-income-documents.md)  
[Inkoop beheren](purchasing-manage-purchasing.md)  
[Werken met Dynamics NAV](ui-work-product.md)


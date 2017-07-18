---
title: 'Procedure: verdeelsleutels in dagboeken gebruiken'
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: d239ab62c4be88ccc4a2ce2669dcc2c20a3c0126
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

#  <a name="how-to-use-allocation-keys-in-general-journals"></a>Procedure: verdeelsleutels in dagboeken gebruiken
U kunt een post in een dagboek verdelen over verschillende rekeningen wanneer u het dagboek boekt. De verdeling kan plaatsvinden op basis van aantal, percentage of bedrag.

## <a name="to-set-up-allocation-keys"></a>Verdeelsleutels instellen 
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Periodiek dagboek** in en kies vervolgens de gerelateerde koppeling.
2. Kies het veld **Batchnaam** om het venster **Fin. dagboekbatches** te openen.
3. U kunt verdeelsleutels in een bestaande batch in de lijst wijzigen of u kunt een nieuwe batch met verdeelsleutels maken.
  * Als u een nieuwe batch wilt maken, kiest u de actie **Nieuw** en gaat u naar de volgende stap.
  * Als u de verdeelsleutels van een bestaand dagboek wilt wijzigen, selecteert u het dagboek en gaat u naar stap 7.    
4. Voer in het veld **Naam** een naam voor de batch in, bijvoorbeeld Schoonmaak. Voer in het veld **Omschrijving** een omschrijving in, bijvoorbeeld Dagboek schoonmaakkosten.
5. Wanneer u klaar bent, sluit u het venster. Er wordt een nieuw, leeg periodiek dagboek geopend. 
6. Vul de velden op de regel in.
7. Kies de actie **Verdeelsleutels**. 
8. Voeg voor elke verdeelsleutel een regel toe. U moet ofwel het veld **Verdeelsleutel %**, of **Verdeelsleutelaantal**, of **Bedrag** invullen. U moet ook het veld **Rekeningnr.** invullen en, als u de transactie verdeelt over globale dimensies, ook de globale dimensievelden.
9. Als u een percentage op de regel invoert, wordt het bedrag in het veld **Bedrag** automatisch berekend. Deze bedragen hebben het tegengestelde teken van het totale bedrag in het veld **Bedrag** in het periodieke dagboek.
10. Kies **OK** na het invoeren van de verdeelsleutelregels om terug te keren naar het venster **Periodiek dagboek**. Het veld **Verdeeld bedrag (LV)** wordt ingevuld en de inhoud komt overeen met het veld **Bedrag**.
11. Boek het dagboek.

## <a name="to-change-an-allocation-key-that-has-already-been-set-up"></a>Een reeds ingestelde verdeelsleutel wijzigen
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Periodiek dagboek** in en kies vervolgens de gerelateerde koppeling.
2. Selecteer in het venster **Periodiek dagboek** het dagboek met de verdeling.
3. Kies de regel met de verdeelsleutel en kies vervolgens **Verdeelsleutels**.
4. Wijzig de betreffende velden en sluit het venster.

## <a name="see-also"></a>Zie ook
[Werken met diversendagboeken](ui-work-general-journals.md)  
[Documenten en dagboeken boeken](ui-post-documents-journals.md)





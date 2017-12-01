---
title: Overzicht van taken voor het toewijzen van kosten en inkomsten
description: Beschrijft de taken om een post in een dagboek te verdelen over verschillende rekeningen wanneer u het dagboek boekt.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 06/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: fdb03090dc9ba024d84a175e313f7d530bd0feae
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-allocate-costs-and-income"></a>Procedure: Kosten en inkomsten toewijzen
U kunt een post in een dagboek verdelen over verschillende rekeningen wanneer u het dagboek boekt. De verdeling kan plaatsvinden op basis van drie verschillende methoden.

* Aantal
* Percentage (%)
* Bedrag

De toewijzingsfuncties kunnen worden gebruikt met periodieke dagboeken en in VA-dagboeken.
<!--You can also distribute the cost or revenue of a line to an intercompany partner when you post a sales or purchase document. When you post the document, a line will be posted in your general journal, and a corresponding line will be created in the intercompany outbox.-->

In de volgende procedures wordt beschreven hoe voorbereidingen moeten worden getroffen om kosten in een periodiek dagboek te verdelen door verdeelsleutels te definiëren. Wanneer verdeelsleutels worden gedefinieerd, voltooit en boekt u het dagboek zoals elk ander periodiek dagboek. Zie [Werken met diversendagboeken](ui-work-general-journals.md) voor meer informatie.

## <a name="to-set-up-allocation-keys"></a>Verdeelsleutels instellen
U kunt een post in een periodiek dagboek verdelen over verschillende rekeningen wanneer u het dagboek boekt. De verdeling kan plaatsvinden op basis van aantal, percentage of bedrag.
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Periodiek dagboek** in en klik vervolgens op de gerelateerde koppeling.
2. Kies het veld **Batchnaam** om het venster **Fin. dagboekbatches** te openen.
3. U kunt verdeelsleutels in een bestaande batch in de lijst wijzigen of u kunt een nieuwe batch met verdeelsleutels maken.
   * Als u een nieuwe batch wilt maken, kiest u de actie **Nieuw** en gaat u naar de volgende stap.
   * Als u de verdeelsleutels van een bestaand dagboek wilt wijzigen, selecteert u het dagboek en gaat u naar stap 7.    
4. Voer in het veld **Naam** een naam voor de batch in, bijvoorbeeld Schoonmaak. Voer in het veld **Omschrijving** een omschrijving in, bijvoorbeeld Dagboek schoonmaakkosten.
5. Wanneer u klaar bent, sluit u het venster. Er wordt een nieuw, leeg periodiek dagboek geopend.
6. Vul de velden op de regel in.
7. Kies de actie **Verdeelsleutels**.
8. Voeg voor elke verdeelsleutel een regel toe. U moet ofwel het veld **Verdeelsleutel %**, of **Verdeelsleutelaantal**, of **Bedrag** invullen. U moet ook het veld **Rekeningnr.** invullen. Als u de transactie wilt toewijzen aan verschillende globale dimensies, moet u ook de globale dimensievelden invullen.
9. Als u een percentage op de regel invoert, wordt het bedrag in het veld **Bedrag** automatisch berekend. Deze bedragen hebben het tegengestelde teken van het totale bedrag in het veld **Bedrag** in het periodieke dagboek.
10. Kies **OK** na het invoeren van de verdeelsleutelregels om terug te keren naar het venster **Periodiek dagboek**. Het veld **Verdeeld bedrag (LV)** wordt ingevuld en de inhoud komt overeen met het veld **Bedrag**.
11. Boek het dagboek.

## <a name="to-change-an-allocation-key-that-has-already-been-set-up"></a>Een reeds ingestelde verdeelsleutel wijzigen
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Periodiek dagboek** in en klik vervolgens op de gerelateerde koppeling.
2. Selecteer in het venster **Periodiek dagboek** het dagboek met de verdeling.
3. Kies de regel met de verdeelsleutel en kies vervolgens **Verdeelsleutels**.
4. Pas de relevante velden aan en kies vervolgens de knop **OK**.

## <a name="see-also"></a>Zie ook
[Afsluitingsjaren en -perioden](year-close-years-periods.md)  
[Werken met diversendagboeken](ui-work-general-journals.md)    
[Documenten en dagboeken boeken](ui-post-documents-journals.md)    
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


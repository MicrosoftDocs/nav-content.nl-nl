---
title: 'Procedure: Vaste activa afschrijven of aflossen'
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
ms.openlocfilehash: af71f30681d436ed5da1cd6cb3c2e13f86558631
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-depreciate-or-amortize-fixed-assets"></a>Procedure: Vaste activa afschrijven of aflossen
Afschrijvingen worden gebruikt om de kosten van vaste activa, zoals machines en apparatuur, te spreiden over de afschrijfbare levensduur. Voor elk vast activum moet u aangeven hoe de afschrijving wordt toegepast.  

 U kunt een afschrijving op twee manieren boeken:
- Automatisch, door de batchverwerking **Afschrijving berekenen** uit te voeren.
- Handmatig, met behulp van het financieel dagboek voor vaste activa.  

In Dynamics NAV kan dagelijkse afschrijving worden berekend zodat u de afschrijving voor elke willekeurige periode kunt berekenen. Zodoende kunt u de huidige bedrijfsresultaten per maand, per kwartaal of jaarlijks analyseren. Bij deze berekening worden een standaardjaar van 360 dagen en een standaardmaand van 30 dagen gebruikt. Zie [Afschrijvingsmethoden](fa-depreciation-methods.md) voor meer informatie.

Als een vast activum door verschillende afdelingen wordt gebruikt, kan de periodieke afschrijving automatisch worden toegewezen aan deze afdelingen volgens een zelfgedefinieerde toewijzingstabel.  

U kunt onjuiste afschrijvingsposten annuleren met de batchverwerking **VA-posten annuleren** . Nadat de posten zijn geannuleerd, kunt u het juiste afschrijvingsbedrag boeken door de batchverwerking **Afschrijving berekenen** opnieuw uit te voeren. Als u fouten corrigeert, worden deze geboekt als foutieve VA-posten.  

Indexering wordt gebruikt om waarden aan te passen voor algemene prijswijzigingen. Met de batchverwerking **Vast activum indexeren** kunt u de afschrijvingen opnieuw berekenen.  

## <a name="to-calculate-a-depreciation-automatically"></a>Een afschrijving automatisch berekenen
U kunt de batchverwerking **Afschrijving berekenen** eens per maand, of op een tijdstip naar keuze uitvoeren. Vaste activa die zijn verkocht, activa die zijn geblokkeerd of inactieve activa en vaste activa waarin de handmatige afschrijving wordt gebruikt, worden genegeerd.    

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Afschrijving berekenen** in en kies vervolgens de gerelateerde koppeling.  
2. Vul indien nodig de velden in. Kies een veld om een korte omschrijving van het veld of een koppeling naar meer informatie te lezen.
3. Kies de knop **Ok**.  

    Met de batchverwerking wordt de afschrijving berekend en worden regels in het financieel dagboek voor vaste activa gemaakt.  
4. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Financieel dagboek voor vaste activa** in en kies vervolgens de gerelateerde koppeling.

    In het venster **Financieel dagboek van vaste activa** in het veld **Aantal afschrijvingsdagen** kunt u zien hoeveel afschrijvingsdagen er zijn berekend.  
5. Kies de actie **Boeken**.

## <a name="to-post-a-depreciation-manually-from-the-fixed-asset-gl-journal"></a>Een afschrijving handmatig boeken vanuit het financieel dagboek voor vaste activa
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Financieel dagboek van vaste activa** in en kies vervolgens de gerelateerde koppeling.  
2. Maak een eerste dagboekregel en vul de velden indien nodig in.
3. In het veld **VA-boekingssoort** selecteert u **Afschrijving**.
4. Kies de actie **VA-tegenrekening invoegen**. Er wordt een tweede dagboekregel gemaakt voor de tegenrekening die voor de afschrijvingsboeking is ingesteld. Zie het gedeelte "Boekingsgroepen voor vaste activa instellen" in de [Procedure: Algemene gegevens voor vaste activa instellen](fa-how-setup-general.md) voor meer informatie.
5. Kies op het tabblad **Start** de optie **Boeken** om het dagboek te boeken.

Als u verdeelsleutels voor vaste activa hebt ingesteld om bedragen over verschillende afdelingen of projecten te verdelen, kunnen de bedragen tijdens de boeking worden verdeeld. Zie [Procedure: Algemene gegevens voor vaste activa instellen](fa-how-setup-general.md) voor meer informatie.

## <a name="to-calculate-allocations-in-the-fixed-asset-gl-journal"></a>Verdelingen in het financieel dagboek voor vaste activa berekenen
Als een vast activum door verschillende afdelingen wordt gebruikt, kan de periodieke afschrijving automatisch worden toegewezen aan deze afdelingen volgens een zelfgedefinieerde toewijzingstabel.  

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Financieel dagboek van vaste activa** in en kies vervolgens de gerelateerde koppeling.   
Maak een eerste regel en vul de velden indien nodig in.
3. In het veld **VA-boekingssoort** selecteert u **Verdeelsleutel**.
4. Kies de actie **VA-tegenrekening invoegen**. Er wordt een tweede dagboekregel gemaakt voor de tegenrekening die voor de boeking van de verdeelsleutel is ingesteld.
5. Kies op het tabblad **Start** de optie **Boeken** om het dagboek te boeken.

## <a name="use-duplication-lists-to-prepare-to-post-to-multiple-depreciation-books"></a>Duplicatielijsten gebruiken ter voorbereiding op de boeking naar meerdere afschrijvingsboeken  
Als u dagboekregels invult die naar een afschrijvingsboek moeten worden geboekt, kunt u de regels naar een apart dagboek dupliceren, zodat ze van daaruit naar een ander afschrijvingsboek kunnen worden geboekt. Zie het gedeelte "Posten boeken naar verschillende afschrijvingsboeken" voor meer informatie.

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Afschrijvingsboeken** in en kies vervolgens de gerelateerde koppeling.  
2. Open het betreffende afschrijvingsboek en schakel vervolgens het selectievakje **Deel van duplicatielijst** in.  

**Belangrijk**: als u het veld **Duplicatielijst gebruiken** hebt geselecteerd, moet u geen nummerreeksen gebruiken voor het dagboek. De reden is dat de nummerreeks voor het financieel dagboek voor vaste activa niet overeenkomt met de nummerreeks voor het dagboek voor vaste activa.

## <a name="to-post-entries-to-different-depreciation-books"></a>Posten naar verschillende afschrijvingsboeken boeken  
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Financieel dagboek van vaste activa** in en kies vervolgens de gerelateerde koppeling.
2. Schakel in het dagboek waarmee u de afschrijving wilt boeken, het selectievakje **Duplicatielijst gebruiken** in.
3. Vul indien nodig de resterende velden in.
4. Kies de actie **Boeken**.
5. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **VA-dagboeken** in en kies vervolgens de gerelateerde koppeling.

    Het venster **VA-dagboek** bevat nieuwe regels voor verschillende afschrijvingsboeken volgens de duplicatielijst.   

6. Controleer of bewerk de regels en kies vervolgens de actie **Boeken**.

**Opmerking**: u kunt een post ook naar een apart boek dupliceren door tijdens het invullen van een dagboekregel in het veld **Dupliceren in afschrijvingsboek** de code van een afschrijvingsdagboek op te geven.

Met behulp van de batchverwerking **Afschrijvingsboek kopiëren** kunt u posten uit afschrijvingsboeken naar andere afschrijvingsboeken kopiëren. Met de batchverwerking worden dagboekregels gemaakt in de dagboekbatch die u hebt opgegeven in het venster **VA-dagboekinstellingen** voor het afschrijvingsboek waarnaar u wilt kopiëren. Zie de volgende procedure voor meer informatie.

## <a name="to-copy-fixed-asset-ledger-entries-between-depreciation-books"></a>Posten voor vaste activa tussen afschrijvingsboeken kopiëren  
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Afschrijvingsboeken** in en kies vervolgens de gerelateerde koppeling.
2. Open de betreffende afschrijvingsboekkaart en kies vervolgens de actie **Afschrijvingsboek kopiëren**.  
3. Vul in het venster **Afschrijvingsboek kopiëren** indien nodig de velden in.  
4. Kies de knop **Ok**.  

De gekopieerde regels worden in het financieel dagboek voor vaste activa of het dagboek voor vaste activa gemaakt, afhankelijk van de vraag of het afschrijvingsboek dat u kopieert, geïntegreerd is met het grootboek.

## <a name="see-also"></a>Zie ook
[Vaste activa beheren](fa-manage.md)  
[Vaste activa instellen](fa-setup.md)  
[Financiën](finance-setup.md)  
[Welkom bij Dynamics NAV](across-get-started.md)


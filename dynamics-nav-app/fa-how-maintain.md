---
title: Vaste activa onderhouden
description: U houdt een onderhoudsrecord bij van de reparaties en onderhoud aan een vast activum.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: repair, service
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: c43ed582294a5f77408e076a13d3cd07eb9f4d0f
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-maintain-fixed-assets"></a>Procedure: Vaste activa onderhouden.
Onderhoudskosten zijn periodieke kosten die worden gemaakt om de waarde van vaste activa te behouden. In tegenstelling tot belangrijke verbeteringen zorgen ze niet voor waardevermeerdering.

U kunt een bijgewerkt bestand over het onderhoud en de beurten voor uw vaste activa bijhouden, zodat u altijd het onderhoudsoverzicht van een vast activum bij de hand hebt. Telkens wanneer een vast activum een onderhoudsbeurt krijgt, registreert u alle relevante informatie, zoals de datum van de onderhoudsbeurt, het leveranciersnummer en het telefoonnummer van de onderhoudsdienst. De onderhoudsregistratie wordt voor elk vast activum opgeslagen op de betreffende VA-kaart.

Indexering wordt gebruikt om waarden aan te passen voor algemene prijswijzigingen. Met de batchverwerking **Vast activum indexeren** kunt u de onderhoudskosten opnieuw berekenen.

## <a name="to-record-maintenance-work-on-a-fixed-asset"></a>Onderhoudswerk aan een vast activum registreren
Elke keer dat onderhoud wordt uitgevoerd, zoals een onderhoudsbeurt, kunt u dit registreren voor het betreffende vaste activum in het venster **Onderhoudsregistratie**.  

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Vaste activa** in en klik vervolgens op de gerelateerde koppeling.  
2. Selecteer het vaste activum waarvoor u onderhoud wilt registreren en kies vervolgens de actie **Onderhoudsregistratie**.
3. Vul in het venster **Onderhoudsregistratie** indien nodig de velden in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-post-maintenance-costs-from-a-fixed-asset-gl-journal"></a>Onderhoudskosten boeken vanuit een financieel dagboek voor vaste activa
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Afschrijvingsboekoverzicht** in en klik vervolgens op de gerelateerde koppeling.  
2. Selecteer het afschrijvingsboek dat aan het vaste activum is toegewezen en kies vervolgens de actie **Bewerken**.
3. Zorg er in het venster **Afschrijvingsboek** voor dat het selectievakje **Onderhoud** niet is ingeschakeld. Hierdoor worden onderhoudskosten niet naar het grootboek geboekt.
4. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **VA-fin. dagboeken** in en klik vervolgens op de gerelateerde koppeling.  
5. Maak een eerste dagboekregel en vul de velden indien nodig in.
6. In het veld **VA-boekingssoort** selecteert u **Onderhoud**.
7. Kies de actie **VA-tegenrekening invoegen**. Er wordt een tweede dagboekregel gemaakt voor de tegenrekening die voor de boeking van het onderhoud is ingesteld.

    > [!NOTE]  
>   Stap 7 werkt alleen als u het volgende hebt ingesteld: in het venster **VA-boekingsgroep** voor de boekingsgroep van het vaste activum bevat het veld **Onderhoudskostenrekening** de grootboekdebetrekening en het veld **Tegenrekening onderhoud** bevat de grootboekrekening waarnaar u tegenrekeningsposten voor afschrijving wilt boeken. Zie het gedeelte "Boekingsgroepen voor vaste activa instellen" in de [Procedure: Algemene gegevens voor vaste activa instellen](fa-how-setup-general.md) voor meer informatie.
8. Kies de actie **Boeken**.

## <a name="to-follow-up-on-fixed-assets-service-visits"></a>Onderhoudsbeurten voor vaste activa opvolgen
U kunt het rapport **Onderhoud - Volgende beurt** afdrukken om na te gaan voor welke activa er een onderhoudsbeurt is gepland. U kunt dit rapport ook gebruiken bij het bijwerken van het veld **Volgende onderhoudsbeurt** op de kaarten voor vaste activa.  

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "Zoeken naar pagina of rapport")-pictogram, voer **Onderhoud - Volgende beurt** in en klik vervolgens op de gerelateerde koppeling.  
2. Vul de velden **Begindatum** en **Einddatum** in.  
3. Kies de knop **Afdrukken** of **Voorbeeld**.

## <a name="to-monitor-maintenance-costs"></a>Onderhoudskosten controleren
U kunt de onderhoudskosten bekijken wanneer u de statistische gegevens van een vast activum controleert.  

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Vaste activa** in en klik vervolgens op de gerelateerde koppeling.
2. Selecteer het vaste activum waarvoor u onderhoudskosten wilt bekijken en kies vervolgens de actie **Afschrijvingsboeken**.
3. In het venster **Afschrijvingsboeken voor vaste activa** selecteert u het betreffende afschrijvingsboek voor vaste activa en kiest u vervolgens de actie **Statistieken**.
4. Kies in het venster **VA-statistiek** het veld **Onderhoud**.

Het venster **Onderhoudsposten** wordt geopend met de posten die het bedrag in het veld **Onderhoud** vormen.

## <a name="to-view-or-print-maintenance-costs-for-multiple-fixed-assets"></a>Onderhoudskosten voor meerdere vaste activa weergeven of afdrukken
In het rapport **Onderhoud - Analyse** kunt u aangeven of u onderhoud van één, twee of drie onderhoudscodes wilt zien voor een opgegeven datum of periode. U kunt het totaal van alle geselecteerde activa of het totaal per activum bekijken.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Onderhoud - Analyse** in en klik vervolgens op de gerelateerde koppeling.
2. Vul indien nodig de velden in.
3. Kies de knop **Afdrukken** of **Voorbeeld**.

## <a name="to-view-maintenance-ledger-entries"></a>Onderhoudsposten bekijken
U kunt ook de onderhoudsposten bestuderen door de onderhoudsposten te bekijken.  

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Vaste activa** in en klik vervolgens op de gerelateerde koppeling.
2. Selecteer het vaste activum waarvoor u posten wilt bekijken en kies vervolgens de actie **Afschrijvingsboeken**.
3. In het venster **Afschrijvingsboeken voor vaste activa** selecteert u het betreffende afschrijvingsboek voor vaste activa en kiest u vervolgens de actie **Onderhoudsposten**.

## <a name="to-view-or-print-maintenance-ledger-entries-for-multiple-fixed-assets"></a>Onderhoudskosten voor meerdere vaste activa weergeven of afdrukken
In het rapport **Onderhoud - Details** kunt u onderhoudsposten voor een of meerdere vaste activa afdrukken of weergeven.  

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Onderhoud - Detail** in en klik vervolgens op de gerelateerde koppeling.
2. Vul indien nodig de velden in.
3. Kies de knop **Afdrukken** of **Voorbeeld**.

## <a name="see-also"></a>Zie ook
[Vaste activa](fa-manage.md)  
[Vaste activa instellen](fa-setup.md)  
[Financiën](finance.md)  
[Welkom bij [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


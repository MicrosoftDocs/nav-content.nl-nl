---
title: 'Procedure: Vaste activa onderhouden.'
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
ms.openlocfilehash: 58077a38433a73b981a6f3d05ce7ed106acf32f4
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-maintain-fixed-assets"></a>Procedure: Vaste activa onderhouden.
Onderhoudskosten zijn periodieke kosten die worden gemaakt om de waarde van vaste activa te behouden. In tegenstelling tot belangrijke verbeteringen zorgen ze niet voor waardevermeerdering.

U kunt een bijgewerkt bestand over het onderhoud en de beurten voor uw vaste activa bijhouden, zodat u altijd het onderhoudsoverzicht van een vast activum bij de hand hebt. Telkens wanneer een vast activum een onderhoudsbeurt krijgt, registreert u alle relevante informatie, zoals de datum van de onderhoudsbeurt, het leveranciersnummer en het telefoonnummer van de onderhoudsdienst. De onderhoudsregistratie wordt voor elk vast activum opgeslagen op de betreffende VA-kaart.

Indexering wordt gebruikt om waarden aan te passen voor algemene prijswijzigingen. Met de batchverwerking **Vast activum indexeren** kunt u de onderhoudskosten opnieuw berekenen.

## <a name="to-record-maintenance-work-on-a-fixed-asset"></a>Onderhoudswerk aan een vast activum registreren  
Elke keer dat onderhoud wordt uitgevoerd, zoals een onderhoudsbeurt, kunt u dit registreren voor het betreffende vaste activum in het venster **Onderhoudsregistratie**.  

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Vaste activa** in en kies vervolgens de gerelateerde koppeling.  
2. Selecteer het vaste activum waarvoor u onderhoud wilt registreren en kies vervolgens de actie **Onderhoudsregistratie**.
3. Vul in het venster **Onderhoudsregistratie** indien nodig de velden in. Kies een veld om een korte omschrijving van het veld of een koppeling naar meer informatie te lezen.  

## <a name="to-post-maintenance-costs-from-a-fixed-asset-gl-journal"></a>Onderhoudskosten boeken vanuit een financieel dagboek voor vaste activa
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Afschrijvingsboekoverzicht** in en kies vervolgens de gerelateerde koppeling.  
2. Selecteer het afschrijvingsboek dat aan het vaste activum is toegewezen en kies vervolgens de actie **Bewerken**.
3. Zorg er in het venster **Afschrijvingsboek** voor dat het selectievakje **Onderhoud** niet is ingeschakeld. Hierdoor worden onderhoudskosten niet naar het grootboek geboekt.
4. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Financieel dagboek voor vaste activa** in en kies vervolgens de gerelateerde koppeling.  
5. Maak een eerste dagboekregel en vul de velden indien nodig in.
6. In het veld **VA-boekingssoort** selecteert u **Onderhoud**.
7. Kies de actie **VA-tegenrekening invoegen**. Er wordt een tweede dagboekregel gemaakt voor de tegenrekening die voor de boeking van het onderhoud is ingesteld.

    **Opmerking**: stap 7 werkt alleen als u het volgende hebt ingesteld: in het venster **VA-boekingsgroep** voor de boekingsgroep van het vaste activum bevat het veld **Onderhoudskostenrekening** de gootboekdebetrekening en het veld **Tegenrekening onderhoud** bevat de grootboekrekening waarnaar u tegenrekeningsposten voor onderhoud wilt boeken. Zie het gedeelte "Boekingsgroepen voor vaste activa instellen" in de [Procedure: Algemene gegevens voor vaste activa instellen](fa-how-setup-general.md) voor meer informatie.
8. Kies de actie **Boeken**.

## <a name="to-follow-up-on-fixed-assets-service-visits"></a>Onderhoudsbeurten voor vaste activa opvolgen
U kunt het rapport **Onderhoud - Volgende beurt** afdrukken om na te gaan voor welke activa er een onderhoudsbeurt is gepland. U kunt dit rapport ook gebruiken bij het bijwerken van het veld **Volgende onderhoudsbeurt** op de kaarten voor vaste activa.  

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Onderhoud - Volgende beurt** in en kies vervolgens de gerelateerde koppeling.  
2. Vul de velden **Begindatum** en **Einddatum** in.  
3. Kies de knop **Afdrukken** of **Voorbeeld**.

## <a name="to-monitor-maintenance-costs"></a>Onderhoudskosten controleren  
U kunt de onderhoudskosten bekijken wanneer u de statistische gegevens van een vast activum controleert.  

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Vaste activa** in en kies vervolgens de gerelateerde koppeling.
2. Selecteer het vaste activum waarvoor u onderhoudskosten wilt bekijken en kies vervolgens de actie **Afschrijvingsboeken**.
3. In het venster **Afschrijvingsboeken voor vaste activa** selecteert u het betreffende afschrijvingsboek voor vaste activa en kiest u vervolgens de actie **Statistieken**.
4. Kies in het venster **VA-statistiek** het veld **Onderhoud**.

Het venster **Onderhoudsposten** wordt geopend met de posten die het bedrag in het veld **Onderhoud** vormen.

## <a name="to-view-or-print-maintenance-costs-for-multiple-fixed-assets"></a>Onderhoudskosten voor meerdere vaste activa weergeven of afdrukken  
In het rapport **Onderhoud - Analyse** kunt u aangeven of u onderhoud van één, twee of drie onderhoudscodes wilt zien voor een opgegeven datum of periode. U kunt het totaal van alle geselecteerde activa of het totaal per activum bekijken.

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Onderhoud - Analyse** in en kies vervolgens de gerelateerde koppeling.
2. Vul indien nodig de velden in.
3. Kies de knop **Afdrukken** of **Voorbeeld**.

## <a name="to-view-maintenance-ledger-entries"></a>Onderhoudsposten bekijken
U kunt ook de onderhoudsposten bestuderen door de onderhoudsposten te bekijken.  
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Vaste activa** in en kies vervolgens de gerelateerde koppeling.
2. Selecteer het vaste activum waarvoor u posten wilt bekijken en kies vervolgens de actie **Afschrijvingsboeken**.
3. In het venster **Afschrijvingsboeken voor vaste activa** selecteert u het betreffende afschrijvingsboek voor vaste activa en kiest u vervolgens de actie **Onderhoudsposten**.

## <a name="to-view-or-print-maintenance-ledger-entries-for-multiple-fixed-assets"></a>Onderhoudskosten voor meerdere vaste activa weergeven of afdrukken  
In het rapport **Onderhoud - Details** kunt u onderhoudsposten voor een of meerdere vaste activa afdrukken of weergeven.  

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Onderhoud - Details** in en kies vervolgens de gerelateerde koppeling.
2. Vul indien nodig de velden in.
3. Kies de knop **Afdrukken** of **Voorbeeld**.

## <a name="see-also"></a>Zie ook
[Vaste activa beheren](fa-manage.md)  
[Vaste activa instellen](fa-setup.md)  
[Financiën](finance-setup.md)  
[Welkom bij Dynamics NAV](across-get-started.md)


---
title: 'Procedure: Inkomsten en kosten uitstellen'
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
ms.openlocfilehash: 865bc307e8635b5a5aba11b5bc2e2e448c05e769
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-defer-revenues-and-expenses"></a>Procedure: Inkomsten en kosten uitstellen
Als u inkomsten of kosten wilt verantwoorden in een andere periode dan waarin de transactie is geboekt, kunt u deze functionaliteit gebruiken om kosten en inkomsten automatisch uit te stellen via een opgegeven schema.

Om kosten of omzet over de betrokken boekhoudperioden te verdelen stelt u een uitstelsjabloon in voor de bron, het artikel of de grootboekrekening waarnaar de inkomsten of kosten worden geboekt. Wanneer u het gerelateerde verkoop- of inkoopdocument boekt, worden de inkomsten of kosten uitgesteld tot de betrokken boekhoudperioden, volgens een uitstelschema dat wordt bepaald door instellingen in de uitstelsjabloon en de boekingsdatum.

## <a name="to-set-up-a-gl-account-for-deferral"></a>Een grootboekrekening instellen voor uitstel
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Rekeningschema** in en kies vervolgens de gerelateerde koppeling.
2. Kies de actie **Nieuw**.
3. Vul de velden in om een grootboekrekening te maken voor uitgestelde inkomsten. Zie voor meer informatie [Het grootboek en het rekeningschema](finance-setup-general-ledger.md).
3. Herhaal stap 2 en 3 om een nieuwe grootboekrekening te maken voor uitgestelde kosten.

Selecteer voor beide soorten uitstel **Balans** in het veld **Type** en geef de rekeningen geschikte namen, zoals "Niet-gerealiseerde onkosten" voor uitgestelde inkomsten en "Niet-gerealiseerde onkosten" voor uitgestelde onkosten.

## <a name="to-set-up-a-deferral-template"></a>Een uitstelsjabloon instellen
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Uitstelsjablonen** in en kies vervolgens de gerelateerde koppeling.
2. Kies de actie **Nieuw**.
3. Vul indien nodig de velden in.
4. Geef in het veld **Berekeningsmethode** op hoe het veld **Bedrag** voor elke periode in het venster **Uitstelschema** wordt berekend. U hebt de volgende mogelijkheden:
    - **Lineair**: de periodieke uitstelbedragen worden berekend volgens het aantal perioden, verdeeld volgens de periodelengte.
    - **Gelijk per periode**: de periodieke uitstelbedragen worden berekend volgens het aantal perioden, gelijkelijk verdeeld over perioden.
    - **Dagen per periode**: de periodieke uitstelbedragen worden berekend volgens het aantal dagen in de periode.
    - **Door gebruiker gedefinieerd**: de periodieke uitstelbedragen worden niet berekend. U moet het veld Bedrag handmatig invullen voor elke periode in het venster Uitstelschema. Zie voor meer informatie het gedeelte "Een uitstelschema wijzigen vanuit een verkoopfactuur".

5. Geef in het veld **Periodebeschrijving** een omschrijving op die wordt weergegeven op posten voor de uitstelboeking. U kunt de volgende codes voor tijdelijke aanduidingen invoeren voor veel voorkomende waarden, die automatisch worden ingevoegd wanneer de periodebeschrijving wordt weergegeven.
    - %1 = het dagnummer van de periodeboekingsdatum
    - %2 = het weeknummer van de periodeboekingsdatum
    - %3 = het maandnummer van de periodeboekingsdatum
    - %4 = de maandnaam van de periodeboekingsdatum
    - %5 = de boekhoudperiodenaam van de periodeboekingsdatum
    - %6 = het boekjaar van de periodeboekingsdatum

Voorbeeld: de boekingsdatum is 06-02-2016. Als u "Kosten uitgesteld voor %4 %6" invoert, wordt de weergegeven beschrijving "Kosten uitgesteld voor februari 2016".

## <a name="to-assign-a-deferral-template-to-an-item"></a>Een uitstelsjabloon toewijzen aan een artikel
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Uitstelsjablonen** in en kies vervolgens de gerelateerde koppeling.
2. Open de kaart voor het artikel waarvoor de inkomsten en de kosten moeten worden uitgesteld naar de boekhoudperioden waarin het artikel is verkocht of gekocht.
3. Selecteer in het veld **Standaarduitstellingssjabloon** de relevante uitstelsjabloon.

## <a name="to-change-a-deferral-schedule-from-a-sales-invoice"></a>Een uitstelschema wijzigen vanuit een verkoopfactuur
**Opmerking**: de stappen in deze procedure zijn hetzelfde als wanneer u een uitstelschema voor onkosten wijzigt vanuit een inkoopfactuur.

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Verkoopfacturen** in en kies vervolgens de gerelateerde koppeling.
2. Maak een verkoopfactuur voor een artikel waaraan een uitstelsjabloon is toegewezen. Zie [Procedure: Verkopen factureren](sales-how-invoice-sales.md) voor meer informatie.

    U ziet dat wanneer u het artikel (of de bron of grootboekrekening) op de factuurregel invoert, het veld **Uitstelcode** wordt gevuld met de code van de toegewezen uitstelsjabloon.
3. Kies de actie **Uitstelschema**.
4. Wijzig in het veld **Uitstelschema** instellingen in de kop of waarden op de regels, bijvoorbeeld om het bedrag naar een extra boekhoudperiode uit te stellen.
5. Kies de actie **Schema berekenen**.
6. Kies de knop **Ok**. Het uitstelschema wordt bijgewerkt voor de verkoopfactuur. De relateerde uitstelsjabloon is ongewijzigd.

## <a name="to-preview-how-deferred-revenues-or-expenses-will-be-posted-to-the-general-ledger"></a>Zien hoe uitgestelde kosten of inkomsten naar het grootboek worden geboekt
**Opmerking**: de stappen in deze procedure zijn hetzelfde als wanneer u bekijkt hoe uitgestelde onkosten worden geboekt.

1. Kies in het venster **Verkoopfactuur** de actie **Voorbeeld van boeking weergeven**.
2. Kies in het venster **Voorbeeld van boeking weergeven** de actie **Grootboekpost** en kies vervolgens de actie **Verwante posten weergeven**.

Grootboekposten die moeten worden geboekt naar de opgegeven uitstelrekening, bijvoorbeeld Niet-gerealiseerde inkomsten, worden aangegeven door de omschrijving die u hebt ingevoerd in het veld **Periodebeschrijving** in de uitstelsjabloon, bijvoorbeeld "Uitgestelde kosten voor februari 2016".

## <a name="to-review-posted-deferrals-in-the-sales-deferral-summary-report"></a>Geboekte uitstellingen bekijken in het rapport Overzicht van verkoopuitstel
**Opmerking**: de stappen in deze procedure zijn hetzelfde als wanneer u het rapport Overzicht van inkoopuitstel bekijkt.

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Overzicht van verkoopuitstel** in en kies vervolgens de gerelateerde koppeling.
2. Voer in het venster **Overzicht van verkoopuitstel** in het veld **Saldo per** de datum in tot wanneer u uitgestelde inkomsten wilt zien.
3. Kies de knop **Voorbeeld**.

## <a name="see-also"></a>Zie ook
[Financiën](finance-setup.md)  
[Financiële kernprocessen instellen](finance-setup-setup-finance-setup.md)  
[Procedure: Werken met diversendagboeken.](ui-work-general-journals.md)


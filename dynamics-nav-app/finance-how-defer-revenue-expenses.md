---
title: 'Procedure: Inkomsten en kosten uitstellen'
description: Als u inkomsten en kosten wilt verantwoorden in andere perioden dan waarin de transactie is geboekt, kunt u kosten en inkomsten automatisch uitstellen via een opgegeven schema.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: postpone
ms.date: 06/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: f06d241d07bc613bb54cc0a278de419fafffbb58
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-defer-revenues-and-expenses"></a>Procedure: Inkomsten en kosten uitstellen
Als u inkomsten of kosten wilt verantwoorden in een andere periode dan waarin de transactie is geboekt, kunt u deze functionaliteit gebruiken om kosten en inkomsten automatisch uit te stellen via een opgegeven schema.

Om kosten of omzet over de betrokken boekhoudperioden te verdelen stelt u een uitstelsjabloon in voor de bron, het artikel of de grootboekrekening waarnaar de inkomsten of kosten worden geboekt. Wanneer u het gerelateerde verkoop- of inkoopdocument boekt, worden de inkomsten of kosten uitgesteld tot de betrokken boekhoudperioden, volgens een uitstelschema dat wordt bepaald door instellingen in de uitstelsjabloon en de boekingsdatum.

## <a name="to-set-up-a-gl-account-for-deferral"></a>Een grootboekrekening instellen voor uitstel
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Rekeningschema** in en klik vervolgens op de gerelateerde koppeling.
2. Kies de actie **Nieuw**.
3. Vul de velden in om een grootboekrekening te maken voor uitgestelde inkomsten. Zie voor meer informatie [Het grootboek en het rekeningschema](finance-general-ledger.md).
4. Herhaal stap 2 en 3 om een nieuwe grootboekrekening te maken voor uitgestelde kosten.

Selecteer voor beide soorten uitstel **Balans** in het veld **Type** en geef de rekeningen geschikte namen, zoals "Niet-gerealiseerde onkosten" voor uitgestelde inkomsten en "Niet-gerealiseerde onkosten" voor uitgestelde onkosten.

## <a name="to-set-up-a-deferral-template"></a>Een uitstelsjabloon instellen
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Uitstelsjablonen** in en klik vervolgens op de gerelateerde koppeling.
2. Kies de actie **Nieuw**.
3. Vul indien nodig de velden in.
4. Geef in het veld **Berekeningsmethode** op hoe het veld **Bedrag** voor elke periode in het venster **Uitstelschema** wordt berekend. U hebt de volgende mogelijkheden:

   * **Lineair**: de periodieke uitstelbedragen worden berekend volgens het aantal perioden, verdeeld volgens de periodelengte.
   * **Gelijk per periode**: de periodieke uitstelbedragen worden berekend volgens het aantal perioden, gelijkelijk verdeeld over perioden.
   * **Dagen per periode**: de periodieke uitstelbedragen worden berekend volgens het aantal dagen in de periode.
   * **Door gebruiker gedefinieerd**: de periodieke uitstelbedragen worden niet berekend. U moet het veld **Bedrag** handmatig invullen voor elke periode in het venster Uitstelschema. Zie voor meer informatie het gedeelte "Een uitstelschema wijzigen vanuit een verkoopfactuur".
5. Geef in het veld **Periodebeschrijving** een omschrijving op die wordt weergegeven op posten voor de uitstelboeking. U kunt de volgende codes voor tijdelijke aanduidingen invoeren voor veel voorkomende waarden, die automatisch worden ingevoegd wanneer de periodebeschrijving wordt weergegeven.

   * %1 = het dagnummer van de periodeboekingsdatum
   * %2 = het weeknummer van de periodeboekingsdatum
   * %3 = het maandnummer van de periodeboekingsdatum
   * %4 = de maandnaam van de periodeboekingsdatum
   * %5 = de boekhoudperiodenaam van de periodeboekingsdatum
   * %6 = het boekjaar van de periodeboekingsdatum

Voorbeeld: de boekingsdatum is 06-02-2016. Als u "Kosten uitgesteld voor %4 %6" invoert, wordt de weergegeven beschrijving "Kosten uitgesteld voor februari 2016".

## <a name="to-assign-a-deferral-template-to-an-item"></a>Een uitstelsjabloon toewijzen aan een artikel
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Uitstelsjablonen** in en klik vervolgens op de gerelateerde koppeling.
2. Open de kaart voor het artikel waarvoor de inkomsten en de kosten moeten worden uitgesteld naar de boekhoudperioden waarin het artikel is verkocht of gekocht.
3. Selecteer in het veld **Standaarduitstellingssjabloon** de relevante uitstelsjabloon.

## <a name="to-change-a-deferral-schedule-from-a-sales-invoice"></a>Een uitstelschema wijzigen vanuit een verkoopfactuur
> [!NOTE]  
>   De stappen in deze procedure zijn hetzelfde als wanneer u een uitstelschema voor onkosten wijzigt vanuit een inkoopfactuur.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Verkoopfacturen** in en klik vervolgens op de gerelateerde koppeling.
2. Maak een verkoopfactuur voor een artikel waaraan een uitstelsjabloon is toegewezen. Zie [Procedure: Verkopen factureren](sales-how-invoice-sales.md) voor meer informatie.

    U ziet dat wanneer u het artikel (of de bron of grootboekrekening) op de factuurregel invoert, het veld **Uitstelcode** wordt gevuld met de code van de toegewezen uitstelsjabloon.
3. Kies de actie **Uitstelschema**.
4. Wijzig in het veld **Uitstelschema** instellingen in de kop of waarden op de regels, bijvoorbeeld om het bedrag naar een extra boekhoudperiode uit te stellen.
5. Kies de actie **Schema berekenen**.
6. Kies de knop **Ok**. Het uitstelschema wordt bijgewerkt voor de verkoopfactuur. De relateerde uitstelsjabloon is ongewijzigd.

## <a name="to-preview-how-deferred-revenues-or-expenses-will-be-posted-to-the-general-ledger"></a>Zien hoe uitgestelde kosten of inkomsten naar het grootboek worden geboekt
> [!NOTE]  
>   De stappen in deze procedure zijn hetzelfde als wanneer u bekijkt hoe uitgestelde onkosten worden geboekt.

1. Kies in het venster **Verkoopfactuur** de actie **Voorbeeld van boeking weergeven**.
2. Kies in het venster **Voorbeeld van boeking weergeven** de actie **Grootboekpost** en kies vervolgens de actie **Verwante posten weergeven**.

Grootboekposten die naar de opgegeven uitstelrekening moeten worden geboekt, bijvoorbeeld Niet-gerealiseerde inkomsten, worden aangeduid door de omschrijving die u in het veld **Periodebeschrijving** in de uitstelsjabloon hebt ingevoerd, bijvoorbeeld "Uitgestelde kosten voor februari 2016".

## <a name="to-review-posted-deferrals-in-the-sales-deferral-summary-report"></a>Geboekte uitstellingen bekijken in het rapport Overzicht van verkoopuitstel
> [!NOTE]  
>   De stappen in deze procedure zijn hetzelfde als wanneer u het rapport Overzicht van inkoopuitstel bekijkt.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Overzicht van verkoopuitstel** in en klik vervolgens op de gerelateerde koppeling.
2. Voer in het venster **Overzicht van verkoopuitstel** in het veld **Saldo per** de datum in tot wanneer u uitgestelde inkomsten wilt zien.
3. Kies de knop **Voorbeeld**.

## <a name="see-also"></a>Zie ook
[Financiën](finance.md)  
[Financiën instellen](finance-setup-finance.md)  
[Werken met diversendagboeken](ui-work-general-journals.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


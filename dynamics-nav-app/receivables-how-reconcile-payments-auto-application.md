---
title: "Procedure: Betalingen reconciliëren met automatische vereffening"
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
ms.openlocfilehash: bde263424bb8e5b60d2c9a139ddc8bfef0a90062
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-reconcile-payments-using-automatic-application"></a>Procedure: Betalingen reconciliëren met automatische vereffening
In het venster **Dagboek betalingsreconciliatie** worden inkomende of uitgaande betalingen opgegeven die als transacties zijn vastgelegd op uw online bankrekening en die u kunt vereffenen met de gerelateerde openstaande, klant-, leveranciers- en bankrekeningposten. De dagboekregels worden ingevuld door een bankafschrift als een bankfeed of bestand te importeren.

Een betalingsreconciliatiedagboek is gerelateerd aan één bankrekening in Dynamics NAV waarmee de online bankrekening wordt weergegeven waarin de betalingstransacties worden vastgelegd. Eventuele open bankrekeningposten die gerelateerd zijn aan de vereffende klant- of leveranciersposten, worden gesloten wanneer u de actie **Betalingen boeken en bankrekening reconciliëren** kiest. Dit betekent dat de bankrekening automatisch wordt gereconcilieerd voor betalingen die u met het dagboek boekt.

Als u bankafschriften als bankfeeds wilt importeren, moet u eerst de service Envestnet Yodlee Bank Feeds instellen en vervolgens de bankrekening aan de gerelateerde online bankrekening koppelen. Het dagboek van de betalingreconciliatie detecteert vervolgens automatisch bankfeeds wanneer u de actie **Banktransacties importeren** kiest. Bovendien kunt u een bankrekening zo instellen dat automatisch elk uur nieuwe bankafschriftfeeds worden geïmporteerd. Transacties voor betalingen die reeds zijn geboekt als vereffend en/of gereconcilieerd worden niet geïmporteerd. Zie voor meer informatie [Procedure: De feedservice van de Envestnet Yodlee Bank instellen](bank-how-setup-bank-statement-service.md).

**Opmerking**: de Envestnet Yodlee Bank Feeds-service of de bankfeedservice van een andere provider is mogelijk niet beschikbaar in uw systeem. Neem contact op met uw Microsoft-partner als u een bankfeedservice wilt gebruiken om bankafschriften te importeren.

Met de actie **Tekst afstemmen op rekening** kunt u toewijzingen instellen tussen tekst op betalingen en specifieke debet-, credit- en tegenrekeningen zodat dergelijke betalingen worden geboekt naar de opgegeven rekeningen wanneer u het betalingsreconciliatiedagboek boekt. Zie stap 9. Zie [Procedure: Tekst op herhalende betalingen aan rekeningen toewijzen voor automatisch reconciliëren](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md) voor meer informatie.

Er bestaat vergelijkbare functionaliteit om te grote bedragen op de dagboekregels voor betalingreconciliatie op ad-hocbasis te reconciliëren. Zie [Procedure: Betalingen reconciliëren die niet kunnen worden vereffend](receivables-how-reconcile-payments-cannot-apply-auto.md) voor meer informatie.

U gebruikt de functie **Automatisch vereffenen** automatisch wanneer u een bankbestand of -feed met betalingstransacties importeert of wanneer u de functie activeert, om betalingen te vereffenen met de gerelateerde openstaande posten op basis van een afstemming van gegevens op een dagboekregel met gegevens in een of meer openstaande posten.

Op dagboekregels waar een betaling automatisch is vereffend met een of meer openstaande posten, heeft het veld **Zekerheid afstemming** een waarde tussen Laag en Hoog om de kwaliteit aan te geven van de gegevensafstemming waarop de voorgestelde betalingsvereffening is gebaseerd. Bovendien wordt in de velden **Rekeningsoort** en **Rekeningnr.** informatie ingevuld over de klant of leverancier met wie de betaling wordt vereffend. Als u geen tekst-naar-rekening toewijzing hebt ingesteld, kan de automatische vereffening leiden tot de afstemmingszekerheidswaarde **Hoog - Tekst-aan-rekening toewijzing**.

Voor elke dagboekregel in het venster **Dagboek betalingsreconciliatie** kunt u het venster **Betalingsvereffening** openen om alle openstaande kandidaatposten voor de betaling te zien en gedetailleerde informatie voor elke post weer te geven over de gegevensafstemming waarop een betalingsvereffening wordt gebaseerd. Hier kunt u handmatig betalingen vereffenen of betalingen die automatisch met een verkeerde post zijn vereffend, opnieuw vereffenen. Zie [Procedure: Betalingen controleren of vereffenen na automatische vereffening](receivables-how-review-apply-payments-auto-application.md) voor meer informatie.

**Opmerking**: u kunt het importeren van banktransacties starten op het moment dat u het venster **Dagboek betalingsreconciliatie** opent voor een bestaand betalingsreconciliatiedagboek in het venster **Betalingsreconciliatiedagboeken**. In de volgende procedure wordt beschreven hoe u banktransacties importeert in het venster **Dagboek betalingsreconciliatie** nadat u een nieuw dagboek hebt gemaakt.

## <a name="to-reconcile-payments-using-automatic-application"></a>Betalingen reconciliëren met automatische vereffening
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Betalingsreconciliatiedagboeken** in en kies vervolgens de gerelateerde koppeling.
2. Als u in een nieuw betalingsreconciliatiedagboek wilt werken, kiest u de actie **Nieuw dagboek**.
3. Selecteer in het venster **Bankrekeninglijst betaling** de bankrekening waarvoor u betalingen wilt vereffenen en kies vervolgens de knop **OK**.
Het venster **Dagboek betalingsreconciliatie** wordt geopend en is voorbereid op de geselecteerde bankrekening.
4. Kies de actie **Banktransacties importeren**.
Als de bankrekening voor het geselecteerde dagboek niet is ingesteld voor het importeren van banktransacties, wordt een dialoogvenster geopend om u te helpen de relevante velden in te vullen.
5. Selecteer in het venster **Te importeren bestand selecteren** het bestand dat banktransacties voor betalingen bevat die u wilt reconciliëren, en kies vervolgens de knop **Openen**.  
6. Als de bankafschriftservice is ingeschakeld, wordt in het venster **Bankafschriftfilter** dat automatisch wordt geopend, het datuminterval opgegeven voor de bankafschriften die moeten worden geïmporteerd.

    Het venster **Dagboek betalingsreconciliatie** wordt gevuld met regels voor betalingen die banktransacties in het bankafschrift vertegenwoordigen.

    Op regels voor betalingen die automatisch zijn vereffend met de gerelateerde openstaande posten ervan, heeft het veld **Zekerheid afstemming** een waarde tussen **Laag** en **Hoog** om de kwaliteit aan te geven van de gegevensafstemming waarop de voorgestelde betalingsvereffening is gebaseerd. Bovendien wordt in de velden **Rekeningsoort** en **Rekeningnr.** informatie ingevuld over de klant of leverancier met wie de betaling wordt vereffend.
7. Selecteer een dagboekregel en kies vervolgens de actie **Handmatig afstemmen** om de betaling handmatig te bekijken, opnieuw te vereffenen of te vereffenen in het venster **Betalingsvereffening**. Zie [Procedure: Betalingen controleren of vereffenen na automatische vereffening](receivables-how-review-apply-payments-auto-application.md) voor meer informatie.

    Als u klaar bent met de handmatige vereffening, bevat het veld **Zekerheid afstemming** op de dagboekregel die u handmatig hebt verwerkt, **Goedgekeurd**.
8. Selecteer een niet-vereffende dagboekregel voor een periodieke ontvangst of periodieke kosten, zoals een aankoop van autobenzine, en kies vervolgens op het tabblad Start in de groep Controleren de optie Tekst afstemmen op rekening. Zie [Procedure: Tekst op herhalende betalingen aan rekeningen toewijzen voor automatisch reconciliëren](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md) voor meer informatie
9. Wanneer u de toewijzing van betalingstekst aan rekeningen hebt voltooid, kiest u de actie **Handmatig vereffenen**.
10. Wanneer u tevreden bent dat alle betalingen op de dagboekregels correct worden vereffend of zijn ingesteld op direct boeken, kiest u de actie **Boeken**.

Als u het dagboek van de betalingsreconciliatie boekt, worden de vereffende openstaande-postennota's gesloten en worden de gerelateerde klant-, leverancier- of grootboekrekeningen bijgewerkt. Voor betalingen op dagboekregels die zijn gebaseerd op tekst-aan-rekening toewijzing, worden de opgegeven klant-, leveranciers- en grootboekrekeningen bijgewerkt. Voor alle dagboekregels worden bankposten gemaakt. Als u de actie **Betalingen boeken en bankrekening reconciliëren** kiest, worden eventuele open bankrekeningposten gesloten die zijn gerelateerd aan de vereffende klant- of leveranciersposten. Dit betekent dat de bankrekening automatisch wordt gereconcilieerd voor betalingen die u met het dagboek boekt.

U kunt de waarde in het veld **Saldo op bankrekening na boeking** met de waarde in het veld **Eindsaldo afschrift** vergelijken om te traceren wanneer de bankrekening wordt gereconcilieerd op basis van betalingen die u boekt.

**Opmerking**: als u de bankrekening van het venster **Dagboek betalingsreconciliatie** niet wilt reconciliëren, moet u het venster **Bankreconciliatie** gebruiken. Zie [Procedure: Bankrekeningen apart reconciliëren](bank-how-reconcile-bank-accounts-separately.md) voor meer informatie.

## <a name="see-also"></a>Zie ook
[Tegoeden beheren](receivables-manage-receivables.md)  
[Verkoop beheren](sales-manage-sales.md)


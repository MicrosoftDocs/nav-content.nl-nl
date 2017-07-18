---
title: 'Procedure: Betalingen naar een bankbestand exporteren'
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
ms.openlocfilehash: 09bdf56b3d5e76b12d868091e89232ce9c08e215
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-export-payments-to-a-bank-file"></a>Procedure: Betalingen naar een bankbestand exporteren
Wanneer u klaar bent om betalingen te doen naar uw leveranciers met behulp van het venster **Betalingsdagboek**, kunt u een bestand met de betalingsgegevens op de dagboekregels exporteren. Vervolgens kunt u het bestand uploaden naar uw elektronische banksite voor verwerking van de verwante overboekingen.

In de algemene versie van Dynamics NAV wordt een algemene provider van services ingesteld en verbonden die bankgegevens converteert naar een bestandsindeling die uw bank vereist.

**Opmerking**: voordat u een betalingsdagboek kunt exporteren, moet u exporteren inschakelen in de gerelateerde dagboekbatch. Bovendien moeten uw bankrekening en die van de leverancier zijn ingesteld voor elektronische betaling. Zie voor meer informatie [Procedure: De conversieservice bankgegevens instellen](bank-how-setup-bank-data-conversion-service.md).

U gebruikt het venster **Krediettransferregisters** om de betalingsbestanden weer te geven die vanuit het betalingsdagboek zijn geëxporteerd. Vanuit dit venster kunt u ook betalingsbestanden opnieuw exporteren, in het geval van technische fouten of bestandswijzigingen.

## <a name="to-export-payments-to-a-bank-file"></a>Betalingen naar een bankbestand exporteren
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Betalingsdagboeken** in en kies vervolgens de gerelateerde koppeling.
2. Vul betalingsdagboekregels in, bijvoorbeeld met behulp van de functie **Leveranciersbetalingen voorstellen**. Zie voor meer informatie [Procedure: Leveranciersbetalingen voorstellen](payables-how-suggest-vendor-payments.md).  
3. Wanneer u alle betalingsdagboekregels hebt voltooid, kiest u **Betaling naar bestand exporteren**.

    Eventuele foutmeldingen worden weergegeven in het feitenblok **Fouten betalingsbestand**, waar u ook een foutbericht kunt kiezen om gedetailleerde gegevens te bekijken. U moet alle fouten oplossen voordat het betalingsbestand kan worden geëxporteerd.

    **Tip**: wanneer u de functie voor conversie van bankgegevens gebruikt, wordt een algemeen foutbericht weergegeven met de melding dat het bankrekeningnummer niet de lengte heeft die uw bank vereist. Om de fout te voorkomen of op te lossen moet u de waarde in het veld **IBAN** in het venster **Bankrekeningkaart** verwijderen en vervolgens in het veld **Bankrekeningnr.** een bankrekeningnummer invoeren in de indeling die uw bank vereist.
4. Geef in het venster **Opslaan als** de locatie op waar het bestand naartoe wordt geëxporteerd en kies vervolgens **Opslaan**.

Het bankbetalingsbestand wordt geëxporteerd naar de locatie die u opgeeft, en u kunt doorgaan met uploaden naar uw elektronische bankrekening en de werkelijke betalingen doen.

Wanneer u bevestiging ontvangt dat de betalingen met succes zijn verwerkt in de bank, kunt u de geëxporteerde betalingsdagboekregels boeken.

## <a name="to-plan-when-to-post-exported-payments"></a>Plannen wanneer geëxporteerde betalingen worden geboekt
Als u geen betalingsdagboekregel voor een geëxporteerde betaling wilt boeken, bijvoorbeeld omdat u op bevestiging wacht dat de transactie door de bank is verwerkt, kunt u eenvoudig de dagboekregel verwijderen. Wanneer u later een betalingsdagboekregel maakt om het restbedrag op de factuur te betalen, bevat het veld **Tot. geëxporteerd bedrag** hoeveel van het betalingsbedrag al is geëxporteerd. U kunt ook gedetailleerde gegevens vinden over het geëxporteerde totaal door de knop **Krediettransferregisterposten** te kiezen om details over geëxporteerde betalingsbestanden te bekijken.

Als u een proces volgt waarbij u geen betalingen boekt totdat u bevestiging hebt dat ze zijn verwerkt in de bank, kunt u dit op twee manieren bepalen.

* U kunt in een betalingsdagboek met voorgestelde betalingsregels sorteren op de kolom **Naar betalingsbestand geëxporteerd** of **Tot. geëxporteerd bedrag** en vervolgens betalingsvoorstellen verwijderen voor openstaande facturen waarvoor al betalingen zijn verricht en waarvoor u geen betalingen meer wilt verrichten.
* In het venster **Leveranciersbetalingen voorstellen**, waar u ook opgeeft welke betalingen in het betalingsdagboek worden ingevoegd, kunt u het selectievakje **Geëxporteerde betalingen overslaan** inschakelen als u geen dagboekregels wilt invoegen voor betalingen die al zijn geëxporteerd.

Als u informatie over geëxporteerde gegevens wilt bekijken, kiest u de actie **Historie betalingsexport**.

## <a name="to-re-export-payments-to-a-bank-file"></a>Betalingen naar een bankbestand opnieuw exporteren
U kunt betalingsbestanden opnieuw exporteren vanuit het venster **Krediettransferregisters**. Voordat u betalingsdagboekregels verwijdert of boekt, kunt u het betalingsbestand ook opnieuw exporteren vanuit het venster **Betalingsdagboek** door het nogmaals te importeren.

Als u betalingsdagboekregels hebt verwijderd of geboekt nadat u deze hebt geëxporteerd, kunt u hetzelfde betalingsbestand opnieuw exporteren vanuit het venster **Krediettransferregisters**. Selecteer de regel voor de batch kredietoverboekingen die u opnieuw wilt exporteren, en gebruik vervolgens de actie **Betalingen opnieuw exporteren naar bestand**.

## <a name="see-also"></a>Zie ook
[Schulden](payables-manage-payables.md)  
[Inkoop beheren](purchasing-manage-purchasing.md)  
[Inkoop instellen](purchasing-setup-purchasing.md)


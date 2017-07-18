---
title: 'Procedure: Betalingen na automatische vereffening handmatig controleren of vereffenen'
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
ms.openlocfilehash: 556a0f74a7407d247008e2d74420803123056eff
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-review-or-apply-payments-manually-after-automatic-application"></a>Procedure: Betalingen na automatische vereffening handmatig controleren of vereffenen
Voor elke dagboekregel die een betaling vertegenwoordigt in het venster **Dagboek betalingsreconciliatie** kunt u het venster **Betalingsvereffening** openen om alle openstaande kandidaatposten voor de betaling te zien en gedetailleerde informatie voor elke post weer te geven over de gegevensafstemming waarop een betalingsvereffening wordt gebaseerd. Hier kunt u handmatig betalingen vereffenen of betalingen die automatisch met een verkeerde post zijn vereffend, opnieuw vereffenen. Zie [Procedure: Betalingen reconciliëren met automatische vereffening](receivables-how-reconcile-payments-auto-application.md) voor meer informatie over automatische vereffening.

**Belangrijk**: wanneer de bankrekening waarvoor u betalingen reconcilieert, is ingesteld voor de lokale valuta, bevat het venster **Betalingsvereffening** alle openstaande posten in de lokale valuta, inclusief openstaande posten voor documenten die oorspronkelijk in vreemde valuta's zijn gefactureerd. Betalingen die worden vereffend met posten met omgezette valuta's, kunnen daarom worden geboekt met andere bedragen dan op het oorspronkelijke document, vanwege de mogelijk verschillende wisselkoersen die respectievelijk worden gebruikt door de bank en Dynamics NAV.

Daarom is het raadzaam dat u controleert op vreemde valutacodes in het veld **Valutacode** in het venster **Betalingsvereffening** om te zien of vereffeningen zijn gebaseerd op omgezette valuta's. Als u het oorspronkelijke documentbedrag in de vreemde valuta wilt controleren en als u de gebruikte wisselkoers wilt zien, kiest u het veld **Vereffenen met postnr.** en kiest u vervolgens in het snelmenu de detailknop om het venster **Klantposten** of **Leveranciersposten** te openen.

Eventuele vereiste winst-en-verliescorrectie vanwege valutakoersen wordt niet automatisch afgehandeld door Dynamics NAV.

**Opmerking**: u kunt geen posten vereffenen met een ander teken dan het teken op de betaling. Als u bijvoorbeeld zowel een creditnota met een negatief teken als de gerelateerde factuur met een positief teken wilt afsluiten, moet u eerst de creditnota vereffenen met de factuur, en vervolgens de betaling vereffenen met de factuur met het verminderde restbedrag.

**Waarschuwing**: als u contantkortingen gebruikt en als de betaaldatum vóór de vervaldatum van de betaling is, wordt het veld **Restbedrag incl. korting** in het venster **Betalingsvereffening** gebruikt voor afstemming. Anders wordt de waarde in het veld **Restbedrag** gebruikt. Als de betaling met een gekort bedrag na de vervaldatum is verricht, of als het volledige bedrag is betaald maar een korting is verleend, wordt het bedrag niet afgestemd.

**Opmerking**: u kunt een betaling slechts met één rekening vereffenen. Als u de vereffening over meerdere openstaande posten wilt splitsen, bijvoorbeeld om een betaling ineens te vereffenen, moeten de openstaande posten voor dezelfde rekening zijn. Zie voor meer informatie stap 7 en 8 in de procedure in dit onderwerp.

## <a name="to-review-or-apply-payments-after-automatic-application"></a>Betalingen na automatische vereffening controleren of vereffenen
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Betalingsreconciliatiedagboeken** in en kies vervolgens de gerelateerde koppeling.
2. Open het betalingreconciliatiedagboek voor een bankrekening waarvoor u betalingen wilt reconciliëren. Zie voor meer informatie [Procedure: Betalingen reconciliëren met automatische vereffening](receivables-how-reconcile-payments-auto-application.md).
3. In het venster **Dagboek betalingsreconciliatie** selecteert u een betaling die u wilt controleren of handmatig vereffenen met een of meer openstaande posten. Vervolgens kiest u de actie **Handmatig vereffenen**.
4. Schakel het selectievakje **Vereffend** in op de regel voor de openstaande post waarmee u de betaling wilt vereffenen.
5. Het betalingsbedrag, dat ook in het veld **Transactiebedrag** in het venster **Betalingsvereffening** wordt weergegeven, wordt ingevoegd in het veld **Vereffend bedrag**, maar u kunt het veld wijzigen, bijvoorbeeld als u het bedrag met meerdere openstaande posten wilt vereffenen.
6. Als u een deel van het betaalde bedrag met een andere openstaande post voor de rekening wilt vereffenen, bijvoorbeeld om een bedrag ineens te vereffenen, schakelt u het selectievakje **Vereffend** voor de regel in. Het vereffende bedrag wordt automatisch afgetrokken van het transactiebedrag, in overeenstemming met de distributie over de twee openstaande posten.
7. Als u een deel van een betaling wilt vereffenen met een of meer openstaande posten die niet in de database voorkomen, maakt u een nieuwe regel onder de regel voor dezelfde rekening. In het veld **Vereffend bedrag** voert u het te vereffenen bedrag op de nieuwe regel in en past u het veld **Vereffend bedrag** op de bestaande regel aan.
8. Herhaal stap 5, 6 of 7 voor andere openstaande posten waarmee u een deel van het betalingsbedrag of het gehele bedrag wilt vereffenen.
9. Wanneer u een betalingsvereffening hebt gecontroleerd of handmatig hebt vereffend met een of meer openstaande posten, kiest u de actie **Vereffening accepteren**.

Het venster **Betalingsvereffening** wordt gesloten en in het venster **Dagboek betalingsreconciliatie** verandert de waarde in het veld **Zekerheid afstemming** in **Goedgekeurd** om aan te geven dat u de betaling hebt gecontroleerd of handmatig hebt vereffend.

## <a name="see-also"></a>Zie ook
[Tegoeden beheren](receivables-manage-receivables.md)  
[Verkoop beheren](sales-manage-sales.md)


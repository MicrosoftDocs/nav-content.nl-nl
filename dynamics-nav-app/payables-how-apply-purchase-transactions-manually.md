---
title: 'Procedure: Leveranciersbetalingen handmatig vereffenen'
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
ms.openlocfilehash: d3aaafc9ac3dcfd1fba3802b1158bde890e09110
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-apply-vendor-payments-manually"></a>Procedure: Leveranciersbetalingen handmatig vereffenen

Wanneer u een betaling of terugbetaling van een leverancier ontvangt, moet u beslissen of u de betaling of terugbetaling vereffent met een of meer openstaande posten. U kunt het exacte bedrag opgeven waarmee u de betalingsontvangst of terugbetaling wilt vereffenen, en de leveranciersposten vervolgens slechts gedeeltelijk vereffenen. U moet alle leveranciersposten vereffenen om correcte leverancierstatistieken en -rapporten te verkrijgen van de rekeningoverzichten en rentefacturen.

**Opmerking**: leveranciers geven soms een terugbetaling in plaats van een creditnota die als tegenrekening dient voor toekomstige facturen, met name wanneer u artikelen terugzendt die u al hebt betaald of wanneer u te veel hebt betaald voor een factuur.

U kunt als volgt leveranciersposten vereffenen op drie verschillende manieren:

- Door gegevens in bepaalde vensters in te voeren, zoals het venster **Betalingsdagboek** en het venster **Dagboek betalingsreconciliatie**.
- Vanuit inkoopcreditnotadocumenten.
- Vanuit leveranciersposten, nadat inkoopdocumenten zijn geboekt maar nog niet vereffend.

**Opmerking**: als het veld **Vereffeningsmethode** op de leverancierskaart **Saldo** bevat, kunnen betalingen handmatig worden vereffend met de oudste openstaande creditpost, als u niet handmatig opgeeft met welke post moet worden vereffend. Als de vereffeningsmethode voor een klant **Handmatig** is, moet u posten handmatig vereffenen.

U kunt leveranciersbetalingen handmatig op de gerelateerde inkoopdocumenten toepassen wanneer u de betalingen boekt in het venster **Betalingsdagboek**. Zie voor meer informatie over het invullen van het betalingsdagboek [Procedure: Betalingen doen](payables-make-payments.md).

U kunt ook leveranciersbetalingen en klantbetalingen vereffenen nadat de betalingen worden weergegeven als negatieve banktransacties bij uw bank. In het venster **Dagboek betalingsreconciliatie** kunt u functies voor het importeren van bankafschriften, automatische vereffening en bankrekeningvereffening gebruiken. Zie voor meer informatie [Betalingen vereffenen met automatische vereffening](receivables-how-reconcile-payments-auto-application.md).

## <a name="to-apply-a-payment-to-a-single-or-multiple-vendor-ledger-entries"></a>Een betaling vereffenen met een of meer leveranciersposten
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Betalingsdagboek** in en kies vervolgens de gerelateerde koppeling.
2. Voer in het venster **Betalingsdagboek** op de eerste dagboekregel de betreffende gegevens over de betalingspost in.
3. Eén leverancierspost vereffenen:
4. Kies in het veld **Vereffeningsnr.** het veld om het venster **Leveranciersposten vereffenen** te openen.
5. Selecteer in het venster **Leveranciersposten vereffenen** de post waarmee de betaling moet worden vereffend.
6. Voer op de regel in het veld **Te vereffenen bedrag** het bedrag in waarmee u de post wilt vereffenen.
7. Of meerdere leveranciersposten vereffenen:
8. Kies de actie **Posten vereffenen**.
9. In het venster **Leveranciersposten vereffenen** selecteert u de regels met de posten die u met de betaling wilt vereffenen.
10. Kies de actie **Id toekennen**.  
11. Voer op elke regel in het veld **Te vereffenen bedrag** het bedrag in waarmee u de afzonderlijke post wilt vereffenen.

    Als u geen bedrag opgeeft, wordt automatisch het maximumbedrag gebruikt. Onder aan het venster **Leveranciersposten vereffenen** ziet u het bedrag in het veld Vereffend bedrag en kunt u controleren of de vereffening sluitend is.
12. Kies de knop **Ok**.
13. Kies de actie **Boeken** om het betalingsdagboek te boeken.

## <a name="to-apply-a-credit-memo-to-a-single-or-multiple-vendor-ledger-entries"></a>Een creditnota vereffenen met een of meer leveranciersposten:
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Inkoopcreditnota** in en kies vervolgens de gerelateerde koppeling.
2. Open de creditnota die u wilt vereffenen.
3. Voer de betreffende gegevens in de kop in.
4. Eén leverancierspost vereffenen:
5. Kies op het sneltabblad **Vereffening** in het veld **Vereffeningsnr.** de post waarmee de credit moet worden vereffend.
6. Voer op de regel in het veld **Te vereffenen bedrag** het bedrag in waarmee u de post wilt vereffenen.
7. Of meerdere leveranciersposten vereffenen:
8. Kies de actie **Posten vereffenen**.
9. Selecteer de regels met de posten waarmee u de creditnota wilt vereffenen.
10. Kies de actie **Id toekennen**.  
11. Voer op elke regel in het veld **Te vereffenen bedrag** het bedrag in waarmee u de afzonderlijke post wilt vereffenen.

    Als u geen bedrag opgeeft, wordt automatisch het maximumbedrag gebruikt. Onder aan het venster **Leveranciersposten vereffenen** ziet u het bedrag in het veld **Vereffend bedrag** en kunt u controleren of de vereffening sluitend is.
12. Kies de knop **Ok**.  
Het venster **Inkoopcreditnota** bevat de post die u hebt geselecteerd in het veld **Vereffeningssoort** en het **Vereffeningsnr.** in. Het venster bevat ook het bedrag van de creditnota dat moet worden geboekt, geherwaardeerd voor de mogelijke contantkortingen.
13. Kies de knop **Boeken** om de inkoopcreditnota te boeken.

## <a name="to-apply-posted-vendor-ledger-entries"></a>Geboekte leveranciersposten vereffenen

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Leveranciers** in en kies vervolgens de gerelateerde koppeling.
2. Open de betreffende leverancier met posten die reeds zijn geboekt.
3. Kies de actie **Posten** en kies vervolgens de actie **Posten vereffenen**.
4. In het venster **Leveranciersposten vereffenen** ziet u de openstaande posten voor de leverancier.
5. Selecteer de regel met de post die wordt vereffend.
6. Kies de actie **Id toekennen**.
7. Het veld **Vereffenings-id** bevat drie sterretjes als u in een systeem met één gebruiker werkt, of bevat uw gebruikers-id als u in een systeem met meerdere gebruikers werkt.  
8. Voer op elke regel in het veld **Te vereffenen bedrag** het bedrag in waarmee u de afzonderlijke post wilt vereffenen.

    Als u geen bedrag opgeeft, wordt automatisch het maximumbedrag gebruikt. U ziet het bedrag in het veld **Vereffend bedrag**, onder aan het venster **Leveranciersposten vereffenen**.
9. Kies de actie **Vereffening boeken**.  
Het venster **Vereffening boeken** verschijnt met het documentnummer van de vereffeningspost en de boekingsdatum van de post met de meest recente boekingsdatum.
10. Kies de knop **OK** om de vereffening te boeken.

## <a name="to-apply-vendor-ledger-entries-in-different-currencies-to-one-another"></a>Leveranciersposten in verschillende valuta's onderling vereffenen
Als u van een leverancier koopt in de ene valuta en betaalt in de andere, kunt u de factuur toch met de betaling vereffenen.

Als u een post (Post 1) in de ene valuta vereffent met een post (Post 2) in een andere valuta, wordt de boekingsdatum van Post 1 gebruikt om de juiste wisselkoers te bepalen voor de conversie van de bedragen van Post 2. De juiste wisselkoers wordt opgezocht in het venster **Valutawisselkoersen**.

Het vereffenen van leveranciersposten in verschillende valuta's moet zijn ingeschakeld. Zie voor meer informatie [Procedure: Vereffening van posten in verschillende valuta's inschakelen](finance-setup-how-enable-application-ledger-entries-different-currencies.md)

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Betalingsdagboek** in en kies de gerelateerde koppeling.
2. Open het journaal dat u wilt gebruiken en vul de eerste lege dagboekregel in met een valutacode.
3. Kies de actie **Posten vereffenen**.
4. Selecteer de regel met de post waarmee u de post in het betalingsdagboek wilt vereffenen, kies de actie **Id toekennen** en selecteer vervolgens de post waarmee u wilt vereffenen.
5. Klik op **OK** om terug te gaan naar het betalingsdagboek.
6. Boek het betalingsdagboek.

**Belangrijk**: wanneer u posten in verschillende valuta's onderling vereffent, worden de posten automatisch omgezet in de lokale valuta. Zelfs bij een vaste wisselkoers tussen de twee relevante valuta's, bijvoorbeeld USD en EUR, kan er een klein verschilbedrag ontstaan wanneer bedragen in de vreemde valuta worden omgezet naar de lokale valuta. Deze kleine verschilbedragen worden als winst- of verliesbedragen geboekt naar de rekening die u hebt opgegeven in de velden **Gereal. koerswinstrekening** of **Gereal. koersverliesrekening** van het venster **Valuta's**. Het veld **Bedrag (lokale valuta)** wordt ook aangepast in de relevante leveranciersposten.

## <a name="to-unapply-an-application-of-vendor-entries"></a>De vereffening van leveranciersposten ongedaan maken
Als u een verkeerde vereffening ongedaan maakt, worden er stornoposten gemaakt die identiek zijn aan de oorspronkelijke post maar met een tegengesteld teken in het bedragveld, en geboekt voor alle posten, inclusief alle GB-boekingen die uit de vereffening voortkomen zoals contantkortingen en valutawinst- en verlies. De posten de waren afgesloten door de toepassing worden heropend.

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Leveranciers** in en kies vervolgens de gerelateerde koppeling.
2. Open de desbetreffende leverancierskaart.
3. Kies de actie **Posten**.
4. Selecteer de betreffende post en kies de actie **Vereffening posten ongedaan maken**.
5. Of kies de actie **Gedetailleerde post**.
6. Selecteer de vereffeningspost en kies de actie **Vereffening posten ongedaan maken**.
7. Vul de velden in de kop in en klik vervolgens op de knop **Vereffening ongedaan maken**.

**Belangrijk**: als een post is vereffend door meer dan één vereffeningspost, moet u de vereffening van de laatste vereffeningspost het eerst ongedaan maken.

## <a name="see-also"></a>Zie ook
[Schulden](payables-manage-payables.md)  
[Inkoop beheren](purchasing-manage-purchasing.md)


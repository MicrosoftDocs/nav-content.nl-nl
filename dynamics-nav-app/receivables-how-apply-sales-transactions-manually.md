---
title: "Procedure: Klantbetalingen handmatig reconciliëren"
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
ms.openlocfilehash: de0c94386ad5a0bbfba5cc0516fa7faa5cdcc0b4
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-reconcile-customer-payments-manually"></a>Procedure: Klantbetalingen handmatig reconciliëren
Wanneer u een bedrag ontvangt van een klant of een terugbetaling aan een klant doet, moet u bedenken of de ontvangst of betaling moet worden vereffend met een of meer openstaande debet- of creditposten. U kunt het exacte bedrag opgeven dat u wilt toepassen. U wilt misschien slechts een gedeelte van de betaling toepassen en de klantenposten dus slechts gedeeltelijk vereffenen. Wel moet u op een bepaald moment alle klantenposten afsluiten (vereffenen) om ervoor te zorgen dat de klantstatistieken en de afgedrukte rekeningafschriften en rentefacturen kloppen.

U kunt klantposten vereffenen op drie verschillende manieren:

- Door gegevens in bepaalde vensters in te voeren, zoals het venster **Ontvangstendagboek** en het venster **Dagboek betalingsreconciliatie**.
- Vanuit verkoopcreditnotadocumenten.
- Vanuit klantposten worden after sales-documenten geboekt, maar niet vereffend.

**Opmerking**: als het veld **Vereffeningsmethode** op de klantenkaart **Saldo** bevat, kunnen betalingen handmatig worden vereffend met de oudste openstaande creditpost, als u niet handmatig opgeeft met welke post moet worden vereffend. Als de vereffeningsmethode voor een klant **Handmatig** is, moet u posten handmatig vereffenen.

In het venster **Ontvangstendagboek** kunt u klantbetalingen handmatig vereffenen. Een ontvangstendagboek is een soort algemeen dagboek, waarmee u transacties boekt naar grootboek-, bank-, klanten-, leveranciers- en vaste-activumrekeningen. U kunt de betaling met een of meer debetposten vereffenen wanneer u de betaling boekt of u kunt deze later vanuit de geboekte posten vereffenen.

U kunt klantbetalingen en leveranciersbetalingen in het venster **Dagboek betalingsreconciliatie** vereffenen met functies voor import van bankafschriften, automatische vereffening en bankrekeningreconciliatie. Zie voor meer informatie [Betalingen vereffenen met automatische vereffening](receivables-how-reconcile-payments-auto-application.md). U kunt klantbetalingen ook reconciliëren op basis van een lijst met onbetaalde verkoopdocumenten in het venster **Betalingsregistratie**. Zie [Procedure: Klantbetalingen van een lijst met onbetaalde verkoopdocumenten reconciliëren](receivables-how-reconcile-customer-payments-list-unpaid-sales-documents.md) voor meer informatie.

## <a name="to-fill-and-post-a-cash-receipt-journal"></a>Een ontvangstendagboek invullen en boeken
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Ontvangstendagboek** in en kies vervolgens de gerelateerde koppeling.
2. Selecteer in het veld **Batchnaam** de juiste batch.
3. Vul het veld **Boekingsdatum** in.  
4. Selecteer **Betaling** in het veld **Documentsoort**.

    Het veld **Documentnr.** wordt ingevuld met de nummerreeks die aan de batch is toegewezen.
5. Gebruik het veld **Extern documentnr.** als u een identificatie, bijvoorbeeld het chequenummer van de klant, wilt opslaan.
6. Selecteer **Klant** in het veld **Rekeningsoort** .
7. Selecteer in het veld **Rekeningnr.** selecteert u de relevante grootboekrekening.
8. Als u de vereffening tegelijkertijd met het dagboek wilt boeken, kunt u op een van de volgende manieren te werk gaan.
9. Selecteer in het veld **Tegenrekeningsoort** de optie **Grootboekrekening** voor contante betalingen en **Bankrekening** voor andere betalingen.
10. Selecteer in het veld **Tegenrekeningnr.** de kasrekening voor contante betalingen of de desbetreffende bankrekening voor andere betalingen.
11. Boek het dagboek.

## <a name="to-apply-a-payment-to-a-single-customer-ledger-entry"></a>Een betaling vereffenen met één klantenpost
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Ontvangstendagboek** in en kies de gerelateerde koppeling.
2. Geef op de eerste dagboekregel de betreffende gegevens op over de post die u wilt vereffenen.
3. Voer **Betaling** in het veld **Documentsoort** in.
4. Voer **Klant** in het veld **Rekeningsoort** in.
5. Voer **Bank** in het veld **Tegenrekeningsoort** in.
6. Kies in het veld **Vereffeningsnr.** selecteert u het veld om het venster **Klantposten vereffenen** te openen.
7. Selecteer in het venster **Klantposten vereffenen** de post waarmee de betaling moet worden vereffend.
8. Voer in het veld **Te vereffenen bedrag** het bedrag in waarmee u de post wilt vereffenen. Als u geen bedrag invoert, wordt automatisch het maximumbedrag gebruikt.

    Onder aan het venster **Klantposten vereffenen** kunt u het specifieke bedrag in het veld **Vereffend bedrag** zien en ook of de vereffening sluitend is.
9. Kies de knop **Ok**. In het venster **Ontvangstendagboek** ziet u nu de post die u hebt geselecteerd in het veld **Vereffeningssoort** en het veld **Vereffeningsnr.** in.
10. Boek het ontvangstendagboek.

## <a name="to-apply-a-payment-to-multiple-customer-ledger-entries"></a>Een betaling vereffenen met meerdere klantenposten
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Ontvangstendagboek** in en kies de gerelateerde koppeling.
2. Geef op de eerste dagboekregel de betreffende gegevens op over de post die u wilt vereffenen.
3. Voer **Betaling** in het veld **Documentsoort** in.
4. Voer **Klant** in het veld **Rekeningsoort** in.
5. Voer **Bank** in het veld **Tegenrekeningsoort** in.
6. Voer in het veld **Bedrag** de volledige betaling in als een negatief bedrag.
7. Kies de actie **Posten vereffenen** als u de betaling tijdens het boeken wilt vereffenen met meerdere klantposten.
8. Selecteer de regels met de posten die u met de vereffeningspost wilt vereffenen en kies de actie **Id toekennen** .
9. Voer op elke regel in het veld **Te vereffenen bedrag** het bedrag in waarmee u de afzonderlijke post wilt vereffenen. Als u geen bedrag invoert, wordt automatisch het maximumbedrag gebruikt.

    Onder aan het venster **Klantposten vereffenen** kunt u het specifieke bedrag in het veld **Vereffend bedrag** zien en ook of de vereffening sluitend is.
10. Kies de knop **Ok**.
11. Boek het ontvangstendagboek.

## <a name="to-apply-a-credit-memo-to-a-single-customer-ledger-entry"></a>Een creditnota vereffenen met één klantenpost
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Verkoopcreditnota's** in en kies vervolgens de gerelateerde koppeling.
2. Open de relevante verkoopcreditnota.
3. Als u de creditnota tijdens het boeken wilt vereffenen met één klantpost, selecteert u in het veld **Vereffeningsnr.** de post waarmee u de betaling wilt vereffenen.
4. Voer op de regel in het veld **Te vereffenen bedrag** het bedrag op waarmee u de post wilt vereffenen.

    Als u geen bedrag opgeeft, wordt automatisch het maximumbedrag gebruikt. Onder aan het venster **Klantposten vereffenen** kunt u het specifieke bedrag in het veld **Vereffend bedrag** zien en ook of de vereffening sluitend is.
5. Kies de knop **Ok**. In het venster **Verkoopcreditnota** ziet u nu de post die u hebt geselecteerd in het veld **Vereffeningssoort** en het veld **Vereffeningsnr.** in. En het bedrag van de creditnota dat moet worden geboekt, geherwaardeerd voor de mogelijke contantkortingen.
6. Boek de creditnota.

## <a name="to-apply-a-credit-memo-to-multiple-customer-ledger-entries"></a>Een creditnota vereffenen met meerdere klantenposten
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Verkoopcreditnota's** in en kies vervolgens de gerelateerde koppeling.
2. Open de relevante verkoopcreditnota.
3. Kies de actie **Posten vereffenen** als u de creditnota tijdens het boeken wilt vereffenen met meerdere klantposten.
4. Selecteer de regels met de posten die u met de vereffeningspost wilt vereffenen en kies de actie **Id toekennen** .
5. Voer op elke regel in het veld **Te vereffenen bedrag** het bedrag in waarmee u de afzonderlijke post wilt vereffenen. Als u geen bedrag invoert, wordt automatisch het maximumbedrag gebruikt.

  Onder aan het venster **Klantposten vereffenen** kunt u het specifieke bedrag in het veld **Vereffend bedrag** zien en ook of de vereffening sluitend is.
6. Kies de knop **Ok**. Het venster **Verkoopcreditnota** bevat nu het bedrag van de creditnota die moet worden geboekt, geherwaardeerd voor alle mogelijke contantkortingen.
7. Boek de creditnota.

## <a name="to-apply-posted-customer-ledger-entries"></a>Geboekte klantenposten vereffenen
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Klanten** in en kies vervolgens de gerelateerde koppeling.
2. Open de klantenkaart voor de klant met de posten die u wilt vereffenen.
3. Kies de actie **Posten** en selecteer de regel met de post die u als de vereffeningspost wilt gebruiken.
4. Kies de actie **Posten vereffenen**. Het venster **Klantposten vereffenen** wordt geopend met daarin de openstaande posten voor de klant.
5. Selecteer de regels met de posten die u met de vereffeningspost wilt vereffenen en kies de actie **Id toekennen** .
6. Voer voor elke regel in het veld **Te vereffenen bedrag** het bedrag in waarmee u de afzonderlijke post wilt vereffenen. Als u geen bedrag invoert, wordt automatisch het maximumbedrag gebruikt.

    U ziet het specifieke bedrag in het veld **Vereffend bedrag** onder aan het venster **Klantposten vereffenen**.
7. Kies de actie **Vereffening boeken**. Het venster **Vereffening boeken** verschijnt met het documentnummer van de vereffeningspost en de boekingsdatum van de post met de meest recente boekingsdatum.  
8. Kies de knop **OK** om de vereffening te boeken.

    Als de vereffening geboekt is en dit heeft tot resultaat gehad dat klantenposten zijn afgesloten, staat er geen vinkje meer bij deze grootboekposten in het veld **Open**.
9. Als u de posten wilt bekijken, kiest u in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voert u **Klanten** in en kiest u de gerelateerde koppeling Ga naar de kaart voor de relevante klant om de posten te zien.

In het overzicht met posten kunt u zien dat het selectievakje **Open** is uitgeschakeld op de regel met de post die volledig is vereffend.  

**Opmerking**: nadat u een post hebt geselecteerd in het venster **Klantposten vereffenen** of nadat u diverse posten hebt geselecteerd door de **Vereffenings-id** in te stellen, bevat het veld **Vereffend bedrag** op de dagboekregel de som van de resterende bedragen voor de geboekte posten die u hebt geselecteerd, tenzij het veld al een andere waarde bevat. Als u **Saldo** selecteert in het veld **Vereffeningsmethode** op de klantenkaart, wordt de betaling automatisch vereffend.

## <a name="to-apply-customer-ledger-entries-in-different-currencies-to-one-another"></a>Klantenposten in verschillende valuta's met elkaar vereffenen
Als u een artikel aan een klant verkoopt in een bepaalde valuta en een betaling in een andere valuta ontvangt, kunt u de betaling nog steeds vereffenen met de factuur.

Als u een post (Post 1) in de ene valuta vereffent met een post (Post 2) in een andere valuta, wordt de boekingsdatum van Post 1 gebruikt om de juiste wisselkoers te bepalen voor de conversie van de bedragen van Post 2. De juiste wisselkoers wordt opgezocht in het venster **Valutawisselkoersen**.

Het vereffenen van klantposten in verschillende valuta's moet zijn ingeschakeld. Zie [Procedure: Vereffening van posten in verschillende valuta's inschakelen](finance-setup-how-enable-application-ledger-entries-different-currencies.md) voor meer informatie.

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Ontvangstendagboek** in en kies de gerelateerde koppeling.
2. Open het gewenste dagboek en vul de eerste lege dagboekregel in met een valutacode.
3. Kies de actie **Posten vereffenen**.
4. Selecteer de regel met de post waarmee u de post in het ontvangstendagboek wilt vereffenen, kies de actie **Id toekennen** en selecteer vervolgens de post waarmee u wilt vereffenen.
5. Klik op de knop **OK** om terug te gaan naar het ontvangstendagboek.
6. Boek het verkoopdagboek.

**Belangrijk**: wanneer u posten in verschillende valuta's onderling vereffent, worden de posten automatisch omgezet in de lokale valuta. Zelfs bij een vaste wisselkoers tussen de twee relevante valuta's, bijvoorbeeld USD en EUR, kan er een klein verschilbedrag ontstaan wanneer bedragen in de vreemde valuta worden omgezet naar de lokale valuta. Deze kleine verschilbedragen worden als winst- of verliesbedragen geboekt naar de rekening die u hebt opgegeven in de velden **Gereal. koerswinstrekening** of **Gereal. koersverliesrekening** van het venster **Valuta's**. Het veld **Bedrag (lokale valuta)** wordt ook aangepast in de relevante leveranciersposten.

## <a name="to-unapply-an-application-of-customer-entries"></a>De vereffening van klantposten ongedaan maken
Als u een verkeerde vereffening ongedaan maakt, worden er stornoposten gemaakt die identiek zijn aan de oorspronkelijke post maar met een tegengesteld teken in het bedragveld, en geboekt voor alle posten, inclusief alle GB-boekingen die uit de vereffening voortkomen zoals contantkortingen en valutawinst- en verlies. De posten de waren afgesloten door de toepassing worden heropend.

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Klanten** in en kies vervolgens de gerelateerde koppeling.
2. Open de relevante klantenkaart.
3. Kies de actie **Posten**.
4. Selecteer de betreffende post en kies de actie **Vereffening posten ongedaan maken**.
5. Of kies de actie **Gedetailleerde post**.
6. Selecteer de vereffeningspost en kies de actie **Vereffening posten ongedaan maken**.
7. Vul de velden in de kop in en klik vervolgens op de knop **Vereffening ongedaan maken**.

**Belangrijk**: als een post is vereffend door meer dan één vereffeningspost, moet u de vereffening van de laatste vereffeningspost het eerst ongedaan maken.

## <a name="see-also"></a>Zie ook
[Tegoeden beheren](receivables-manage-receivables.md)  
[Verkoop beheren](sales-manage-sales.md)


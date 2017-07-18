---
title: "Procedure: Bankrekeningen apart reconciliëren"
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
ms.openlocfilehash: 8b05bc9d09fa1e1a7a01eb4816ffba727611b776
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-reconcile-bank-accounts-separately"></a>Procedure: Bankrekeningen apart reconciliëren
Als u bankrekeningen in Dynamics NAV wilt reconciliëren met afschriften die u van de bank hebt ontvangen, moet u eerst de regels vullen in het venster **Bankreconciliatie**.

**Opmerking**: u kunt bankrekeningen ook reconciliëren in het venster **Betalingsreconciliatiedagboek**. Eventuele open bankrekeningposten die gerelateerd zijn aan de vereffende klant- of leveranciersposten, worden gesloten wanneer u de actie **Betalingen boeken en bankrekening reconciliëren** kiest. Dit betekent dat de bankrekening automatisch wordt gereconcilieerd voor betalingen die u met het dagboek boekt. Zie voor meer informatie [Procedure: Betalingen reconciliëren met automatische vereffening](receivables-how-reconcile-payments-auto-application.md).

Als u de import van bankafschriften als bankfeeds wilt inschakelen, moet u eerst de feedservice van de Envestnet Yodlee Bank instellen en inschakelen en vervolgens uw bankrekeningen aan de gerelateerde online bankrekeningen koppelen. Zie voor meer informatie [Procedure: De feedservice van de Envestnet Yodlee Bank instellen](bank-how-setup-bank-statement-service.md).

**Opmerking**: de Envestnet Yodlee Bank Feeds-service of de bankfeedservice van een andere provider is mogelijk niet beschikbaar in uw systeem. Neem contact op met uw Microsoft-partner als u een bankfeedservice wilt gebruiken om bankafschriften te importeren.

De regels in het venster **Bankreconciliatie** zijn verdeeld in twee deelvensters. Het deelvenster **Bankafschriftregels** bevat geïmporteerde bankafschriften of posten met openstaande betalingen. Het deelvenster **Bankposten** bevat de posten op de bankrekening.

Het opzoeken en vereffenen van posten die moeten worden gereconcilieerd, wordt *afstemmen* genoemd. U kunt kiezen om afstemming automatisch uit te voeren via de functie **Automatisch afstemmen**. U kunt ook handmatig regels selecteren in beide deelvensters om elke bankafschriftregel te koppelen aan een of meer verwante bankposten, en vervolgens de functie **Handmatig afstemmen** gebruiken. Het selectievakje **Vereffend** is ingeschakeld op regels waar posten overeenkomen.

U kunt het deelvenster **Bankafschriftregels** in het venster **Bankreconciliatie** als volgt vullen:

* Automatisch, door de functie **Bankafschrift importeren** te gebruiken om de regels in te vullen overeenkomstig werkelijke bankafschriften op basis van een bestand dat door de bank wordt geleverd.
* Handmatig met de functie **Regels voorstellen** om de regels te vullen met posten voor facturen die openstaande betalingen hebben.

Wanneer de waarde in het veld **Totaalsaldo** in het deelvenster **Bankafschriftregels** gelijk is aan de waarde in het veld **Af te stemmen saldo** in het deelvenster **Bankposten**, kunt u de actie **Boeken** kiezen om de vereffende bankposten te vereffenen. Niet-vereffende bankposten blijven in het venster. Dit geeft aan dat betalingen die zijn verwerkt voor de bankrekening, niet worden weergegeven op het laatste bankafschrift of dat voor sommige betalingen cheques zijn ontvangen.

**Opmerking**: als bankafschriftregels op chequeposten betrekking hebben, kunt u de afstemfuncties niet gebruiken. In plaats hiervan moet u de actie **Posten vereffenen** kiezen en de relevante chequepost selecteren om de bankafschriftregel mee af te stemmen.

## <a name="to-fill-bank-reconciliation-lines-by-importing-a-bank-statement"></a>Bankreconciliatieregels vullen door een bankafschrift te importeren  
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Reconciliatie van bankrekening** in en kies vervolgens de gerelateerde koppeling.
2. Kies de actie **Nieuw**.
3. Selecteer in het veld **Bankrekeningnr.** de relevante bankrekening. De bankposten die bestaan voor de bankrekening, worden weergegeven in het deelvenster **Bankposten**.
4. Voer de datum van het rekeningoverzicht van de bank in het veld **Afschriftdatum** in.
5. Voer het saldo van het bankafschrift in het veld **Eindsaldo afschrift** in.
6. Als u een bankafschriftbestand hebt ingesteld, kiest u de actie **Bankafschrift importeren**.
7. Zoek het bestand en kies **Openen** om de banktransacties te importeren in de regels van het venster **Bankreconciliatie**.

## <a name="to-fill-bank-reconciliation-lines-with-the-suggest-lines-function"></a>Bankreconciliatieregels vullen met de functie Regels voorstellen
1. Kies in het venster **Bankreconciliatie** de actie **Regels voorstellen**.
2. Voer in het veld **Begindatum** de vroegste boekingsdatum in voor de posten waarop u de reconciliatie wilt uitvoeren.
3. Voer in het veld **Einddatum** de laatste boekingsdatum in voor de posten waarop u de reconciliatie wilt uitvoeren.
4. Schakel het selectievakje **Inclusief cheques** in om chequeposten voor te stellen in plaats van de corresponderende bankposten.
5. Kies de knop **Ok**.

## <a name="to-match-bank-statement-lines-with-bank-account-ledger-entries-automatically"></a>Bankafschriftregels automatisch afstemmen met bankrekeningposten
1. Kies in het venster **Bankreconciliatie** de actie **Automatisch afstemmen**. Het venster **Bankposten afstemmen** verschijnt.
2. Geef in het veld **Datumtolerantie van transactie (dagen)** het aantal dagen op vóór en na de boekingsdatum van de bankpost waarbinnen de functie naar overeenkomstige transactiedatums in het bankafschrift zoekt.

    Als u 0 typt of het veld leeg laat, zoekt de functie **Automatisch afstemmen** alleen naar overeenkomende transactiedatums op de bankpostboekingsdatum.  
3. Kies de knop **Ok**.  
Alle bankafschriftregels en bankrekeningposten die kunnen worden afgestemd, worden in groene letters weergegeven, en het selectievakje **Vereffend** wordt geselecteerd.
4. Als u een afstemming wilt verplaatsen, selecteert u de bankafschriftregel en kiest u vervolgens **Afstemming verwijderen**.

## <a name="to-match-bank-statement-lines-with-bank-account-ledger-entries-manually"></a>Bankafschriftregels handmatig afstemmen met bankrekeningposten
1. Selecteer in het venster **Bankreconciliatie** een niet-vereffende regel in het deelvenster **Bankafschriftregels**.
2. Selecteer in het deelvenster **Bankposten** een of meer bankrekeningposten die met de geselecteerde bankafschriftregel kunnen worden afgestemd. Om meerdere regels te kiezen drukt u op de Ctrl-toets en houdt u deze ingedrukt.  
3. Kies de actie **Handmatig afstemmen**.

    De geselecteerde bankafschriftregel en de geselecteerde bankrekeningposten worden in groene letters weergegeven en het selectievakje **Vereffend** in het rechtervenster wordt geselecteerd.
4. Herhaal stap 1 t/m 3 voor alle bankafschriftregels die niet overeenkomen.
5. Als u een afstemming wilt verplaatsen, selecteert u de bankafschriftregel en kiest u vervolgens **Afstemming verwijderen**.

## <a name="to-create-missing-ledger-entries-to-match-bank-transactions-with"></a>Ontbrekende posten maken om banktransacties mee af te stemmen
Soms bevat een bankafschrift bedragen voor in rekening gebrachte rente of toeslagen. Dergelijke banktransacties kunnen niet worden afgestemd omdat geen posten bestaan in Dynamics NAV. U moet vervolgens voor elke transactie een dagboekregel boeken om een gerelateerde post te maken waarmee deze kan worden afgestemd.

1. Kies in het venster **Bankreconciliatie** de actie **Naar dagboek overbrengen**.  
2. Geef in het venster **Bankreconciliatie naar dagboek** op welk dagboek moet worden gebruikt en kies vervolgens de knop **OK**.

    Het venster **Diversendagboek** wordt geopend met nieuwe dagboekregels voor bankafschriftregels met ontbrekende posten.
3. Vul de dagboekregel met de relevante gegevens, zoals de tegenrekening. Zie voor meer informatie [Werken met diversendagboeken](ui-work-general-journals.md).  
4. Kies de actie **Boeken**.  
Wanneer de post wordt geboekt, stemt u de banktransactie ermee af.
5. Het venster **Bankreconciliatie** vernieuwen of opnieuw openen. De nieuwe post wordt in het deelvenster **Bankposten** weergegeven.
6. Stem de bankafschriftregel handmatig of automatisch af met de bankpost.

## <a name="see-also"></a>Zie ook  
[Bankrekeningen beheren.](bank-manage-bank-accounts.md)  
[Bankieren instellen](bank-setup-banking.md)


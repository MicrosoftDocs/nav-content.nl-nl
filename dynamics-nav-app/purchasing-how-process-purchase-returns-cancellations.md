---
title: 'Procedure: Inkoopretouren of annuleringen verwerken'
author: SorenGP
ms.custom: na
ms.date: 11/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 94067fb3d10975c1db29d2e3f1d5d6373fcbf9f2
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-process-purchase-returns-or-cancellations"></a>Procedure: Inkoopretouren of annuleringen verwerken
Als u artikelen wilt retourneren naar uw leverancier of services die u hebt aangeschaft, wilt annuleren, kunt u een inkoopcreditnota maken en boeken met de aangevraagde wijziging voor de oorspronkelijke inkoopfactuur. Als u de juiste inkoopfactuurinformatie wilt opnemen kunt u de inkoopcreditnota maken van de geboekte inkoopfactuur of een kopieerfunctie gebruiken.

Doorgaans maakt u een inkoopcreditnota als reactie op een creditnota die naar u wordt verzonden door een leverancier. De inkoopcreditnota fungeert als interne documentatie van het creditnotaproces voor administratieve doeleinden.

De wijziging kan op alle producten op de oorspronkelijke inkoopfactuur, of slechts op sommige producten, betrekking hebben. Dienovereenkomstig kunt u ontvangen artikelen gedeeltelijk retourneren of gedeeltelijke terugbetaling van ontvangen services aanvragen. In dat geval moet u de gekopieerde inkoopfactuurinformatie bewerken.

Naast de oorspronkelijke geboekte inkoopfactuur kunt u de inkoopcreditnota op andere inkoopdocumenten toepassen, bijvoorbeeld een andere geboekte inkoopfactuur, omdat u ook artikelen terugzendt die met die factuur zijn geleverd.

## <a name="to-create-a-purchase-credit-memo-from-a-posted-purchase-invoice"></a>Een nieuwe inkoopcreditnota maken vanuit een geboekte inkoopfactuur
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Inkoopcreditnota's** in en kies vervolgens de gerelateerde koppeling.  
2. Selecteer in het venster **Geboekte inkoopfacturen** de geboekte inkoopfactuur die u wilt tegenboeken en kies vervolgens de actie **Corrigerende creditnota maken**.

    De meeste velden op de inkoopcreditnotakop worden ingevuld met de gegevens van de geboekte inkoopfactuur. U kunt alle velden bewerken, bijvoorbeeld met nieuwe gegevens die overeenkomen met de retourovereenkomst.
3. Bewerk informatie op de regels volgens de overeenkomst, zoals het nummer van geretourneerde artikelen of het terug te betalen bedrag.
4. Kies de actie **Posten vereffenen**.
5. Selecteer in het venster **Leveranciersposten vereffenen** de regel met het geboekte inkoopdocument waarmee u de inkoopcreditnota wilt vereffenen, en kies vervolgens de actie **Vereffenings-id**. Het nummer van de inkoopcreditnota wordt ingevoegd in het veld **Vereffenings-id**.
6. Voer in het veld **Te vereffenen bedrag** het bedrag in dat u wilt vereffenen als het kleiner is dan het oorspronkelijke bedrag.

    Onder in het venster **Leveranciersposten vereffenen** ziet u het totale te vereffenen bedrag om alle betrokken posten tegen te boeken, namelijk als de waarde in het **Saldo** nul is.
7. Kies de knop **Ok**. Wanneer u de inkoopcreditnota boekt, wordt deze vereffend met de opgegeven geboekte inkoopdocumenten.

    Wanneer u de nodige inkoopcreditnotaregels hebt gemaakt of bewerkt en de enkele of meerdere vereffeningen worden opgegeven, kunt u doorgaan om de inkoopcreditnota te boeken.
8. Kies de actie **Boeken**.

De geboekte inkoopfacturen die u met de creditnota vereffent, worden nu tegengeboekt. Als u de oorspronkelijke factuur al hebt betaald, moet de leverancier de betaling nu aan u terugbetalen. Als de creditnota slechts voor een gedeelte van het product op de oorspronkelijke factuur is, kunt u alleen het resterende bedrag op de oorspronkelijke inkoopfactuur betalen om deze te sluiten.

De inkoopcreditnota wordt verwijderd en vervangen door een nieuw document in de lijst met geboekte inkoopcreditnota's.

## <a name="to-create-a-purchase-credit-memo-from-scratch"></a>Een volledig nieuwe inkoopcreditnota maken
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Geboekte inkoopfacturen** in en kies vervolgens de gerelateerde koppeling.
2. Kies de actie **Nieuw** om een nieuwe lege inkoopcreditnota te openen.
3. Voer in het veld **Leverancier** de naam in van een bestaande leverancier.
4. Kies de actie **Document kopiëren**.
5. Selecteer in het venster **Inkoopdocument kopiëren** in het veld **Documentsoort** **Geboekte factuur**.
6. Kies het veld **Documentnr.** om het venster **Geboekte inkoopfacturen** te openen en selecteer vervolgens de geboekte inkoopfactuur die regels bevat die u wilt tegenboeken.
7. Schakel het selectievakje **Regels opnieuw berekenen** in als u wilt dat de gekopieerde geboekte inkoopfactuurregels worden bijgewerkt met de wijzigingen in de artikelprijs en kostprijs sinds de factuur is geboekt.
8. Kies de knop **Ok**. De gekopieerde factuurregels worden ingevoegd in de kredietnota van de aankoop.
9. Voltooi de inkoopcreditnota, zoals is uitgelegd in het gedeelte "Een nieuwe inkoopcreditnota maken vanuit een geboekte inkoopfactuur" in dit onderwerp.

## <a name="see-also"></a>Zie ook
[Inkoop beheren](purchasing-manage-purchasing.md)  
[Procedure: Inkopen vastleggen](purchasing-how-record-purchases.md)  


---
title: 'Procedure: Verkoopretouren of annuleringen verwerken'
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
ms.openlocfilehash: 92b65379f2ec633712a2b2c0f06615c6de61cc6e
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-process-sales-returns-or-cancellations"></a>Procedure: Verkoopretouren of annuleringen verwerken
Als uw klant artikelen of services wil retourneren of terugbetalingen wil krijgen voor artikelen of services die u aan de klant hebt verkocht en waarvoor u een betaling hebt ontvangen, moet u een verkoopcreditnota maken en boeken waarmee de gevraagde wijziging wordt opgegeven. Als u de juiste verkoopfactuurinformatie wilt opnemen, kunt u de verkoopcreditnota maken op basis van de geboekte verkoopfactuur of kunt u een kopieerfunctie gebruiken.

Naast de oorspronkelijke geboekte verkoopfactuur kunt u de verkoopcreditnota op andere verkoopdocumenten toepassen, bijvoorbeeld een andere geboekte verkoopfactuur, omdat de klant ook artikelen terugzendt die met die factuur zijn geleverd.

Een retour of terugbetaling kan betrekking hebben op slechts enkele artikelen of services op de oorspronkelijke verkoopfactuur. In dat geval moet u gegevens over de regels op de verkoopcreditnota bewerken. Wanneer u de verkoopcreditnota boekt, worden de door de wijziging beïnvloede verkoopdocumenten tegengeboekt en een terugbetaling voor de klant worden gemaakt.

U kunt de geboekte verkoopcreditnota naar de klant verzenden om de retournering of annulering te bevestigen en mede te delen dat de betreffende waarde wordt terugbetaald, bijvoorbeeld wanneer de artikelen zijn geretourneerd.

## <a name="to-create-a-sales-credit-memo-from-a-posted-sales-invoice"></a>Een verkoopcreditnota maken op basis van een geboekte verkoopfactuur
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Geboekte verkoopfacturen** in en kies vervolgens de gerelateerde koppeling.  
2. Selecteer in het venster **Geboekte verkoopfacturen** de geboekte verkoopfactuur die u wilt tegenboeken en kies vervolgens de actie **Corrigerende creditnota maken**.

    De meeste velden in de verkoopcreditnotakop worden ingevuld met de gegevens van de geboekte verkoopfactuur. U kunt alle velden bewerken, bijvoorbeeld met nieuwe gegevens die overeenkomen met de retourovereenkomst.
3. Bewerk informatie op de regels volgens de overeenkomst, zoals het aantal geretourneerde artikelen of het terug te betalen bedrag.
4. Kies de actie **Posten vereffenen**.
5. Selecteer in het venster **Klantposten vereffenen** de regel met het geboekte verkoopdocument waarmee u de verkoopcreditnota wilt vereffenen, en kies vervolgens de actie **Vereffenings-id**.

    Het nummer van de verkoopcreditnota wordt ingevoegd in het veld **Vereffenings-id**.  
6. Voer in het veld **Te vereffenen bedrag** het bedrag in dat u wilt vereffenen als het kleiner is dan het oorspronkelijke bedrag.

    Onder in het venster **Klantposten vereffenen** ziet u het totale te vereffenen bedrag om alle betrokken posten tegen te boeken, namelijk als de waarde in het veld **Saldo** nul is.  
7. Kies de knop **Ok**. Wanneer u de verkoopcreditnota boekt, wordt het vereffend met de opgegeven geboekte verkoopdocumenten.

    Wanneer u de benodigde verkoopcreditnotaregels hebt gemaakt of bewerkt en de enkele vereffening of meerdere vereffeningen zijn opgegeven, kunt u doorgaan met het boeken van de verkoopcreditnota.
8. Kies de actie **Boeken en verzenden**.

Het dialoogvenster **Boeken en verzenden bevestigen** wordt geopend met de geprefereerde verzendmethode voor de klant. U kunt de verzendmethode wijzigen door de opzoekknop voor het veld **Document verzenden naar** te kiezen. Zie [Procedure: Verzendprofielen voor documenten instellen](sales-how-setup-document-send-profiles.md) voor meer informatie.

De geboekte verkoopdocumenten die u op de creditnota hebt vereffend, worden nu tegengeboekt en een terugbetaling kan worden gemaakt voor de klant. De verkoopcreditnota wordt verwijderd en vervangen door een nieuw document in de lijst met geboekte verkoopcreditnota's.

## <a name="to-create-a-sales-credit-memo-from-scratch"></a>Een geheel nieuwe verkoopcreditnota maken
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Geboekte verkoopfacturen** in en kies vervolgens de gerelateerde koppeling.
2. Kies de actie **Nieuw** om een nieuwe lege verkoopcreditnota te openen.
3. Voer in het veld **Klant** de naam in van een bestaande klant.
4. Kies de actie **Document kopiëren**.
5. Selecteer in het venster **Verkoopdocument kopiëren** in het veld **Documentsoort** **Geboekte factuur**.
6. Kies het veld **Documentnr.** om het venster **Geboekte verkoopfacturen** te openen en selecteer vervolgens de geboekte verkoopfactuur die regels bevat die u wilt tegenboeken.
7. Schakel het selectievakje **Regels opnieuw berekenen** in als u wilt dat de gekopieerde geboekte verkoopfactuurregels worden bijgewerkt met de wijzigingen in de artikelprijs en kostprijs sinds de factuur is geboekt.
8. Kies de knop **Ok**. De gekopieerde factuurregels worden ingevoegd in de kredietnota van de verkoop.
9. Voltooi de verkoopcreditnota zoals is uitgelegd in de sectie "Een nieuwe verkoopcreditnota maken op basis van een geboekte verkoopfactuur" in dit onderwerp.

## <a name="see-also"></a>Zie ook  
[Verkoop beheren](sales-manage-sales.md)  
[Verkopen instellen](sales-setup-sales.md)  
[Procedure: Documenten per e-mail verzenden](ui-how-send-documents-email.md)  
[Werken met Dynamics NAV](ui-work-product.md)


---
title: 'Procedure: Documenten per e-mail verzenden'
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
ms.openlocfilehash: e4476c2ab903001017dcd6c8bdaa84892ba79c9e
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-send-documents-by-email"></a>Procedure: Documenten per e-mail verzenden
Om de inhoud van bedrijfsdocumenten snel aan uw zakelijke partners door te geven, zoals de betalingsgegevens over verkoopdocumenten aan klanten, kunt u de functie Rapportlay-out gebruiken om documentspecifieke inhoud te definiëren die automatisch wordt ingevoegd in hoofdteksten van e-mail.

Als u e-mails vanuit Dynamics NAV wilt inschakelen, start u de begeleide instelling **E-mail instellen** op de startpagina.

U kunt vrijwel alle documentsoorten als bijlagen bij e-mailberichten direct e-mailen vanuit het venster dat het document bevat. Naast de bijlage kunt u documentspecifieke hoofdteksten van e-mail met basisgegevens van het document instellen voorafgegaan door standaardtekst waarin de e-mailgeadresseerde wordt begroet en het betreffende document wordt geïntroduceerd. Om uw klanten aan te bieden voor verkoop elektronisch te betalen met een betalingsservice, zoals PayPal, kunt u de PayPal-informatie en hyperlink in de hoofdtekst van de e-mail invoegen.

Vanuit alle documenten start u het e-mailen door in geboekte documenten de actie **Verzenden** te kiezen of in niet-geboekte documenten de actie **Boeken en verzenden**.

Als het veld **E-mail** in het venster **Document verzenden naar** is ingesteld op **Ja (prompt voor instellingen)**, wordt het venster **E-mail verzenden** geopend waarin de contactpersoon al is ingevuld in het veld **Aan:** en het document als een PDF-bestand is bijgevoegd. In het veld **Hoofdtekst** kunt u tekst handmatig invoeren of kunt u in het veld een documentspecifieke e-mailhoofdtekst invoeren die u hebt ingesteld.

In de volgende procedure wordt beschreven hoe u het rapport **Verkoop - factuur** zo instelt dat het kan worden gebruikt voor documentspecifieke e-mailhoofdteksten wanneer u geboekte verkoopfacturen via e-mail verstuurt.

## <a name="to-set-up-a-document-specific-email-body-for-sales-invoices"></a>Een documentspecifieke e-mailhoofdtekst instellen voor verkoopfacturen
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Rapportselectie - Verkoop** in en kies vervolgens de gerelateerde koppeling.
2. Selecteer in het venster **Rapportselectie - Verkoop** in het veld **Gebruik** de optie **Factuur**.
3. Selecteer op een nieuwe regel in het veld **Rapport-ID** bijvoorbeeld standaardrapport 1306.
4. Schakel het selectievakje **Gebruiken voor hoofdtekst van e-mailbericht** in.
5. Kies het veld **Indelings-id van hoofdtekst van e-mailbericht** en selecteer een van de beschikbare lay-outs in het venster **Aangepaste rapportlay-outs**.
6. Met rapportlay-outs wordt zowel de stijl als de inhoud van de e-mailhoofdtekst gedefinieerd, inclusief de standaardtekst die voorafgaat aan de basisdocumentinformatie in de hoofdtekst van de e-mail.
7. Als u de lay-out waarop de e-mailhoofdtekst is gebaseerd, wilt weergeven of bewerken, kiest u in het venster **Aangepaste rapportlay-outs** de actie **Lay-out bewerken**.
8. Als u klanten wilt aanbieden om voor verkoop elektronisch te betalen, kunt u de gerelateerde betalingsservice, zoals PayPal, instellen en vervolgens ook de PayPal-informatie en hyperlink in de hoofdtekst van de e-mail invoegen. Zie [Procedure: Klantbetalingen mogelijk maken via PayPal](sales-how-enable-customer-payments-paypal.md) voor meer informatie.
9. Kies de knop **Ok**.

Wanneer u nu bijvoorbeeld de actie Verzenden kiest in het venster **Geboekte verkoopfactuur**, bevat de e-mailhoofdtekst de documentgegevens van rapport 1306 voorafgegaan door gestileerde standaardtekst in overeenstemming met de rapportlay-out die u in stap 5 hebt geselecteerd.

In de volgende procedure wordt beschreven hoe u een geboekte verkoopfactuur als een e-mailbericht verzendt met het document als een PDF-bestand bijgevoegd en met een documentspecifieke e-mailhoofdtekst.
## <a name="to-send-documents-by-email"></a>Documenten per e-mail verzenden
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Geboekte verkoopfacturen** in en kies vervolgens de gerelateerde koppeling.
2. Selecteer de relevante verkoopfactuur en kies de actie **Verzenden**. Het venster **Document verzenden naar** verschijnt.
3. Selecteer in het veld **E-mail** **Ja (prompt voor instellingen)**. Zie [Procedure: Verzendprofielen voor documenten instellen](sales-how-setup-document-send-profiles.md) voor meer informatie.
4. Kies de knop **Ok**. Het venster **E-mail verzenden** wordt geopend.
5. Voer in het veld **Aan** een geldig e-mailadres. De standaardwaarde is het e-mailadres van de klant.
6. Geef in het veld **Cc** een e-mailadres op om een kopie van het e-mailbericht naar een andere ontvanger te verzenden.
7. Geef in het veld **Bcc** een e-mailadres op om een kopie van de e-mail te verzenden naar een andere ontvanger zonder dat het e-mailadres en de naam aan andere ontvangers worden getoond.
8. Voer in het veld **Onderwerp** een beschrijvende onderwerptekst in. De standaardwaarde is de naam van de klant en het factuurnummer.
9. In het veld **Bijlage** wordt de gegenereerde factuur standaard gekoppeld als een PDF-bestand. Kies de opzoekknop om het bestand te openen of nog een bestand bij te voegen.
10. Voer in het veld **Hoofdgedeelte** een kort bericht aan de ontvanger in.

    Als een documentspecifieke e-mailhoofdtekst is ingesteld in het venster **Rapportselectie - Verkoop**, wordt het veld **Hoofdtekst** automatisch ingevuld. Zie de sectie “Een documentspecifieke e-mailhoofdtekst instellen voor verkoopfacturen” in dit onderwerp voor meer informatie.
11. Schakel het selectievakje **In Outlook-webapp bewerken** in om het e-mailbericht in de e-mailapp voor Office 365 te openen.
12. Kies de knop **OK** om het e-mailbericht te verzenden.

**Opmerking**: als u geen e-mailinstellingen hoeft op te geven steeds wanneer u een document e-mailt, kunt u de optie **Ja (standaardinstellingen gebruiken)** in het veld E-mail van het venster **Document verzenden naar** selecteren. In dat geval wordt het venster **E-mail verzenden** niet geopend. Zie stap 4. Zie [Procedure: Verzendprofielen voor documenten instellen](sales-how-setup-document-send-profiles.md) voor meer informatie.

## <a name="see-also"></a>Zie ook  
[Werken met Dynamics NAV](ui-work-product.md)  
[Procedure: Verkopen factureren](sales-how-invoice-sales.md)


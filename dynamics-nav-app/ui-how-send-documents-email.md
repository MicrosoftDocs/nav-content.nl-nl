---
title: Documentspecifieke inhoud en bijlagen instellen voor e-mailberichten
description: "U kunt inhoud definiëren die moet worden ingevoegd in het hoofdgedeelte van een e-mailbericht, bijvoorbeeld een PayPal-koppeling. U kunt ook documenten koppelen aan e-mailberichten."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: SMTP, mail, Office 365, cover, body, PayPal, layout
ms.date: 03/30/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 06c8eeb49cc02533314192cb089dc8786c226095
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-send-documents-by-email"></a>Procedure: Documenten per e-mail verzenden
Om de inhoud van bedrijfsdocumenten snel aan uw zakelijke partners door te geven, zoals de betalingsgegevens over verkoopdocumenten aan klanten, kunt u de functie Rapportlay-out gebruiken om documentspecifieke inhoud te definiëren die automatisch wordt ingevoegd in hoofdteksten van e-mail. Zie voor meer informatie [Lay-outs van rapporten en documenten beheren](ui-manage-report-layouts.md).

Als u e-mails vanuit [!INCLUDE[d365fin](includes/d365fin_md.md)] wilt inschakelen, start u de begeleide instelling **E-mail instellen** op de startpagina.

U kunt vrijwel alle documentsoorten als bijlagen bij e-mailberichten direct e-mailen vanuit het venster dat het document bevat. Naast de bijlage kunt u documentspecifieke hoofdteksten van e-mail met basisgegevens van het document instellen voorafgegaan door standaardtekst waarin de e-mailgeadresseerde wordt begroet en het betreffende document wordt geïntroduceerd. Om uw klanten aan te bieden voor verkoop elektronisch te betalen met een betalingsservice, zoals PayPal, kunt u de PayPal-informatie en hyperlink in de hoofdtekst van de e-mail invoegen.

Vanuit alle documenten start u het e-mailen door in geboekte documenten de actie **Verzenden** te kiezen of in niet-geboekte documenten de actie **Boeken en verzenden**.

Als het veld **E-mail** in het venster **Document verzenden naar** is ingesteld op **Ja (prompt voor instellingen)**, wordt het venster **E-mail verzenden** geopend waarin de contactpersoon al is ingevuld in het veld **Aan:** en het document als een pdf-bestand is bijgevoegd. In het veld **Hoofdtekst** kunt u tekst handmatig invoeren of kunt u in het veld een documentspecifieke e-mailhoofdtekst invoeren die u hebt ingesteld.

In de volgende procedure wordt beschreven hoe u het rapport **Verkoop - factuur** zo instelt dat het kan worden gebruikt voor documentspecifieke e-mailhoofdteksten wanneer u geboekte verkoopfacturen via e-mail verstuurt.

## <a name="to-set-up-a-document-specific-email-body-for-sales-invoices"></a>Een documentspecifieke e-mailhoofdtekst instellen voor verkoopfacturen
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Rapportselectie - Verkoop** in en klik vervolgens op de gerelateerde koppeling.
2. Selecteer in het venster **Rapportselectie - Verkoop** in het veld **Gebruik** de optie **Factuur**.
3. Selecteer op een nieuwe regel in het veld **Rapport-ID** bijvoorbeeld standaardrapport 1306.
4. Schakel het selectievakje **Gebruiken voor hoofdtekst van e-mailbericht** in.
5. Kies het veld **Indelingscode van hoofdtekst van e-mailbericht** en selecteer een indeling in de vervolgkeuzelijst.

    Met rapportlay-outs wordt zowel de stijl als de inhoud van de e-mailhoofdtekst gedefinieerd, inclusief de standaardtekst die voorafgaat aan de basisdocumentinformatie in de hoofdtekst van de e-mail. U kunt alle beschikbare lijstindelingen bekijken als u de knop **Selecteren vanuit volledige lijst** kiest in de vervolgkeuzelijst.
6. Als u de lay-out wilt weergeven of bewerken waarop de e-mailhoofdtekst is gebaseerd, selecteert u in het venster **Aangepaste rapportlay-outs** de gewenste lay-out en vervolgens de actie **Lay-out bewerken**.
7. Als u klanten wilt aanbieden om voor verkoop elektronisch te betalen, kunt u de gerelateerde betalingsservice, zoals PayPal, instellen en vervolgens ook de PayPal-informatie en hyperlink in de hoofdtekst van de e-mail invoegen. Zie [Procedure: Klantbetalingen mogelijk maken via PayPal](sales-how-enable-payment-service-extensions.md) voor meer informatie.
8. Kies de knop **Ok**.

Wanneer u nu bijvoorbeeld de actie **Verzenden** kiest in het venster **Geboekte verkoopfactuur**, bevat de e-mailhoofdtekst de documentgegevens van rapport 1306, voorafgegaan door standaardtekst die is geformatteerd volgens de rapportlay-out die u in stap 5 hebt geselecteerd.

In de volgende procedure wordt beschreven hoe u een geboekte verkoopfactuur als een e-mailbericht verzendt met het document als een PDF-bestand bijgevoegd en met een documentspecifieke e-mailhoofdtekst.

## <a name="to-send-documents-by-email"></a>Documenten per e-mail verzenden
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Geboekte verkoopfacturen** in en klik vervolgens op de gerelateerde koppeling.
2. Selecteer de relevante geboekte verkoopfactuur en kies de actie **Verzenden**. Het venster **Document verzenden naar** verschijnt.
3. Selecteer in het veld **E-mail** **Ja (prompt voor instellingen)**. Zie [Procedure: Verzendprofielen voor documenten instellen](sales-how-setup-document-send-profiles.md) voor meer informatie.
4. Kies de knop **Ok**. Het venster **E-mail verzenden** wordt geopend.
5. Voer in het veld **Aan** een geldig e-mailadres. De standaardwaarde is het e-mailadres van de klant.
6. Voer in het veld **Onderwerp** een beschrijvende onderwerptekst in. De standaardwaarde is de naam van de klant en het factuurnummer.
7. In het veld **Bijlage** wordt de gegenereerde factuur standaard gekoppeld als een PDF-bestand. Kies de opzoekknop om het bestand te openen of nog een bestand bij te voegen.
8. Voer in het veld **Hoofdgedeelte** een kort bericht aan de ontvanger in.

    Als een documentspecifieke e-mailhoofdtekst is ingesteld in het venster **Rapportselectie - Verkoop**, wordt het veld **Hoofdtekst** automatisch ingevuld. Zie de sectie "Een documentspecifieke e-mailhoofdtekst instellen voor verkoopfacturen" in dit onderwerp voor meer informatie.
9. Kies de knop **OK** om het e-mailbericht te verzenden.

> [!NOTE]  
>   Als u geen e-mailinstellingen wilt opgeven telkens wanneer u een document e-mailt, kunt u de optie **Ja (standaardinstellingen gebruiken)** in het veld **E-mail** van het venster **Document verzenden naar** selecteren. In dat geval wordt het venster **E-mail verzenden** niet geopend. Zie stap 4. Zie [Procedure: Verzendprofielen voor documenten instellen](sales-how-setup-document-send-profiles.md) voor meer informatie.

## <a name="see-also"></a>Zie ook
[Lay-outs van rapporten en documenten beheren](ui-manage-report-layouts.md)  
[Procedure: E-mail instellen](madeira-how-setup-email.md)  
[Procedure: Verkopen factureren](sales-how-invoice-sales.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


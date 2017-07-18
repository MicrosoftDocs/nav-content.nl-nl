---
title: 'Procedure: Voorstellen maken'
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
ms.openlocfilehash: e126c755a9121c3a91f3af72f3f1ae14702a4701
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-make-offers"></a>Procedure: Voorstellen maken
U maakt een verkoopofferte aan om uw aanbod aan een klant vast te leggen om producten tegen bepaalde leverings- en betalingscondities te verkopen. U kunt de verkoopofferte aan de klant verzenden om het aanbod te bevestigen. U kunt het document als een PDF-bijlage via e-mail versturen. U kunt ook de hoofdtekst van de e-mail vooraf laten invullen met een overzicht van de offerte. Zie [Procedure: Documenten per e-mail verzenden](ui-how-send-documents-email.md) voor meer informatie.

Terwijl u met de klant onderhandelt, kunt u zo veel als u wenst de verkoopofferte wijzigen en opnieuw zenden. Als de klant de offerte accepteert, zet u de verkoopofferte om in een verkoopfactuur of een verkooporder waarin u de verkoop verwerkt. Zie [Procedure: Verkopen factureren](sales-how-invoice-sales.md) of [Procedure: Producten verkopen](sales-how-sell-products.md) voor meer informatie.

Producten kunnen zowel voorraadartikelen als services zijn. Zie voor meer informatie [Procedure: Nieuwe producten registreren](inventory-how-register-new-products.md). Het verkoopofferteproces is gelijk voor beide productsoorten.

**Opmerking**: in Dynamics NAV wordt naar een product verwezen met de term “artikel”.

U kunt klantvelden op de verkoopofferte op twee manieren invullen afhankelijk van de vraag of de klant reeds is geregistreerd.

## <a name="to-create-a-sales-quote"></a>Een verkoopofferte maken
1. Kies op de startpagina de actie **Verkoopofferte**.  
2. Voer in het veld **Klant** de naam in van een bestaande klant.

    Overige velden in het venster **Verkoopofferte** worden ingevuld met de standaardinformatie over de geselecteerde klant. Als de klant niet is geregistreerd, volgt u deze stappen:

3. Voer in het veld **Klant** de naam van de nieuwe klant in.
4. Kies in dialoogvenster voor het registreren van de nieuwe klant de knop **Ja**.
5. Kies in het venster **Selecteer een sjabloon voor een nieuwe klant** een sjabloon waarop u de nieuwe klantenkaart wilt baseren en kies vervolgens de knop **OK**.
6. Een nieuwe klantenkaart wordt geopend, die vooraf is ingevuld met de informatie over de geselecteerde klantensjabloon. Het veld **Naam** is vooraf ingevuld met de naam van de nieuwe klant die u op de verkoopfactuur hebt ingevoerd.
7. Ga door met het invullen van de overige velden op de klantenkaart. Zie [Procedure: Nieuwe klanten registreren](sales-how-register-new-customers.md) voor meer informatie.  
8. Wanneer u de klantenkaart hebt ingevuld, kiest u de knop **OK** om terug te keren naar het venster **Verkoopofferte**.

    Verschillende velden op de verkoopofferte worden nu ingevuld met gegevens die u hebt opgegeven op de nieuwe klantenkaart.
9. Vul indien nodig de overige velden in het venster **Verkoopofferte** in. Kies een veld om een korte omschrijving van het veld of een koppeling naar meer informatie te lezen.

    U kunt nu de verkoopofferteregels vullen met voorraadartikelen of services die u aan de klant wilt aanbieden.

    **Opmerking**: als u terugkerende verkoopregels voor de klant hebt ingesteld, zoals een maandelijkse aanvullingsorder, kunt u deze regels invoegen op de offerte door de actie **Terugkerende verkoopregels ophalen** te kiezen.
10. Voer op het sneltabblad **Regels** in het veld **Artikelnr.** het nummer in van een voorraadartikel of service.
11. Voer in het veld **Aantal** het aantal artikelen in dat moet worden aangeboden.

    **Opmerking**: voor artikelen van de soort Service is de hoeveelheid een tijdseenheid, bijvoorbeeld uren, zoals aangegeven in het veld **Eenheidscode** op de regel.

    Het veld **Regelbedrag** wordt bijgewerkt met de waarde in het veld **Eenheidsprijs**, vermenigvuldigd met de waarde in het veld **Aantal**.

    De prijs en de regelbedragen worden weergegeven met of zonder btw afhankelijk van wat u hebt geselecteerd in het veld **Prijzen inclusief btw** op de klantenkaart.
12. In het veld **Regelkorting %** voert u een percentage in als u de klant een korting op het product wilt verlenen. De waarde in het veld **Regelbedrag** wordt dienovereenkomstig bijgewerkt.

    **Opmerking**: als u speciale artikelprijzen hebt ingesteld op het sneltabblad **Verkoopprijzen en verkoopregelkortingen** op de klantenkaart of de artikelkaart, worden de prijs en het bedrag op de offerteregel automatisch bijgewerkt als aan de overeengekomen prijscriteria is voldaan. Zie voor meer informatie [Afspraken over prijzen, kortingen en betalingen van verkopen vastleggen](sales-how-record-sales-price-discount-payment-agreements.md).
13. Als u een opmerking over de offerteregel wilt toevoegen die de klant op de afgedrukte verkoopofferte kan zien, schrijft u een tekst in het veld **Omschrijving** op een lege regel.  
14. Herhaal stap 10 t/m 13 voor elk artikel dat u aan de klant wilt aanbieden.

    De totalen onder de regels worden automatisch berekend wanneer u regels maakt of wijzigt.
15. In het veld **Kortingsbedrag op factuur** voert u een bedrag in dat moet worden afgetrokken van de waarde in het veld **Totaal incl. btw**.

    **Opmerking**: als u factuurkortingen voor de klant hebt opgegeven, wordt het opgegeven percentage automatisch ingevoegd in het veld **Factuurkorting %** als aan de voorwaarden wordt voldaan, en het gerelateerde bedrag wordt ingevoegd in het veld **Factuurkortingsbedrag excl. btw**. Zie voor meer informatie [Afspraken over prijzen, kortingen en betalingen van verkopen vastleggen](sales-how-record-sales-price-discount-payment-agreements.md).
16. Wanneer de verkoopofferteregels zijn ingevuld, kiest u de actie **E-mail** of **Afdrukken**.

    Als u de actie **E-mail** selecteert, wordt automatisch een PDF-bestand gekoppeld aan een e-mail aan de klant. U kunt de e-mail zo instellen dat deze een overzicht van de offerte bevat. Zie [Procedure: Documenten per e-mail verzenden](ui-how-send-documents-email.md) voor meer informatie.
17. Als de klant de offerte accepteert, kiest u de actie **Factuur maken** of de actie **Order maken**.

De verkoopofferte wordt verwijderd uit de database. Een verkoopfactuur of een verkooporder wordt gemaakt op basis van de informatie in de verkoopofferte waarin u de verkoop kunt verwerken. In het veld **Offertenr.** op de verkoopfactuur of verkooporder ziet u het nummer van de verkoopofferte op basis waarvan deze is gemaakt. Zie [Procedure: Verkopen factureren](sales-how-invoice-sales.md) of [Procedure: Producten verkopen](sales-how-sell-products.md) voor meer informatie.

## <a name="see-also"></a>Zie ook  
[Verkoop beheren](sales-manage-sales.md)  
[Verkopen instellen](sales-setup-sales.md)  
[Procedure: Documenten per e-mail verzenden](ui-how-send-documents-email.md)  
[Werken met Dynamics NAV](ui-work-product.md)


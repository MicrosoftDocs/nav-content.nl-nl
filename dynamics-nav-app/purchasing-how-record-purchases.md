---
title: 'Procedure: Inkopen vastleggen'
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
ms.openlocfilehash: 6d1933bf1e1c9236d34d429a4da84c907df13708
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-record-purchases"></a>Procedure: Inkopen vastleggen
U maakt een inkoopfactuur of inkooporder om de kosten van inkopen vast te leggen en leveranciers te volgen. Als u voorraad moet controleren, worden inkoopfacturen en inkooporders ook gebruikt om voorraadniveaus dynamisch aan te passen zodat u uw voorraadkosten kunt beperken en betere klantenservice kunt bieden. De inkoopkosten, inclusief servicekosten, en voorraadwaarden die resulteren uit boekingsinkoopfacturen of -orders, dragen bij aan winstcijfers en andere financiële KPI's op uw startpagina.

**Opmerking**: u moet inkooporders gebruiken als uw inkoopproces vereist dat u gedeeltelijke ontvangsten van een orderhoeveelheid registreert, bijvoorbeeld omdat de volledige hoeveelheid niet in één keer beschikbaar was bij de leverancier. Als u artikelen verkoopt door rechtstreeks van uw leverancier bij de klant te leveren, als een doorverzending, moet u ook inkooporders gebruiken. Zie [Procedure: Doorverzendingen maken](sales-how-drop-shipment.md) voor meer informatie. Wat betreft alle andere aspecten werken inkooporders op dezelfde manier als inkoopfacturen. De volgende procedure is gebaseerd op een inkoopfactuur. De stappen zijn vergelijkbaar met de stappen voor een inkooporder.

Wanneer u de voorraadartikelen ontvangt of wanneer de ingekochte service wordt voltooid, boekt u de inkoopfactuur of -order om de voorraad en financiële records bij te werken en betaling aan de leverancier te activeren volgens de betalingscondities. Zie voor meer informatie [Betalingen doen](payables-make-payments.md).

**Pas op**: boek geen inkoopfactuur totdat u de producten ontvangt en de uiteindelijke kosten van de inkoop kent, inclusief eventuele toeslagen. Anders kloppen uw voorraadwaarde en winstcijfers mogelijk niet.

Als u al hebt betaald voor producten op de geboekte inkoopfactuur, moet u een inkoopcreditnota maken om de inkoop tegen te boeken. Zie voor meer informatie [Procedure: Inkoopretouren of annuleringen verwerken](purchasing-how-process-purchase-returns-cancellations.md).

Producten kunnen zowel voorraadartikelen als services zijn. Zie voor meer informatie [Procedure: Nieuwe producten registreren](inventory-how-register-new-products.md). Het inkoopfactuurproces is gelijk voor beide productsoorten.



U kunt leveranciersvelden op de inkoopfactuur op twee manieren invullen afhankelijk van of de leverancier reeds is geregistreerd.

## <a name="to-create-a-purchase-invoice"></a>Een inkoopfactuur maken
1. Kies op de startpagina de actie **Inkoopfactuur**.  
2. Voer in het veld **Leverancier** de naam in van een bestaande klant.

    Overige velden in het venster **Inkoopfactuur** worden nu ingevuld met de standaardinformatie over de geselecteerde leverancier. Als de leverancier niet is geregistreerd, volgt u deze stappen:
3. Voer in het veld **Leverancier** de naam van de nieuwe leverancier in.
4. Kies in dialoogvenster voor het registreren van de nieuwe leverancier de knop **Ja**.
5. Kies in het venster **Selecteer een sjabloon voor een nieuwe leverancier** een sjabloon om de leverancierskaart op te baseren en kies vervolgens de knop **OK**.
6. Een nieuwe leverancierskaart wordt geopend, die vooraf is ingevuld met de informatie over de geselecteerde leveranciersjabloon. Het veld **Naam** is vooraf ingevuld met de naam van de nieuwe leverancier die u op de inkoopfactuur hebt ingevoerd.
7. Ga verder met het invullen van de overige velden op de leverancierskaart. Zie voor meer informatie [Procedure: Nieuwe leveranciers registreren](purchasing-how-register-new-vendors.md).  
8. Wanneer u de leverancierskaart hebt voltooid, kiest u de knop **OK** om terug te keren naar het venster **Inkoopfactuur**.

    Verschillende velden in het venster **Inkoopfactuur** worden gevuld met gegevens die u op de nieuwe leverancierskaart hebt opgegeven.
9. Vul indien nodig de overige velden in het venster **Inkoopfactuur** in. Kies een veld om een korte omschrijving van het veld of een koppeling naar meer informatie te lezen.

    U kunt nu de inkoopfactuurregels invullen met voorraadartikelen of services die u hebt gekocht van de leverancier.

    **Opmerking**: als u terugkerende inkoopregels voor de leverancier hebt ingesteld, zoals een maandelijkse aanvullingsorder, kunt u deze regels invoegen op de factuur door de actie **Terugkerende inkoopregels ophalen** te kiezen.
10. Voer op het sneltabblad **Regels** in het veld **Artikelnr.** het nummer in van een voorraadartikel of service.
11. Voer in het veld **Aantal** het in te kopen aantal van een artikel in.

    **Opmerking**: voor artikelen van de soort **Service** is de hoeveelheid een tijdseenheid, bijvoorbeeld uren, zoals aangegeven in het veld **Eenheidscode** op de regel.

    Het veld **Regelbedrag** wordt bijgewerkt met de waarde in het veld **Directe kostprijs**, vermenigvuldigd met de waarde in het veld **Aantal**.

    De prijs en het regelbedrag worden weergegeven met of zonder btw afhankelijk van wat u hebt geselecteerd in het veld **Prijzen inclusief btw** op de leverancierskaart.
12. In het veld **Kortingsbedrag op factuur** voert u een bedrag in dat moet worden afgetrokken van de waarde in het veld **Totaal incl. btw** onder in de factuur.

    **Opmerking**: als u factuurkortingen voor de leverancier hebt opgegeven, wordt het percentage automatisch ingevoegd in het veld **Kortingspercentage op leveranciersfactuur** als aan de voorwaarden wordt voldaan, en het gerelateerde bedrag wordt ingevoegd in het veld **Kortingsbedrag op factuur**.
13. Als u de ingekochte artikelen of diensten ontvangt, kiest u **Boeken**.

De inkoop wordt nu weerspiegeld in de voorraad en financiële records, en de leveranciersbetaling is ingeschakeld. De inkoopfactuur wordt verwijderd uit het overzicht met inkoopfacturen en wordt vervangen door een nieuw document in het overzicht van geboekte inkoopfacturen.

## <a name="see-also"></a>Zie ook  
[Inkoop beheren](purchasing-manage-purchasing.md)  
[Inkoop instellen](purchasing-setup-purchasing.md)  
[Procedure: Producten kopen voor een verkoop](purchasing-how-purchase-products-sale.md)  
[Procedure: Nieuwe leveranciers registreren](purchasing-how-register-new-vendors.md)  
[Procedure: Doorverzendingen voorbereiden](sales-how-drop-shipment.md)  
[Werken met Dynamics NAV](ui-work-product.md)


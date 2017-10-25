---
title: Betalingsscenario 2 - buitenlandse betaling (VV naar VV)
description: U kunt telebankieren gebruiken voor handel met binnenlandse en buitenlandse klanten en leveranciers. Dit onderwerp beschrijft een scenario waarin de handel met buitenlandse klanten en leveranciers geschiedt die dezelfde vreemde valuta gebruiken als waarvoor uw bankrekening is ingesteld.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: f0ce9c3e83ed41fd25cd06abea8607f3f2d79563
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="payment-scenario-2---foreign-payment-fcy-to-fcy"></a>Betalingsscenario 2 - buitenlandse betaling (VV naar VV)
U kunt telebankieren gebruiken voor handel met binnenlandse en buitenlandse klanten en leveranciers. Dit onderwerp beschrijft een scenario waarin de handel met buitenlandse klanten en leveranciers geschiedt die dezelfde vreemde valuta gebruiken als waarvoor uw bankrekening is ingesteld.  
  
 De volgende lijst bevat de belangrijkste stappen:  
  
1.  Leverancier/klant maken.  
  
2.  Bankrekening leverancier/klant maken.  
  
3.  Inkoopfactuur voor leverancier of verkoopfactuur voor klant maken en boeken.  
  
4.  Voorstel maken.  
  
5.  Betaalrun maken.  
  
6.  Betaalrun exporteren.  
  
7.  Bankafschrift importeren.  
  
> [!NOTE]  
>  In de volgende voorbeelden zijn enkele standaard-CRONUS-gegevens gebruikt. En in plaats van een leverancier/klant en een Bankrekening leverancier/klant te maken, zou u ook bestaande gegevens kunnen gebruiken.  
  
## <a name="create-vendorcustomer"></a>Leverancier/klant maken  
 Maak een leverancier/klant en vul alle noodzakelijke gegevens in. Besteed extra aandacht aan het volgende:  
  
-   **Valutacode**: stel in dit veld de vreemde valuta (VV) in.  
  
-   **Transactiewijze**: selecteer een geschikte standaardtransactiewijze, dat wil zeggen, een transactiewijze die geschikt is voor betalingen in vreemde valuta voor uw buitenlandse bank.  
  
-   **Bankrekening van voorkeur**: selecteer een geschikte standaardbankrekening van leveranciers/klanten met dezelfde valutacode als de leverancier/klant zelf.  
  
> [!NOTE]  
>  U kunt alleen een bankrekening in het veld **Bankrekening** invullen als er Bankrekeningen leverancier/klant beschikbaar zijn. Zie hieronder.  
  
### <a name="example"></a>Voorbeeld  
 Jannet Carter (code *JANNET*) is een van onze Amerikaanse leveranciers. Inkoopfacturen worden door middel van onze buitenlandse bankrekening (code *ABN-USD*) aan haar bankrekening (code *JCBA*) betaald. Zowel bankrekening ABN-USD als bankrekening JCBA worden uitgedrukt in dezelfde vreemde valuta (VV), in dit geval Amerikaanse dollars (USD). Daarom stellen we op de leverancierskaart van Jannet Carter het veld *Valutacode* in op *USD*, vullen we in het veld *Transactiewijze* *ABN-USD* in die aan onze bankrekening *ABN-USD* is gekoppeld en stellen we het veld *Bankrekening* in op *JCBA*.  
  
## <a name="create-vendorcustomer-bank-account"></a>Bankrekening leverancier/klant maken  
 Maak een bankrekening leverancier/klant en vul alle noodzakelijke gegevens in. Besteed extra aandacht aan het volgende:  
  
-   **Bankrekening van voorkeur**: voer een geldig bankrekeningnummer in.  
  
-   **Valutacode**: stel in dit veld de vreemde valuta (VV) in.  
  
-   **Rekeninghouder**: zorg ervoor dat alle gegevens zijn ingevuld.  
  
### <a name="example"></a>Voorbeeld  
 De bankrekening van Jannet Carter (code *JCBA*) wordt uitgedrukt in vreemde valuta (VV), in dit geval USD. Daarom vullen we op de bankrekeningkaart leverancier van Jannet Carter een geldig nummer in het veld *Bankrekeningnr.* in *,* stellen we het veld *Valutacode* in op *USD* en vullen we in de velden op het tabblad Rekeninghouder de juiste waarden in.  
  
## <a name="create-and-post-purchase-invoice-for-vendor-or-sales-invoice-for-customer"></a>Inkoopfactuur voor leverancier of verkoopfactuur voor klant maken en boeken  
 Maak een inkoop-/verkoopfactuur en vul alle noodzakelijke gegevens in. Besteed extra aandacht aan het volgende:  
  
-   **Valutacode**: stel in dit veld de vreemde valuta (VV) in.  
  
-   **Transactiewijze**: selecteer een geschikte standaardtransactiewijze, dat wil zeggen, een transactiewijze die geschikt is voor betalingen in vreemde valuta voor uw buitenlandse bank.  
  
-   **Bankrekening van voorkeur**: selecteer een geschikte standaardbankrekening van leveranciers/klanten met dezelfde valutacode als de leverancier/klant zelf.  
  
 Standaard zijn in deze drie velden waarden ingevuld die zijn overgenomen uit de leveranciers-/klantenkaart.  
  
 Als de factuur is voltooid, kan deze worden geboekt.  
  
### <a name="example"></a>Voorbeeld  
 Als we een inkoopfactuur voor Jannet Carter maken, vullen we *JANNET* in het veld ***Orderleveranciersnr.*** in. Standaard zijn in de velden *Valutacode*, *Transactiewijze* en *Bankrekening* waarden overgenomen vanuit de leverancierskaart van Jannet Carter. Daarom is in de velden *Valutacode*, *Transactiewijze* en *Bankrekening* respectievelijk *USD*, *ABN-USD* en *JCBA* ingevuld. Deze waarden kunnen echter worden gewijzigd.  
  
## <a name="create-proposal"></a>Voorstel maken  
 Open het venster Telebankieren - bankoverzicht en blader naar de bank die we voor onze betaling willen gebruiken. Open het venster Voorstel en genereer betalingsvoorstellen met de batchverwerking Voorstelposten ophalen.  
  
### <a name="example"></a>Voorbeeld  
 Door middel van het venster Telebank - bankoverzicht openen we het venster Voorstel voor onze bank *ABN*. Met de batchverwerking wordt één voorstelregel gemaakt voor de inkoopfactuur die we zojuist voor leverancier *JANNET* hebben gemaakt en geboekt.  
  
## <a name="create-payment-history"></a>Betaalrun maken  
 Vanuit het venster Voorstel verwerken we ons voorstel in een betaalrun. Het voorstel verdwijnt en kan worden gevonden in het venster Betaalrunoverzicht voor dezelfde bank.  
  
### <a name="example"></a>Voorbeeld  
 We verwerken ons voorstel met betrekking tot de betaling aan leverancier *JANNET* en openen het venster Betaalrunoverzicht voor onze bank *ABN-USD*. De laatste betaalrun is de betaalrun die we zojuist hebben gemaakt.  
  
## <a name="export-payment-history"></a>Betaalrun exporteren  
 Open het venster Betaalrunoverzicht, blader naar de relevante betaalrun en klik op **Exporteren**. De exportbatchverwerking voor het exportprotocol dat aan deze betaling is gekoppeld, verschijnt. Voor deze export zijn de juiste filters al automatisch ingevuld. Controleer desgewenst velden van het tabblad Opties en klik op OK om de betaling te exporteren. Er wordt een tekstbestand gegenereerd met een bestandsnaam zoals die is gedefinieerd in het veld Standaardbestandsnamen van het exportprotocol, dat nu gereed is voor verzending naar onze bank.  
  
### <a name="example"></a>Voorbeeld  
 Aangezien de transactiewijze die aan onze betaling is gekoppeld *ABN-USD* is, verschijnt de batchverwerking BBV of PAYMUL.  
  
## <a name="import-bank-statement"></a>Bankafschrift importeren  
 Nadat we elektronische bankafschriften van onze bank hebben ontvangen, kunnen we ze importeren door vanuit het venster Importprotocoloverzicht het betreffende importprotocol uit te voeren.  
  
### <a name="example"></a>Voorbeeld  
 Het bankafschrift met onze betaling aan Jannet Carter wordt door onze bank *ABN-USD* naar ons gestuurd. Daarom moeten we *OFFICE NET EXTRA* als het juiste importprotocol kiezen.  
  
## <a name="see-also"></a>Zie ook  
 [Procedure: Voorstellen maken](how-to-create-proposals.md)   
 [Procedure: Betalingsrun maken en exporteren](how-to-create-and-export-payment-history.md)

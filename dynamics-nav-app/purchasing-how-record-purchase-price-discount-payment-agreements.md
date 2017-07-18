---
title: 'Procedure: Inkoopprijzen en kortingen registreren'
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
ms.openlocfilehash: f99bb0aeef2c25048b0da3e0476ae2d612bff562
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

#<a name="how-to-record-purchase-prices-and-discounts"></a>Procedure: Inkoopprijzen en kortingen registreren
De verschillende prijs- en kortingsovereenkomsten die van toepassing zijn wanneer u koopt van verschillende leveranciers, moeten worden gedefinieerd, zodat de overeengekomen regels en waarden worden toegepast op documenten die u voor de leveranciers maakt.

U kunt een speciale inkoopprijs op inkoopregels laten invoegen als een bepaalde combinatie bestaat van leverancier, artikel, minimumaantal, maateenheid of begin- en einddatum.

U kunt twee soorten inkoopkortingen instellen en gebruiken:

|Type korting |Omschrijving |
|--------------|------------|
|**Inkoopregelkorting**|Een kortingsbedrag dat op inkoopregels wordt ingevoegd als een bepaalde combinatie bestaat van leverancier, artikel, minimumaantal, maateenheid of begin- en einddatum. Dit werkt op dezelfde manier als bij inkoopprijzen.|
|**Factuurkorting**|Een percentagekorting die van het documenttotaal wordt afgetrokken als het waardebedrag van alle regels in een inkoopdocument een bepaald minimum overschrijdt.|

Omdat inkoopregelkortingen en inkoopprijzen gebaseerd zijn op een combinatie van artikel en leverancier, kunt u deze configuratie ook invoeren vanuit de artikelkaart, waarop de regels en waarden zijn gedefinieerd. Zie voor meer informatie [Procedure: Nieuwe producten registreren](inventory-how-register-new-products.md).

## <a name="to-set-up-a-special-purchase-price-for-a-vendor"></a>Een speciale inkoopprijs voor een leverancier instellen
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Leveranciers** in en kies vervolgens de gerelateerde koppeling.
2. Open de desbetreffende leverancierskaart en kies vervolgens de actie **Prijzen**.

    Het veld **Soort inkoop** wordt vooraf ingevuld met **Leverancier** en het veld **Inkoopcode** wordt vooraf ingevuld met het leveranciersnummer.
3. Vul de velden indien nodig op de regel in. Kies een veld om een korte omschrijving van het veld of een koppeling naar meer informatie te lezen.
4. Vul een regel in voor elke combinatie waarvoor de leverancier u een inkoopregelkorting verleent.

## <a name="to-set-up-a-line-discount-for-a-vendor"></a>Een speciale regelkorting voor een leverancier instellen
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Leveranciers** in en kies vervolgens de gerelateerde koppeling.
2. Open de desbetreffende leverancierskaart en kies vervolgens de actie **Regelkortingen**.

    Het veld **Soort inkoop** wordt vooraf ingevuld met **Leverancier** en het veld **Inkoopcode** wordt vooraf ingevuld met het leveranciersnummer.
3. Vul de velden indien nodig op de regel in. Kies een veld om een korte omschrijving van het veld of een koppeling naar meer informatie te lezen.
4. Vul een regel in voor elke combinatie waarvoor de leverancier u een inkoopregelkorting verleent.

## <a name="to-set-up-an-invoice-discount-for-a-vendor"></a>Een factuurkorting voor een leverancier instellen
Wanneer uw leveranciers u hebben geïnformeerd welke factuurkortingen ze verlenen, voert u de factuurkortingscodes op de leverancierskaarten in en stelt u de condities voor elke code in.

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Leveranciers** in en kies vervolgens de gerelateerde koppeling.
2. Open de leverancierskaart voor een leverancier die voor factuurkortingen in aanmerking komt.
3. Selecteer in het veld **Factuurkortingscode** een code voor de desbetreffende factuurkortingscondities om te gebruiken voor het berekenen van factuurkortingen voor de leverancier.

    **Opmerking**: factuurkortingscodes worden weergegeven door bestaande leverancierskaarten. Zo kunt u snel factuurkortingscondities aan leveranciers toewijzen door de naam van een andere leverancier te kiezen die dezelfde condities heeft.

    Ga door met het instellen van de condities voor de nieuwe inkoopfactuurkorting.
4. Kies in het venster **Leverancierskaart** de actie **Factuurkortingen**. Het venster **Inkoopfactuurkortingen** verschijnt.
5. Geef in het veld **Valutacode** de code op voor een valuta waarvoor de factuurkortingscondities op de regel van toepassing zijn. Laat het veld leeg als u factuurkortingscondities in de lokale valuta wilt instellen.
6. Geef in het veld **Minimumbedrag** op hoe hoog het factuurbedrag minimaal moet zijn voordat een korting wordt berekend.
7. Voer in het veld **Korting %** de factuurkorting in als percentage van het factuurbedrag.
8. Herhaal stap 5 tot en met 7 voor elke valuta waarvoor de leverancier een andere factuurkorting ontvangt.

De factuurkorting is nu ingesteld en toegewezen aan de leverancier in kwestie. Wanneer u de leveranciercode selecteert in het veld **Factuurkortingscode** op andere leverancierskaarten, wordt dezelfde factuurkorting toegewezen aan die leverancier.

## <a name="see-also"></a>Zie ook  
[Inkoop instellen](purchasing-setup-purchasing.md)  
[Inkoop beheren](purchasing-manage-purchasing.md)


---
title: 'Procedure: Verkoopprijzen en kortingen registreren'
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
ms.openlocfilehash: 2d6438108fb2c36bb6f0d44efddc053bd628d068
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-record-sales-prices-and-discounts"></a>Procedure: Verkoopprijzen en kortingen registreren
De verschillende prijs- en kortingsovereenkomsten voor de verkoop aan verschillende klanten moeten zijn vastgesteld zodat de overeengekomen regels en waarden worden toegepast op verkoopdocumenten die u maakt voor de klanten.

U kunt een speciale verkoopprijs op verkoopregels laten invoegen als een bepaalde combinatie bestaat van klant, artikel, minimumaantal, maateenheid of begin- en einddatum.

U kunt twee soorten verkoopkortingen instellen en gebruiken:

|Type korting |Omschrijving |
|--------------|------------|
|**Verkoopregelkorting**|Een kortingsbedrag dat op verkoopregels wordt ingevoegd als een bepaalde combinatie bestaat van klant, artikel, minimumaantal, maateenheid of begin- en einddatum. Dit werkt op dezelfde manier als bij verkoopprijzen.|
|**Factuurkorting**|Een percentagekorting die van het documenttotaal wordt afgetrokken als het waardebedrag van alle regels in een verkoopdocument een bepaald minimum overschrijdt.|

Doordat verkoopprijzen en verkoopregelkortingen worden gebaseerd op een combinatie van artikel en klant, kunt u dit ook configureren vanaf de artikelkaart van het artikel waarop de regels en waarden van toepassing zijn.

## <a name="to-set-up-a-sales-price-for-a-customer"></a>Een verkoopprijs voor een klant instellen
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Klanten** in en kies vervolgens de gerelateerde koppeling.
2. Open de desbetreffende klantenkaart en kies vervolgens de actie **Prijzen**.

    Het veld **Verkoopsoort** wordt vooraf ingevuld met de waarde **Klant** en het veld **Verkoopcode** wordt vooraf ingevuld met het klantnummer.
3. Vul de velden indien nodig op de regel in. Kies een veld om een korte omschrijving van het veld of een koppeling naar meer informatie te lezen.
4. Vul een regel in voor elke combinatie waarmee een speciale verkoopprijs aan de klant wordt verleend.

## <a name="to-set-up-a-sales-line-discount-for-a-customer"></a>Een verkoopregelkorting instellen voor een klant
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Klanten** in en kies vervolgens de gerelateerde koppeling.
2. Open de desbetreffende klantenkaart en kies vervolgens de actie **Regelkortingen**.

    Het veld **Verkoopsoort** wordt vooraf ingevuld met de waarde **Klant** en het veld **Verkoopcode** wordt vooraf ingevuld met het klantnummer.
3.  Vul de velden indien nodig op de regel in. Kies een veld om een korte omschrijving van het veld of een koppeling naar meer informatie te lezen.
4. Vul een regel in voor elke combinatie waarmee een speciale verkoopregelkorting aan de klant wordt verleend.

## <a name="to-set-up-an-invoice-discount-for-a-customer"></a>Een factuurkorting voor een klant instellen
Wanneer u hebt bepaald welke klanten in aanmerking komen voor factuurkortingen, geeft u de factuurkortingscode op de klantenkaarten op en stelt u de voorwaarden voor elke code in.

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Klanten** in en kies vervolgens de gerelateerde koppeling.
2. Open de klantenkaart voor een klant die voor factuurkortingen in aanmerking komt.
3. Selecteer in het veld **Factuurkortingscode** een code voor de desbetreffende factuurkortingsvoorwaarden die moeten worden gehanteerd voor het berekenen van factuurkortingen voor de klant.

    **Opmerking**: factuurkortingscodes worden vertegenwoordigd door bestaande klantenkaarten. Zo kunt u snel factuurkortingsvoorwaarden aan klanten toewijzen door de naam van een andere klant te kiezen die dezelfde voorwaarden heeft.

    Ga door met het instellen van de nieuwe voorwaarden voor de nieuwe verkoopfactuurkorting.
4. Kies in het venster **Klantenkaart** de actie **Factuurkortingen**. Het venster **Verkoopfactuurkorting** verschijnt.
5. Geef in het veld **Valutacode** de code op voor een valuta waarvoor de factuurkortingscondities op de regel van toepassing zijn. Laat het veld leeg als u factuurkortingscondities in de lokale valuta wilt instellen.
6. Geef in het veld **Minimumbedrag** op hoe hoog het factuurbedrag minimaal moet zijn voordat een korting wordt berekend.
7. Voer in het veld **Korting %** de factuurkorting in als percentage van het factuurbedrag.
8. Herhaal stap 5 tot en met 7 voor elke valuta waarvoor de klant een andere factuurkorting ontvangt.

De factuurkorting is nu ingesteld en toegewezen aan de klant in kwestie. Wanneer u de klantcode selecteert in het veld **Factuurkortingscode** op andere klantenkaarten, wordt dezelfde factuurkorting toegewezen aan die klanten.

## <a name="see-also"></a>Zie ook  
[Verkopen instellen](sales-setup-sales.md)  
[Verkoop beheren](sales-manage-sales.md)


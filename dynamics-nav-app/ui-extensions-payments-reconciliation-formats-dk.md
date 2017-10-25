---
title: De extensie Afsstemingen en betalingen (DK) gebruiken
description: Deze extensie maakt het eenvoudig bestanden te exporteren die vooraf zijn ingedeeld om te voldoen aan de vereisten van de bank betreffende elektronische verzendingen.
author: bholtorf
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: extension, bank, formats
ms.date: 09/15/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 226dc84494a1bfb979c6e230f14f0826c963adc9
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---

# <a name="the-payments-and-reconciliations-dk-extension-for-microsoft-dynamics-for-finance-and-operations-business-edition"></a>De extensie Betalingen en afstemmingen (DK) voor Microsoft Dynamics for Finance and Operations, Business edition
Snelle, foutloze betalingen doen door bestanden te exporteren die specifiek voor uitwisselingen met uw leverancier of bank zijn ingedeeld. Deze bestanden versnellen de betalings- en afstemmingprocessen, en voorkomen fouten die kunnen optreden als u handmatig de gegevens op een bankwebsite invoert.  
  
De extensie ondersteunt bestandsindelingen voor diverse Deense banken. Wanneer u betalingsgegevens naar een bestand exporteert, verpakt de extensie de gegevens in de indeling die door de bank wordt vereist. Deze indelingen zijn onder andere Bankdata-vl, BEC, SDC en FIK, die door allerlei banken worden gebruikt, en een aantal dat specifieker voor bepaalde banken is, zoals Danske Bank en Nordea. De extensie bevat ook sommige indelingen voor het importeren van en de reconciliatie van bankafschriften.  
  
> [!Note]
> Als u de extensie wilt gebruiken, moet u weten welke indeling voor uw bank of leverancier is vereist. Sommige banken of leveranciers verstrekken deze informatie op hun website, maar het kan ook nodig zijn om contact op te nemen met hun klantenservice om deze informatie op te vragen.  
  
## <a name="supported-bank-formats"></a>Indelingen voor banken die worden ondersteund
De extensie kan de volgende activiteiten voor betalingbestanden vereffenen:  
  
* Bankdata-V3  
* BEC-INDLAND  
* BEC-CSV  
* DANSKEBANK-CMKV  
* DANSKEBANK-CMKXKSX  
* DANSKEBANK  
* FIK71  
* NORDEA-ERHVERV-CSV  
* NORDEA  
* NORDEA-UNITEL-V3  
* SDC  
* SDC-CSV  

## <a name="to-set-up-the-extension"></a>De extensie instellen
Er zijn een aantal stappen vereist als u aan de slag wilt.  
  
* Sta het exporteren van betalingsgegevens toe. Ter bescherming van uw gegevens, is dit niet direct beschikbaar.  
* Stel inkoop en crediteuren in, zodat externe documentnummers op facturen niet zijn vereist. Indien nodig kunt u het referentienummer gebruiken om naar een bepaalde factuur te verwijzen.  
* Geef de betalingswijze voor elke leverancier op. Betalingswijzen bepalen hoe u facturen van de leverancier betaalt. Bijvoorbeeld bank, contant, cheque of rekening.  
* Geef het type indeling op dat voor elk van uw bankrekeningen moet worden gebruikt. Voorbeelden zijn NORDEA, DANSKEBANK, SDC enzovoort.  
  
Daarnaast moet u leveranciers toewijzen aan een binnenlandse **bedrijfsboekingsgroep** en een **leveranciersboekingsgroep**. De instelling Land/regio voor de leverancier moet Denemarken (DK) zijn. Zie [Boekingsgroepen instellen](finance-posting-groups.md) voor meer informatie.  
  
### <a name="to-allow-included365finincludesd365finmdmd-to-export-payment-data"></a>[!INCLUDE[d365fin](includes/d365fin_md.md)] toestaan betalingsgegevens te exproteren
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Betalingsdagboek** in en klik vervolgens op de gerelateerde koppeling.  
2. Kies in het venster **Betalingsdagboek bewerken** de batch **Bank**.  
3. Schakel het selectievakje **Exporteren betaling toestaan** in.  

### <a name="to-specify-a-payment-method-for-a-vendor"></a>Een betalingswijze voor een leverancier opgeven
De volgende tabel bevat de combinaties van de betalingswijzen FIK en GIRO die door [!INCLUDE[d365fin](includes/d365fin_md.md)] worden ondersteund.

||Soort 01 | Soort 04 | Soort 71 | Soort 73 |
|----|---|---|---|---|
|Girorekeningnr of FIK-crediteurennr? | Girorekeningnr | Girorekeningnr | FIK-crediteurennummer | FIK-crediteurennummer|
|Bericht aan ontvanger toestaan? | Ja |Nr. |Nr. | Ja |
|Bevat betalingreferentienummer? | Nr. | Ja, 16 cijfers. | Ja, 15 cijfers. | Nr.|

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Leveranciers** in en klik vervolgens op de gerelateerde koppeling.  
2. Open de kaart, vouw het tabblad **Betalingen** uit, kies in het veld **Betalingswijze** de betalingswijze.  
3. Afhankelijk van uw selectie moet u andere velden invullen. Zie de bovenstaande tabel voor een omschrijving van de combinaties.  

### <a name="to-specify-the-format-to-use-for-a-bank-account"></a>De indeling opgeven die voor een bankrekening moet worden gebruikt
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Bankrekeningen** in en klik vervolgens op de gerelateerde koppeling.  
2. Open de kaart voor de bankrekening.  
3. In het veld **Exportindeling betaling** kiest u de indeling voor uw exportbestand.  

## <a name="choosing-the-fik-or-giro-payment-information-for-vendor-invoices"></a>De betalingsgevens FIK of Giro voor facturen van leveranciers kiezen
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Inkoopfacturen** in en klik vervolgens op de gerelateerde koppeling.
2. Kies de leverancier. Dit moet een Deense leverancier zijn met een adres in Denemarken.
3. Maak een factuur. De velden **Betalingswijze** en **Leveranciersnummer** worden ingevuld op basis van instellingen op de leverancierskaart. U kunt desgewenst wijzigingen aanbrengen.
4. In het veld **Betalingsreferentie** voert u het nummer van 15 cijfers van de factuur van de leverancier in. 
  
    > [!Tip]
    > U hoeft slechts de laatste 11 cijfers van het nummer toe te voegen. Dynamics NAV voegt vier nullen aan het begin van het nummer toe.  
  <!--ASK ANDREI WHY AND WHAT THIS NUMBER IS-->
5. Boek de factuur.

## <a name="to-use-the-extension-to-export-payment-data"></a>De extensie gebruiken om betalingsgegevens te exporteren
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Betalingsdagboeken** in en klik vervolgens op de gerelateerde koppeling.  
2. Kies de actie **Leveranciersbetalingsdagboeken voorstellen**.  
  
    > [!Tip]
    > Als u alleen bepaalde betalingen wilt exporteren, gebruikt u de opties om de gegevens te filteren.  
  
3. Indien nodig kunt u filters toevoegen als u alleen bepaalde betalingen wilt exporteren.  
4. Selecteer **Elektronische betaling** in het veld **Betalingssoort**.  
5. Kies de actie **Exporteren**.  

## <a name="see-also"></a>Zie ook 
[Dynamics NAV aanpassen met behulp van extensies](ui-extensions.md)  
[Procedure: SEPA-verzamelingsposten van automatische incasso maken en exporteren naar een bankbestand](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md)  
[Procedure: Automatische incasso via SEPA instellen](finance-how-to-set-up-sepa-direct-debit.md)  
[Procedure: SEPA-betalingsontvangsten via automatische incasso boeken](finance-how-to-post-sepa-direct-debit-payment-receipts.md)  
[Betalingen verzamelen via automatische incasso van SEPA](finance-collect-payments-with-sepa-direct-debit.md)  
[Werken met diversendagboeken](ui-work-general-journals.md)  






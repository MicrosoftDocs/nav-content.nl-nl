---
title: Veldtoewijzing bij het importeren van SEPA CAMT-bestanden
description: In Europese markten kunt u bankafschriftbestanden in de regionale SEPA-norm (Single Euro Payments Area) importeren.
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/18/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 88f949bb211845a1c3c0e5f0b364d4ea26cfd13f
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="field-mapping-when-importing-sepa-camt-files"></a>Veldtoewijzing bij het importeren van SEPA CAMT-bestanden
[!INCLUDE[d365fin](includes/d365fin_md.md)] ondersteunt de regionale SEPA-norm (Single Euro Payments Area) voor het importeren van SEPA-bankafschriften (CAMT-indeling). Zie voor meer informatie [Procedure: De conversieservice bankgegevens instellen](bank-how-setup-bank-data-conversion-service.md).  

 De SEPA CAMT-standaard heeft zelf lokale variaties. U moet daarom mogelijk de algemene definitie voor gegevensuitwisseling, aangeduid door de code **SEPA CAMT** in het venster **Uitwisselingsdefinities van boeking**, wijzigen om deze aan de lokale variant van de vaste verrekenprijs aan te passen. De volgende tabellen tonen de element-aan-veld-toewijzing voor tabellen 81, 273 en 274 in de SEPA CAMT-implementatie in [!INCLUDE[d365fin](includes/d365fin_md.md)].  

 Voor informatie over het maken of het aanpassen van de definitie van gegevensuitwisseling raadpleegt u [Procedure: Definities voor gegevensuitwisseling instellen](across-how-to-set-up-data-exchange-definitions.md).  

## <a name="camt-data-mapping-to-fields-in-the-general-journal-table-81"></a>CAMT-gegevenstoewijzing aan velden in de tabel Dagboek (81)  

|Elementpad|Berichtelement|Gegevenssoort|Omschrijving|Identificatie voor een negatief teken|Veldnr.|Veldnaam|  
|------------------|---------------------|---------------|-----------------|-------------------------------|---------------|----------------|  
|Stmt/Ntry/Amt|Bedrag|Decimaal|Het geldbedrag in de kaspost||13|Bedrag|  
|Stmt/Ntry/CdtDbtInd|CreditDebitIndicator|Tekst|Geeft aan of de post een credit- of een debetpost is|DBIT|13|Bedrag|  
|Stmt/Ntry/BookgDt/Dt|Datum|Datum|De datum waarop een post wordt geboekt naar een rekening in de boeken van de rekeningservice||5|Boekingsdatum|  
|Stmt/Ntry/BookgDt/DtTm|DateTime|DateTime|De datum en tijd waarop een post wordt geboekt naar een rekening in de boeken van de rekeningservice||5|Boekingsdatum|  
|Stmt/Ntry/NtryDtls/TxDtls/RltdPties/Dbtr/Nm|Naam|Tekst|De naam van de partij die een geldbedrag is verschuldigd aan de (uiteindelijke) incassant||1221|Informatie over betaler|  
|Stmt/Ntry/NtryDtls/TxDtls/RmtInf/Ustrd|Ongestructureerd|Tekst|Informatie die wordt verschaft om de afstemming/reconciliatie mogelijk te maken van een post met de artikelen die de betaling wordt geacht te vereffenen, zoals commerciële facturen in een vorderingsysteem, in een ongestructureerde vorm||8|Omschrijving|  
|Stmt/Ntry/AddtlNtryInf|AdditionalEntryInformation|Tekst|Extra informatie over de invoer||1222|Transactie-informatie|  

## <a name="camt-data-mapping-to-fields-in-the-bank-acc-reconciliation-table-273"></a>CAMT-gegevenstoewijzing aan velden in de tabel Bankreconciliatie (273)  

|Elementpad|Berichtelement|Gegevenssoort|Omschrijving|Identificatie voor een negatief teken|Veldnr.|Veldnaam|  
|------------------|---------------------|---------------|-----------------|-------------------------------|---------------|----------------|  
|Stmt/CreDtTm|CreationDateTime|Datum|De datum en tijd waarop het bericht is gemaakt.||3|Afschriftdatum|  
|Stmt/Bal/Amt|Bedrag|Decimaal|Het bedrag dat resulteert uit de tot een nettowaarde teruggebrachte bedragen voor alle debet- en creditposten||4|Eindsaldo afschrift|  

## <a name="camt-data-mapping-to-fields-in-the-bank-acc-reconciliation-line-table-274"></a>CAMT-gegevenstoewijzing aan velden in de tabel Bankreconciliatieregel (274)  

|Elementpad|Berichtelement|Gegevenssoort|Omschrijving|Identificatie voor een negatief teken|Veldnr.|Veldnaam|  
|------------------|---------------------|---------------|-----------------|-------------------------------|---------------|----------------|  
|Stmt/Ntry/Amt|Bedrag|Decimaal|Het geldbedrag in de kaspost||7|Afschrifttotaal|  
|Stmt/Ntry/CdtDbtInd|CreditDebitIndicator|Tekst|Geeft aan of de post een credit- of een debetpost is|DBIT|7|Afschrifttotaal|  
|Stmt/Ntry/BookgDt/Dt|Datum|Datum|De datum waarop een post wordt geboekt naar een rekening in de boeken van de rekeningservice||5|Transactiedatum|  
|Stmt/Ntry/BookgDt/DtTm|DateTime|DateTime|De datum en tijd waarop een post wordt geboekt naar een rekening in de boeken van de rekeningservice||5|Transactiedatum|  
|Stmt/Ntry/ValDt/Dt|Datum|Datum|De datum waarop activa beschikbaar worden voor de rekeninghouder in het geval van een creditpost, of niet meer beschikbaar zijn voor de rekeninghouder in het geval van een debetpost||12|Waardedatum|  
|Stmt/Ntry/ValDt/DtTm|DateTime|DateTime|De datum en tijd waarop activa beschikbaar worden voor de rekeninghouder in het geval van een creditpost, of niet meer beschikbaar zijn voor de rekeninghouder in het geval van een debetpost||12|Waardedatum|  
|Stmt/Ntry/NtryDtls/TxDtls/RltdPties/Dbtr/Nm|Naam|Tekst|De naam van de partij die een geldbedrag is verschuldigd aan de (uiteindelijke) incassant||15|Informatie over betaler|  
|Stmt/Ntry/NtryDtls/TxDtls/RmtInf/Ustrd|Ongestructureerd|Tekst|Informatie die wordt verschaft om de afstemming/reconciliatie mogelijk te maken van een post met de artikelen die de betaling wordt geacht te vereffenen, zoals commerciële facturen in een vorderingsysteem, in een ongestructureerde vorm||6|Omschrijving|  
|Stmt/Ntry/AddtlNtryInf|AdditionalEntryInformation|Tekst|Extra informatie over de invoer||16|Transactie-informatie|  

 Elementen in het knooppunt **Ntry** die worden geïmporteerd in [!INCLUDE[d365fin](includes/d365fin_md.md)] maar niet aan velden worden toegewezen, worden opgeslagen in de tabel **Kolomdef. boekingsuitwisseling**. Gebruikers kunnen deze elementen vanuit de vensters **Betalingsreconciliatiedagboek**, **Betalingsvereffening** en **Bankreconciliatie** weergeven door de actie **Details bankrekeningafschriftregel** te kiezen. Zie voor meer informatie [Procedure: Betalingen reconciliëren met automatische vereffening](receivables-how-reconcile-payments-auto-application.md).  
## <a name="see-also"></a>Zie ook  
[Gegevensuitwisseling instellen](across-set-up-data-exchange.md)  
[Gegevens elektronisch uitwisselen](across-data-exchange.md)  
[Procedure: Conversieservice voor bankgegevens instellen](bank-how-setup-bank-data-conversion-service.md)   
[Procedure: XML-schema's gebruiken om gegevensuitwisselingsdefinities voor te bereiden](across-how-to-use-xml-schemas-to-prepare-data-exchange-definitions.md)  
[Procedure: Betalingen reconciliëren met automatische vereffening](receivables-how-reconcile-payments-auto-application.md)  


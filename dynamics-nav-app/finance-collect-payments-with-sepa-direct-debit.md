---
title: SEPA Automatische incasso in Dynamics NAV
description: U kunt betalingen rechtstreeks van de bankrekening van de klant verzamelen volgens de SEPA-indeling.
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 9ead1f76883e3c8d98bef8c61175766ccf1414e7
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="collecting-payments-with-sepa-direct-debit"></a>Betalingen verzamelen via automatische incasso van SEPA
Met instemming van de klant, kunt u betalingen rechtstreeks vanaf de bankrekening van de klant verzamelen volgens de SEPA-notatie.  

 Stel eerst de exportindeling van het bankbestand in waarmee u uw bank opdracht geeft een automatische incasso uit te voeren. Installeer vervolgens de betalingswijze van de klant. Stel tot slot de machtiging voor automatische incasso in die overeenkomt met uw overeenkomst met de klant voor het verzamelen van hun betalingen in een bepaalde overeenkomstperiode.  

 Om de bank het bedrag van de bankrekening van de klant over te laten brengen naar de account van uw bedrijf, moet u een verzameling van incasso maken met gegevens over bankrekeningen, de betrokken verkoopfacturen en de incassomachtiging. U exporteert vervolgens een XML-bestand dat is gebaseerd op de verzamelingspost en verzendt dat naar uw bank voor verwerking. Betalingen die niet konden worden verwerkt worden aan u gemeld door uw bank. U moet vervolgens handmatig de desbetreffende verzamelingsposten van automatische incasso weigeren.  

 U kunt standaardklantenverkoopcodes instellen met de informatie over de betalingsmethode voor automatische incasso en de machtigingen voor automatische incasso. Vervolgens kunt u de batchverwerking **Std. klantfacturen maken** gebruiken om meerdere verkoopfacturen te genereren waarvoor de gegevens voor automatische incasso automatisch zijn ingevuld. Dit kan handmatig of automatisch worden uitgevoerd volgens de vervaldatum van de betaling.  

 Wanneer betalingen met succes worden verwerkt, zoals aangegeven door uw bank, kunt u de betalingsontvangsten rechtstreeks vanuit het venster **Verzamelingsposten van incasso** boeken of door de betalingsregels naar het dagboek te verplaatsen waarin u betalingsontvangsten boekt, zoals in het venster **Ontvangstendagboek**. Afhankelijk van uw proces voor kasbeheer kunt u ook wachten en de betalingen alleen vereffenen als onderdeel van de bankreconciliatie.  

> [!NOTE]  
>  Om betalingen te innen via SEPA Incasso, moet de valuta op de verkoopfactuur EURO zijn.  

 In de volgende tabel wordt een reeks taken beschreven, met koppelingen naar de beschrijvende onderwerpen.   

|**Als u dit wilt doen**|**Zie**|  
|------------|-------------|  
|Bankrekening-indelingen, betalingsmethoden en klant overeenkomsten voor automatische incasso van SEPA voorbereiden.|[Procedure: Automatische incasso via SEPA instellen](finance-how-to-set-up-sepa-direct-debit.md)|  
|Vraag uw bank bedragen van betalingen van bankrekeningen van uw klanten over te brengen naar uw bedrijfsrekening volgens uw instellingen voor automatische incasso van SEPA.|[Procedure: SEPA-verzamelingsposten van automatische incasso maken en exporteren naar een bankbestand](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md)|  
|Standaard klantverkoopcodes voor automatische incasso-facturen instellen en verkoopfacturen met automatische incasso-informatie genereren wanneer de facturen betaald moeten worden.|[Procedure: Periodieke verkoop- en inkoopregels maken](sales-how-work-standard-lines.md)|  
|Betalingen gemaakt als SEPA-incasso's boeken.|[Procedure: SEPA-betalingsontvangsten via automatische incasso boeken](finance-how-to-post-sepa-direct-debit-payment-receipts.md)|  

## <a name="see-also"></a>Zie ook  
[Tegoeden beheren](receivables-manage-receivables.md)


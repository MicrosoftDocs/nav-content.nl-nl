---
title: De methode voor elektronische betalingen kiezen
description: Verwerk betalingen aan uw leveranciers door samen met de betalingsgegevens van de dagboekregels een bestand te exporteren.
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: baafa833fb170fb05f866aac91a05085545aaf97
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer"></a>Betalingen verrichten met de conversieservice van bankgegevens of SEPA-overmaking
U kunt in het venster **Betalingsdagboek** betalingen naar uw leveranciers verwerken door samen met de betalingsgegevens van de dagboekregels een bestand te exporteren. Vervolgens kunt u het bestand uploaden naar uw elektronische banksite waar de gerelateerde overboekingen worden verwerkt. [!INCLUDE[d365fin](includes/d365fin_md.md)] ondersteunt de indeling voor SEPA-kredietoverboekingen, maar in uw land of regio kunnen andere indelingen voor elektronische betalingen beschikbaar zijn.   

 Voor het mogelijk maken van SEPA-kredietoverboekingen moet u eerst een bankrekening, leverancier, en dagboekbatch instellen waarop het betalingsdagboek is gebaseerd. Bereid vervolgens betalingen aan leveranciers voor door het venster **Betalingsdagboek** automatisch te vullen met verschuldigde betalingen met een opgegeven boekingsdatum.  

> [!NOTE]  
>  Wanneer u hebt gecontroleerd dat de betalingen zijn verwerkt door de bank, kunt u doorgaan met het boeken van de betalingsdagboekregels.  

 In de volgende tabel wordt een reeks taken beschreven, met koppelingen naar de beschrijvende onderwerpen.   

|**Als u dit wilt doen**|**Zie**|  
|------------|-------------|  
|Activeer de conversieservice voor bankgegevens om een bankafschriftbestand te laten converteren naar een indeling die u kunt importeren of om uw geëxporteerde betalingsbestanden te laten converteren naar de indeling die uw bank vereist.|[Procedure: Conversieservice voor bankgegevens instellen](bank-how-setup-bank-data-conversion-service.md)|  
|Stel een bankrekening, leverancier en betalingsdagboek in voor SEPA-kredietoverboeking.|[Procedure: SEPA-krediettransfer instellen](finance-how-to-set-up-sepa-credit-transfer.md)|  
|Vul het betalingsdagboek met regels voor verschuldigde betalingen aan leveranciers, met de mogelijkheid boekingsdatums in te voegen op basis van de vervaldatum van de verwante inkoopdocumenten.|[Betalingsverplichtingen beheren](payables-manage-payables.md)|  
|Exporteer betalingsdagboekregels naar een bestand in de SEPA-overmakingsindeling.|[Procedure: Betalingen naar een bankbestand exporteren](payables-how-export-payments-bank-file.md)|  
|Controleer welke betalingen zijn geëxporteerd en in welke bestanden.|Krediettransferregisters|  
|Wanneer de elektronische betaling is verwerkt door de bank, boekt u de betalingen.|[Werken met diversendagboeken](ui-work-general-journals.md)|  

## <a name="see-also"></a>Zie ook  
[Procedure: Conversieservice voor bankgegevens instellen](bank-how-setup-bank-data-conversion-service.md)  
[Procedure: SEPA-krediettransfer instellen](finance-how-to-set-up-sepa-credit-transfer.md)  
[Betalingsverplichtingen beheren](payables-manage-payables.md)   
[Werken met diversendagboeken](ui-work-general-journals.md)  
[Betalingen verzamelen via automatische incasso van SEPA](finance-collect-payments-with-sepa-direct-debit.md)   


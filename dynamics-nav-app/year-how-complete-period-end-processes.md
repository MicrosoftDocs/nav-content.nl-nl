---
title: Optionele activiteiten voor het afsluiten van periodes
description: Dit onderwerp schetst de optionele processen en activiteiten voor het sluiten van boekingsperioden in Dynamics NAV.
documentationcenter: 
author: jswymer
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: year closing, close accounting period, close fiscal year, aging, creditor payments, vendor payments
ms.date: 06/19/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: ca22e72552c69d3bcb0b85101b586796ff026896
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="overview-of-tasks-to-close-accounting-periods"></a>Overzicht van taken voor het sluiten van boekingsperioden
[!INCLUDE[d365fin](includes/d365fin_md.md)] dwingt u niet om perioden te sluiten, maar er zijn veel activiteiten voor periode-einden (maandeinden) die u kunt uitvoeren. In dit onderwerp vindt u een overzicht van optionele processen en activiteiten voor het afsluiten van perioden.  

## <a name="general-ledger"></a>Grootboek
* Geef de boekingsperioden voor het gehele systeem of een specifieke gebruiker op.  

    Hiermee worden de datums opgegeven waartussen u boekingen wilt toestaan. Afhankelijk van uw zakelijke processen wilt u het boeken mogelijk toestaan aan het begin of juist aan het einde van de periode. Zie [Procedure: Boekingsperioden opgeven](finance-how-specify-posting-periods.md) voor meer informatie.  
* Voer alle noodzakelijke grootboekherwaarderingen uit.  
* Wijzig en boek periodieke dagboeken.  
  <!--* Process Consolidations-->
* Voer rapportageschema's als volgt uit:  
  * Open het venster **Rapportageschema** en kies de actie **Afdrukken**.  

## <a name="sales-and-receivables"></a>Verkopen en tegoeden
* Boek alle verkooporders, facturen, creditnota's en retourorders.  
* Boek alle ontvangstendagboeken.  
* Wijzig en boek periodieke dagboeken die zijn gerelateerd aan Verkoop.  
* Reconcilieer klanten met het grootboek.  
* Voer de batchverwerking **Gefactureerde verkooporders verwijderen** uit.  

## <a name="purchases-and-payables"></a>Inkopen en schulden
* Boek alle inkooporders, facturen, creditnota's en retourorders.  
* Boek alle betalingsdagboeken.  
* Wijzig en boek periodieke dagboeken die zijn gerelateerd aan Inkoop.  
* Voer het rapport **Vervallen betalingen** uit en reconcilieer leveranciers met het grootboek.  
* Voer de batchverwerking **Gefactureerde inkooporders verwijderen** uit.  

Vast activum
* Boek alle onderhoudskosten via de VA-dagboeken of Facturen.
* Boek herwaarderingen.
* Boek waardevermeerdering.
* Boek afschrijving.
* Wijzig en boek het periodiek VA-dagboek.

Intercomp
* IC-transacties verwerken

## <a name="calculate-and-process-sales-tax"></a>Btw berekenen en verwerken
* Vul belastingaangiften in.  

## <a name="see-also"></a>Zie ook
[Afsluitingsjaren en -perioden](year-close-years-periods.md)  
[Boeken afsluiten](year-close-books.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


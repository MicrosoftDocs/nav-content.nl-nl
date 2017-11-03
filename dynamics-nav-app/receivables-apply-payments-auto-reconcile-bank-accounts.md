---
title: "Taken om bankrekeningen te reconciliëren en betalingen te vereffenen met gerelateerde posten"
description: "Schetst taken om uw bank-, tegoeden- en schuldenrekeningen te reconciliëren, kasontvangsten of onkosten te boeken en betalingen automatisch te vereffenen."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: payment process, direct payment posting, reconcile payment, expenses, cash receipts
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 33c0661a2ebf9b8d9b817c026a8c9abf0f0eff91
ms.contentlocale: nl-nl
ms.lasthandoff: 10/23/2017

---
# <a name="applying-payments-automatically-and-reconciling-bank-accounts"></a>Betalingen automatisch vereffenen en bankrekeningen reconciliëren
U moet regelmatig uw bankrekening en de rekeningen met tegoeden en betalingsverplichtingen reconciliëren, door betalingen die op de bank zijn vastgelegd te vereffenen met de gerelateerde onbetaalde facturen en creditnota's of andere openstaande posten in [!INCLUDE[d365fin](includes/d365fin_long_md.md)].  

U kunt deze taak in het venster **Dagboek betalingsreconciliatie** uitvoeren door een bankafschriftbestand of -feed te importeren om de betalingen snel in project te registreren. Betalingen worden vereffend met openstaande leveranciers- of klantenposten, op basis van overeenkomsten tussen de betalingtekst en de informatie in de posten. U kunt automatische vereffeningen controleren en wijzigen voordat u het dagboek boekt. U kunt ervoor kiezen om openstaande bankrekeningposten met betrekking tot de vereffende posten te sluiten wanneer u het dagboek boekt. De bankrekening wordt automatisch gereconcilieerd wanneer alle betalingen worden vereffend.  

Als u bankafschriften wilt kunnen importeren als bankfeed, moet u eerst de conversieservice voor bankgegevens instellen en inschakelen. Zie voor meer informatie [Procedure: De conversieservice bankgegevens instellen](bank-how-setup-bank-data-conversion-service.md).  

In de volgende tabel wordt een reeks taken beschreven, met koppelingen naar de beschrijvende onderwerpen.  

| Als u dit wilt doen | Zie |
| --- | --- |
| Vereffen betalingen om klant- of leveranciersposten te openen door een bankafschrift te importeren en de bankrekening te reconciliëren wanneer alle betalingen zijn vereffend. |[Procedure: Betalingen reconciliëren met automatische vereffening](receivables-how-reconcile-payments-auto-application.md) |
| Vereffen handmatig betalingen door gedetailleerde informatie over afgestemde gegevens weer te geven en suggesties voor openstaande kandidaatposten om betalingen mee te vereffenen. |[Procedure: Betalingen na automatische vereffening controleren of vereffenen](receivables-how-review-apply-payments-auto-application.md) |
| Betalingen oplossen die niet automatisch met de gerelateerde openstaande posten kunnen worden vereffend. Bijvoorbeeld omdat bedragen afwijken, of omdat geen gerelateerde post bestaat. |[Procedure: Betalingen reconciliëren die niet automatisch kunnen worden vereffend](receivables-how-reconcile-payments-cannot-apply-auto.md) |
| Koppel tekst op betalingen aan specifieke klant-, leverancier- of grootboekrekeningen om periodieke ontvangsten of kosten altijd naar deze rekeningen te boeken als er geen documenten zijn voor vereffening. |[Procedure: Tekst op herhalende betalingen aan rekeningen toewijzen voor automatische afstemming](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md) |

## <a name="see-also"></a>Zie ook
[Tegoeden beheren](receivables-manage-receivables.md)  
[Verkoop](sales-manage-sales.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


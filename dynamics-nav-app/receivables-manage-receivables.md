---
title: Tegoeden beheren
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 3f2be627dfda9720e9f31fd227164d1c27116d2c
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="manage-receivables"></a>Tegoeden beheren#
Een centrale taak in het beheren van tegoeden is het vereffenen van inkomende betalingen met de relateerde klant- of leveranciersposten en daarmee de gerelateerde verkoopfacturen of inkoopcreditnota's als betaald te sluiten. Wanneer alle betalingen zijn vereffend, kunt u de bankrekening reconciliëren.  

U kunt deze taak in het venster **Dagboek betalingsreconciliatie** uitvoeren door een bankafschriftbestand of -feed te importeren om de betalingen snel in Dynamics NAV te registreren. Met een automatische vereffeningsfunctie worden de betalingen vereffend met de gerelateerde openstaande leveranciers- of klantposten op basis van gegevensovereenkomsten tussen betalingstekst en postgegevens. U kunt automatische vereffeningen controleren en wijzigen voordat u het dagboek boekt. U kunt ervoor kiezen om openstaande bankrekeningposten met betrekking tot de vereffende posten te sluiten wanneer u het dagboek boekt. Dit betekent dat de bankrekening automatisch wordt gereconcilieerd wanneer alle betalingen worden vereffend.

**Opmerking**: u kunt bankrekeningen reconciliëren als een aparte taak in het venster **Bankreconciliatie**, inclusief chequeposten. Zie [Procedure: Bankrekeningen apart reconciliëren](bank-how-reconcile-bank-accounts-separately.md) voor meer informatie.

U kunt betalingen ook vereffenen in het venster **Betalingsregistratie** door betalingen die zijn ontvangen als contant, cheque of banktransactie, handmatig te controleren aan de hand van een gegenereerde lijst met niet-betaalde verkoopdocumenten. Deze functionaliteit is alleen beschikbaar voor verkoopdocumenten.

Als andere handmatige reconciliatie van betalingen kunt u elke ontvangst naar de betreffende grootboek-, klant-, of andere rekening boeken door een betalingsregel in het venster **Ontvangstendagboek** in te voeren. In dat geval kunt u de ontvangst of terugbetaling vereffenen met een of meer openstaande posten voordat u het ontvangstendagboek boekt of u kunt de vereffening uitvoeren via de gemaakte klantposten.

Een andere taak bij het beheer van tegoeden is het innen van openstaande saldi, inclusief het beheer van rentefacturen en versturen van aanmaningen.

In de volgende tabel wordt een reeks taken beschreven, met koppelingen naar de beschrijvende onderwerpen.

|Als u dit wilt doen |Zie |
|---|----|
|Vereffen betalingen om klant- of leveranciersposten te openen op basis van een geïmporteerd bankafschriftbestand of een bankfeed en de bankrekening te reconciliëren wanneer alle betalingen zijn vereffend.|[Betalingen automatisch vereffenen en bankrekeningen reconciliëren](receivables-apply-payments-auto-reconcile-bank-accounts.md)|
|Vereffen betalingen met openstaande klantposten op basis van handmatige invoer in een lijst met onbetaalde verkoopdocumenten. | [Procedure: Klantbetalingen van een lijst met onbetaalde verkoopdocumenten handmatig reconciliëren](receivables-how-reconcile-customer-payments-list-unpaid-sales-documents.md)|
|Boek ontvangsten of terugbetalingen voor klanten in het ontvangstendagboek en vereffen deze met klantposten via het dagboek of via geboekte posten. | [Procedure: Klantbetalingen handmatig reconciliëren](receivables-how-apply-sales-transactions-manually.md) |
|Klanten te herinneren aan achterstallige bedragen, rente en rentefacturen berekenen en rekeningen met vorderingen beheren. | [Procedure: Openstaande saldi innen](receivables-collect-outstanding-balances.md) |

## <a name="see-also"></a>Zie ook
[Verkoop beheren](sales-manage-sales.md)  
[Betalingsverplichtingen beheren](payables-manage-payables.md)  
[Werken met Dynamics NAV](ui-work-product.md)  
[Verschillende bedrijfsgebieden](ui-across-business-areas.md)


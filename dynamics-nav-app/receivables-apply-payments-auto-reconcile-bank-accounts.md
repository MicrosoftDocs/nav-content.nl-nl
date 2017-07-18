---
title: "Betalingen automatisch vereffenen en bankrekeningen reconciliëren"
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
ms.openlocfilehash: 11df387c16e19421090531fd03c209103b9989d9
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="apply-payments-automatically-and-reconcile-bank-accounts"></a>Betalingen automatisch vereffenen en bankrekeningen reconciliëren
U moet uw bankrekening en de rekeningen met tegoeden en schulden in Dynamics NAV regelmatig reconciliëren door betalingen die op de bank zijn vastgelegd, te vereffenen met de gerelateerde onbetaalde facturen en creditnota's of andere openstaande posten in Dynamics NAV.

U kunt deze taak in het venster **Dagboek betalingsreconciliatie** uitvoeren door een bankafschriftbestand of -feed te importeren om de betalingen snel in Dynamics NAV te registreren. Met een automatische vereffeningsfunctie worden de betalingen vereffend met de gerelateerde openstaande leveranciers- of klantposten op basis van gegevensovereenkomsten tussen betalingstekst en postgegevens. U kunt automatische vereffeningen controleren en wijzigen voordat u het dagboek boekt. U kunt ervoor kiezen om openstaande bankrekeningposten met betrekking tot de vereffende posten te sluiten wanneer u het dagboek boekt. Dit betekent dat de bankrekening automatisch wordt gereconcilieerd wanneer alle betalingen worden vereffend.

Als u de import van bankafschriften als een bankfeed wilt inschakelen, moet u eerst de feedservice van de Envestnet Yodlee Bank instellen en inschakelen en vervolgens uw bankrekeningen aan de gerelateerde online bankrekeningen koppelen. Zie voor meer informatie [Procedure: De feedservice van de Envestnet Yodlee Bank instellen](bank-how-setup-bank-statement-service.md).

**Opmerking**: de Envestnet Yodlee Bank Feeds-service of de bankfeedservice van een andere provider is mogelijk niet beschikbaar in uw systeem. Neem contact op met uw Microsoft-partner als u een bankfeedservice wilt gebruiken om bankafschriften te importeren.

U kunt ook de conversieservice voor bankgegevens gebruiken om een bankafschriftbestand in een willekeurige indeling om te zetten in een gegevensstroom die u kunt importeren in Dynamics NAV. Zie voor meer informatie [Procedure: De conversieservice bankgegevens instellen](bank-how-setup-bank-data-conversion-service.md).

In de volgende tabel wordt een reeks taken beschreven, met koppelingen naar de beschrijvende onderwerpen.

|Als u dit wilt doen |Zie |
|---|----|
|Vereffen betalingen om klant- of leveranciersposten te openen door een bankafschrift te importeren en de bankrekening te reconciliëren wanneer alle betalingen zijn vereffend. | [Procedure: Betalingen reconciliëren met automatische vereffening](receivables-how-reconcile-payments-auto-application.md) |
|Vereffen handmatig betalingen door gedetailleerde informatie over afgestemde gegevens weer te geven en suggesties voor openstaande kandidaatposten om betalingen mee te vereffenen. | [Procedure: Betalingen na automatische vereffening controleren of vereffenen](receivables-how-review-apply-payments-auto-application.md)
|Los problemen met betalingen op die niet automatisch met de relateerde openstaande posten kunnen worden vereffend, bijvoorbeeld omdat de bedragen verschillen of omdat er geen relateerde post bestaat. | [Procedure: Betalingen reconciliëren die niet automatisch kunnen worden vereffend](receivables-how-reconcile-payments-cannot-apply-auto.md)
|Koppel tekst op betalingen aan specifieke klant-, leverancier- of grootboekrekeningen om periodieke ontvangsten of kosten altijd naar deze rekeningen te boeken als er geen documenten zijn voor vereffening.| [Procedure: Tekst op herhalende betalingen aan rekeningen toewijzen voor automatische afstemming](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md)|

## <a name="see-also"></a>Zie ook
[Tegoeden beheren](receivables-manage-receivables.md)  
[Verkoop beheren](sales-manage-sales.md)


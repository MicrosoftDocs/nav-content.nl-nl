---
title: 'Procedure: betalingsvoorstellen maken'
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
ms.openlocfilehash: 11bfba9f279f6bd84c5d169f6f97fd48759bc6df
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-suggest-vendor-payments"></a>Procedure: betalingsvoorstellen maken
In het venster **Betalingsdagboek** kunt u een functie gebruiken om betalingsregels voor te stellen volgens uw instellingen, zoals betalingen die binnenkort moeten worden betaald of betalingen waarvoor een betalingskorting beschikbaar is.

Als u maximaal wilt profiteren van de functie Leveranciersbetalingen voorstellen, moet u uw leveranciers eerst een prioriteit geven. Zie voor meer informatie [Procedure: leveranciers in een prioriteitsvolgorde plaatsen](purchasing-how-prioritize-vendors.md).

Leveranciersposten die niet zijn gemarkeerd als **Afwachten**, worden niet in de batchverwerking opgenomen.  

**Belangrijk**: als u wilt profiteren van contantkortingen en een beschikbaar bedrag hebt ingevoerd, wordt het bedrag eerst gebruikt voor vervallen posten met een prioriteitsnummer (in volgorde van prioriteit), vervolgens voor vervallen posten zonder prioriteitsnummer en tot slot voor openstaande posten die in aanmerking komen voor contantkortingen (in volgorde van leveranciersnummer).

## <a name="to-use-the-suggest-vendor-payments-function"></a>De functie Leveranciersbetalingen voorstellen gebruiken
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Betalingsdagboeken** in en kies vervolgens de gerelateerde koppeling.
2. Open het desbetreffende dagboek en kies vervolgens de actie **Leveranciersbetalingen voorstellen**.
3. Vul indien nodig de velden in. Kies een veld om een korte omschrijving van het veld of een koppeling naar meer informatie te lezen.
4. Kies de knop **Ok**.

## <a name="to-insert-the-due-date-as-posting-date-on-payment-journal-lines"></a>De vervaldatum als boekingsdatum invoegen op betalingsdagboekregels
Wanneer u de batchverwerking **Leveranciersbetalingen voorstellen** gebruikt om betalingsregels voor uw leveranciers te maken, kunt u twee speciale velden invullen om te zorgen dat de gegenereerde regels de vervaldatum gebruiken om de boekingsdatum te berekenen. Deze velden zijn **Bereken boekingsdatum via vervaldatum vereffeningsdoc.** en **Vervaldatumafwijking vereffeningsdoc.**.

**Belangrijk**: u kunt het veld **Bereken boekingsdatum via vervaldatum vereffeningsdoc.** niet gebruiken met het veld **Contantkorting nemen** of het veld **Een regel per leverancier** . De reden is dat als de boekingsdatum is gebaseerd op de vervaldatum, enkele contantkortingen mogelijk niet correct worden berekend, omdat de boekingsdatum kan plaatsvinden na de vervaldatum voor contantkorting.
Als de berekende boekingsdatum in het verleden ligt, wordt de boekingsdatum ook voorwaarts verplaatst naar de volgende werkdatum en wordt een waarschuwing weergegeven.

U kunt ook handmatig betalingsregels maken waarbij de vervaldatum wordt gebruikt om de boekingsdatum te berekenen. Nadat u leveranciersposten hebt vereffend, kunt u de actie **Boekingsdatum berekenen** gebruiken. Hierdoor wordt de boekingsdatum op de dagboekregel bijgewerkt met de vervaldatum van de gerelateerde inkoopfactuur. Zie voor meer informatie [Procedure: Inkooptransacties handmatig vereffenen](payables-how-apply-purchase-transactions-manually.md).  

**Opmerking**: als de inkoopfactuur achterstallig is, wordt de boekingsdatum ingesteld op de werkdatum en wordt het lettertype op de regel rood.

## <a name="see-also"></a>Zie ook
[Betalingsverplichtingen beheren](payables-manage-payables.md)  
[Betalingen doen](payables-make-payments.md)  
[Werken met diversendagboeken](ui-work-general-journals.md)


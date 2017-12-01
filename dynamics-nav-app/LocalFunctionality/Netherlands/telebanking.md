---
title: Telebankieren
description: Op basis van zowel verkoop- als inkooptransacties kunt u met telebankieren betalingen en incasso's genereren die u elektronisch met uw bank kunt uitwisselen.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 65909dce33c801ce8b8b6537887b5c154243cc96
ms.contentlocale: nl-nl
ms.lasthandoff: 10/23/2017

---
# <a name="telebanking"></a>Telebankieren
Op basis van zowel verkoop- als inkooptransacties kunt u met telebankieren betalingen en incasso's genereren die u elektronisch met uw bank kunt uitwisselen. Hieronder vallen ook de export van betalings- en incassogegevens die naar de bank moeten worden doorgestuurd en de import van bankafschriften die door de bank naar u worden verzonden.  

## <a name="transactions"></a>Transacties  
Over het algemeen worden alle financiële interacties met leveranciers en klanten uitgevoerd door middel van inkoop- of verkoopfacturen en creditnota's. Zodra deze transacties zijn geregistreerd en geboekt, kunnen betalingen of incasso's door uw bedrijf worden uitgevoerd.  

## <a name="proposals"></a>Voorstellen  
Op basis van leveranciers- en klantenposten kunt u met telebankieren betalings- en incassovoorstellen genereren. Dit kan voor elke bank worden gedaan die voor uw bedrijf is ingesteld. Zowel binnen- als buitenlandse betalingen en incasso's zijn mogelijk.  

U kunt [!INCLUDE[navnow](../../includes/navnow_md.md)] zodanig instellen dat betalingen aan of incasso's van dezelfde bankrekening automatisch worden gecombineerd.  

Als u akkoord gaat met het voorstel, moet het in een betaalrun worden verwerkt.  

> [!NOTE]  
>  Over het algemeen kan voor alle openstaande leveranciers- en klantenposten een voorstel worden gegenereerd als dat aan een aantal criteria voldoet. Zie [Procedure: Voorstellen maken](how-to-create-proposals.md) voor meer informatie.  

## <a name="payment-histories"></a>Betaalruns  
Een betaalrun is eigenlijk precies hetzelfde als een voorstel, het enige verschil is dat gegevens in een betaalrun niet kunnen worden gewijzigd. De betalings- of incassogegevens zijn gereed om naar de bank te worden geëxporteerd en verzonden.  

 Zie voor meer informatie [Procedure: Betaalrun maken en exporteren](how-to-create-and-export-payment-history.md).  

## <a name="bank-statements"></a>Bankafschriften  
 Voor alle financiële interacties die via uw bank plaatsvinden, kan de bank u elektronische bankafschriften toesturen. Deze afschriften kunnen in de Bank-/Giroboeken worden geïmporteerd. Als u wilt kunt u [!INCLUDE[navnow](../../includes/navnow_md.md)] deze afschriften tijdens het importproces automatisch laten reconciliëren en kan worden vastgesteld of een afschrift kan worden vereffend met openstaande posten voor de betreffende leverancier/klant.  

 Zie [Procedure: Bankafschriften importeren en reconciliëren](how-to-import-and-reconcile-bank-statements.md) voor meer informatie.  

## <a name="exchange-protocols"></a>Uitwisselingsprotocollen  
 Voor zowel het exporteren als importeren is een aantal protocollen gedefinieerd. [!INCLUDE[navnow](../../includes/navnow_md.md)] ondersteunt de volgende protocollen:  

- BTL91 (exporteren)  
- BBV (exporteren)  
- PAYMUL (exporteren)  
- Rabobank mut.asc (importeren)  
- Rabobank vvmut.asc (importeren)  
- Rabobank ASCII (importeren)  
- SEPA CAMT  

## <a name="see-also"></a>Zie ook  
 [Procedure: Verkoopbewerkingen](../../sales-how-invoice-sales.md)   
 [Procedure: Inkopen vastleggen](../../purchasing-how-record-purchases.md)   
 [Procedure: Voorstellen maken](how-to-create-proposals.md)   
 [Procedure: Betalingsrun maken en exporteren](how-to-create-and-export-payment-history.md)


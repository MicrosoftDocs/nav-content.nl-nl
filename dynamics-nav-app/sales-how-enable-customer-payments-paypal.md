---
title: 'Procedure: Klantbetalingen inschakelen via PayPal'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: HT
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 15f30a03c3e7ccc865ef527a707794c2c6428b2f
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---

# <a name="how-to-enable-customer-payments-through-paypal"></a>Procedure: Klantbetalingen inschakelen via PayPal#
Als alternatief voor het innen van betalingen door middel van bankoverschrijving of creditcards kunt u klanten aanbieden met hun PayPal-rekening te betalen.

Wanneer een klant de PayPal-koppeling op een verkoopfactuur of een verkooporderdocument kiest, wordt de servicepagina van hun PayPal-rekening geopend waarin de betalingsdetails voor de verkoop worden weergegeven. De klant kan de factuur vervolgens als elke andere PayPal-betaling betalen.

Als u klantbetalingen via PayPal wilt inschakelen, moet u het volgende doen:

1. Stel PayPal-betalingsstandaard als een betalingsservice in het venster **Betalingsservices** in.
2. Selecteer PayPal-betalingsstandaard in het veld **Betalingsservice** in het desbetreffende verkoopdocument.

De PayPal-betalingsstandaardservice wordt geïnstalleerd als een extensie voor Dynamics NAV en kan worden ingeschakeld. Zie voor meer informatie [Dynamics NAV aanpassen met extensies](ui-extensions.md).

## <a name="to-enable-the-paypal-payments-standard-service"></a>De PayPal-betalingsstandaardservice inschakelen
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, kies **Betalingsservices** en kies vervolgens de gerelateerde koppeling.  
2. Kies in het venster **Betalingsservices** de actie **Nieuw**.
3. Selecteer **PayPal-standaard** en sluit vervolgens het venster.
4. Kies in het venster **Betalingsservices** de actie **Instellen**.
5. Vul indien nodig de velden in. Kies een veld om een korte omschrijving van het veld of een koppeling naar meer informatie te lezen.

    **Opmerking**: schakel het selectievakje **Altijd opnemen in documenten** in als de hyperlink voor de PayPal-betalingsservice altijd zichtbaar moet zijn in verkoopdocumenten waarin de betaling via PayPal wordt ingeschakeld.

6. Sluit het venster.

## <a name="to-select-paypal-payments-standard-on-a-sales-invoice"></a>PayPal-betalingsstandaard op een verkoopfactuur selecteren
1. Kies op de startpagina **Verkoopfacturen**.
2. Open de verkoopfactuur waarvoor u PayPal-betalingen u wilt inschakelen.
3. Kies in het veld **Betalingsservice** een PayPal-betalingsstandaard.

**Opmerking**: het veld **Betalingsservice** is alleen zichtbaar als de PayPal-betalingsstandaardservice wordt ingeschakeld.   

## <a name="see-also"></a>Zie ook  
[Verkopen instellen](sales-setup-sales.md)  
[Verkoop beheren](sales-manage-sales.md)  
[Dynamics NAV aanpassen met behulp van extensies](ui-extensions.md)


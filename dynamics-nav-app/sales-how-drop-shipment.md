---
title: 'Procedure: Doorverzendingen maken'
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
ms.openlocfilehash: f636de789dc6b006a449ec59c390fab85e62b443
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-make-drop-shipments"></a>Procedure: Doorverzendingen maken
Een doorverzending is de directe verzending van artikelen van een van uw leveranciers naar een van uw klanten.

Wanneer een verkooporder voor doorverzending is gemarkeerd en u maakt een inkooporder waarin de klant in het veld **Orderklantnr.** is opgegeven, kunt u de twee documenten koppelen en daarbij de leverancier opdragen om direct naar de klant te verzenden.

## <a name="to-create-a-sales-order-for-drop-shipment"></a>Een verkooporder voor doorverzending maken
Ter voorbereiding op een doorverzending maakt u een verkooporder voor een artikel zoals u dat normaal doet, maar u moet wel op de verkoopregel aangeven dat voor de verkoop doorverzending vereist is.

1. Maak een verkooporder voor een artikel. Zie [Procedure: Producten verkopen](sales-how-sell-products.md) voor meer informatie.
2. Op de verkooporderregel voor het doorverzendingsartikel schakelt u het selectievakje **Doorverzending** in.

## <a name="to-create-the-purchase-order-for-drop-shipment"></a>De inkooporder voor doorverzendingen maken
Ter voorbereiding op een doorverzending van het artikel dat u wilt verkopen, maakt u een inkooporder zoals u dat normaal doet, maar u moet op de inkooporder wel aangeven dat het artikel naar de klant moet worden verzonden en niet naar uzelf.

1. Inkooporder maken. Vul geen velden op de regels in. Zie voor meer informatie [Procedure: Inkopen vastleggen](purchasing-how-record-purchases.md).
2. Selecteer in het veld **Orderklantnr.** de klant aan wie u verkoopt.
3. Kies de actie **Doorverzendingen** en kies vervolgens de actie **Verkooporder ophalen**.
4. Selecteer in het venster **Verkoopoverzicht** de verkooporder die u hebt voorbereid in de sectie "Een verkooporder voor doorverzending maken".
5. Kies de knop **Ok**.

De regelgegevens van de verkooporder worden ingevoegd op de inkooporderregel(s).

U kunt de leverancier nu opdragen om de artikelen naar de klant te verzenden, bijvoorbeeld door de inkooporder als een PDF via e-mail te verzenden.     

## <a name="to-view-the-linked-purchase-order-from-the-sales-order"></a>De gekoppelde inkooporder weergeven op basis van de verkooporder
1. Selecteer de verkooporderregel van de doorverzending, kies de actie **Order**, kies de actie **Doorverzending** en kies vervolgens de actie **Inkooporder**.

De gekoppelde inkooporder wordt geopend.

## <a name="to-post-a-drop-shipment"></a>Een doorverzending boeken
Als de leverancier de artikelen heeft verzonden, kunt u de verkooporder boeken als verzonden. U kunt de inkooporder ook boeken, maar alleen met de optie **Ontvangen**, totdat de verkooporder is gefactureerd.
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Verkooporders** in en kies vervolgens de gerelateerde koppeling.
2. Open de verkooporder die u hebt gemaakt in de sectie "Een verkooporder voor een doorverzending maken".
3. Geef in het veld **Te verzenden aantal** op hoeveel van de orderhoeveelheid moet worden verzonden, de volledige of gedeeltelijke orderhoeveelheid.
3. Kies de actie **Boeken** of **Boeken en verzenden**.
4. Kies vervolgens **de optie Verzenden** om later te factureren of de optie **Verzenden en factureren** om meteen te factureren.

## <a name="see-also"></a>Zie ook
[Procedure: Producten verkopen](sales-how-sell-products.md)    
[Procedure: Inkopen vastleggen](purchasing-how-record-purchases.md)  
[Verkoop beheren](sales-manage-sales.md)  
[Voorraad beheren](inventory-manage-inventory.md)      
[Werken met Dynamics NAV](ui-work-product.md)


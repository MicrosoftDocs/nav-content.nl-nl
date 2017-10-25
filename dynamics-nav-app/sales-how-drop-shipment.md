---
title: Een verkooporder maken die is gekoppeld aan een inkooporder voor een directe verzending
description: Hierin wordt beschreven hoe u een verkooporder kunt maken die is gekoppeld aan een inkooporder om verzending direct van de leverancier naar de klant mogelijk te maken.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: direct shipment
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 6a8210808532ff8945660c23f0bf91719e2f2963
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-make-drop-shipments"></a>Procedure: Doorverzendingen maken
Een doorverzending is de directe verzending van artikelen van een van uw leveranciers naar een van uw klanten.

Wanneer een verkooporder voor doorverzending is gemarkeerd en u maakt een inkooporder waarin de klant in het veld **Orderklantnr.** is opgegeven, kunt u de twee documenten koppelen en daarbij de leverancier opdragen om direct naar de klant te verzenden.

## <a name="to-create-a-sales-order-for-drop-shipment"></a>Een verkooporder voor doorverzending maken
Ter voorbereiding op een doorverzending maakt u een verkooporder voor een artikel zoals u dat normaal doet, maar u moet wel op de verkoopregel aangeven dat voor de verkoop doorverzending vereist is.

1. Maak een verkooporder voor een artikel. Zie [Procedure: Producten verkopen](sales-how-sell-products.md) voor meer informatie.
2. Op de verkooporderregel voor de doorverzending schakelt u het selectievakje **Doorverzending** in. Gebruik de functie **Kolommen kiezen** als het veld niet zichtbaar is. Zie [Persoonlijke gebruikersinstellingen](ui-user-personalization.md) voor meer informatie.

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
* Selecteer de verkooporderregel van de doorverzending, kies de actie **Order**, kies de actie **Doorverzending** en kies vervolgens de actie **Inkooporder**.

## <a name="to-post-a-drop-shipment"></a>Een doorverzending boeken
Nadat de leverancier de artikelen heeft verzonden, kunt u de verkooporder boeken als verzonden. U kunt de inkooporder ook boeken, maar alleen met de optie **Ontvangen**, totdat de verkooporder is gefactureerd.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Verkooporders** in en klik vervolgens op de gerelateerde koppeling.
2. Open de verkooporder die u hebt gemaakt in de sectie "Een verkooporder voor een doorverzending maken".
3. Geef in het veld **Te verzenden aantal** op hoeveel van de orderhoeveelheid moet worden verzonden, de volledige of gedeeltelijke orderhoeveelheid.
4. Kies de actie **Boeken** of **Boeken en verzenden**.
5. Kies vervolgens **de optie Verzenden** om later te factureren of de optie **Verzenden en factureren** om meteen te factureren.

## <a name="see-also"></a>Zie ook
[Procedure: Speciale orders maken](sales-how-to-create-special-orders.md)|  
[Procedure: Producten verkopen](sales-how-sell-products.md)  
[Procedure: Inkopen vastleggen](purchasing-how-record-purchases.md)  
[Verkoop](sales-manage-sales.md)  
[Voorraad](inventory-manage-inventory.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


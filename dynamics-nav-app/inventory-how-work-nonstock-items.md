---
title: Niet-voorraadartikelen maken en beheren
description: Beschrijft hoe u handelt in niet-inventariseerbare artikelen of artikelen die niet in voorraad worden beheerd.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: non-inventoriable
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: dd1497d0727935d4954f826eceb303761850dada
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# Procedure: Werken met niet-voorraadartikelen
U kunt bepaalde artikelen aan uw klanten aanbieden voor hun gemak. U wilt deze artikelen pas in voorraad houden als u ze gaat verkopen. Wanneer u deze artikelen in voorraad gaat houden, kunt u ze op twee manieren naar normale artikelkaarten converteren.

* Maak op basis van een sjabloon een nieuwe artikelkaart in een niet-voorraadartikelkaart.
* Selecteer een niet-voorraadartikel op een verkooporderregel van het type **Artikel** met een leeg veld voor *Nr.* Er wordt automatisch een artikelkaart gemaakt voor het niet-voorraadartikel.

> [!NOTE]  
>   U kunt geen niet-voorraadartikel selecteren in het venster **Verkoopfactuur**. U kunt een niet-voorraadartikel in het venster **Verkoopofferte** selecteren, maar het niet-voorraadartikel wordt niet geconverteerd naar een normaal artikel wanneer u de functie **Order maken** gebruikt.

Een niet-voorraadartikel heeft doorgaans het artikelnummer van de leverancier die het levert. Als u conversie van een niet-voorraadartikelkaart naar een normale artikelkaart wilt inschakelen, moet u eerst instellen hoe leverancierartikelnummering naar uw eigen artikelnummering wordt geconverteerd.   

## Een niet-voorraadartikel maken
Niet-voorraadartikelkaarten hebben minder informatie dan normale artikelkaarten omdat u deze alleen gebruikt op offertes en op andere manieren. Om die reden moeten ze naar normale artikelkaarten worden converteerd voordat u er verkooptransacties voor kunt boeken.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Niet-voorraadartikelen** in en klik vervolgens op de gerelateerde koppeling.
2. Kies de actie **Nieuw**.
3. Vul indien nodig de velden in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## Instellen hoe niet-voorraadartikelnummers naar uw eigen nummering worden geconverteerd
Als u conversie van een niet-voorraadartikelkaart naar een normale artikelkaart wilt inschakelen, moet u eerst instellen hoe de leverancierartikelnummering naar uw eigen artikelnummeropmaak wordt geconverteerd.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Niet-voorraadartikelinstellingen** in en klik vervolgens op de gerelateerde koppeling.
2. Vul indien nodig de velden in.

## Een niet-voorraadartikel converteren naar een normaal artikel
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Niet-voorraadartikelen** in en klik vervolgens op de gerelateerde koppeling.
2. Open de kaart voor een niet-voorraadartikel dat u wilt converterennaar een normaal artikel.
3. Kies in het venster **Niet-voorraadartikelkaart** de actie **Artikel maken**.

Er worden een nieuwe artikelkaart die vooraf is ingevuld met gegevens van het niet-voorraadartikel, en een relevante artikelsjabloon gemaakt. U kunt vervolgens indien nodig velden op de nieuwe artikelkaart invullen of bewerken. Zie [Procedure: Nieuwe artikelen registreren](inventory-how-register-new-items.md) voor meer informatie.

## Een niet-voorraadartikel verkopen en converteren naar een normaal artikel
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Verkooporders** in en klik vervolgens op de gerelateerde koppeling.
2. Kies de actie **Nieuw**. Vul de velden op het sneltabblad **Algemeen** in, zoals u dat voor elke verkooporder doet. Zie [Procedure: Producten verkopen](sales-how-sell-products.md) voor meer informatie.
3. Selecteer op een nieuwe verkoopregel in het veld **Soort** **Artikel**, maar laat het veld **Nr.** leeg laten.
4. Kies de actie **Regel** en kies vervolgens de actie **Niet-voorraadartikelen selecteren**.

    Het niet-voorraadartikel wordt naar een normaal artikel geconverteerd. Er worden een nieuwe artikelkaart die vooraf is ingevuld met gegevens van het niet-voorraadartikel, en een relevante artikelsjabloon gemaakt.
5. Selecteer in het venster **Niet-voorraadartikelen** het niet-voorraadartikel dat u wilt verkopen en klik vervolgens op **OK**.
6. Wanneer de verkooporder is ingevuld, kiest u de actie **Boeken**.

U kunt vervolgens indien nodig velden op de nieuwe artikelkaart invullen of bewerken. Zie [Procedure: Nieuwe artikelen registreren](inventory-how-register-new-items.md) voor meer informatie.

> [!NOTE]  
>   Er wordt automatisch een artikelkruisverwijzingsrecord gemaakt voor de leverancier van het artikel tussen het artikelnummer van de leverancier en uw nieuwe artikelnummer.

## Zie ook
[Procedure: Nieuwe artikelen registreren](inventory-how-register-new-items.md)  
[Procedure: Speciale orders maken](sales-how-to-create-special-orders.md)|  
[Voorraad](inventory-manage-inventory.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


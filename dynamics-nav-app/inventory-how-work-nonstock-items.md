---
title: 'Procedure: Werken met niet-voorraadartikelen'
author: SorenGP
ms.custom: na
ms.date: 09/29/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 2b49d95904732dcf091fd060a96006fdcb477ec1
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# Procedure: Werken met niet-voorraadartikelen
U kunt bepaalde artikelen aan uw klanten aanbieden voor hun gemak. U wilt deze artikelen pas in voorraad houden als u ze gaat verkopen. Wanneer u deze artikelen in voorraad gaat houden, kunt u ze op twee manieren naar normale artikelkaarten converteren.

- Maak op basis van een sjabloon een nieuwe artikelkaart in een niet-voorraadartikelkaart.
- Selecteer een niet-voorraadartikel op een verkooporderregel met een leeg **Artikel**-veld. Wanneer u de verkoop boekt, wordt automatisch een artikelkaart gemaakt voor het niet-voorraadartikel.

**Opmerking**: u kunt geen niet-voorraadartikel selecteren in het venster **Verkoopfactuur**. U kunt een niet-voorraadartikel in het venster **Verkoopofferte** selecteren, maar het niet-voorraadartikel wordt niet geconverteerd naar een normaal artikel wanneer u de functie **Order maken** gebruikt.

Een niet-voorraadartikel heeft doorgaans het artikelnummer van de leverancier die het levert. Als u conversie van een niet-voorraadartikelkaart naar een normale artikelkaart wilt inschakelen, moet u eerst instellen hoe leverancierartikelnummering naar uw eigen artikelnummering wordt geconverteerd.   

## Een niet-voorraadartikel maken
Niet-voorraadartikelkaarten hebben minder informatie dan normale artikelkaarten omdat u deze alleen gebruikt op offertes en op andere manieren. Om die reden moeten ze naar normale artikelkaarten worden converteerd voordat u er verkooptransacties voor kunt boeken.

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Niet-voorraadartikelen**  in en kies vervolgens de gerelateerde koppeling.
2. Kies de actie **Nieuw**.
2. Vul indien nodig de velden in. Kies een veld om een korte omschrijving van het veld of een koppeling naar meer informatie te lezen.

## Instellen hoe niet-voorraadartikelnummers naar uw eigen nummering worden geconverteerd  
Als u conversie van een niet-voorraadartikelkaart naar een normale artikelkaart wilt inschakelen, moet u eerst instellen hoe de leverancierartikelnummering naar uw eigen artikelnummeropmaak wordt geconverteerd.

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Niet-voorraadartikelinstellingen** in en kies vervolgens de gerelateerde koppeling.
2. Vul indien nodig de velden in.

## Een niet-voorraadartikel converteren naar een normaal artikel
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Niet-voorraadartikelen**  in en kies vervolgens de gerelateerde koppeling.
2. Open de kaart voor een niet-voorraadartikel dat u wilt converterennaar een normaal artikel.
3. Kies in het venster **Niet-voorraadartikelkaart** de actie **Artikel maken**.

Er worden een nieuwe artikelkaart die vooraf is ingevuld met gegevens van het niet-voorraadartikel, en een relevante artikelsjabloon gemaakt. U kunt vervolgens indien nodig velden op de nieuwe artikelkaart invullen of bewerken. Zie voor meer informatie [Procedure: Nieuwe producten registreren](inventory-how-register-new-products.md).

## Een niet-voorraadartikel verkopen en converteren naar een normaal artikel
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Verkooporders** in en kies vervolgens de gerelateerde koppeling.
2. Kies de actie **Nieuw**. Vul de velden op het sneltabblad **Algemeen** in, zoals u dat voor elke verkooporder doet.
3. Laat op een nieuwe verkoopregel het veld **Artikel** leeg, kies **Regel**, **Functies** en kies vervolgens **Niet-voorraadatikelen**.

    Het niet-voorraadartikel wordt naar een normaal artikel geconverteerd. Er worden een nieuwe artikelkaart die vooraf is ingevuld met gegevens van het niet-voorraadartikel, en een relevante artikelsjabloon gemaakt.
4. Selecteer in het venster **Niet-voorraadartikelen** het niet-voorraadartikel dat u wilt verkopen en klik vervolgens op **OK**.
5. Wanneer de verkooporder is ingevuld, kiest u de actie **Boeken**.

U kunt vervolgens indien nodig velden op de nieuwe artikelkaart invullen of bewerken. Zie voor meer informatie [Procedure: Nieuwe producten registreren](inventory-how-register-new-products.md).

**Opmerking**: er wordt automatisch een artikelkruisverwijzingsrecord gemaakt voor de leverancier van het artikel tussen het artikelnummer van de leverancier en uw nieuwe artikelnummer.

## Zie ook
[Procedure: Nieuwe producten registreren](inventory-how-register-new-products.md)  
[Voorraad beheren](inventory-manage-inventory.md)  
[Werken met Dynamics NAV](ui-work-product.md)


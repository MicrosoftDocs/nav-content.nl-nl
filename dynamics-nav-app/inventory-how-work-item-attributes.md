---
title: 'Procedure: Werken met artikelkenmerken'
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
ms.openlocfilehash: eaf539f1d4d00c2cd5679f39f29a3428e33ee1fd
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-work-with-item-attributes"></a>Procedure: Werken met artikelkenmerken
Wanneer klanten informeren naar een artikel, via correspondentie of via een geïntegreerde webwinkel, kunnen ze ernaar vragen of zoeken op basis van kenmerken, zoals hoogte en model. Als u deze klantenservice wilt bieden, kunt u artikelkenmerkwaarden van verschillende typen aan uw artikelen toewijzen, die vervolgens kunnen worden gebruikt bij het zoeken naar artikelen.

U kunt ook artikelkenmerken aan artikelcategorieën toewijzen, die vervolgens worden toegepast op de artikelen die de artikelcategorieën gebruiken. Zie [Procedure: Artikelen categoriseren](inventory-how-categorize-items.md) voor meer informatie.

## <a name="to-create-item-attributes"></a>Artikelkenmerken maken
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Artikelkenmerken** in en kies vervolgens de gerelateerde koppeling.
2. Kies in het venster **Artikelkenmerken** de actie **Nieuw**.
3. Vul in het venster **Artikelkenmerk** indien nodig de velden in. Kies een veld om een korte omschrijving van het veld of een koppeling naar meer informatie te lezen.

**Opmerking**: als u **Optie** selecteert in het veld **Soort**, kunt u de actie **Artikelkenmerkwaarden** kiezen om waarden voor het artikelkenmerk te maken. Zie het gedeelte "Waarden voor artikelkenmerken van het soort Optie maken" voor meer informatie.  

## <a name="to-create-values-for-item-attributes-of-type-option"></a>Waarden voor artikelkenmerken van het soort Optie maken
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Artikelkenmerken** in en kies vervolgens de gerelateerde koppeling.
2. Selecteer in het venster **Artikelkenmerken** een artikelkenmerk van het soort Optie waarvoor u waarden wilt maken, en kies vervolgens de actie **Artikelkenmerkwaarden**.
3. Vul in het venster **Artikelkenmerkwaarden** indien nodig de velden in. Kies een veld om een korte omschrijving van het veld of een koppeling naar meer informatie te lezen.

## <a name="to-assign-item-attributes-to-items"></a>Artikelkenmerken aan artikelen toewijzen
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Artikelen** in en kies vervolgens de gerelateerde koppeling.
2. Selecteer in het venster **Artikelen** het artikel waaraan u kenmerkwaarden wilt toewijzen, en kies vervolgens de actie **Kenmerken**.
3. Kies in het venster **Artikelkenmerkwaarden** de actie **Nieuw**.
4. Kies in het veld **Kenmerk** de knop AssistEdit en selecteer een bestaand artikelkenmerk. U kunt ook de actie **Nieuw** kiezen om eerst een nieuw artikelkenmerk te maken, zoals is uitgelegd in het gedeelte "Artikelkenmerken maken".
5. Voer in het veld **Waarde** de artikelkenmerkwaarde in, zoals "2010" voor het kenmerk Modeljaar.
6. Kies voor artikelkenmerken van het soort Optie de knop AssistEdit in het veld **Waarde** en selecteer een artikelkenmerkwaarde. U kunt ook de actie **Nieuw** kiezen om eerst een nieuwe artikelkenmerkwaarde te maken, zoals is uitgelegd in het gedeelte "Waarden voor artikelkenmerken van het soort Optie maken".
7. Herhaal stap 4 tot en met 6 voor alle artikelkenmerken die u wilt toewijzen aan het artikel.

## <a name="to-assign-item-attributes-to-item-categories"></a>Artikelkenmerken aan artikelcategorieën toewijzen
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Artikelcategorieën** in en kies vervolgens de gerelateerde koppeling.
2. Selecteer in het venster **Artikelcategorieën** de artikelcategorie waaraan u artikelkenmerken wilt toewijzen en kies vervolgens de actie **Bewerken**.
3. Kies in het venster **Artikelcategoriekaart** op het sneltabblad **Kenmerken** de actie **Nieuw**.
4. Kies in het veld **Kenmerk** de knop AssistEdit en selecteer een bestaand artikelkenmerk. U kunt ook de actie **Nieuw** kiezen om eerst een nieuw artikelkenmerk te maken, zoals is uitgelegd in het gedeelte "Artikelkenmerken maken".
5. Kies in het veld **Standaardwaarde** de knop AssistEdit en selecteer een artikelkenmerkwaarde.
6. Herhaal stap 4 en 5 voor alle artikelkenmerken die u wilt toewijzen aan de artikelcategorie.

**Opmerking**: artikelkenmerken voor bovenliggende artikelcategorieën worden doorgegeven aan onderliggende artikelcategorieën. Dit wordt aangegeven door het veld **Overgenomen van** op het sneltabblad **Kenmerken**. Zie [Procedure: Artikelen categoriseren](inventory-how-categorize-items.md) voor meer informatie.

## <a name="to-filter-by-item-attributes"></a>Filteren op artikelkenmerken
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Artikelen** in en kies vervolgens de gerelateerde koppeling.
2. Kies in het venster **Artikelen** de actie **Filteren op kenmerken**.
3. Kies in het venster **Artikelen filteren op kenmerk** de knop AssistEdit in het veld **Kenmerk** en selecteer een artikelkenmerk.
4. Kies in het veld **Waarde** de knop AssistEdit en selecteer een bestaande kenmerkwaarde om artikelen op te filteren.

    **Opmerking**: u kunt alleen rechtstreeks waarden selecteren voor artikelkenmerken die vaste waarden hebben, zoals Kleur. Voor artikelkenmerken die variabele waarden hebben, zoals Breedte, moet u de artikelkenmerkwaarde opgeven door eerst een voorwaarde te selecteren. Zie stap 5.
5. Kies in het veld **Waarde** voor een variabel artikelkenmerk de knop AssistEdit.
6. Kies in het venster **Filterwaarde opgeven**, in het veld **Voorwaarde** de vervolgkeuzepijl en selecteer een voorwaarde.
7. Voer in het veld **Waarde** een kenmerkwaarde in om artikelen op te filteren.

    **Voorbeeld:** als u wilt filteren op artikelen waarvan de materiaalomschrijving begint met "blauw", vult u de velden als volgt in: veld **Kenmerk**: Materiaalomschrijving, veld **Voorwaarde**: Begint met, veld **Waarde**: blauw.
8. Kies de knop **Ok**.   

De artikelen in de **Artikelen**-vensters worden gefilterd door de opgegeven artikelkenmerkwaarden.

## <a name="see-also"></a>Zie ook
[Procedure: Artikelen categoriseren](inventory-how-categorize-items.md)    
[Procedure: Nieuwe producten registreren](inventory-how-register-new-products.md)  
[Voorraad beheren](inventory-manage-inventory.md)  
[Werken met Dynamics NAV](ui-work-product.md)


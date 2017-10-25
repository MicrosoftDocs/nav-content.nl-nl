---
title: Magazijn herstructureren
description: Misschien wilt u op een dag de magazijnstructuur aanpassen en nieuwe opslaglocaties en kenmerken instellen.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 852aa1a36b150d13d763e2c398265b9eaec5c3ea
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-restructure-warehouses"></a>Procedure: magazijn herstructureren
Misschien wilt u op een dag de magazijnstructuur aanpassen en nieuwe opslaglocaties en kenmerken instellen. Dit zal niet vaak voorkomen, maar in sommige gevallen is een aanpassing van het magazijn noodzakelijk om een meer efficiënte bedrijfsvoering te bereiken of behouden. Voorbeeld:  

- Misschien wilt u omschakelen naar opslaglocaties die het gebruik van automatische gegevensverwerking ondersteunen, bijvoorbeeld met draagbare apparatuur.  
- Er is mogelijk een nieuw rekkensysteem aangeschaft met extra opslagmogelijkheden voor artikelen.  
- Het bedrijfsassortiment kan zijn gewijzigd en het magazijn is dientengevolge verplaatst naar een nieuwe vestiging.  

Indien voor het magazijn opslaglocaties worden gebruikt, maar niet gestuurde opslag en pick, kunt u het magazijn herstructureren door nieuwe opslaglocaties te maken die u in de toekomst wilt gebruiken.  

## <a name="to-restructure-a-basic-warehouse-that-uses-bins-only"></a>Herstructureren van een standaardmagazijn dat alleen opslaglocaties gebruikt  
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Vestigingen** in en klik vervolgens op de gerelateerde koppeling.  
2.  Stel op het sneltabblad **Magazijn** het veld **Std. opslaglocatieselectie** in op **Laatst gebruikte opslaglocatie**.  
3.  Verplaats alle inhoud van de huidige opslaglocaties naar de nieuwe opslaglocaties die u zojuist hebt gemaakt.  

    1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Artikelherindelingsdagboek** in en klik vervolgens op de gerelateerde koppeling.  
    2.  Selecteer een dagboekregel en kies de actie **Opslaglocatie-inhoud ophalen**.  
    3.  Stel op het sneltabblad **Opslaglocatie-inhoud** filters in de velden **Locatiecode**, **Opslaglocatiecode** en **Artikelnr.** in voor het opgeven van de inhoud die u wilt verplaatsen.  
    4.  Kies de knop **OK** om een dagboekregel te vullen.  
    5.  Selecteer de opslaglocatie waarnaar de artikelen moeten worden verplaatst in het veld **Nieuwe opslaglocatie**.  
    6.  Herhaal stap b tot en met e voor alle opslaglocatie-inhoud die u wilt verplaatsen.  
    7.  Kies de actie **Boeken**.  

U hebt nu de opslaglocaties leeggemaakt waar de artikelen eerst waren. De standaardopslaglocaties voor de artikelen zijn nu gewijzigd in de nieuwe opslaglocaties.  

## <a name="to-restructure-an-advanced-warehouse-that-uses-directed-put-away-and-pick"></a>Herstructureren van een geavanceerd magazijn met gestuurde opslag en pick  

1.  Maak de nieuwe opslaglocaties aan die u voortaan wilt gebruiken. Zie [Procedure: Opslaglocaties maken](warehouse-how-to-create-individual-bins.md) voor meer informatie.  
2.  Verplaats alle inhoud van de huidige opslaglocaties naar de nieuwe opslaglocaties die u zojuist hebt gemaakt.  

    1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Magazijnherindelingsdagboek** in en klik vervolgens op de gerelateerde koppeling.  
    2.  Als u opslaglocaties hebt waarvan de inhoud niet wordt verplaatst, maakt u een regel voor elke huidige opslaglocatie in het **magazijnherindelingsdagboek**. Hierin neemt u zowel de oude opslaglocatie **Van opslaglocatie** als de nieuwe opslaglocatie **Naar opslaglocatie** op.  
    3.  Als sommige verplaatsingen fysiek moeten worden uitgevoerd door magazijnmedewerkers, gebruikt u **Verplaatsingsvoorstellen** om verplaatsingsinstructies te maken. U gebruikt in dit geval niet het herindelingsdagboek van het magazijn. Zie [Procedure: Artikelen verplaatsen in geavanceerde magazijnconfiguraties](warehouse-how-to-move-items-in-advanced-warehousing.md) voor meer informatie.  

3.  Wanneer de oude opslaglocaties worden leeggemaakt, moeten ze als opslaglocatie van het type **QC** worden ingedeeld zodat ze niet worden opgenomen in de artikelstroom.  

    1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Vestigingen** in en klik vervolgens op de gerelateerde koppeling.  
    2.  Selecteer de regel met de locatie en kies vervolgens de actie **Opslaglocaties**.  
    3.  Voer in het venster **Opslaglocaties**, in het veld **Code opslaglocatiesoort**, **QC** in voor elk van de oude opslaglocaties die u in stap 3 in de vorige procedure hebt leeggemaakt.  

U hebt nu de opslaglocaties verwijderd uit de magazijnstroom en ze opnieuw ingedeeld als QC-opslaglocaties. Dit zijn opslaglocaties die niet beschikken over de activiteitenvelden in het venster **Opslaglocatiesoorten** en daarom niet door de artikelstroom worden meegenomen. Zie [Procedure: Opslaglocatiesoorten instellen](warehouse-how-to-set-up-bin-types.md) voor meer informatie.  

## <a name="to-delete-a-bin"></a>Een opslaglocatie verwijderen  

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Vestigingen** in en klik vervolgens op de gerelateerde koppeling.  
2.  Selecteer de vestiging waar u opslaglocaties wilt gebruiken en kies de actie **Opslaglocaties**.  
3.  Selecteer de regels voor de opslaglocaties die u wilt verwijderen.  
4.  Kies de actie **Verwijderen**.  

Als u op **Ja** klikt, wordt de opslaglocatie verwijderd voor toekomstig gebruik. De opslaglocatie blijft echter ongewijzigd voor alle geboekte magazijnposten.  

Als u een opslaglocatie wilt hernoemen, zodat alle records die zijn gekoppeld aan de opslaglocatie eveneens worden hernoemd, kunt u deze wijziging doorvoeren in het venster **Opslaglocaties**. Het gaat hierbij om regels met opslaglocatie-inhoud, magazijnactiviteiten, magazijnvoorstelregels, regels voor magazijnontvangst, magazijnverzending en magazijnposten.  

## <a name="to-rename-a-bin-and-change-the-bin-code-in-all-records"></a>Een opslaglocatie een andere naam geven en de opslaglocatie in alle records wijzigen  

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Vestigingen** in en klik vervolgens op de gerelateerde koppeling.  
2.  Selecteer de vestiging waar u de naam of code van een opslaglocatie wilt wijzigen en kies vervolgens de actie **Opslaglocaties**.  
3.  Selecteer de opslaglocatie die u wilt wijzigen en voer in het veld **Code** een code voor een nieuwe opslaglocatie in.  
4.  Kies de knop **Ja**.  

> [!NOTE]  
>  Als u op **Ja** klikt en veel posten van toepassing zijn op deze opslaglocatie, bijvoorbeeld omdat u een lange tijd geen magazijndocumenten hebt verwijderd, kan het een tijd duren voordat alle records zijn hernoemd. Overweeg daarom, indien u deze methode gebruikt, om de batchtaak **Geregistreerde magazijndocumenten verwijderen** uit te voeren voordat u begint met het wijzigen van het proces. Voor deze batchverwerking geldt dat alleen opslag-, pick- en verplaatsingsdocumenten worden verwijderd.  
>   
>  Als u een opslaglocatie voor ontvangst of verzending wilt hernoemen, moeten ook alle geboekte ontvangsten en verzendingen worden hernoemd die betrekking hebben op de opslaglocatie.  

## <a name="see-also"></a>Zie ook  
[Magazijnbeheer](warehouse-manage-warehouse.md)  
[Voorraad](inventory-manage-inventory.md)  
[Magazijnbeheer instellen](warehouse-setup-warehouse.md)     
[Assemblagebeheer](assembly-assemble-items.md)    
[Ontwerpdetails: Magazijnbeheer](design-details-warehouse-management.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


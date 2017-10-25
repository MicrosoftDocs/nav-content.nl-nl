---
title: Artikelkaarten maken voor goederen of services
description: U maakt artikelkaarten voor services die u als uren en voor fysieke producten verkoopt, zoals componenten, gereedgemelde goederen, onderdelen of grondstoffen, die u uit uw voorraad verkoopt.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: item, finished good, component, raw material, assembly item
ms.date: 08/31/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: f26207e07539da790a0ffab38a0fd2b732231300
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-register-new-items"></a>Procedure: Nieuwe artikelen registreren
Artikelen vormen met andere producten de basis van uw bedrijf, de goederen of services waarin u handelt. Elk artikelproduct moet worden geregistreerd als een artikelkaart.

Artikelkaarten bevatten de informatie die is vereist om artikelen te kopen, op te slaan, te verkopen, te leveren en te verantwoorden.

Een artikel kan als bovenliggend artikel met onderliggende artikelen in een stuklijst worden gestructureerd. In [!INCLUDE[d365fin](includes/d365fin_md.md)] kan een stuklijst een assemblagestuklijst of productiestuklijst zijn, afhankelijk van het gebruik. Zie [Procedure: Werken met stuklijsten](inventory-how-work-BOMs.md) voor meer informatie.

> [!NOTE]  
>   Als klantsjablonen voor verschillende klantsoorten bestaan, wordt een venster automatisch weergegeven wanneer u een nieuwe artikelkaart maakt van waaruit u een geschikte sjabloon kunt selecteren. Als er slechts één artikelsjabloon bestaat, gebruiken nieuwe artikelkaarten altijd deze sjabloon.

Als u hetzelfde artikel inkoopt bij meerdere leveranciers, kunt u die leveranciers aan de artikelkaart koppelen. De leveranciers worden vervolgens weergegeven in het venster **Artikelleveranciers**, zodat u gemakkelijk een alternatieve leverancier kunt selecteren.

## <a name="to-create-a-new-item-card"></a>Een nieuwe artikelkaart maken
1. Kies op de startpagina de actie **Artikelen** om de lijst met bestaande artikelen te openen.  
2. Kies in het venster **Artikelen** de actie **Nieuw**.

    Als er slechts één artikelsjabloon bestaat, wordt vervolgens een nieuwe artikelkaart geopend waarin enkele velden zijn ingevuld met informatie van de sjabloon.
3. Kies in het venster **Selecteer een sjabloon voor een nieuw artikel** de sjabloon die u wilt gebruiken voor de nieuwe artikelkaart.
4. Kies de knop **Ok**. Een nieuwe artikelkaart wordt geopend met enkele velden met informatie uit de sjabloon.
5. Ga door met velden op de artikelkaart in te vullen of te wijzigen. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]
> In het veld **Waarderingsmethode** bepaalt u hoe de eenheidskostprijs van het artikel wordt berekend door de veronderstellingen die worden gemaakt over de stroom van artikelen in het bedrijf. Afhankelijk van het type item zijn vijf waarderingsmethoden beschikbaar. Zie [Ontwerpdetails: Waarderingsmethoden](design-details-costing-methods.md) voor meer informatie.
>
> Als u de waarderingsmethode **Gemiddeld** gebruikt, worden de eenheidskosten van een artikel berekend als de gemiddelde eenheidskosten op een bepaald moment na een aanschaf. Voorraad wordt gewaardeerd met de aanname dat alle voorraad tegelijkertijd wordt verkocht. Met deze instelling kunt u het veld **Kostprijs** kiezen en zo in het venster **Overzicht gemiddelde-kostenberekening** de historie bekijken van de transacties waaruit de gemiddelde kostprijs wordt berekend.

Op het sneltabblad **Prijs en boeken** kunt u speciale prijzen of kortingen weergeven die u voor het artikel verleent als aan bepaalde criteria wordt voldaan, zoals klant, minimaal orderaantal of einddatum. Elke rij vertegenwoordigt een speciale prijs of regelkorting. Elke kolom vertegenwoordigt een criterium dat moet worden toegepast om de speciale prijs te garanderen die u invoert in het veld **Eenheidsprijs** of de regelkorting die u invoert in het veld **Regelkorting %**. Zie voor meer informatie [Afspraken over prijzen, kortingen en betalingen van verkopen vastleggen](sales-how-record-sales-price-discount-payment-agreements.md).

Het artikel is nu geregistreerd en de artikelkaart is klaar om voor inkoop- en verkoopdocumenten te worden gebruikt.

Als u deze artikelkaart als sjabloon wilt gebruiken wanneer u nieuwe artikelkaarten maakt, kunt u deze opslaan als een sjabloon. Zie de volgende onderwerpen voor meer informatie.

## <a name="to-save-the-item-card-as-a-template"></a>De artikelkaart als sjabloon opslaan
1. Kies in het venster **Artikelkaart** de actie **Opslaan als sjabloon**. Het venster **Artikelsjabloon** opent de weergave van de artikelkaart als sjabloon.
2. Vul indien nodig de velden in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Als u sjablonen wilt hergebruiken, kiest u de actie **Dimensies**. Het venster **Dimensiesjablonen** geeft alle dimensiecodes weer die voor het item zijn ingesteld.
4. Bewerk of typ dimensiecodes die van toepassing zijn op nieuwe artikelkaarten die worden gemaakt met de sjabloon.
5. Wanneer u de nieuwe artikelsjabloon hebt voltooid, kiest u de knop **OK**.

De artikelsjabloon wordt toegevoegd aan de lijst met artikelsjablonen, zodat u deze kunt gebruiken om nieuwe artikelkaarten te maken.

## <a name="to-set-up-multiple-vendors-for-an-item"></a>Meerdere leveranciers voor een artikel instellen  
Als u hetzelfde artikel bij meerdere leveranciers inkoopt, moet u informatie over elk van deze leveranciers invoeren, bijvoorbeeld informatie over prijzen, levertermijn, kortingen, enzovoort.  

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Artikelen** in en klik vervolgens op de gerelateerde koppeling.  
2.  Selecteer het betreffende artikel en kies vervolgens de actie **Bewerken**.  
3.  Kies de actie **Leveranciers**.  
4.  Klik op het veld **Leveranciersnr.** en selecteer vervolgens de leverancier waarvoor u het artikel wilt instellen.  
5.  Het invullen van de overige velden is optioneel.  
6.  Herhaal stap 2 t/m 5 voor elke leverancier waarbij u het artikel wilt kunnen inkopen.

Deze leveranciers worden vervolgens weergegeven in het venster **Artikelleveranciers**, dat u opent vanuit de artikelkaart, zodat u gemakkelijk een alternatieve leverancier kunt selecteren.

## <a name="see-also"></a>Zie ook
  [Voorraad](inventory-manage-inventory.md)  
  [Inkoop](purchasing-manage-purchasing.md)  
  [Verkoop](sales-manage-sales.md)  
  [Werken met [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](ui-work-product.md)

##


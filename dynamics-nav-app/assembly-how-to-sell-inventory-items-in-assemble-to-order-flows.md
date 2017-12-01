---
title: Voorraadartikelen in assembleren voor order-stromen verkopen
description: Als het artikel is ingesteld voor assembleren-op-order, neemt het standaardproces voor de verkooporder aan dat het item niet in voorraad is en voor deze verkooporder geassembleerd moet worden. Daarom wordt er automatisch een gekoppelde assemblageorder gemaakt wanneer u een artikel aan de verkooporderregel wilt toevoegen.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 0d907c5f96c4af0e28a04292bee2c21865346593
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-sell-inventory-items-in-assemble-to-order-flows"></a>Procedure: voorraadartikelen in assembleren-op-order-stromen verkopen
Als het veld **Assemblagebeleid** op de artikelkaart van assemblageartikel **Op order assembleren** bevat, neemt het standaardproces voor de verkooporder aan dat het item niet in voorraad is en voor deze verkooporder geassembleerd moet worden. Daarom wordt er automatisch een gekoppelde assemblageorder gemaakt wanneer u een artikel aan de verkooporderregel wilt toevoegen. Zie voor meer informatie [Procedure: op order geassembleerde artikelen verkopen](assembly-how-to-sell-items-assembled-to-order.md). Echter als een deel van de hoeveelheid van de verkooporder al beschikbaar in voorraad is, kunt u de assemblageorder verkleinen door het veld **Aantal voor op order assembleren** op de verkooporderregel te veranderen.  

Dit scenario is zeldzaam omdat op-order-assembleren-artikelen altijd worden aangepast en de kans dat ze in voorraad zijn in de configuratie die is aangevraagd door een andere klant laag is. Maar als een bedrijf aantallen voor assembleren op basis van orders in voorraad heeft als gevolg van retouren of annuleringen, moeten deze hoeveelheden worden verzameld en verkocht voordat nieuwe worden samengesteld.  

> [!NOTE]  
>  Er bestaat geen functionaliteit op verkooporders die automatisch waarschuwen of u helpt assemblyorderhoeveelheden die reeds beschikbaar zijn af te trekken. In plaats daarvan moet u de beschikbaarheidsinformatie controleren, zoals het feitenblok **Verkoopregeldetails**.  

Vergelijkbare functionaliteit is beschikbaar wanneer u assemblageartikelen uit voorraad verkoopt en een deel of de gehele hoeveelheid is niet beschikbaar en kan worden geleverd door een assemblageorder. Zie voor meer informatie [Procedure: op-order-assembleren-artikelen en voorraadartikelen samen verkopen](assembly-how-to-sell-assemble-to-order-items-and-inventory-items-together.md).  

> [!NOTE]  
>  Bepaalde regels zijn van toepassing op het veld **Te verzenden aantal** op verkooporderregels die een combinatie van het op-order-assembleren-aantallen en voorraadaantallen bevatten. Zie voor meer informatie de sectie Combinatiescenario's in [Op voorraad assembleren of Op order assembleren begrijpen](assembly-assemble-to-order-or-assemble-to-stock.md).  

Vervang in deze procedure de aantallen voor assembleren op basis van orders met de voorraadaantallen op een verkooporderregel. De stappen omvatten het opsporen of beschikbaarheid bestaat, het aftrekken van die hoeveelheid van de gekoppelde assemblageorder en vervolgens het reserveren van de voorraadhoeveelheid om ervoor te zorgen dat deze wordt gepickt en voor de order worden verzonden.  

## <a name="to-sell-inventory-items-in-assemble-to-order-flows"></a>Voorraadartikelen in assembleren-op-order-stromen verkopen  
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Verkooporders** in en klik vervolgens op de gerelateerde koppeling.  
2.  Een verkooporder maken. Zie [Procedure: Producten verkopen](sales-how-sell-products.md) voor meer informatie.  
3.  Op een verkooporderregel voor een op-order-assembleren-artikel voert u in het veld **Hoeveelheid** de gevraagde hoeveelheid in.  
4.  In het feitenblok **Verkoopregeldetails** bepaalt u of de gevraagde hoeveelheid geheel of gedeeltelijk beschikbaar is.  
5.  In het veld **Aantal voor op order assembleren** trekt u de beschikbare hoeveelheid af zodat alleen niet-beschikbare hoeveelheid op de order wordt geassembleerd. Het veld **Gereserveerde hoeveelheid** wordt dienovereenkomstig verlaagd om aan te geven dat de order-naar-order-koppeling of reservering alleen van toepassing is op de te assembleren hoeveelheid.  
6.  Op het sneltabblad **Regels** kiest u **Functies** en vervolgens kiest u de actie **Reserveren**.  
7.  Selecteer in het venster **Reservering** de artikelpostregel of -regels die de beschikbare hoeveelheden bevatten, kies de actie **Vanuit huidige regel reserveren** en kies vervolgens de knop **OK**.  

    In het veld **Verkooporder** toont het veld **Gereserveerd aantal** nu dat het gehele aantal op de orderregel is gereserveerd. Het veld **Aantal voor op order assembleren** weerspiegelt nog steeds de subhoeveelheid die moet worden geassembleerd.  

8.  Geef de verkooporder vrij voor het picken van de voorraadartikelen en assemblage van de niet beschikbare artikelen. Zie [Procedure: Artikelen assembleren](assembly-how-to-assemble-items.md) voor meer informatie.  

> [!CAUTION]  
>  Het veld **Opslaglocatie** in de verkooporder kan al vooraf zijn ingevuld volgens het veld **Opslaglocatiecode assembleren-op-order verzending** of **Opslagloc.code Vanuit-assembl.** op de locatiekaart. In dat geval is het veld **Opslaglocatie** op de verkooporderregel mogelijk onjuist in deze combinatie van hoeveelheden assembleren voor order en assembleren voor voorraad. Het is verstandig om het veld **Opslaglocatie** te bekijken en te controleren of de plaatsing voor alle hoeveelheden werkt. U kunt ook twee verschillende hoeveelheden invoeren op aparte verkooporderregels.  

## <a name="see-also"></a>Zie ook  
[Assemblagebeheer](assembly-assemble-items.md)  
[Procedure: Artikelen reserveren](inventory-how-to-reserve-items.md)  
[Procedure: Werken met stuklijsten](inventory-how-work-BOMs.md)  
[Voorraad](inventory-manage-inventory.md)  
[Ontwerpdetails: Magazijnbeheer](design-details-warehouse-management.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


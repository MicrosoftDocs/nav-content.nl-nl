---
title: Assembleren voor order-artikelen verkopen
description: Als het artikel is ingesteld voor assembleren-voor-order, wordt het artikel niet verwacht in voorraad te zijn en moet het specifiek voor een verkooporder worden geassembleerd. Wanneer u het artikel invoert op een verkooporderregel, wordt automatisch een assemblageorder gemaakt en gekoppeld aan de verkooporder.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: fc140a0fa7d58c38234f67471323241ac94ca489
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-sell-items-assembled-to-order"></a>Procedure: op order geassembleerde artikelen verkopen
Als het veld **Assemblagebeleid** op de artikelkaart van assemblageartikel **Op order assembleren**, wordt niet verwacht dat het artikel in voorraad is, en moet het worden samengesteld op een verkooporder. Wanneer u het artikel invoert op een verkooporderregel, wordt automatisch een assemblageorder gemaakt en gekoppeld aan de verkooporder.  

> [!NOTE]  
>  Als sommige op-order-assembleren-artikelen al in de voorraad zijn, kunt u die hoeveelheid aftrekken van de assemblageorder en reserveren uit de voorraad. Zie voor meer informatie [Procedure: voorraadartikelen verkopen in assembleren-op-order-stromen](assembly-how-to-sell-assemble-to-order-items-and-inventory-items-together.md).  

In deze procedure kunt u de verkoop van een artikel verwerken dat wordt samengesteld volgens de specificaties die zijn aangevraagd door de klant. De stappen omvatten het initiëren van de verkooporderregel, het aanpassen van het assemblageartikel door het bewerken van de onderdelen en bronnen, controle van de beschikbaarheid om een leverdatum vast te stellen en het vrijgeven van de verkooporder voor onmiddelijke assemblage en verzending.  

> [!NOTE]  
>  De volgende procedure bevat niet de standaard verkooporderstappen die u moet volgen vóór de stap waarin u het op-order-assembleren-artikel invoert op een verkooporderregel.  

## <a name="to-sell-an-item-that-is-assembled-to-order"></a>Een artikel verkopen dat is samengesteld voor een order  
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Verkooporders** in en klik vervolgens op de gerelateerde koppeling.  
2.  Een verkooporder maken. Zie [Procedure: Producten verkopen](sales-how-sell-products.md) voor meer informatie.  
3.  Selecteer in het veld **Nr.** een artikel in dat is ingesteld om op order te worden geassembleerd.  
4.  Definieer vanuit welke vestiging het artikel moet worden verkocht in het veld **Vestiging**. Het assemblageproces wordt uitgevoerd in die vestiging.  
5.  Voer het aantal te verkopen artikelen in in het veld **Hoeveelheid**.  

    > [!NOTE]  
    >  Als een of meer onderdelen van het aantal aangevraagde assemblageartikelen niet beschikbaar is, verschijnt een venster met een gedetailleerde beschikbaarheidswaarschuwing. Zie voor meer informatie Beschikbaarheid assemblage.  

    Een assemblageorder wordt nu automatisch gemaakt en gekoppeld aan de verkooporderregel. De vervaldatum van de assemblageorder wordt gesynchroniseerd met de verzenddatum van de verkooporderregel.  

    Het te verkopen aantal wordt gekopieerd naar het veld **Aantal voor op order assembleren**. Dat geeft aan dat de artikelinstellingen verwacht dat het volledige aantal op de verkoopregel wordt geassembleerd op order. U kunt een kleinere hoeveelheid op order assembleren, bijvoorbeeld als u weet dat sommige items al beschikbaar zijn. Zie voor meer informatie [Procedure: voorraadartikelen verkopen in assembleren-op-order-stromen](assembly-how-to-sell-inventory-items-in-assemble-to-order-flows.md).  

6.  Om aan te geven dat de klant nog een artikel in een kit wil, kiest u op het sneltabblad **Regels** de actie **Regel**, kiest u de actie **Op order assembleren** en kiest u vervolgens de actie **Op orderregels assembleren** om de standaard assemblagecomponenten weer te geven en te wijzigen. U kunt ook het veld **Aantal voor op order assembleren** kiezen.  
7.  In het venster **Op orderregels assembleren** maakt u een nieuwe regel van het type **Artikel** voor de gevraagde aanvullende kit-inhoud. De regel verwijst naar een extra assemblagecomponent.  

    U kunt de volgorde ook aanpassen door de hoeveelheid van één standaard artikel in de kit te verhogen. U kunt dit doen door de waarde in het veld **Aantal per** op de specifieke assemblageorderregel te verhogen.  

    > [!NOTE]  
    >  Het venster **Op orderregels assembleren** bevat alleen de basisvelden die een verkoper moet gebruiken om het onderdeeloverzicht aan te passen, artikeltraceringsnummers toe te voegen of problemen met de beschikbaarheid op te lossen. Voor meer informatie over assemblageorders, zoals de begindatum van een assemblageorder, kies op het tabblad **Start** in de groep **Proces** de optie **Documenten weergeven**. Hiermee opent u een volledige weergave van de assemblageorder die is gekoppeld aan de verkooporderregel. U kunt de inhoud van de meeste velden op de assemblageorderkop niet wijzigen en u kunt de assemblageuitvoer niet boeken omdat u de optie verzending boeken van de verkooporderregel moet gebruiken.  
    >   
    >  Op de kop van gekoppelde assemblageorders kan alleen het veld **Begindatum** worden gewijzigd zodat assemblagemedewerkers een eerdere datum dan de vervaldatum kunnen opgeven wanneer zij het proces starten. Alle velden op de regels van de gekoppelde assemblageorder kunnen worden gewijzigd, zodat magazijnmedewerkers verbruikcijfers kunnen invoeren tijdens het proces.  

8.  Op problemen met de beschikbaarheid componenten of controleren. Selecteer bijvoorbeeld een beschikbaar vervangingsartikel of stel een latere vervaldatum in.  
9. Sluit het venster **Op orderregels assembleren**. De gekoppelde assemblageorder is nu klaar om de aangepaste items op de vervaldatum te assembleren.  
10. Kies in de verkooporder de actie **Vrijgeven** om de assemblageafdeling te informeren dat het assemblageproces kan worden gestart.  
11. Voer de stappen uit van de montage van de artikelen die in deze procedure worden verkocht in de montageafdeling. Zie [Procedure: Artikelen assembleren](assembly-how-to-assemble-items.md) voor meer informatie.  

## <a name="see-also"></a>Zie ook  
[Assemblagebeheer](assembly-assemble-items.md)  
[Procedure: Werken met stuklijsten](inventory-how-work-BOMs.md)  
[Voorraad](inventory-manage-inventory.md)  
[Ontwerpdetails: Magazijnbeheer](design-details-warehouse-management.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


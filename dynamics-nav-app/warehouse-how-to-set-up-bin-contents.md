---
title: Opslaglocatie-inhoud maken
description: "Nadat u opslaglocaties hebt gemaakt, kunt u de opslaglocatie-inhoud instellen. U kunt instellen welke artikelen u in een bepaalde opslaglocatie wilt opslaan en opslagrichtlijnen voor de locatie definiëren."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 2fe2b29ff5c374d7b40f18bddfde4c66ce032e18
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-bin-contents"></a>Procedure: opslaglocatie-inhoud maken
Nadat u opslaglocaties hebt gemaakt, kunt u de opslaglocatie-inhoud instellen. U kunt instellen welke artikelen u in een bepaalde opslaglocatie wilt opslaan en opslagrichtlijnen voor de locatie definiëren. U kunt dit handmatig doen in het venster **Opslaglocatie-inhoud** of automatisch met het venster **Opslaglocatie-inhoud maken**.

## <a name="to-create-bin-content-manually"></a>Opslaglocatie-inhoud handmatig maken  
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Vestigingen** in en klik vervolgens op de gerelateerde koppeling.  
2.  Selecteer de locatie waarin u opslaglocatie-inhoud wilt instellen en kies de actie **Opslaglocaties**.  
3.  Selecteer de opslaglocatie waarin u opslaglocatie-inhoud wilt instellen en kies de actie **Inhoud**.  
4.  Voor elk artikel dat u in de vestiging wilt opslaan voert u de juiste informatie in op een regel in het venster **Opslaglocatie-inhoud**. Sommige velden zijn al automatisch ingevuld met gegevens over de opslaglocatie.  
5.  Vul eerst het veld **Artikelnr.** in en vervolgens, als u gestuurde opslag en pick gebruikt, de andere velden, zoals **Eenheidscode**, **Max. Aantal** en **Min. Aantal**.  

Selecteer het veld **Vast** indien nodig. Indien de opslaglocatie als standaardopslaglocatie voor het item moet worden gebruikt, selecteert u het veld **Standaardopslaglocatie**.  

Als u met gestuurde opslag en pick werkt en via de artikelkaart de juiste gegevens hebt ingevoerd over de maten van elk artikel, wordt het maximumaantal dat u opgeeft in het venster **Opslaglocatie-inhoud** automatisch vergeleken met de fysieke capaciteit van de opslaglocatie. Vervolgens worden de minimum- en maximumwaarden gebruikt bij het berekenen van aanvullingen en bij het maken van opslagvoorstellen.  

Als u het veld **Vast** selecteert, koppelt u het artikel aan de opslaglocatie. Dit betekent dat [!INCLUDE[d365fin](includes/d365fin_md.md)] zal proberen het artikel in de opslaglocatie te plaatsen als er ruimte voor is. Bovendien blijft de record behouden waarin het artikel is gekoppeld aan de opslaglocatie, ook als het aantal in de opslaglocatie 0 is. Andere artikelen kunnen in de opslaglocatie worden opgeslagen, ook als een bepaald artikel aan de opslaglocatie is toegewezen.  

> [!NOTE]  
>  U kunt de inhoud van meerdere opslaglocaties tegelijkertijd instellen in het **opslaglocatie-inhoudmaakvoorstel**.  

## <a name="to-create-bin-content-with-a-worksheet"></a>Opslaglocatie-inhoud met een voorstel maken  
Wanneer u de opslaglocaties hebt gemaakt, kunt u in het maakvoorstel voor opslaglocatie-inhoud instellen wat u in per opslaglocatie wilt opslaan.

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Voorstel opslaglocatie-inhoudaanmaak** in en klik vervolgens op de gerelateerde koppeling.  
2.  Selecteer het voorstel van de vestiging waarvoor u de opslaglocatie-inhoud wilt maken in het veld **Naam** op de voorstelkop.  
3.  Selecteer de opslaglocatie waarvan u de inhoud wilt definiëren in het veld **Opslaglocatie**.   

    Als u in deze vestiging met gestuurde opslag en pick werkt, worden de velden met betrekking tot de desbetreffende opslaglocatie automatisch ingevuld, bijvoorbeeld **Opslaglocatiesoort**, **Magazijnklasse** en **Opslaglocatievolgorde**. U moet deze informatie in acht nemen wanneer u de opslaglocatie-inhoud definieert.  
4.  Selecteer het artikel dat u aan de opslaglocatie wilt toewijzen en vul de velden in die van toepassing zijn op de opslaglocatie-inhoud. Als u met gestuurde opslag en pick werkt en de functie **Opslaglocatieaanvulling berekenen** wilt gebruiken, vult u de velden **Max. aantal** en **Min. aantal** in.  

    Als u wilt dat deze opslaglocatie voor het artikel voorrang krijgt, zelfs als het aantal voor de opslaglocatie **0** is bij gelijke waarden voor alle andere opslagcriteria, schakelt u het selectievakje **Vast** in.  
5.  Herhaal stap 3 tot en met 4 voor elk artikel dat u aan een opslaglocatie wilt toewijzen.  
6.  Kies de actie **Afdrukken** om de zojuist in het voorstel ingevoerde opslaglocatie-inhoud weer te geven en af te drukken. Indien nodig kunt u de gegevens wijzigen, totdat alles naar wens is.  
7.  Als u klaar bent, kiest u de actie **Opslaglocatie-inhoud maken**.  

In dit voorstel werkt u met een aantal regels voor de inhoud van verschillende opslaglocaties, zodat u een goed overzicht krijgt van de inhoud van de opslaglocaties in een bepaalde zone, gang of rek.  

## <a name="see-also"></a>Zie ook
[Procedure: Opslagloc.-aanvulling berekenen](warehouse-how-to-calculate-bin-replenishment.md)    
[Magazijnbeheer](warehouse-manage-warehouse.md)  
[Voorraad](inventory-manage-inventory.md)  
[Magazijnbeheer instellen](warehouse-setup-warehouse.md)     
[Assemblagebeheer](assembly-assemble-items.md)    
[Ontwerpdetails: Magazijnbeheer](design-details-warehouse-management.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


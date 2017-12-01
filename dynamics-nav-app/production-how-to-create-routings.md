---
title: Bewerkingsplannen maken
description: Een bewerkingsplan bevat de belangrijkste gegevens met betrekking tot wat er nodig is voor het productieproces voor een bepaald geproduceerd artikel. Zodra er voor een artikel een productieorder is gemaakt, worden op basis van het bewerkingsplan ervan de bewerkingen gepland zoals weergegeven in het venster **Prod.-orderbewerkingsplan** onder de productieorder.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/04/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 49cce1f32f1d66dc17c0d9758937541ef1baaae7
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-routings"></a>Procedure: bewerkingsplannen maken
Productiebedrijven maken gebruik van bewerkingsplannen om het productieproces te visualiseren en aan te sturen.

Een bewerkingsplan vormt de basis voor procesplanning, capaciteitsplanning, de geplande toewijzing van materiaalbehoeften en productiedocumenten.  

Voor productiestuklijsten worden de bewerkingsplannen toegewezen aan het productie-eindartikel. Een bewerkingsplan bevat de belangrijkste gegevens met betrekking tot wat er nodig is voor het productieproces voor een bepaald geproduceerd artikel. Zodra er voor een artikel een productieorder is gemaakt, worden op basis van het bewerkingsplan ervan de bewerkingen gepland zoals weergegeven in het venster **Prod.-orderbewerkingsplan** onder de productieorder.  

Voordat u een bewerkingsplan kunt instellen, moet het volgende zijn gedaan:  

- Er zijn artikelkaarten gemaakt voor hoofdartikelen die onderdeel zijn van de productie. Zie [Procedure: Nieuwe artikelen registreren](inventory-how-register-new-items.md) voor meer informatie.
- Er zijn productieresources ingesteld. Zie voor meer informatie [Procedure: Afdelingen en bewerkingsplaatsen instellen](production-how-to-set-up-work-and-machine-centers.md).

## <a name="to-create-a-routing"></a>Een bewerkingsplan maken  
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Bewerkingsplannen** in en klik op de gerelateerde koppeling.  
2.  Kies de actie **Nieuw**.  
3. Vul de velden in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4.  Selecteer in het veld **Soort** de optie **Serieel** om bewerkingen in het productiebewerkingsplan te berekenen op basis van de waarde in het veld **Bewerkingsnr.**. te kiezen.   
    Selecteer **Parallel** om de bewerkingen te berekenen op basis van de waarde in het **Volgend bewerkingsnr.** te kiezen.  
5.  Als u het bewerkingsplan wilt bewerken, stelt u het veld **Status** in op **Nieuw** of **In ontwikkeling**. Als u het wilt inschakelen, stelt u het veld **Status** in op **Gecertificeerd**.  

    Vul de bewerkingsplanregels in.
6.  Voer in het veld **Bewerkingsnr.** het nummer in van de eerste bewerking in, bijvoorbeeld **10**.  
7.  In het veld **Soort** geeft u op wat voor soort resource wordt gebruikt (bijvoorbeeld **Afdeling**).  
8.  Selecteer in het veld **Nr.** de resource of typ deze resource in het veld.  
9.  In het veld **Bewerkingsplankoppeling** voert u een code in om het onderdeel aan een bepaalde bewerking te koppelen. Zie de sectie Bewerkingsplankoppelingen maken voor meer informatie.
10.  Geef in de velden **Bewerkingstijd** en **Insteltijd** de verwerkingstijden op die nodig zijn voor de uitvoering van de bewerking.  

    > [!NOTE]  
    >  De insteltijd wordt per productieorder berekend en de bewerkingstijd per geproduceerd artikel.  

11.  Geef in het veld **Gelijktijdige capaciteit** op hoeveel eenheden van de geselecteerde resource worden gebruikt om de bewerking uit te voeren. Bij toewijzing van twee personen aan één verpakkingsbewerking wordt de bewerkingstijd bijvoorbeeld gehalveerd  
12.  Ga door met het invullen van de regels voor alle bewerkingen die betrokken zijn bij de productie van het desbetreffende artikel.  
13.  Als u regels wilt kopiëren uit een bestaand bewerkingsplan, kiest u de actie **Bewerkingsplan kopiëren** om bestaande regels te selecteren.  
14. Certificeer het bewerkingsplan.  
15. U kunt nu het nieuwe bewerkingsplan aan de kaart van het desbetreffende productieartikel koppelen door het veld **Bew.-plannr.** in te vullen. Zie [Procedure: Nieuwe artikelen registreren](inventory-how-register-new-items.md) voor meer informatie.  

> [!NOTE]  
>  Zorg ervoor dat u de vaste verrekenprijs van het artikel opnieuw berekent vanuit de kaart **Artikel**: kies hiervoor achtereenvolgens de acties **Productie**, **Vaste verrekenprijs berekenen** en **Alle niveaus**.  

## <a name="to-create-routing-links"></a>Bewerkingsplankoppelingen maken
Met bewerkingsplankoppelingen kunt u materialen zodanig aan bepaalde bewerkingen koppelen dat hun relatie behouden blijft ook al wordt de productiestuklijst of het bewerkingsplan gewijzigd. Ook kunnen hierdoor gemakkelijker materialen nog op het laatste moment worden afgeboekt, namelijk op het moment dat de specifieke gekoppelde bewerking wordt opgestart in plaats van wanneer de gehele productieorder wordt vrijgegeven. Zie voor meer informatie [Procedure: materialen afboeken op basis van de uitvoer van een bewerking](production-how-to-flush-components-according-to-operation-output.md).  

Een ander belangrijk voordeel van het koppelen van materialen en bewerkingen is dat beide elementen in een logische processtructuur worden weergegeven wanneer u het venster **Productiedagboek** gebruikt voor het boeken van output en verbruik.  

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Bewerkingsplannen** in en klik op de gerelateerde koppeling.  
2.  Open het bewerkingsplan dat de bewerkingen bevat die moeten worden gekoppeld.  

    Controleer of de status van het bewerkingsplan **In ontwikkeling** is.  

3.  Op de desbetreffende bewerkingsplanregel in de **Bewerkingsplankoppeling** selecteert u een code.  
4.  Voeg in het bewerkingsplan desgewenst nog andere koppelingen toe aan andere bewerkingen.  

    > [!NOTE]  
    >  U kunt het beste niet meer dan één bewerking in een bewerkingsplan koppelen om te voorkomen dat u per ongeluk hetzelfde materiaal aan twee verschillende bewerkingen koppelt, zodat het tweemaal wordt verbruikt.  
    >   
    >  Het is aan te raden om de bewerkingsplankoppeling dezelfde naam te geven als de bewerking zelf om er zeker van te zijn dat materialen maar aan één bewerking worden gekoppeld.

5.  Stel de status van het bewerkingsplan in op **Gecertificeerd**.  

    Nu worden bewerkingsplankoppelingen aan bewerkingen toegewezen. Vervolgens moet u de feitelijke koppeling maken door dezelfde codes toe te wijzen aan bepaalde materialen in de desbetreffende productiestuklijst.  

6.  Open de **productiestuklijst** met de onderdelen die aan de bovenstaande bewerkingen moeten worden gekoppeld. Zie voor meer informatie [Procedure: productiestuklijsten maken](production-how-to-create-production-boms.md).
7.  Controleer of de status van de stuklijst **In ontwikkeling** is.  
8.  Op de regel van de desbetreffende productiestuklijst in het veld **Bewerkingsplankoppeling** selecteert u de code die u zojuist hebt toegewezen aan de desbetreffende bewerking.  
9. Ga door met het toevoegen van materialen aan unieke bewerkingen waar dat nodig is.  
10. Stel de status van de productiestuklijst in op **Gecertificeerd**.  

    > [!NOTE]  
    >  In een bestaande productieorder kunnen de bewerkingsplankoppelingen pas worden gebruikt nadat u die order hebt vernieuwd. Zie voor meer informatie [Procedure: productieorders maken](production-how-to-create-production-orders.md).  

De geselecteerde materialen worden gekoppeld aan de geselecteerde bewerkingen zodra u een productieorder maakt of vernieuwt met behulp van de desbetreffende productiestuklijst en het desbetreffende bewerkingsplan. Dit is in het venster **Prod.-ordermaterialen** te zien onder de productieorder. In dit venster kunt u ook op elk moment bewerkingsplankoppelingen verwijderen en toevoegen.

## <a name="to-assign-personnel-tools-and-quality-measures-to-routing-operations"></a>Medewerkers, tools en kwaliteitsmetingen toewijzen aan bewerkingsplannen
Als u voor een bewerking medewerkers met speciale kwalificaties, speciale kennis of speciale autorisaties nodig hebt, kunt u deze medewerkers toewijzen aan de bewerking. Daarnaast kunt u tools en kwaliteitsvereisten toewijzen aan de bewerking. In deze procedure wordt beschreven hoe u personeel toewijst. De stappen zijn vergelijkbaar voor andere soorten bewerkinginformatie.

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Bewerkingsplannen** in en klik op de gerelateerde koppeling.  
2.  Open het betreffende bewerkingsplan.  
3.  Op het sneltabblad **Regels** selecteert u de regel die u wilt verwerken en vervolgens kiest u de actie **Medewerkers**.  
4.  Vul de velden in het venster **Medewerkers bewerkingsplan** in.  
5.  Kies de knop **OK** om het venster te verlaten. De ingevoerde waarden worden gekopieerd en toegewezen aan de bewerking.    

## <a name="to-create-a-new-versions-of-a-routing"></a>Nieuwe versies maken van bewerkingsplannen  
Het versieprincipe stelt u in staat verschillende versies van een bewerkingsplan te beheren. De structuur van de bewerkingsplanversie komt overeen met de structuur van het bewerkingsplan: een bewerkingsplanversiekop en -regels. Het belangrijkste verschil wordt bepaald door de begindatum.  

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Bewerkingsplannen** in en klik op de gerelateerde koppeling.  
2.  Selecteer het bewerkingsplan dat u wilt kopiëren en kies de actie **Versies**.  
3. Kies in het venster **Bewerkingsplanversies** de actie **Nieuw**.
4. Vul de velden in.
5.  Voer in het veld **Versiecode** de unieke identificatie van de versie in. Alle combinaties van cijfers en letters zijn toegestaan.  

    De nieuwe versie krijgt automatisch de status **Nieuw**.  
6.  Als u bewerkingsregels wilt maken, selecteert u de eerste lege regel en vult u bij **Bewerkingsnr.** de waarde in die overeenkomt met de volgorde van de bewerkingen.

    De bewerkingsregels worden in oplopende volgorde gesorteerd op bewerkingsnummers. Als u later nog wijzigingen of toevoegingen wilt maken, is het raadzaam dat u tussen iedere stap voldoende ruimte voor tussenstappen laat. Het veld **Volgend bewerkingsnr.** verwijst naar de volgende bewerking. Het nummer van de bewerking kan rechtstreeks worden ingevoerd.

7. Wanneer de bewerkingsplanversie is voltooid, wordt het veld **Status** ingesteld op **Gecertificeerd**.

De geldigheid van de versie wordt aangegeven in het veld **Begindatum**.  

## <a name="see-also"></a>Zie ook  
[Procedure: productiestuklijsten maken](production-how-to-create-production-boms.md)  
[Productie instellen](production-configure-production-processes.md)  
[Productie](production-manage-manufacturing.md)    
[Gepland](production-planning.md)   
[Voorraad](inventory-manage-inventory.md)  
[Inkoop](purchasing-manage-purchasing.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


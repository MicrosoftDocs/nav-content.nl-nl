---
title: 'Procedure: Ontvangen en opslaan in standaardmagazijnconfiguraties'
description: In [!INCLUDE[d365fin](includes/d365fin_md.md)] kunnen de inkomende processen voor ontvangst en opslag op vier manieren worden uitgevoerd met verschillende functionaliteiten, afhankelijk van het complexiteitsniveau van het magazijn.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 0a540f5813ed67ee62e43390d6d11b7c3a137f13
ms.contentlocale: nl-nl
ms.lasthandoff: 10/23/2017

---
# <a name="walkthrough-receiving-and-putting-away-in-basic-warehouse-configurations"></a>Procedure: ontvangen en opslaan in standaardmagazijnconfiguraties
In [!INCLUDE[d365fin](includes/d365fin_md.md)] kunnen de inkomende processen voor ontvangst en opslag op vier manieren worden uitgevoerd met verschillende functionaliteiten, afhankelijk van het complexiteitsniveau van het magazijn.  

|Methode|Inkomend proces|Opslaglocaties|Ontvangsten|Magazijnopslag|Complexiteitsniveau (zie [Ontwerpdetails: Magazijninstelling](design-details-warehouse-setup.md))|  
|------------|---------------------|----------|--------------|----------------|--------------------------------------------------------------------------------------------------------------------|  
|A|Ontvangst en opslag van de orderregel boeken|X|||2|  
|B|Ontvangst en opslag van een voorraadopslagdocument boeken|||X|3|  
|L|Ontvangst en opslag van een magazijnontvangstdocument boeken||X||5-4-6|  
|D|Ontvangst van een magazijnontvangstdocument en opslag van een magazijnopslagdocument boeken||X|X|5-4-6|  

Zie voor meer informatie [Ontwerpdetails: Inkomende magazijnstroom](design-details-inbound-warehouse-flow.md).  

De volgende procedure geeft methode B in de vorige tabel weer.  

## <a name="about-this-walkthrough"></a>Informatie over deze procedure  
In standaardmagazijnconfiguraties waarbij voor uw vestiging de verwerking van opslag, maar niet van ontvangst vereist is, gebruikt u het venster **Voorraadopslag** om opslag- en ontvangstinformatie voor de inkomende brondocumenten te verzamelen en boeken. Het inkomende brondocument kan een inkooporder zijn, maar ook een verkoopretourorder, een inkomende transferorder of een productieorder met output die kan worden opgeslagen.

> [!NOTE]
> Hoewel de instellingen **Pick vereist** en **Opslag vereist** worden genoemd, kunt u nog wel ontvangsten en verzendingen rechtstreeks vanuit de bronbedrijfsdocumenten boeken voor vestigingen waarvoor u deze selectievakjes inschakelt.  

In deze procedure worden de volgende taken gedemonstreerd.  

-   Locatie ZILVER instellen voor voorraadopslag.  
-   Locatie ZILVER instellen voor opslaglocatieverwerking.  
-   Een standaardopslaglocatie voor artikel LS-81 definiëren. (LS-75 is al ingesteld in CRONUS.)  
-   Maak een inkooporder voor leverancier 10000 voor 40 luidsprekers.  
-   Controleren of de opslaglocaties vooringesteld zijn.  
-   De inkooporder vrijgeven voor magazijnverwerking.  
-   Een voorraadopslag maken op basis van een vrijgegeven brondocument.  
-   Verifiëren dat de opslaglocaties worden overgenomen van de inkooporder.  
-   De magazijnverplaatsing in het magazijn vastleggen en tegelijkertijd de inkoopontvangst voor de broninkooporder boeken.  

## <a name="roles"></a>Rollen  
In dit overzicht worden taken gedemonstreerd voor de volgende gebruikersrollen:  

-   Magazijnbeheerder  
-   Inkoper  
-   Magazijnmedewerker  

## <a name="prerequisites"></a>Vereisten  
U moet het volgende doen om deze procedure uit te voeren:  

-   CRONUS International Ltd. installeren.  
-   Maak van uzelf een magazijnwerknemer bij vestiging ZILVER door de volgende stappen uit te voeren:  

    1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Magazijnwerknemers** in en klik vervolgens op de gerelateerde koppeling.  
    2.  Kies het veld **Gebruikers-ID** en selecteer uw eigen gebruikersaccount in het venster **Gebruikers**.  
    3.  Voer ZILVER in het veld **Vestiging** in.  
    4.  Selecteer het veld **Standaard**.  

## <a name="story"></a>Scenario  
Ellen, de magazijnmanager bij CRONUS International Ltd., maakt een inkooporder voor 10 eenheden van artikel LS-75 en 30 eenheden van artikel LS-81 van leverancier 10000 om te worden afgeleverd bij magazijn ZILVER. Wanneer de bezorging in het magazijn aankomt, zet de magazijnmedewerker Johanna de artikelen in de standaardopslaglocaties die voor de artikelen zijn gedefinieerd. Wanneer Johanna de voorraadopslag boekt, worden de artikelen als ontvangen en beschikbaar voor verkoop of andere oproepen in de voorraad.  

## <a name="setting-up-the-location"></a>De locatie instellen  
 De instellingen van het venster **Vestiging** definiëren de magazijnstromen van het bedrijf.  

### <a name="to-set-up-the-location"></a>Een vestiging instellen  

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Vestigingen** in en klik vervolgens op de gerelateerde koppeling.  
2.  Open de vestigingskaart ZILVER.  
3.  Selecteer het selectievakje **Opslag vereist**.  

    Ga door met het instellen van een standaardopslaglocatie voor de twee artikelnummers om te bepalen waar deze worden opgeslagen.  

4.  Kies de actie **Opslaglocaties**.  
5.  Selecteer de eerste rij voor opslaglocatie S-01-0001 en kies vervolgens de actie **Inhoud**.  

    U ziet in het venster **Opslaglocatie-inhoud** dat artikel LS-75 al is ingesteld als inhoud in opslaglocatie S-01-0001.  

6.  Kies de actie **Nieuw**.  
7.  Selecteer de velden **Vast** en **Standaard**.  
8.  Voer in het veld **Artikelnr.** de waarde LS-81 in.  

## <a name="creating-the-purchase-order"></a>De inkooporder maken  
Inkooporders zijn de meest gebruikte soort inkomend brondocument.  

### <a name="to-create-the-purchase-order"></a>De inkooporder maken  

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Inkooporders** in en klik vervolgens op de gerelateerde koppeling.  
2.  Kies de actie **Nieuw**.  
3.  Maak een inkooporder voor leverancier 10000 op 23 januari (werkdatum) met de volgende inkooporderregels.  

    |Artikel|Vestiging|Opslaglocatie|Aantal|  
    |----------|-------------------|--------------|--------------|  
    |LS_75|ZILVER|S-01-0001|10|  
    |LS-81|ZILVER|S-01-0001|30|  

    > [!NOTE]  
    >  De opslaglocatiecode wordt automatisch ingevoerd op basis van de instellingen die u in de sectie 'De locatie instellen' heeft uitgevoerd.  

    Ga door om het magazijn te informeren dat de inkooporder klaar is voor de magazijnverwerking wanneer de bezorging aankomt.  

4.  Kies de actie **Vrijgeven**.  

    Het leveren van luidsprekers van leverancier 10000 is aangekomen op magazijn SILVER en Jan bergt ze op.  

## <a name="receiving-and-putting-the-items-away"></a>De artikelen ontvangen en opslaan  
In het venster **Voorraadopslag** kunt u alle inkomende magazijnactiviteiten voor een bepaald brondocument beheren, zoals een inkooporder.  

### <a name="to-receive-and-put-the-items-away"></a>De artikelen ontvangen en opslaan  

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Voorraadopslag** in en klik vervolgens op de gerelateerde koppeling.  
2.  Kies de actie **Nieuw**.  
3.  Selecteer het veld **Brondocument** en selecteer vervolgens **Inkooporder**.  
4.  Selecteer het veld **Bronnr.**, selecteer de regel voor de inkoop van leverancier 10000, en kies vervolgens de knop **OK**.  

    Of kies op het tabblad **Acties** in de groep **Functies** de optie **Brondocument ophalen** en selecteer de inkooporder.  

5.  Kies de actie **Te verwerken aantal autom. invullen**.  

    Of voer in het veld **Te verwerken aantal** respectievelijk 10 en 30 in op de twee voorraadopslagregels.  

6.  Kies de actie **Boeken**, selecteer de actie **Ontvangen** en kies vervolgens de knop **OK**.  

    Nu zijn de 40 luidsprekers geregistreerd als opgeslagen in opslaglocatie S-01-0001 en een positieve artikelpost is gemaakt om de geboekte inkoopontvangst te weerspiegelen.  

## <a name="see-also"></a>Zie ook  
 [Procedure: artikelen opslaan met een voorraadopslag](warehouse-how-to-put-items-away-with-inventory-put-aways.md)   
 [Procedure: standaard magazijnen met bewerkingsgebieden instellen](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md)   
 [Procedure: Onderdelen verplaatsen naar een bewerkingsgebied in standaardmagazijnconfiguraties](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md)   
 [Procedure: Picken voor productie of assemblage](warehouse-how-to-pick-for-production.md)   
 [Procedure: Artikelen ad hoc verplaatsen in standaardmagazijnconfiguraties](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md)   
 [Ontwerpdetails: Inkomende magazijnstroom](design-details-inbound-warehouse-flow.md)   
 [Procedures voor bedrijfsprocessen](walkthrough-business-process-walkthroughs.md)  
 [Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


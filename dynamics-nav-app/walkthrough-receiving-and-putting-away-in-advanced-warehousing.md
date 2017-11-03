---
title: 'Procedure: Ontvangen en opslaan in geavanceerde magazijnconfiguraties'
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
ms.openlocfilehash: c0621092f75f5bfcecce29029c67c68c16451901
ms.contentlocale: nl-nl
ms.lasthandoff: 10/23/2017

---
# <a name="walkthrough-receiving-and-putting-away-in-advanced-warehouse-configurations"></a>Procedure: Ontvangen en opslaan in geavanceerde magazijnconfiguraties
In [!INCLUDE[d365fin](includes/d365fin_md.md)] kunnen de inkomende processen voor ontvangst en opslag op vier manieren worden uitgevoerd met verschillende functionaliteiten, afhankelijk van het complexiteitsniveau van het magazijn.  

|Methode|Inkomend proces|Opslaglocaties|Ontvangsten|Magazijnopslag|Complexiteitsniveau (zie [Ontwerpdetails: Magazijninstelling](design-details-warehouse-setup.md))|  
|------------|---------------------|----------|--------------|----------------|--------------------------------------------------------------------------------------------------------------------|  
|A|Ontvangst en opslag van de orderregel boeken|X|||2|  
|B|Ontvangst en opslag van een voorraadopslagdocument boeken|||X|3|  
|L|Ontvangst en opslag van een magazijnontvangstdocument boeken||X||5-4-6|  
|D|Ontvangst van een magazijnontvangstdocument en opslag van een magazijnopslagdocument boeken||X|X|5-4-6|  

Zie voor meer informatie [Ontwerpdetails: Inkomende magazijnstroom](design-details-inbound-warehouse-flow.md).  

De volgende procedure geeft methode D in de vorige tabel weer.  

## <a name="about-this-walkthrough"></a>Informatie over deze procedure  
In geavanceerde magazijnconfiguraties waarbij voor uw vestiging is ingesteld dat naast de opslag ook de ontvangst moet worden verwerkt, gebruikt u het venster **Magazijnontvangst** om de ontvangst van artikelen op meerdere inkomende orders vast te leggen en te boeken. Wanneer de magazijnontvangst wordt geboekt, worden een of meer magazijnopslagdocumenten gemaakt om magazijnmedewerkers te instrueren het ontvangen artikel op aangewezen locaties te plaatsen, op basis van opslaglocatie-instellingen of in verschillende opslaglocaties. De specifieke plaatsing van de artikelen wordt geregistreerd wanneer de magazijnopslag wordt geregistreerd. Het inkomende brondocument kan een inkooporder zijn, maar ook een verkoopretourorder, een inkomende transferorder, assemblageorder of productieorder met output die kan worden opgeslagen. Als de ontvangst van een inkomende order is gemaakt, kan meer dan een inkomend brondocument worden opgehaald voor de ontvangst. Met deze methode kunt u diverse artikelen die worden afgeleverd van verschillende aankomend inkomende orders, registreren met één ontvangst.  

In deze procedure worden de volgende taken gedemonstreerd.  

-   Vestiging WIT instellen voor het ontvangen en opslaan.  
-   Twee inkooporders voor volledige magazijnverwerking maken en vrijgeven.  
-   Een magazijnontvangstdocument voor meerdere inkooporderregels van specifieke leveranciers maken en boeken.  
-   Een magazijnopslag voor de ontvangen artikelen registreren.  

## <a name="roles"></a>Rollen  
In dit overzicht worden taken gedemonstreerd voor de volgende gebruikersrollen:  

-   Magazijnbeheerder  
-   Inkoper  
-   Ontvangend personeel  
-   Magazijnmedewerker  

## <a name="prerequisites"></a>Vereisten  
U moet het volgende doen om deze procedure uit te voeren:  

-   CRONUS International Ltd. installeren.  
-   U maakt van uzelf een magazijnwerknemer bij vestiging WIT door de volgende stappen uit te voeren:  

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Magazijnwerknemers** in en klik vervolgens op de gerelateerde koppeling.  
2.  Kies het veld **Gebruikers-ID** en selecteer uw eigen gebruikersaccount in het venster **Gebruikers**.  
3.  Voer WIT in het veld **Vestiging** in.  
4.  Selecteer het veld **Standaard**.  

## <a name="story"></a>Scenario  
Ellen, de magazijnmanager bij CRONUS International Ltd., maakt twee inkooporders voor accessoires van leverancier 10000 en 20000 om te worden afgeleverd bij magazijn WIT. Als de leveringen in het magazijn aankomen, gebruikt Sammy, die verantwoordelijk is voor de ontvangst van artikelen van leveranciers 10000 en 20000, een filter om ontvangstregels te maken voor inkooporders van de twee leveranciers. Sammy boekt de artikelen als ontvangen in voorraad in een magazijnontvangst en maakt de artikelen beschikbaar voor verkoop of andere vraag. De magazijnmedewerker Johanna neemt de artikelen uit de opslaglocatie en zet ze weg. Hij zet alle eenheden in hun standaardopslaglocaties, behalve 40 van 100 ontvangen scharnieren die hij opslaat in de montageafdeling door de opslagregel te splitsen. Wanneer John de opslag registreert, wordt de inhoud van de opslaglocatie bijgewerkt en worden de artikelen beschikbaar gemaakt om vanuit het magazijn te worden gepickt.  

## <a name="reviewing-the-white-location-setup"></a>Instellingen van de vestiging WIT controleren  
De instellingen van het venster **Vestiging** definiëren de magazijnstromen van het bedrijf.  

### <a name="to-review-the-location-setup"></a>De vestigingsinstellingen controleren  

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Vestigingen** in en klik vervolgens op de gerelateerde koppeling.  
2.  Open de vestigingskaart WIT.  
3.  Controleer op het sneltabblad **Magazijn** of het selectievakje **Gestuurde opslag en pick** is ingeschakeld.  

    Dit betekent dat de vestiging wordt ingesteld voor het hoogste complexiteitniveau, wat wordt aangegeven door het feit dat alle selectievakjes voor magazijnverwerking op het sneltabblad zijn ingeschakeld.  

4.  Controleer op het sneltabblad **Opslaglocaties** of de opslaglocaties in de velden **Ontvangstopslaglocatie** en **Verzendopslaglocatie** zijn opgegeven.  

Dit betekent dat als u een magazijnontvangst maakt, deze opslaglocatiecode standaard naar de koptekst van het magazijnontvangstdocument wordt gekopieerd en naar de regels van de resulterende magazijnopslag.  

## <a name="creating-the-purchase-orders"></a>De inkooporders maken  
Inkooporders zijn de meest gebruikte soort inkomend brondocument.  

### <a name="to-create-the-purchase-orders"></a>De inkooporders maken  

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Inkooporders** in en klik vervolgens op de gerelateerde koppeling.  
2.  Kies de actie **Nieuw**.  
3.  Maak een inkooporder voor leverancier 10000 op 23 januari (werkdatum) met de volgende inkooporderregels.  

    |Artikel|Vestiging|Aantal|  
    |----------|-------------------|--------------|  
    |70200|WIT|100 stuks|  
    |70201|WIT|50 stuks|  

    Ga door om het magazijn te informeren dat de inkooporder klaar is voor de magazijnverwerking wanneer de bezorging aankomt.  

4.  Kies de actie **Vrijgeven**.  

    U kunt nu doorgaan om de tweede inkooporder te genereren.  

5.  Kies de actie **Nieuw**.  
6.  Maak een inkooporder voor leverancier 20000 op de werkdatum met de volgende inkooporderregels.  

    |Artikel|Vestiging|Aantal|  
    |----------|-------------------|--------------|  
    |70100|WIT|10 CAN|  
    |70101|WIT|12 CAN|  

    Kies de actie **Vrijgeven**.  

    De leveringen van artikelen van leveranciers 10000 en 20000 zijn aangekomen in magazijn WIT en Sammy begint inkoopontvangsten te verwerken.  

## <a name="receiving-the-items"></a>De artikelen ontvangen  
In het venster **Magazijnontvangst** kunt u meerdere inkomende orders beheren voor brondocumenten, zoals een inkooporder.  

### <a name="to-receive-the-items"></a>De artikelen ontvangen  
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Magazijnontvangsten** in en klik vervolgens op de gerelateerde koppeling.  
2.  Kies de actie **Nieuw**.  
3.  Voer WIT in het veld **Vestiging** in.  
4.  Kies de actie **Filters om brondoc. op te halen gebruiken**.  
5.  Voer **ACCESSORY** in het veld **Code** in.  
6.  Typ in het veld **Omschrijving** de tekst **Leveranciers 10000 en 20000**.  
7.  Kies de actie **Wijzigen**.  
8.  Voer op het sneltabblad **Inkoop** in het veld **Orderleveranciernr. Filter** de waarde **10000&#124;20000** in.  
9. Kies de actie **Uitvoeren**. De magazijnontvangst wordt gevuld met vier regels die inkooporderregels voor de opgegeven leveranciers vertegenwoordigen. Het veld **Te ontvangen aantal** is ingevuld omdat u niet het selectievakje **Te verwerken aantal niet opvullen** in het venster **Filters om brondoc. op te halen** hebt ingeschakeld.  
10. Als u een filter wilt gebruiken zoals eerder in dit gedeelte beschreven, kunt u ook de actie **Brondocument ophalen** kiezen en vervolgens inkooporders van de leverancier in kwestie selecteren.  
11. Kies de actie **Ontvangst boeken** en kies vervolgens de knop **Ja**.  

    Er worden positieve artikelposten gemaakt die de geboekte inkoopontvangsten van leveranciers 10000 en 20000 aangeven, en de artikelen zijn gereed om in het magazijn van de ontvangende opslaglocatie te worden opgeslagen.  

## <a name="putting-the-items-away"></a>Artikelen opslaan  
In het venster **Magazijnopslag** kunt u opslagactiviteiten beheren voor een specifiek magazijnontvangstdocument dat van toepassing is op meerdere brondocumenten. Net als alle magazijnactiviteitsdocumenten wordt elk artikel in de magazijnopslag weergegeven door een Nemen-regel en een Plaatsen-regel. In de volgende procedure is de opslaglocatie op de Nemen-regels de standaardopslaglocatie op vestiging WIT, W-08-0001.  

### <a name="to-put-the-items-away"></a>De artikelen opslaan  
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Magazijnontvangsten** in en klik vervolgens op de gerelateerde koppeling.  
2.  Selecteer het magazijnopslagdocument in de lijst en kies vervolgens op het tabblad **Start** in de groep **Beheren** de optie **Bewerken**.  

    Het magazijnopslagdocument wordt geopend met in totaal acht Nemen- of Plaatsen-regels voor de vier inkooporderregels.

    De magazijnmedewerker wordt verteld dat er 40 scharnieren op de montageafdeling nodig zijn. Hij splitst de ene Plaatsen-regel om een tweede Plaatsen-regel voor opslaglocatie W-02-0001 op te geven op de montageafdeling waar hij dat een deel van de ontvangen scharnieren plaatst.  

3.  Selecteer de tweede regel in het venster **Magazijnopslag**, de Plaatsen-regel, voor artikel 70200.  
4.  Wijzig de waarde in het veld **Te verwerken aantal** van 100 in 60.  
5.  Kies op het sneltabblad **Regels** de optie **Functies** en kies vervolgens **Regel splitsen**. Er wordt een nieuwe regel ingevoegd voor artikel 70200 met 40 in veld **Te verwerken aantal**.  
6.  Voer W-02-0001 in het veld **Opslaglocatie** in. Het veld **Zonecode** wordt automatisch ingevuld.  

    U kunt nu doorgaan om de opslag te registreren.  

7.  Kies de actie **Opslag registreren** en kies vervolgens de knop **Ja**.  

    De ontvangen accessoires worden nu opgeslagen in de standaardopslaglocaties van de artikelen, en 40 scharnieren worden geplaatst in de montageafdeling. De ontvangen artikelen zijn nu beschikbaar voor picken naar interne vraag, zoals assemblageorders, of naar externe de vraag, zoals verkoopverzendingen.  

## <a name="see-also"></a>Zie ook  
 [Procedure: artikelen opslaan met magazijnopslag](warehouse-how-to-put-items-away-with-warehouse-put-aways.md)   
 [Procedure: Artikelen verplaatsen in geavanceerde magazijnconfiguraties](warehouse-how-to-move-items-in-advanced-warehousing.md)   
 [Ontwerpdetails: Inkomende magazijnstroom](design-details-inbound-warehouse-flow.md)   
 [Procedure: ontvangen en opslaan in standaardmagazijnconfiguraties](walkthrough-receiving-and-putting-away-in-basic-warehousing.md)   
 [Procedures voor bedrijfsprocessen](walkthrough-business-process-walkthroughs.md)


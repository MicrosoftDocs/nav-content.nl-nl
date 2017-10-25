---
title: Dynamics NAV en Power BI Content Packs
description: Inzicht, bedrijfsinformatie en KPI's krijgen uit uw Dynamics NAV-gegevens is gemakkelijk met Power BI en de Dynamics NAV Content Packs.
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account schedule, analysis, reporting, financial report, business intelligence, KPI
ms.date: 09/05/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3442284851f3e392c1108c59b8aa7d0a417f1e51
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="enabling-your-business-data-for-power-bi"></a>Uw bedrijfgegevens gereed maken voor Power BI
Inzicht krijgen in uw [!INCLUDE[d365fin](includes/d365fin_md.md)]-gegevens is gemakkelijk met Power BI en de [!INCLUDE[d365fin](includes/d365fin_md.md)] Content Packs. Power BI haalt uw gegevens op en maakt vervolgens een kant-en-klaar dashboard en rapporteert op basis van die gegevens.  

Microsoft heeft de volgende Content Packs gepubliceerd:

| App | Description |
| --- | --- |
| Microsoft Dynamics NAV | Een dashboard met belangrijke financiële gegevens voor een bepaalde periode, zoals inkomsten tegenover onkosten, de bedrijfsmarge en de cashcyclus.|
| Microsoft Dynamics 365 for Sales | Een dashboard met belangrijke gegevens over verkoopopportunities en contacten.  |
| Microsoft Dynamics 365 for Sales | Een dashboard met belangrijke gegevens over verkopen en voorraad. |

## <a name="using-the-dashboards"></a>De dashboards gebruiken
Elk Content Pack bevat rapporten met verschillende detailniveaus:

* Kies een dashboardfunctie om een van de onderliggende rapporten weer te geven.  
* Filter het rapport of voeg velden toe die u wilt controleren.  
* Vergrendel deze aangepaste weergave op het dashboard om door te gaan met tracking.  
  U kunt gegevens handmatig vernieuwen en u kunt een schema voor vernieuwen instellen. Zie voor meer informatie [Gepland vernieuwen configureren](https://powerbi.microsoft.com/en-us/documentation/powerbi-refresh-scheduled-refresh/).  

De Content Packs zijn vooraf geconfigureerd om te werken met gegevens van het voorbeeldbedrijf die u krijgt wanneer u zich aanmeldt voor [!INCLUDE[d365fin](includes/d365fin_md.md)]. Als u de apps in Power BI installeert en u verbinding met uw eigen gegevens maakt, werken sommige rapporten mogelijk niet omdat deze afhankelijk zijn van gegevens die uw bedrijf niet heeft. In dat geval kunt u dat rapport uit het dashboard verwijderen.  

> [!NOTE]  
>   U kunt ook uw eigen rapporten en dashboards in Power BI samenstellen op basis van de [!INCLUDE[d365fin](includes/d365fin_md.md)]-gegevens. Zie voor meer informatie [Uw bedrijfsgegevens verbinden met Power BI](across-how-use-financials-data-source-powerbi.md).  

## <a name="accessing-included365finincludesd365finmdmd-in-power-bi"></a>Toegang krijgen tot [!INCLUDE[d365fin](includes/d365fin_md.md)] in Power BI
Als u uw [!INCLUDE[d365fin](includes/d365fin_md.md)]-gegevens in Power BI wilt zien, moet u het volgende hebben:  

* Toegang tot [!INCLUDE[d365fin](includes/d365fin_md.md)]. Zie [Dynamics NAV](http://go.microsoft.com/fwlink/?LinkID=759714) voor meer informatie.  
* Toegang tot Power BI. Zie voor meer informatie [Power BI](https://powerbi.microsoft.com).

Op de Power BI-site vindt u meer informatie over het [verbinding maken met services door middel van Content Packs voor Power BI](http://go.microsoft.com/fwlink/?LinkID=760850).  

Om toegang te krijgen tot de [!INCLUDE[d365fin](includes/d365fin_md.md)]-gegevens in Power BI moet u op de verbindingspagina de volgende gegevens opgeven:

| Veld | Omschrijving |
| --- | --- |
| **URL van OData-feed** |De OData-URL waarmee Power BI toegang kan krijgen tot gegevens van uw bedrijf. Voer een URL in in de notatie https://mybusiness.financials.dynamics.com:7048/MS/ODataV4/Company('Mijn%2bedrijf'). |
| **Verificatiemethode** |Kies **Basis**. |
| **Gebruikersnaam** |Voer uw naam in zoals deze wordt getoond voor uw account in [!INCLUDE[d365fin](includes/d365fin_md.md)], bijvoorbeeld *Jan Smit*. |
| **Wachtwoord** |Dit is de webservicetoegangssleutel voor uw gebruikersaccount in [!INCLUDE[d365fin](includes/d365fin_md.md)]. |

Dit betekent dat u twee verschillende gegevens van [!INCLUDE[d365fin](includes/d365fin_md.md)] moet krijgen: de *OData-URL* en de *webservicetoegangssleutel* voor uw gebruikersaccount.  

### <a name="getting-the-url"></a>De URL ophalen
Als u [!INCLUDE[d365fin](includes/d365fin_md.md)] toevoegt aan Power BI, moet u een URL opgeven zodat Power BI toegang kan krijgen tot gegevens uit uw bedrijf. Op de verbindingspagina wordt naar de URL verwezen als **URL van OData-feed** en deze moet de volgende notatie hebben:

         https://mybusiness.financials.dynamics.com:7048/MS/ODataV4/Company('CRONUS%20US')  
In dit voorbeeld is *mybusiness* de naam van uw [!INCLUDE[d365fin](includes/d365fin_md.md)]-service en is *CRONUS US* de naam van het demobedrijf, waarbij *%20* staat voor de spatie in de naam.   
Als u de URL wilt krijgen, zoekt u in [!INCLUDE[d365fin](includes/d365fin_md.md)] het venster **Webservices** en opent u dit. Dit venster bevat de webservices die momenteel beschikbaar zijn en kunt u de koppeling uit het veld **OData-URL** kopiëren voor een van de standaard OData-webservices.  

### <a name="getting-the-user-name-and-the-web-service-access-key"></a>De gebruikersnaam en de webservicetoegangssleutel krijgen
Om gegevens uit [!INCLUDE[d365fin](includes/d365fin_md.md)] te kunnen gebruiken in Power BI, moet u in het venster **Verbinden met Dynamics NAV** een gebruikersnaam en een wachtwoord opgeven. De gebruikersnaam is uw naam zoals deze voor uw account wordt getoond in [!INCLUDE[d365fin](includes/d365fin_md.md)], zodat Power BI de aanmelding bij [!INCLUDE[d365fin](includes/d365fin_md.md)] kan uitvoeren. Het wachtwoord is de webservicetoegangssleutel die voor uw account is ingesteld in [!INCLUDE[d365fin](includes/d365fin_md.md)].  

Om deze informatie te vinden, zoekt u in [!INCLUDE[d365fin](includes/d365fin_md.md)] het venster **Gebruikers**. Open hierin de kaart voor uw gebruikersaccount. Kopieer op het sneltabblad **Algemeen** de inhoud van het veld **Gebruikersnaam** en kopieer op het sneltabblad **Toegang tot webservice** de inhoud van het veld **Toegangssleutel voor webservice**. Als het veld **Toegangssleutel voor webservice** leeg is, kiest u op het lint **Toegangssleutel voor webservice wijzigen**, kiest u het veld **Sleutel verloopt nooit** en klikt u vervolgens op OK. U kunt vervolgens de sleutel kopiëren.  

## <a name="getting-data-from-included365finincludesd365finmdmd"></a>Gegevens ophalen uit [!INCLUDE[d365fin](includes/d365fin_md.md)]
Het [!INCLUDE[d365fin](includes/d365fin_md.md)]-dashboard bevat de meeste algemene rapporten die u zult willen gebruiken om uw bedrijf te traceren. De gegevens worden uit uw [!INCLUDE[d365fin](includes/d365fin_md.md)]-bedrijf opgehaald door middel van webservices die live gegevens uitlezen. In [!INCLUDE[d365fin](includes/d365fin_md.md)] worden in het venster **Webservices** de webservices weergegeven die voor u zijn ingesteld.

> [!NOTE]  
>   Als u de naam van een van deze webservices wijzigt, worden de gegevens niet weergegeven in Power BI.  
Als u andere gegevens wilt toevoegen aan Power BI, moet u de tabellen zoeken in [!INCLUDE[d365fin](includes/d365fin_md.md)], ze beschikbaar maken als webservices en ze vervolgens toevoegen aan het Content Pack. Dit is een geavanceerd scenario en het is raadzaam te beginnen met de gegevens die al in Power BI beschikbaar zijn.  

## <a name="troubleshooting"></a>Problemen oplossen
Het dashboard van Power BI gebruikt de gepubliceerde webservices die hierboven worden genoemd en bevat gegevens van het demobedrijf of uw eigen bedrijf als u gegevens importeert uit uw huidige financiële oplossing. Als er echter iets verkeerd gaat, biedt deze sectie een oplossing voor de meest voorkomende problemen.  

**"Parametervalidatie mislukt; zorg dat alle parameters geldig zijn"**  
Als u deze fout ziet deze nadat u de URL van uw [!INCLUDE[d365fin](includes/d365fin_md.md)] hebt ingevoerd, controleert u of aan de volgende vereisten is voldaan:  

* De URL volgt exact dit patroon:

    https://mybusiness.financials.dynamics.com:7048/MS/ODataV4/Company('CRONUS%20US')  
* Verwijder eventuele tekst na de bedrijfsnaam tussen haakjes  
* Zorg ervoor dat er geen voorwaartse eindslash aan het eind van de URL staat.  
* Controleer of het een veilige verbinding is zoals aangegeven door de URL die begint met *https*.  

**"Aanmelding mislukt"**  
Als u de fout "Aanmelding mislukt" krijgt wanneer u zich aanmeldt bij het dashboard met uw [!INCLUDE[d365fin](includes/d365fin_md.md)]-referenties, kan dat een van de volgende oorzaken hebben:

* De account die u gebruikt, heeft geen machtigingen om de [!INCLUDE[d365fin](includes/d365fin_md.md)]-gegevens uit uw account te lezen.

    Controleer uw gebruikersaccount in [!INCLUDE[d365fin](includes/d365fin_md.md)] en let erop dat u de juiste webservicetoegangssleutel als wachtwoord gebruikt. Probeer het vervolgens opnieuw.  
* Het [!INCLUDE[d365fin](includes/d365fin_md.md)]-exemplaar waarmee u verbinding probeert te maken, heeft geen geldig SSL-certificaat. In dit geval ziet u een gedetailleerde foutmelding ("kan geen vertrouwde SSL-relatie tot stand brengen").

    > [!NOTE]  
>   Zelfondertekende certificaten worden niet ondersteund.  

**"Oops"**  
Als u een "Oops"-foutdialoogvenster ziet na het verificatiedialoogvenster, komt dat meestal door een probleem bij het maken van verbinding met de gegevens voor het Content Pack.

* Controleer of de URL het patroon volgt dat eerder is opgegeven:

    `https://mybusiness.financials.dynamics.com:7048/MS/ODataV4/Company('CRONUS%20US')`  
* Een veel voorkomende vergissing is de volledige URL op te geven voor een specifieke webservice:

    `https://mybusiness.financials.dynamics.com:7048/MS/ODataV4/Company('CRONUS%20US')/powerbifinance`
* Of het kan zijn dat u vergeten bent de bedrijfsnaam op te geven:

    `https://mybusiness.financials.dynamics.com:7048/MS/ODataV4/`

## <a name="see-also"></a>Zie ook
[Bedrijfsinformatie](bi.md)  
[Welkom bij [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Bedrijfsgegevens migreren uit andere financiële systemen](upload-data.md)  
[[!INCLUDE[d365fin_long](includes/d365fin_long_md.md)] gebruiken als Power BI-gegevensbron](across-how-use-financials-data-source-powerbi.md)  


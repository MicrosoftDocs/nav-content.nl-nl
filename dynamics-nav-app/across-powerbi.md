---
title: Het Content Pack Dynamics NAV voor Power BI gebruiken
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: ad9519b8ce9c244480308ccc99c05e78e4926b06
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---

# <a name="using-the-dynamics-nav-content-pack-for-power-bi"></a>Het Content Pack Dynamics NAV voor Power BI gebruiken
Inzicht krijgen in uw Dynamics NAV-gegevens is gemakkelijk met Power BI en de Dynamics NAV Content Pack. Power BI haalt uw gegevens op en maakt vervolgens een kant-en-klaar dashboard en rapporteert op basis van die gegevens.  

Het Content Pack is vooraf geconfigureerd om te werken met verkoopgegevens en financiële gegevens uit het demobedrijf dat u krijgt wanneer u zich aanmeldt voor het Dynamics NAV-voorbeeld.  

- Kies een functie op het dashboard om een van de zeven onderliggende rapporten weer te geven.  
- Filter het rapport of voeg velden toe die u wilt controleren.  
- Vergrendel deze aangepaste weergave op het dashboard om door te gaan met tracking.  
Het dashboard en onderliggende rapporten worden dagelijks vernieuwd. U kunt het vernieuwingsschema bepalen en de frequentie wijzigen voor de gegevensset.  

## <a name="accessing-dynamics-nav-in-power-bi"></a>Toegang krijgen tot Dynamics NAV in Power BI
Als u uw Dynamics NAV-gegevens in Power BI wilt zien, moet u het volgende hebben:  

- Toegang tot Dynamics NAV. Zie [Dynamics NAV](http://go.microsoft.com/fwlink/?LinkID=759714) voor meer informatie.  
- Toegang tot Power BI. Zie voor meer informatie [Power BI](https://powerbi.microsoft.com).

Op de Power BI-site vindt u meer informatie over het [toevoegen van het Dynamics NAV Content Pack aan Power BI](http://go.microsoft.com/fwlink/?LinkID=760850).  

Als u het Dynamics NAV Content Pack wilt openen in Power BI, moet u in het verbindingsvenster de volgende informatie opgeven:

| Veld       | Omschrijving              |
|-------------|--------------------------|
|**URL van OData-feed**|De OData-URL, zodat Power BI toegang kan krijgen tot gegevens van uw bedrijf, zoals https://mybusiness.com:7048/MS/OData/Company('CRONUS%20US').|
|**Verificatiemethode**|Kies **Basis**.|
|**Gebruikersnaam**|Het e-mailaccount dat u hebt gebruikt om u aan te melden voor Dynamics NAV, zoals *me@mybusiness.com*.|
|**Wachtwoord**|Dit is de webservicetoegangssleutel voor uw gebruikersaccount in Dynamics NAV.|

Dit betekent dat u twee verschillende gegevens van Dynamics NAV moet krijgen: de OData-URL en de webservicetoegangssleutel voor uw gebruikersaccount.  
**De URL ophalen**  
Als u Dynamics NAV toevoegt aan Power BI, moet u een URL opgeven zodat Power BI toegang kan krijgen tot gegevens uit uw bedrijf. In het verbindingsvenster wordt naar de URL verwezen als **URL van OData-feed** en het moet de volgende indeling hebben:

         https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')  
In dit voorbeeld is *mybusiness* de naam van uw Dynamics NAV-service en is *CRONUS US* de naam van het demobedrijf, waarbij *%20* staat voor de spatie in de naam.   
Als u de URL wilt krijgen, zoekt u in Dynamics NAV het venster **Webservices** en opent u dit. Dit venster bevat de webservices die momenteel beschikbaar zijn en kunt u de koppeling uit het veld **OData-URL** kopiëren voor een van de standaard OData-webservices.  
**De webservicetoegangssleutel ophalen**  
Als u gegevens uit Dynamics NAV in Power BI wilt gebruiken, moet u in het venster **Koppelen aan Dynamics NAV** uw gebruikersnaam, bestaande uit uw e-mailaccount, en uw wachtwoord opgeven. Het wachtwoord is de webservicetoegangssleutel die voor uw account is ingesteld in Dynamics NAV.  
Als u een webservicetoegangssleutel wilt ophalen, zoekt u in Dynamics NAV het venster **Gebruikers** en opent u de kaart voor uw gebruikersaccount. Kopieer op het sneltabblad **Toegang tot webservice** de inhoud van het veld **Toegangssleutel voor webservice**. Als het veld leeg is, kiest u op het lint **Toegangssleutel voor webservice wijzigen**, kiest u het veld **Sleutel verloopt nooit** en kiest u vervolgens de knop OK. U kunt vervolgens de sleutel kopiëren.  

## <a name="getting-data-from-dynamics-nav"></a>Gegevens ophalen uit Dynamics NAV
Het Dynamics NAV-dashboard bevat de meeste algemene rapporten die u zult willen gebruiken om uw bedrijf te traceren. De gegevens worden uit uw Dynamics NAV-bedrijf opgehaald door middel van webservices die live gegevens uitlezen. In Dynamics NAV bevat het venster **Webservices** de webservices die voor u zijn ingesteld, inclusief de volgende die worden gebruikt door het Content Pack in Power BI:  

- ItemSalesAndProfit  
- ItemSalesByCustomer  
- powerbifinance-setup  
- SalesDashboard  
- SalesOpportunities  
- SalesOrdersBySalesPerson  
- TopCustomerOverview  

**Opmerking**: als u de naam van een van deze webservices wijzigt, worden de gegevens niet weergegeven in Power BI.  
Als u andere gegevens wilt toevoegen aan Power BI, moet u de tabellen zoeken in Dynamics NAV, ze beschikbaar maken als webservices en ze vervolgens toevoegen aan het Content Pack. Dit is een geavanceerd scenario en het is raadzaam te beginnen met de gegevens die al in Power BI beschikbaar zijn.  

## <a name="troubleshooting"></a>Problemen oplossen
Het dashboard van Power BI gebruikt de gepubliceerde webservices die hierboven worden genoemd en bevat gegevens van het demobedrijf of uw eigen bedrijf als u gegevens importeert uit uw huidige financiële oplossing. Als er echter iets verkeerd gaat, biedt deze sectie een oplossing voor de meest voorkomende problemen.  

**"Parametervalidatie mislukt; zorg dat alle parameters geldig zijn"**  
Als u deze fout ziet deze nadat u de URL van uw Dynamics NAV hebt ingevoerd, controleert u of aan de volgende vereisten is voldaan:  

- De URL volgt exact dit patroon:

    https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')  
- Verwijder eventuele tekst na de bedrijfsnaam tussen haakjes  
- Zorg ervoor dat er geen voorwaartse eindslash aan het eind van de URL staat.  
- Controleer of het een veilige verbinding is zoals aangegeven door de URL die begint met *https*.  


**"Aanmelding mislukt"**  
Als u de fout "Aanmelding mislukt" krijgt wanneer u zich aanmeldt bij het dashboard met uw Dynamics NAV-referenties, kan dat een van de volgende oorzaken hebben:

* De account die u gebruikt, heeft geen machtigingen om de Dynamics NAV-gegevens uit uw account te lezen.

    Controleer uw gebruikersaccount in Dynamics NAV en let erop dat u de juiste webservicetoegangssleutel als wachtwoord gebruikt. Probeer het vervolgens opnieuw.  
* Het Dynamics NAV-exemplaar waarmee u verbinding probeert te maken, heeft geen geldig SSL-certificaat. In dit geval ziet u een gedetailleerde foutmelding ("kan geen vertrouwde SSL-relatie tot stand brengen").

    **Opmerking**: zelfondertekende certificaten worden niet ondersteund.  


**"Oops"**  
Als u een "Oops"-foutdialoogvenster ziet na het verificatiedialoogvenster, komt dat meestal door een probleem bij het maken van verbinding met de gegevens voor het Content Pack.

* Controleer of de URL het patroon volgt dat eerder is opgegeven:

    https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')  
* Een veel voorkomende vergissing is de volledige URL op te geven voor een specifieke webservice:

    https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')/powerbifinance-setup  
* Of het kan zijn dat u vergeten bent de bedrijfsnaam op te geven:

    https://mybusiness.projectmadeira.com:7048/MS/OData/  


## <a name="see-also"></a>Zie ook
[Welkom bij Dynamics NAV](across-get-started.md)  


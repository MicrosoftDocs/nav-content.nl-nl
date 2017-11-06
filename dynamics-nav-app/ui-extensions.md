---
title: Extensies installeren om Dynamics NAV aan te passen
description: Meer informatie over het toevoegen van functionaliteit en het aanpassen van Dynamics NAV door extensies te installeren.
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: app, add-in, manifest, customize
ms.date: 07/07/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 109eb8d0e2a38566739878ef513ffa3bec8dcd30
ms.contentlocale: nl-nl
ms.lasthandoff: 10/26/2017

---
# <a name="customizing-dynamics-nav-using-extensions"></a>Dynamics NAV aanpassen met behulp van extensies
U kunt [!INCLUDE[d365fin](includes/d365fin_md.md)] wijzigen door extensies te installeren die bijvoorbeeld functionaliteit toevoegen, gedrag wijzigen of u toegang verlenen tot nieuwe online services.
Wanneer u [!INCLUDE[d365fin](includes/d365fin_md.md)] voor het eerst start, zijn bepaalde extensies al voor u ge�nstalleerd. In de loop van de tijd zullen meer extensies beschikbaar voor u worden gemaakt en u kunt dan zelf bepalen of u de extensie wilt gebruiken of niet.

Zo verschaft Microsoft een extensie die integratie met PayPal Payments Standard biedt. Deze extensie is standaard ge�nstalleerd.
Maar als er een andere extensie beschikbaar komt die integratie met een andere betalingsservice biedt, kunt u de nieuwe extensie installeren en vervolgens bepalen welke van de services moeten worden gebruikt.  

U beheert de extensies in het venster **Extensiebeheer**. U kunt tot dit venster toegang krijgen via de startpagina. U kunt ook in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport** ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "Pictogram Zoeken naar pagina of rapport") kiezen. Voer vervolgens **Extensie** in en klik op de gerelateerde koppeling.  

> [!NOTE]  
>   Als u denkt u dat toegang tot een extensie zou moeten hebben maar de functionaliteit ervan niet vindt, kijk dan in het venster **Extensiebeheer**. Als de extensie daar niet wordt vermeld, kunt u de extensie installeren zoals beschreven in het volgende gedeelte.  

## <a name="installing-an-extension"></a>Een extensie installeren
U kunt nieuwe extensies vinden in de markt op [AppSource.microsoft.com](https://appsource.microsoft.com/en-us/marketplace/apps?product=dynamics-365%3Bdynamics-365-for-financials&page=1). Hier vindt u een overzicht van alle beschikbare extensies voor [!INCLUDE[d365fin](includes/d365fin_md.md)], en u kunt apps, extensies en inhoudspakketten krijgen voor andere producten van Microsoft. Stel de gewenste filters in, bekijk de gegevens voor elke extensie en haal een extensie voor uw [!INCLUDE[d365fin](includes/d365fin_md.md)] op.  
> [!NOTE]  
>   Meld u bij [AppSource.microsoft.com](https://appsource.microsoft.com/) aan met het e-mailaccount dat u gebruikt voor [!INCLUDE[d365fin](includes/d365fin_md.md)]. Gebruik voor het gemak dezelfde e-mailaccount voor andere producten en services.  

U kunt ook naar de marktplaats gaan vanuit [!INCLUDE[d365fin](includes/d365fin_md.md)]. In het venster **Extensiebeheer** kunt u de extensies bekijken die momenteel zijn ge�nstalleerd en kunt u de pagina **Extensiemarktplaats** openen waarop de extensies van [!INCLUDE[d365fin](includes/d365fin_md.md)] worden weergegeven die momenteel beschikbaar zijn in AppSource. Als u de koppeling *Meer apps* kiest, komt u terecht op [AppSource.microsoft.com](https://appsource.microsoft.com/en-us/marketplace/apps?product=dynamics-365%3Bdynamics-365-for-financials&page=1).  

Als u een extensie kiest, kunt u lezen over wat de extensie doet en kunt u Help opvragen voor de extensie voor meer informatie. Wanneer u een extensie wilt verkrijgen, moet u akkoord gaan met de gebruiksvoorwaarden. Als u de extensie van de AppSource-website ophaalt, wordt u aangemeld bij [!INCLUDE[d365fin](includes/d365fin_md.md)] om de installatie uit te voeren.  

Wanneer u een extensie installeert, moet u deze mogelijk instellen. Zo moet u wellicht een rekening opgeven met de **extensie PayPal Payments Standard voor [!INCLUDE[d365fin](includes/d365fin_md.md)]**.
Met andere extensies worden gewoonweg velden aan een bestaande pagina toegevoegd of wordt bijvoorbeeld een nieuwe pagina toegevoegd.   

Als u een extensie verwijdert en vervolgens van gedachten verandert, kunt u deze opnieuw installeren. Wanneer u een extensie verwijdert die u gebruikt, worden de gegevens bewaard zodat deze gegevens nog steeds beschikbaar zijn als u de extensie opnieuw installeert.  

Sommige extensies worden verstrekt door Microsoft en andere extensies worden verstrekt door [andere bedrijven](ui-extensions-other.md). Alle extensies worden getest voordat ze voor u beschikbaar worden gemaakt, maar het is raadzaam dat u toegang hebt tot de koppelingen die met elke extensie worden verschaft als u meer wilt weten over de extensie voordat u ervoor kiest deze te installeren.  

Microsoft biedt de volgende extensies:  

* [Dynamics GP Data Migration](ui-extensions-dynamicsgp-data-migration.md)  
* [PayPal Payments Standard](ui-extensions-paypal-payments-standard.md)  
* [QuickBooks-gegevensmigratie](ui-extensions-quickbooks-data-migration.md)  
* [Verkoop- en voorraadprognose](ui-extensions-sales-forecast.md)  
* [Ceridian Payroll](ui-extensions-ceridian-payroll.md)  
* [Quickbooks-salarisbestand importeren](ui-extensions-quickbooks-payroll.md)  
* [WorldPay Payments Standard](ui-extensions-worldpay-payments-standard.md)
* [GetAddress.io UK Postcodes](ui-extensions-getaddressio.md)
* [QuickBooks Online-gegevensmigratie](ui-extensions-quickbooks-online-data-migration.md)
* [Accountantportal](ui-extensions-accountant-portal.md)  
* [Afbeeldingsanalyse](ui-extensions-image-analyzer.md)

> [!NOTE]  
>  Nieuwe extensies zijn niet direct in AppSource beschikbaar nadat we een update aankondigen. U kunt de extensies in de gaten houden op [AppSource.microsoft.com](https://appsource.microsoft.com/en-us/marketplace/apps?product=dynamics-365%3Bdynamics-365-for-financials&page=1).

## <a name="see-also"></a>Zie ook
[Procedure: Klantbetalingen via PayPal inschakelen](sales-how-enable-payment-service-extensions.md)  
[Bedrijfsgegevens migreren uit andere financi�le systemen](upload-data.md)    
[[!INCLUDE[d365fin](includes/d365fin_md.md)] Extensies door andere providers](ui-extensions-other.md)  
[Welkom bij [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  

##



---
title: Servicestatistiek
description: Krijg een snel overzicht van de inhoud van servicedocumenten, zoals orders, offertes, facturen of creditnota's, van de details op de afzonderlijke serviceregels en van de serviceartikelen.
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/04/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 0fab2eab4cc664696c6f3c3c50286c581e76627b
ms.contentlocale: nl-nl
ms.lasthandoff: 10/23/2017

---

# <a name="viewing-service-statistics"></a>Servicestatistieken weergeven
Dynamics NAV kan bepaalde statistische gegevens bieden die u kunt gebruiken om servicedocumenten te analyseren en te bepalen hoe goed u uw serviceprocessen beheert. U kunt servicecontracten, artikelen, offertes, orders, facturen en creditnota's analyseren door de actie **Statistieken** te kiezen. Voor serviceartikelen en contracten kunt u ook **Serviceartikel Trendscape** of **Contract Trendscape** gebruiken om een overzicht van serviceposten voor een bepaald serviceartikel te bekijken.   

## <a name="viewing-statistics-for-service-orders"></a>Statistieken voor serviceorders weergeven
De functie serviceorderstatistiek biedt u een overzicht van de inhoud van de volledige serviceorder, de details op de serviceregels en gegevens met betrekking tot facturering, verzending en verbruik, evenals het saldo van de klant.  

De statistiekgegevens voor een serviceorder worden weergegeven in het venster **Serviceorderstatistiek** voor de desbetreffende order. U kunt het desbetreffende venster openen vanuit een serviceorder. Kies **Statistieken** in het venster **Serviceorders**. Op de sneltabbladen in dit venster worden gegevens als aantal, bedrag, btw, kosten, winst en de kredietlimiet van de klant weergegeven. De bedragen in het venster zijn gesteld in de valuta van de serviceorder, tenzij anders aangegeven.  

### <a name="view-totals-for-a-service-order"></a>Totalen voor een serviceorder weergeven  
U kunt het totaalbedrag op de serviceregels (inclusief en exclusief btw), het btw-gedeelte, de kosten en de winst op de serviceregels weergeven. Daarnaast wordt er artikelspecifieke informatie weergegeven, zoals het gewicht, het volume en het aantal colli.  

### <a name="view-shipping-information"></a>Verzendgegevens weergeven  
U kunt informatie weergeven over de te verzenden artikelen, resources of kosten. Voor deze informatie worden de waarden gebruikt die zijn opgegeven in het veld **Te verzenden aantal** van elke serviceregel in de order.  

### <a name="view-order-details"></a>Ordergegevens weergeven  
U kunt informatie weergeven over de artikelen, resource-uren en kosten die moeten worden gefactureerd en verbruikt. In de volgende tabel worden deze gegevens beschreven.  

|Kolom | Description|  
|------------|---------------------------------------|  
|**Facturering**|Bevat bedragen die moeten worden geboekt als gefactureerd vanuit de serviceorder.|  
|**Verbruik**|Bevat de hoeveelheid en de kosten van artikelen, of de resources die worden geboekt als verbruikt.|  
|**Totaal**|Hier worden de totaalbedragen voor de serviceorder weergegeven, die worden berekend door de factureringsbedragen op te tellen bij de verbruiksbedragen.|  

### <a name="analyze-service-order-lines"></a>Serviceorderregels analyseren  
U kunt de gegevens analyseren op basis van de soorten serviceregels die zijn opgenomen in de serviceorder. De bedragen worden afzonderlijk weergegeven voor:  

* Artikelen  
* Resources  
* Kosten en grootboekrekeningen  

### <a name="view-customer-information"></a>Klantgegevens weergeven  
Bekijk het saldo van de klantenrekening en het maximale krediet dat kan worden verleend aan de klant voor wie u het servicedocument hebt opgesteld.

## <a name="viewing-service-item-statistics"></a>Serviceartikelstatistieken weergeven
In het venster **Serviceartikelstatistiek** kunt u bijgewerkte gegevens over een serviceartikel bekijken op basis van de volgende serviceboekingssoorten:  

* Resources  
* Artikelen  
* Servicekosten  
* Servicecontracten  
* Totaal  

Voor elk boekingssoort kunt u het gefactureerde bedrag, het verbruik (bedrag), de kosten, het aantal, het gefactureerde en het verbruikte aantal, het winstbedrag en -percentage bekijken. Het winstpercentage wordt berekend volgens de volgende formule:  

* (Gefactureerd bedrag - Gebruik (Kosten)) x 100 / Gefactureerd bedrag  

## <a name="using-trendscapes"></a>Trendscapes gebruiken
Voor serviceartikelen en servicecontracten biedt het venster **Serviceartikel Trendscape** of **Contract Trendscape** een overzicht van serviceposten gedurende een periode voor een bepaald serviceartikel of contract. U kunt de trendscape weergeven door het serviceartikel of contract te openen, de actie **Statistieken** te kiezen en vervolgens **Trendscape** te kiezen.

Wanneer u de lijst doorloopt, worden de bedragen berekend op basis van het opgegeven tijdsinterval en weergegeven in de lokale valuta. De bedragen worden berekend op basis van serviceposten. Dit zijn de posten die worden gemaakt wanneer u serviceorders of servicefacturen boekt.

U kunt de lijst filteren door op te geven welke serviceartikelen moeten worden opgenomen.  

> [!Tip]  
>  Als u **Dag** hebt gekozen als tijdsinterval en een lange periode moet doorlopen, kunt u dat sneller doen door een groter interval te kiezen, bijvoorbeeld **Kwartaal**. Zodra u de gewenste periode hebt gevonden, kunt u teruggaan naar het originele interval om de gegevens gedetailleerder te bekijken.   

## <a name="viewing-gains-and-losses-on-contracts"></a>Winsten en verliezen op contracten weergeven  
Een vermelding van contractwinst of -verlies wordt gegenereerd wanneer een contractofferte wordt omgezet in een servicecontract, als contractregels worden toegevoegd of verwijderd uit een servicecontract of wanneer een contract wordt geannuleerd. U kunt contractwinsten of -verliezen bekijken op de volgende pagina's.  

|Pagina | Description|  
|----------------|---------------------------------------|  
|**Winst/verlies contract (Contract)**|Het winst-/verliescontract per servicecontract weergeven.|  
|**Winst/verlies contract (Groep)**|Het winst-/verliescontract per servicecontractgroep weergeven.|  
|**Winst/verlies contract (Klant)**|Het winst-/verliescontract per klant weergeven.|  
|**Winst/verlies contract (Reden)**|Het winst-/verliescontract per redencode weergeven.|  
|**Winst/verlies contract (Divisie)**|Het winst-/verliescontract per divisie weergeven.|  

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer de naam in van de pagina die moet worden weergegeven en kies vervolgens de gerelateerde koppeling.  
2. Vul de filtercriteria in die u wilt toepassen. Kies bijvoorbeeld in het venster **Winst/verlies contract (Reden)** een waarde voor **Redencodefilter**.  
3. Kies de actie **Matrix weergeven**.

## <a name="viewing-statistics-for-posted-service-documents"></a>Statistieken voor geboekte servicedocumenten weergeven
Met de functie voor servicestatistieken kunt u een statistisch overzicht opstellen van de inhoud van geboekte servicedocumenten, zoals geboekte verzendingen, facturen en creditnota's.  

De statistische informatie wordt weergegeven in het statistiekvenster voor het bijbehorende geboekte servicedocument. U kunt het desbetreffende statistiekvenster openen vanuit een geboekte serviceverzending, geboekte servicefactuur of geboekte servicecreditnota. Kies voor elk van deze documentsoorten op het tabblad **Starten** in de groep **Verwerken** de optie **Statistiek**. Kies bijvoorbeeld in het venster **Geboekte servicefacturen** op het tabblad **Start** in de groep **Verwerken**, de optie **Statistiek**.  

### <a name="posted-service-shipment-statistics"></a>Statistiek geboekte serviceverzendingen  
In het venster **Statistiek serviceverzendingen** wordt een overzicht gegeven van een geboekte serviceverzending. Het venster bevat informatie over de fysieke inhoud van de verzending, zoals het aantal verzonden artikelen, resource-uren of -kosten, en gewicht en volume van de verzonden artikelen.  

### <a name="posted-service-invoice-statistics"></a>Statistiek geboekte servicefacturen  
In het venster **Statistiek servicefacturen** wordt een statistisch overzicht gegeven van een geboekte servicefactuur. U kunt de totalen van de geboekte servicefactuur bekijken. U vindt hier onder andere het totaalbedrag op de serviceregels (inclusief en exclusief btw) dat als gefactureerd is geboekt, het btw-gedeelte, de kosten en de winst op de geboekte factuur. Daarnaast bevat het venster informatie over het volgende:  

* De artikelen op de servicefactuurregels, zoals gewicht, volume en het aantal colli.  
* Het saldo op de rekening van de klant en het maximumkrediet dat u de klant kunt verlenen.  

### <a name="posted-service-credit-memo-statistics"></a>Statistiek Geboekte servicecreditnota  
Het venster **Statistiek servicecreditnota's** biedt een statistisch overzicht van de regels in een geboekte servicecreditnota. Het overzicht kan het volgende bevatten:

* De totale bedragen op de geboekte creditnota, weergegeven als het aantal, het bedrag, de btw, de kosten en de winst. Daarnaast vindt u hier informatie over de artikelen op de serviceregels van de geboekte creditnota, zoals aantal, gewicht en volume.  
* Algemene informatie over de klant, zoals de kredietlimiet van de klant en het rekeningsaldo.  

## <a name="see-also"></a>Zie ook  
[Procedure: Serviceorders maken](service-how-to-create-service-orders.md)   
[Procedure: Serviceartikelen maken](service-how-to-create-service-items.md)   
[Service plannen](service-plan-service.md)  


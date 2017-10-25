---
title: Facturen of creditnota's voor services maken
description: Leer hoe u facturen maakt zodat u kunt worden betaald voor uw service.
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/22/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 8c575cca9e898b31e29cdb86079e56097679b48d
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-service-invoices-or-credit-memos"></a>Procedure: servicefacturen of creditnota's maken
Gemakkelijke facturering van uw serviceorders is een van de belangrijkste kenmerken van [!INCLUDE[d365fin](includes/d365fin_md.md)]. U kunt op elk gewenst moment een factuur naar uw klanten verzenden of u kunt periodiek facturen opstellen.  
  
Als u direct een factuur wilt maken, gebruikt u het venster **Servicecontract**. U kunt uw systeem ook zodanig instellen dat een servicetechnicus op locatie een factuur kan maken voor services die niet aan een contract of order zijn verbonden.  

## <a name="to-invoice-a-service-contract-from-the-service-contract-page"></a>Een servicecontract factureren via de pagina Servicecontract   
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Servicecontractfacturen maken** in en klik vervolgens op de gerelateerde koppeling.  
2. Stel de filters in die u wilt toepassen.  
3. Voer in het veld **Boekingsdatum** de boekingsdatum in voor de gemaakte servicefacturen.  
4. Geef in het veld **Factureren tot datum** aan tot welke datum u contracten wilt factureren. In de batchverwerking worden de contracten met de volgende factuurdatums tot deze datum opgenomen.  
5. Kies in het veld **Actie** de optie **Facturen maken**.  
6. Kies **OK** om de servicefacturen te maken.  
  
  > [!NOTE]  
  >  U kunt geen servicefacturen maken voor het servicecontract als de waarde van het veld **Wijzigingsstatus** is ingesteld op **Open**.  
  
## <a name="to-post-an-invoice-from-a-service-order"></a>Een factuur boeken vanuit een serviceorder  
In de volgende procedure wordt beschreven hoe u het servicedeel opgeeft dat u aan de klant in rekening brengt.  

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Serviceorders** in en klik op de gerelateerde koppeling.  
2. Kies de serviceorder waarvoor u wilt factureren en open de orderkaart.  
3. Kies de actie **Serviceregels**.  
4. Zoek de gewenste posten en geef in het veld **Te factureren aantal** het aantal op dat u in rekening gaat brengen aan de klant.  
  
   > [!NOTE]  
   >  U kunt de klant voor de geregistreerde service factureren geheel of in delen. Als u ervoor kiest de klant volledig te factureren, moet de waarde in het veld **Te factureren aantal** gelijk zijn aan de waarde in het veld **Aantal**. U kunt een volledige factuur samen met een totaalverzending boeken en u kunt een volledige factuur boeken voor een reeds geboekte maar nog niet gefactureerde of verbruikte totaalverzending.  
   >   
   >  Wanneer u een gedeeltelijke factuur boekt, zijn er twee manieren om het te factureren aantal op te geven. Als u de service gaat boeken met de optie **Verzenden en factureren** moet de waarde in het veld **Te factureren aantal** gelijk zijn aan die in het veld **Te verzenden aantal** veld. Als u een al geboekte verzending wilt factureren, mag het te factureren aantal niet groter zijn dan de waarde in het veld **Verzonden aantal**.  
  
5. Kies **Boeken** en klik vervolgens op **Factuur** of **Verzenden en factureren**. Zie [Boeken in CRM - Service](service-service-posting.md) voor meer informatie.  
  
 De serviceregel die u hebt geselecteerd wordt geboekt. U kunt meerdere regels tegelijk selecteren door ze allemaal te selecteren en **Boeken** te kiezen Als u dit doet, zorg er dan voor dat u alle benodigde gegevens hebt ingevuld op de regels die u wilt boeken.  
  
 Wanneer u de order boekt met de optie **Factureren** wordt een geboekte servicefactuur gemaakt samen met de overeenkomende posten en updates van de relevante velden op de serviceregels van de order. Bovendien worden de eerder geboekte verzendingsdocumenten bijgewerkt met de gefactureerde aantallen. Als u de optie **Verzenden en factureren** selecteert, wordt een geboekte verzending gemaakt.

## <a name="to-create-a-service-invoice-manually"></a>Een servicefactuur handmatig maken  
Normaal gesproken, wanneer u een serviceorder boekt met de optie **Factureren** of **Verzenden en factureren**, wordt automatisch een servicefactuur geboekt. Toch kan het nodig zijn dat u een factuur moet verzenden die niet is gekoppeld aan een servicecontract of aan een serviceorder. In deze procedure wordt uitgelegd hoe u een factuur verzendt op hetzelfde moment dat de klant de service ontvangt.  

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Servicefacturen** in en klik vervolgens op de gerelateerde koppeling.  
2. Maak een nieuwe servicefactuur.  
3. Vul het veld **Nr.** te kiezen.  
  
    > [!NOTE]  
    >  Als u nummerreeksen voor servicefacturen in het venster **CRM - Service-instellingen** hebt ingesteld, kunt u op Enter drukken om het eerstvolgende beschikbare servicefactuurnummer in te voeren.  
  
4. Voer in het veld **Klantnr.** het nummer van een klant in. Selecteer de betreffende klant uit de lijst.  
  
    De klantvelden worden automatisch ingevuld met gegevens uit de **Klantenkaart**.  
  
5. Geef een datum op in het veld **Boekingsdatum**. Deze datum wordt in de geboekte posten weergegeven. De huidige werkdatum wordt automatisch in dit veld ingevuld, maar u kunt deze ook wijzigen.  
6. Vul het veld **Documentdatum** in. De datum die u hier opgeeft, wordt op de afgedrukte factuur weergegeven en wordt gebruikt om de vervaldatum te bereken.  
7. Vul de serviceregels van de factuur in. Vul de velden **Soort**, **Nr.** en **Aantal** in om artikelen, resources en kosten te registreren die zijn gebruikt voor de serviceverlening. 

## <a name="to-invoice-posted-shipment-lines"></a>Geboekte verzendregels factureren  
Het kan voorkomen dat u een servicefactuur moet opstellen voor een service die al is geleverd, vanuit één of verschillende serviceorders, maar die nog niet is gefactureerd of verbruikt. U kunt de geselecteerde geboekte verzendregels voor een bepaalde klant automatisch laten invullen op de factuurregels.  

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Servicefacturen** in en klik vervolgens op de gerelateerde koppeling.  
2. Vul de velden indien nodig op de regel in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)] 
3. Maak factuurregels voor services die zijn verzonden maar die nog niet gefactureerd. U kunt ook de actie **Verzendregels ophalen** gebruiken om geboekte verzendregels aan de factuur toe te voegen.  
4. Boek de servicefactuur.  
  
 De geboekte servicefactuur en de bijbehorende posten worden gemaakt. De eerder geboekte verzendingsdocumenten worden bijgewerkt met de gefactureerde aantallen, en de betreffende aantallen worden bijgewerkt op de serviceregels van de bronorders.  

## <a name="to-create-a-combined-invoice"></a>Gecombineerde facturen maken  
U kunt de klant factureren voor services die op basis van verschillende serviceorders zijn geleverd. Er worden factuurregels gemaakt voor artikelen, resource-uren of -kosten die al zijn verzonden vanuit verschillende serviceorders maar die nog niet zijn gefactureerd.  

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Servicefacturen** in en klik vervolgens op de gerelateerde koppeling.  
2. Vul de velden indien nodig op de regel in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
3. Kies de actie **Verzendregels ophalen**. Op de pagina **Serviceverzendingsregels ophalen** worden alle regels weergegeven die wel verzonden, maar nog niet gefactureerd zijn.  
4. Kies de regels voor de te factureren service en kies vervolgens **OK** om de serviceverzendingsregels aan de factuur toe te voegen.  

## <a name="to-create-a-service-credit-memo"></a>Een servicecreditnota maken  
Servicecreditnotadocumenten worden meestal gebruikt wanneer klanten artikelen terugsturen, maar ze kunnen ook worden gebruikt om klanten te compenseren of om foutieve facturen te corrigeren.  

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Servicecreditnota's** in en klik vervolgens op de gerelateerde koppeling.  
2. Vul de velden indien nodig op de regel in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. In de velden **Boekingsdatum** en **Documentdatum** wordt de werkdatum weergegeven. Indien nodig kunt u deze wijzigen.    
4. Voer op de creditnotaregels gegevens in over de artikelen die zijn teruggestuurd of verwijderd of over de vergoeding die aan de klant zal worden gegeven.  

## <a name="see-also"></a>Zie ook
[Procedure: Servicefacturen boeken](service-how-to-post-service-orders.md)  
[CRM - Service instellen](service-setup-service.md)  
[Serviceboekingen](service-service-posting.md)  


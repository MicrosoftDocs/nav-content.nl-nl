---
title: Elektronische btw- en ICP-aangiften instellen
description: Als u uw Digipoort-communicatie wilt laten werken, moet u mogelijk uw netwerkinstellingen aanpassen. Digipoort gebruikt een veilig communicatieprotocol en vereist gebruik van TCP-poort 443.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 8eff49180f8019ca2c0cfafd48bb605bde446fce
ms.contentlocale: nl-nl
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-set-up-electronic-vat-and-icp-declarations"></a>Procedure: Elektronische btw- en ICP-aangiften instellen
Als u uw Digipoort-communicatie wilt laten werken, moet u mogelijk uw netwerkinstellingen aanpassen. Digipoort gebruikt een veilig communicatieprotocol en vereist gebruik van TCP-poort 443. Voordat u met de volgende procedure begint, stelt u uw netwerk in om deze poort te gebruiken.  

Als u elektronische btw- en ICP-aangiften wilt kunnen maken en met de belastingdienst wilt kunnen communiceren, moet u eerst algemene gegevens over elektronische belastingaangiften instellen. Uw bedrijf moet met de belastingdienst geregistreerd zijn voordat u elektronische aangiften kunt verzenden.  

## <a name="to-set-up-electronic-tax-declarations"></a>Elektronische belastingaangiften instellen  

1.  Kies het pictogram ![Pictogram Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "Pictogram Zoeken naar pagina of rapport"), voer **Elek. aangifte-instellingen** in en kies vervolgens de gerelateerde koppeling.  
2.  Selecteer in het venster **Elek. aangifte-instellingen** op het sneltabblad **Algemeen** de optie **BTW-contactpersoonsoort**.

    De opties zijn **Belastingplichtige** en **Expediteur**. Als de contactsoort **Belastingplichtige** is, wordt de contact-id van de elektronische aangifte ingevuld met het btw-nummer van het bedrijf.  

3.  Selecteer het **ICP-contactpersoonsoort**. De opties zijn **Belastingplichtige** en **Expediteur**.  
4.  Als u elektronische ICP-aangiften voor een dochteronderneming van een fiscale eenheid wilt verzenden, schakelt u het veld **Deel van Fiscale eenheid** in.  
5.  Voer op het sneltabblad **Nummering** de nummerreeks voor het veld **Btw-aangiftenrs.** in.  
6.  Voer op het sneltabblad **Digipoort** de benodigde gegevens in voor de Digipoort-verzendingen.  

    1.  Voer in het veld **Naam certificaat Digipoort-client** de algemene (CN) naam in van het certificaat u voor gebruik met Digipoort hebt aangevraagd. U vindt deze gegevens in de certificaateigenschappen van het persoonlijke certificaat dat u in de map **Persoonlijk** hebt geïnstalleerd. Zie voor meer informatie [Procedure: Certificaten instellen voor gebruik met Digipoort](how-to-set-up-certificates-for-use-with-digipoort.md).  
    2.  Voer in het veld **Naam certificaat Digipoort-service** de algemene naam in van het servicecertificaat, die gelijk kan zijn aan de naam van de server waarmee u communiceert voor de Nederlandse overheid. U vindt deze gegevens in de certificaateigenschappen van het openbare certificaat dat in de map **Vertrouwde uitgevers** is geïnstalleerd. Zie voor meer informatie [Procedure: Certificaten instellen voor gebruik met Digipoort](how-to-set-up-certificates-for-use-with-digipoort.md).  
    3.  Geef in het veld **Directe leverings-URL** de URL op voor de productieversie van de Digipoort Aanlever-service. Zie voor meer informatie [http://www.logius.nl/producten/gegevensuitwisseling/digipoort](http://www.logius.nl/producten/gegevensuitwisseling/digipoort).  
    4.  Geef in het veld **Digipoort status-URL** de URL op voor de statusinformatie die komt van de Digipoort Statusinformatie-service.  

    Zie voor meer informatie [Overzicht van Digipoort](digipoort-overview.md).  

Momenteel zijn er twee sets URL's die door de Nederlandse belastingdienst worden verstrekt. Deze zijn echter voor wijzigingen vatbaar en u moet de website van de dienst regelmatig controleren op updates.  

**Productiegebruik**  

- URL van Digipoort-aanlevering: https://www.procesinfrastructuur.nl/wus/2.0/aanleverservice/1.2  
- Status van Digipoort-aanlevering: https://www.procesinfrastructuur.nl/wus/2.0/statusinformatieservice/1.2  

**Gebruik testen**  

- URL van Digipoort-aanlevering: https://preprod.procesinfrastructuur.nl/wus/2.0/aanleverservice/1.2  
- URL van Digipoort-status: https://preprod.procesinfrastructuur.nl/wus/2.0/statusinformatieservice/1.2  

## <a name="see-also"></a>Zie ook  
 [Procedure: Elektronische btw- en ICP-aangiften verzenden](how-to-submit-electronic-vat-and-icp-declarations.md)   
 [Procedure: Responsberichten van de belastingdienst verwerken](how-to-process-response-messages-from-tax-authorities.md)


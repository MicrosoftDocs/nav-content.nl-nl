---
title: Elektronische documenten verzenden
description: Leer hoe u facturen elektronisch verzendt.
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 5920ed97f054b3e7882f40f2fceec76183800297
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-send-electronic-documents"></a>Procedure: Elektronische documenten verzenden
De algemene versie van [!INCLUDE[d365fin](includes/d365fin_md.md)] ondersteunt het verzenden van elektronische facturen en creditnota's in de PEPPOL-indeling, die wordt ondersteund door de grootste aanbieders van documentuitwisselingsservices. Een aanbieder van documentuitwisselingsservices verzendt elektronische documenten tussen handelspartners. Om ondersteuning te bieden voor elektronische documentindelingen, gebruikt u het kader voor gegevensuitwisseling.  

 In de algemene versie van [!INCLUDE[d365fin](includes/d365fin_md.md)] is een service voor documentuitwisseling vooraf geconfigureerd zodat u deze kunt instellen voor uw bedrijf. Zie [Procedure: Een service voor documentuitwisseling instellen](across-how-to-set-up-a-document-exchange-service.md) voor meer informatie.  

 Als u een verkoopfactuur als elektronisch PEPPOL-document wilt versturen, selecteert u de optie **Elektronisch document** in het dialoogvenster **Boeken en verzenden**. Hierin kunt u dit ook instellen als standaardprofiel voor documentverzending van de klant. Eerst moet u diverse stamgegevens instellen, zoals bedrijfsgegevens, klanten, artikelen en eenheden. Deze worden gebruikt om de zakelijke partners en artikelen te identificeren wanneer gegevens worden geconverteerd in velden in [Procedure: Verzending en ontvangst van elektronische documenten instellen](across-how-to-set-up-electronic-document-sending-and-receiving.md).  

### <a name="to-send-an-electronic-sales-invoice"></a>Een elektronische verkoopfactuur verzenden  

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Verkoopfacturen** in en klik vervolgens op de gerelateerde koppeling.  

2.  Maak een nieuwe verkoopfactuur.  

3.  Als de verkoopfactuur gereed is voor facturering, kiest u op het tabblad **Acties** in de groep **Boeken** de optie **Boeken en verzenden**.  

     Als het standaardverzendprofiel van de klant **Elektronisch document** is, wordt dit aangegeven in het dialoogvenster **Boeken en bevestiging verzenden** en hoeft u alleen maar de knop **Ja** te kiezen om de factuur te boeken en elektronisch te verzenden in de geselecteerde indeling.  

4.  In het dialoogvenster **Boeken en bevestiging verzenden** kiest u de Knop AssistEdit rechts van het veld **Document verzenden naar**.  

5.  Kies in het dialoogvenster **Document verzenden naar** in het veld **Elektronisch document** de optie **Via service voor documentuitwisseling**.  

6.  Kies in het veld **Indeling** de optie **PEPPOL**.  

7.  Kies de knop **Ok**. Het dialoogvenster **Boeken en bevestiging verzenden** verschijnt. **Elektronisch document (PEPPOL)** is toegevoegd aan het veld **Document verzenden naar**.  

8.  Kies de knop **Ja**.  

     De verkoopfactuur wordt geboekt en aan de klant gezonden als elektronisch document in de indeling PEPPOL.  

    > [!NOTE]  
    >  U kunt ook een geboekte verkoopfactuur als een elektronisch document verzenden. De procedure is hetzelfde als beschreven in dit onderwerp voor niet-geboekte verkoopdocumenten. Kies in het venster **Geboekte verkoopfactuur**, op het tabblad **Acties**, in de groep **Algemeen** de optie **Activiteitenlogbestand** om de status van het elektronische document te bekijken. Zie voor meer informatie **Activiteitenlogbestand**.  

## <a name="see-also"></a>Zie ook  
[Procedure: Verkopen factureren](sales-how-invoice-sales.md)  
[Procedure: Verzendprofielen voor documenten instellen](sales-how-setup-document-send-profiles.md)  
[Procedure: Verzending en ontvangst van elektronische documenten instellen](across-how-to-set-up-electronic-document-sending-and-receiving.md)  
[Procedure: Een service voor documentuitwisseling instellen](across-how-to-set-up-a-document-exchange-service.md)  
[Procedure: Definities voor gegevensuitwisseling instellen](across-how-to-set-up-data-exchange-definitions.md)  
[Gegevens elektronisch uitwisselen](across-data-exchange.md)  
[Algemene bedrijfsfunctionaliteit](ui-across-business-areas.md)  


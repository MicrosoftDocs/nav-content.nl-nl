---
title: Service- en werkuren instellen
description: U kunt de gebruikelijke servicewerkuren in het bedrijf opgeven. Deze service-uren worden gebruikt om de responsdatum en -tijd voor serviceorders en -offertes te berekenen, en om responstijdwaarschuwingen te verzenden.
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
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7b4d813f734fbaa53bc185e2477ca73705872097
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-work-hours-and-service-hours"></a>Procedure: Service- en werkuren instellen
Met een servicebeheersysteem worden de resource-uren en serviceorderstatus bijgehouden ten behoeve van het voorspellen van de werkbelasting en servicebehoeften. [!INCLUDE[d365fin](includes/d365fin_md.md)] heeft ingebouwde tools die u kunt aanpassen om dit soort informatie vast te leggen.  
  
Nadat u de standaardservice-uren van uw bedrijf hebt ingesteld, kunt u responstijden voor serviceorders berekenen of waarschuwingen verzenden wanneer serviceoproepen worden ontvangen. De waarschuwingsfunctie wordt in combinatie met de projectplanner geïmplementeerd.   
  
Terwijl u aan serviceorder werkt, is het handig om de status te kunnen bijwerken zodat u de voortgang kunt bijhouden. Met de serviceorderstatus wordt de herstelstatus van de serviceartikelen in de serviceorder aangegeven. Zie voor meer informatie [Serviceorderstatus en herstelstatus begrijpen](service-order-repair-status.md). 

## <a name="to-set-up-default-service-hours"></a>Standaardservice-uren instellen  
In het venster **Std. service-uren** kunt u de gebruikelijke servicewerkuren in het bedrijf instellen. Deze service-uren worden gebruikt om de responsdatum en -tijd voor serviceorders en -offertes te berekenen en om responstijdwaarschuwingen te verzenden. De standaardservice-uren voor servicecontracten worden gebruikt tenzij u speciale service-uren voor een contract opgeeft.  
  
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "Zoeken naar pagina of rapport")-pictogram, voer **Std. service-uren** in en klik vervolgens op de gerelateerde koppeling.  
2. Vul de velden in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
  
> [!IMPORTANT]  
>  Als u de regels in het venster **Std. service-uren** niet invult, wordt als standaardwaarde 24 uur gebruikt, die alleen geldig is voor agendawerkdagen.  
  
## <a name="to-set-up-work-hour-templates"></a>Werkuursjablonen instellen
In het venster **Werkuursjabloon** kunt u sjablonen instellen met de standaardwerkuren in het bedrijf. U kunt bijvoorbeeld sjablonen maken voor technici met een volledige baan en voor technici met een deeltijdbaan. U kunt werkuursjablonen gebruiken wanneer u capaciteit toevoegt aan resources.  
  
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Werkuursjablonen** in en klik vervolgens op de gerelateerde koppeling.  
2. Vul de velden in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
  
> [!Note]
> Als u werkuren voor elke dag invoert, wordt de waarde in het veld **Totaal per week** automatisch berekend.  

## <a name="to-set-up-contract-specific-service-hours"></a>Contractspecifieke service-uren instellen  
In het venster **Service-uren** kunt u specifieke service-uren instellen voor de klant die eigenaar is van het servicecontract. Met de service-uren worden de responsdatum en -tijd berekend voor serviceorders en -offertes die bij het servicecontract horen.  
  
Als u geen specifieke service-uren voor het servicecontract instelt, worden de standaardservice-uren voor servicecontracten gebruikt.  
  
1. Kies het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Servicecontracten** in en kies vervolgens de gerelateerde koppeling.  
2. Open het servicecontract waarvoor u specifieke service-uren wilt instellen en kies **Service-uren**.  
4. Als u service-uren op basis van standaardservice-uren wilt instellen, kiest u de actie **Std. service-uren kopiëren**.  
5. De velden in de posten voor service-uren bewerken. Invoegen of verwijderen van vermeldingen voor het instellen van de service-uren voor het contract. Merk op dat de velden **Dag**, **Begintijd** en **Eindtijd** zijn vereist voor elke regel.  
6. Als u de service-uren wilt laten gelden vanaf een specifieke datum, vult u het veld **Begindatum** in.  
7. Als u de service-uren wilt laten gelden op vakantiedagen, schakelt u het selectievakje **Geldig op vakantiedagen** in.  

## <a name="see-also"></a>Zie ook  
[Toewijzingsstatus en herstelstatus begrijpen](service-allocation-status-and-repair-status.md)  
[CRM - Service instellen](service-setup-service.md)  
[Serviceorderstatus en herstelstatus begrijpen](service-order-repair-status.md)  


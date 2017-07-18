---
title: 'Procedure: Voorspellende cashflowprognoses maken'
author: bholtorf
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: f657509fc2195674db81f47bc5ae31b7ba1aa40e
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-make-predictive-cash-flow-forecasts"></a>Procedure: Voorspellende cashflowprognoses maken
Cashflowprognoses helpen u te zorgen dat uw bedrijf over voldoende contant geld beschikt om aan de financiële verplichtingen te voldoen en ze zijn nuttig voor het bepalen van correcties. Als u bijvoorbeeld een kasoverschot hebt, kunt u mogelijk enkele schulden afbetalen, en als u krap zit, waardeert u waarschijnlijk een tijdige waarschuwing. 

Cortana Intelligence gebruikt de Azure Machine Learning-service om betrouwbare, voorspellende prognoses te maken. Prognoses van Cortana Intelligence kunnen u bijvoorbeeld helpen cashtekorten te voorspellen en voorkomen. De service combineert historische gegevens met huidige boekingen voor schulden en tegoeden, inclusief boekingen met vervaldatums in de toekomst. Hieronder vallen:
* Inkooporders
* Verkooporders
* Geboekte verkoop- en inkoopfacturen
* Creditnota's.

## <a name="before-you-start"></a>Voordat u begint  
Er staat een aantal zaken te doen voordat u Cortana Intelligence voor cashflowprognoses kunt gebruiken: 
* Als u nog geen cashflowprognoses gebruikt, moet u het volgende instellen:
    * Een of meer instellingen in **Cashflowinstellingen**. 
    * Rekeningen voor tegoeden, schulden, verkooporders en inkooporders. Cortana Intelligence gebruikt de boekingen in deze rekeningen.
    * Een of meer cashflowprognoses in **Cashflowprognose**. Neem inkooporders, verkooporders, schulden en tegoeden als bronnen op.  
    Zoek voor meer informatie naar _cashflowprognoses_ in het Helpsysteem. 
* Zorg dat u de API-URL en de API-sleutel weet voor de te gebruiken voorspellende webservice.  
    U kunt Azure Machine Learning gebruiken of een andere service als u die hebt. Er is als alternatief een model genaamd _Prognosemodel voor Microsoft Dynamics NAV_ online beschikbaar in de Cortana Intelligence Gallery. Ga als volgt te werk om het model te gebruiken:

    1. Ga in een browser naar [Cortana Intelligence Gallery](https://go.microsoft.com/fwlink/?linkid=828352)
    2. Zoek naar _Prognosemodel voor Microsoft Dynamics NAV_ en open het model in Azure Machine Learning Studio.
    3. Gebruik het Microsoft-account om u aan te melden voor een werkruimte en kopieer vervolgens het model.
    4. Voer het model uit en publiceer het als een webservice.
    5. Noteer de API-URL en de API-sleutel. U gebruikt deze referenties wanneer u Cortana Intelligence instelt in Microsoft Dynamics NAV.  

* Bekijk hoe vaak u de prognose berekent. De Azure Machine Learning-service heeft beperkingen betreffende gebruik. Als u bijvoorbeeld veel artikelen hebt, kan het beter zijn minder vaak te berekenen. 
* Word toegewezen aan het rolcentrum Account. 

## <a name="set-up-cortana-intelligence"></a>Cortana Intelligence instellen
U kunt een begeleide instelling gebruiken om cashflowprognoses in te stellen. De gids helpt u zaken op te geven zoals hoe vaak u de prognose bijwerkt, op welke accounts deze wordt gebaseerd, wanneer u belasting betaalt en of Cortana Intelligence moet worden gebruikt.  

Als u al cashflowprognoses gebruikt en alleen Cortana Intelligence wilt inschakelen, kunt u ook een handmatig proces gebruiken. Als u zich aanmeldt, verschijnt een bericht in een blauwe balk boven in de werkruimte. Als u Cortana Intelligence direct wilt instellen, kiest u **Ja, graag**. Het bericht wordt slechts eenmaal weergegeven. Als u het afsluit, gebruikt u het handmatige proces om Cortana Intelligence in te stellen.  

**Tip:** Overweeg u de lengte van de perioden die de service in de berekeningen gebruikt. Hoe meer gegevens u biedt, hoe nauwkeuriger de voorspellingen zullen zijn. Let ook op grote variaties in perioden. Deze zijn ook van invloed op voorspellingen. Als Cortana Intelligence niet voldoende gegevens vindt of de gegevens sterk variëren, doet de service geen voorspelling. 

De begeleide instelling gebruiken:
1. Kies in het rolcentrum Accountant onder het diagram **Cashflowprognose** de actie **Begeleide instelling openen**.
2. Vul de velden in elke stap van de gids in.

Een handmatig proces gebruiken:
1. Zoek **Cashflowinstelling** en kies vervolgens de verwante koppeling.
2. Vouw het sneltabblad **Cortana Intelligence** uit en vul de velden in.

## <a name="turn-on-cortana-intelligence-for-cash-flow-forecasts"></a>Cortana Intelligence inschakelen voor cashflowprognoses
1. Zoek **Cashflowinstellingen** en kies vervolgens de verwante koppeling.
2. Kies de actie **Cashflowvoorstel**.
3. Kies op de pagina **Cashflowvoorstel** de actie **Voorstelregels voorstellen**.  
4. Kies onder **Op te nemen bronsoorten** het selectievakje **Cortana Intelligence-prognose**.

## <a name="investigate-a-cash-flow-forecast"></a>Een cashflowprognose onderzoeken
Als u de gegevens achter de prognose goed wilt zien, inclusief het verschil, kiest u de kolom **Cortana Intelligence**. De eerste rij in de tabel bevat het verschil. De overige rijen worden gerangschikt op brondocument.  

U kunt bijvoorbeeld zien hoe de prognose:    
* Bevestigde verkopen en inkopen verwerkt 
* Schulden aftrekt en tegoeden optelt
* Dubbele verkooporders en inkooporders overslaat

## <a name="see-also"></a>Zie ook  
[Werken met Dynamics NAV](ui-work-product.md)


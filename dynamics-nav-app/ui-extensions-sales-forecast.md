---
title: Verkoop- en voorraadprognose
author: edupont04
ms.custom: na
ms.date: 09/23/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 765527ed4f4800acec20f0abbd4374e95c9c36dc
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="sales-and-inventory-forecast-for-dynamics-nav"></a>Verkoop- en voorraadprognose voor Dynamics NAV
Voorraadbeheer is een wisselwerking tussen klantenservice en het beheren van uw kosten. Enerzijds is voor weinig voorraad minder werkkapitaal nodig, maar anderzijds leiden nulvoorraden mogelijk tot gemiste verkopen. De extensie Verkoop- en voorraadprognose voorspelt potentiële verkopen aan de hand van historische gegevens en biedt een helder overzicht van verwachte nulvoorraden. Op basis van de prognose helpt de extensie aanvullingsaanvragen aan leveranciers te maken en bespaart u tijd.  

## <a name="setting-up-forecasting"></a>Prognose instellen
In Dynamics NAV moet u de verbinding met Azure Machine Learning (Azure ML) instellen. Voor meer informatie raadpleegt u [Procedure: Dynamics NAV registreren in de Azure Management Portal](ui-how-register-dynamics-nav-azure.md). Nadat u de verbinding tot stand hebt gebracht, kunt u de prognose configureren voor gebruik van een ander soort rapportageperiode. Zo kunt u overschakelen van prognose per maand naar prognose per kwartaal. U kunt ook het aantal perioden kiezen op basis waarvan de prognose moet worden berekend, afhankelijk van hoe specifiek u de prognose wilt. We stellen voor dat u een prognose maakt per maand en met een horizon van 12 maanden voor de prognose.  

## <a name="using-the-forecasts"></a>De prognoses gebruiken
De extensie gebruikt de mogelijkheden van Azure Machine Learning (Azure ML) om toekomstige verkoop op basis van uw verkoophistorie te voorspellen om u te helpen voorraadtekort te voorkomen. Wanneer u bijvoorbeeld een artikel in het venster **Artikelen** kiest, wordt in het diagram in het deelvenster **Artikelprognose** de geschatte verkoop van dit artikel in de komende periode getoond. Op deze manier kunt u zien of uw voorraad van het artikel waarschijnlijk binnenkort op raakt.  

U kunt de extensie ook gebruiken om voorstellen te doen met betrekking tot bevoorrading. Als u bijvoorbeeld een inkooporder maakt voor Fabrikam omdat u de nieuwe bureaustoel wilt kopen, doet de extensie Verkoop- en voorraadprognose het voorstel om ook de LONDON-draaistoel te herbevoorraden die u gewoonlijk van deze leverancier koopt. Dit komt omdat de extensie voorspelt dat uw voorraad van de LONDON-draaistoel in de komende twee maanden op raakt. U kunt dus eventueel nu al meer stoelen bestellen.  

## <a name="see-also"></a>Zie ook
[Verkoop beheren](sales-manage-sales.md)  
[Voorraad beheren](inventory-manage-inventory.md)  
[Dynamics NAV aanpassen met extensies](ui-extensions.md)  
[Procedure: Dynamics NAV registreren in de Azure Management Portal](ui-how-register-dynamics-nav-azure.md)  


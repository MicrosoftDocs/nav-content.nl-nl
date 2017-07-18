---
title: Inkopen boeken
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: c03d031e951bc185b18bedaf428d414c1fe2e7d1
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="posting-purchases"></a>Inkopen boeken
In de **Boekingsgroep** op een inkoopdocument kunt u kiezen uit de volgende boekingsfuncties:

- **Boeken**
- **Voorbeeld van boeking weergeven**
- **Boeken en afdrukken**
- **Testrapport**
- **Batchboeken**

Wanneer u alle regels hebt ingevuld en alle informatie hebt ingevoerd op de inkooporder, kunt u de order boeken. Dit houdt in dat u een ontvangst en een factuur maakt.

Wanneer een inkooporder wordt geboekt, worden de rekening van de leverancier, het grootboek en de artikelposten bijgewerkt.

Voor elke inkooporder wordt een inkooppost gemaakt in de tabel **Grootboekpost**. Ook wordt een post in de leveranciersrekening in de tabel **Leverancierspost** gemaakt en wordt er een grootboekpost in de betreffende schuldenrekening gemaakt. Bovendien kan het boeken van de order resulteren in een btw-post en een grootboekpost voor de totale korting. Of er een post voor de korting wordt geboekt, wordt bepaald door de inhoud van het veld **Korting boeken** in het venster **Inkoopinstellingen**.

Voor elke inkooporderregel wordt een artikelpost gemaakt in de tabel **Artikelpost** (als op de inkoopregels artikelnummers staan) of een grootboekpost in de tabel **Grootboekpost** (als op de inkoopregels een grootboekrekening staat). Daarnaast worden inkooporders altijd vastgelegd in de tabellen **Inkoopontvangst** en **Inkoopfactuur**.

Voordat u gaat boeken, kunt u een controlelijst afdrukken met alle informatie uit de inkooporder en eventuele fouten die erin voorkomen. Kies **Boeken** en vervolgens **Testrapport** als u het rapport wilt afdrukken.

**Belangrijk**: tijdens het boeken van een order kunt u zowel een ontvangst als een factuur maken. Deze kunt u tegelijkertijd, maar ook onafhankelijk van elkaar maken. U kunt ook een gedeeltelijke ontvangst en een gedeeltelijke factuur maken door de velden **Te ontvangen aantal** en **Te factureren aantal** op de afzonderlijke inkooporderregels in te vullen voordat u de boeking uitvoert. U kunt geen factuur maken voor iets dat niet is ontvangen. Dit betekent dat u pas kunt factureren als er een ontvangst is vastgelegd, of u moet tegelijkertijd ontvangen en factureren.

U kunt de optie Boeken of Boeken en afdrukken kiezen. Als u ervoor kiest om te boeken en af te drukken, wordt een lijst afgedrukt nadat de order is geboekt. U kunt ook de functie **Batchboeken** kiezen, waarmee u verschillende orders tegelijkertijd kunt boeken.

Na de boeking worden de geboekte inkoopregels verwijderd uit de order. Er verschijnt een bericht als de boeking is voltooid. Hierna kunt u de geboekte posten bekijken in de verschillende vensters die geboekte posten bevatten, zoals de vensters **Leveranciersposten**, **Grootboekposten**, **Artikelposten**, **Geboekte inkoopontvangsten** en **Geboekte inkoopfacturen**.

## <a name="see-also"></a>Zie ook
[Documenten en dagboeken boeken](ui-post-documents-journals.md)


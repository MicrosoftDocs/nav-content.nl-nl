---
title: Verkopen boeken
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 0ce8b5d9e77d40a5f10c9242e7368add5b75b12a
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="posting-sales"></a>Verkopen boeken
In de **Boekingsgroep** op een verkoopdocument kunt u kiezen uit de volgende boekingsfuncties:

- **Boeken**
- **Testrapport**
- **Boeken en verzenden**
- **Boeken en afdrukken**
- **Boeken en e-mailen**
- **Batchboeken**
- **Voorbeeld van boeking weergeven**

Wanneer u alle regels hebt ingevuld en alle informatie hebt ingevoerd op de verkooporder, kunt u de order boeken. Hiermee worden een verzending en een factuur gemaakt.

Wanneer een verkooporder wordt geboekt, worden de rekening van de klant, het grootboek en de artikelposten bijgewerkt.

Voor elke verkooporder wordt een verkooppost gemaakt in de tabel **Grootboekpost**. Ook wordt er een post in de klantrekening in de tabel **Klantpost** en een grootboekpost wordt in de desbetreffende rekening voor tegoeden gemaakt. Bovendien kan het boeken van de order resulteren in een btw-post en een grootboekpost voor de totale korting. Of er een post voor de korting wordt geboekt, hangt af van de inhoud van het veld **Korting boeken** in het venster **Verkoopinstellingen**.

Voor elke verkooporderregel wordt een artikelpost gemaakt in de tabel **Artikelpost** (als de verkoopregels artikelnummers bevatten) of wordt een grootboekpost gemaakt in de tabel **Grootboekpost** (als de verkoopregels een grootboekrekening bevatten). Daarnaast worden verkooporders altijd geregistreerd in de tabellen **Verkoopverzendkop** en **Verkoopfactuurkop**.

**Belangrijk**: wanneer u een order boekt, kunt u zowel een verzending als een factuur maken. Deze kunnen tegelijk of afzonderlijk worden uitgevoerd. U kunt ook een gedeeltelijke verzending en een gedeeltelijke factuur maken door de velden **Te verzenden aantal** en **Te factureren aantal** op de afzonderlijke verkooporderregels in te vullen voordat u de boeking uitvoert. U kunt geen factuur maken voor iets wat niet is verzonden. U kunt dus pas factureren nadat u een verzending hebt geregistreerd, of u moet ervoor kiezen om tegelijkertijd te verzenden en factureren. 

Na de boeking worden de geboekte verkoopregels verwijderd uit de order. Er verschijnt een bericht als de boeking is voltooid. Hierna kunt u de geboekte posten bekijken in de verschillende vensters die geboekte posten bevatten, zoals de vensters **Klantposten**, **Grootboekposten**, **Artikelposten**, **Geboekte verkoopverzendingen** en **Geboekte verkoopfacturen**.

## <a name="see-also"></a>Zie ook
[Procedure: Documenten per e-mail verzenden](ui-how-send-documents-email.md)


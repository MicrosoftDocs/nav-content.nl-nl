---
title: Dimensies
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: a1b38e74717e87bea6efb46f8f4e5236b6ec4e64
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

#<a name="dimensions"></a>Dimensies
Dimensies zijn gegevens die u kunt toevoegen aan posten om deze te categoriseren voor analyse. Er zijn bijvoorbeeld dimensies om aan te geven tot welk project of welke afdeling een post behoort.
Vervolgens kunt u dimensies gebruiken in plaats van het instellen van aparte grootboekrekeningen voor elke afdeling en elk project. Zodoende beschikt u over uitgebreide analysegegevens zonder een ingewikkeld rekeningschema te hoeven gebruiken.
U kunt een onbeperkt aantal dimensies definiëren met een onbeperkt aantal dimensiewaarden.  

U stelt bijvoorbeeld een dimensie met de naam *Afdeling* in en gebruikt deze dimensie en een dimensiewaarde wanneer u verkoopdocumenten boekt. Vervolgens kunt u bedrijfsinformatie krijgen over welke artikelen zijn verkocht door welke afdelingen, enzovoort.
Hoe meer dimensies u instelt en gebruikt, hoe gedetailleerder de rapporten waarop u uw bedrijfsbeslissingen kunt baseren. Bijvoorbeeld één verkooppost kan meerdere dimensiegegevens bevatten over de rekening waarop de verkoop van het artikel is geboekt, waar het artikel is verkocht, wie het heeft verkocht, en welk type klant de aankoop heeft gedaan.  

## <a name="using-dimensions"></a>Dimensies gebruiken
In een document zoals een verkooporder kunt u dimensiegegevens toevoegen voor een afzonderlijke documentregel en voor het document zelf. In het venster **Verkooporder** kunt u bijvoorbeeld dimensiewaarden invoeren voor de eerste twee shortcutdimensies, direct in het document, en u kunt meer dimensiegegevens toevoegen als u de knop **Dimensies** kiest.  
Als u in plaats daarvan in een dagboek werkt, kunt u ook op dezelfde manier dimensiegegevens toevoegen aan een post als u shortcutdimensies direct als velden hebt ingesteld op dagboekregels.  
U kunt standaarddimensies instellen voor rekeningen of rekeningsoorten, zodat dimensies en dimensiewaarden automatisch worden ingevuld.  

## <a name="dimension-sets"></a>Dimensiesets
Een dimensieset is een unieke combinatie dimensiewaarden. Een dimensieset wordt als dimensiesetposten in de database opgeslagen. Elke dimensiesetpost vertegenwoordigt één dimensiewaarde. De dimensiesetpost wordt geïdentificeerd door een gemeenschappelijke dimensieset-id die is toegewezen aan elke dimensiesetpost die tot de dimensieset behoort.  

Wanneer u een nieuwe dagboekregel, documentkop of documentregel maakt, kunt u een combinatie van dimensiewaarden opgeven. In plaats van elke dimensiewaarde expliciet in de database op te slaan, wordt een dimensieset-id toegewezen aan de dagboekregel, documentkop of documentregel om zo de dimensieset op te geven.  

## <a name="see-also"></a>Zie ook
[Financiën](finance-setup.md)  
[Dimensies instellen](finance-setup-setup-dimensions.md)  


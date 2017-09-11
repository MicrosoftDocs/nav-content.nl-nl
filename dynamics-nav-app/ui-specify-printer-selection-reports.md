---
title: Printerselectie opgeven voor rapporten
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
ms.openlocfilehash: 55b48aef2bc108ced7f581f0ff6c11263ee467df
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---
    
# <a name="specify-printer-selection-for-reports"></a>Printerselectie opgeven voor rapporten
U kunt rapporten instellen zodat ze op een specifieke printer worden afgedrukt. Hier volgen enkele toepassingen van de printerselectie: 

- U kunt rapporten afdrukken op speciaal briefpapier van het bedrijf.
- U kunt rapporten afdrukken op verschillende papierformaten.
- U kunt rapporten afdrukken op de standaardprinter van een opgegeven werknemer.

U gebruikt het venster **Printerselecties** om verschillende waarden in te stellen om verschillende uitvoer te verkrijgen. Als u een specifieke printer selecteert, heeft dat voorrang op een meer algemene printerselectie. Zo kunt u instellen printerselectie met de waarden in de **Gebruikersnaam**, **Rapport-ID**, en **Printernaam**. Deze printerselectie heeft voorrang op een printerselectie met lege velden **Gebruikersnaam** of **Rapport-ID**. 

De volgende tabel beschrijft de combinatie van waarden wanneer u printerinstellingen instelt voor een rapport.

|Als u dit wilt doen                                                 |Stel de volgende waarden in                                             |
|---------------------------------------------------|---------------------------------------------------------------------|
|Een rapport afdrukken naar een specifieke printer voor alle gebruikers |Geef waarden op in de velden **Rapport-ID** en **Printernaam** en laat het veld **Gebruikersnaam** leeg.|
|Alle rapporten naar een specifieke printer afdrukken voor een specifieke gebruiker|Geef waarden op in de velden **Gebruikers-ID** en **Printernaam** en laat het veld **Rapport-ID** leeg.|
|De standaardprinter voor alle rapporten instellen|Geef een waarde op in het veld **Printernaam** en laat de velden **Gebruikers-ID** en **Rapport-ID** leeg.|
|Een specifiek rapport afdrukken naar de standaardprinter van de gebruiker|Geef een waarde op in het veld **Rapport-ID** en laat de velden **Printernaam** en **Gebruikers-ID** leeg.|
|Een specifiek rapport naar een specifieke printer afdrukken voor een specifieke gebruiker|Geef waarden in alle drie de velden op.|

## <a name="see-also"></a>Zie ook
[Werken met Dynamics NAV](ui-work-product.md)


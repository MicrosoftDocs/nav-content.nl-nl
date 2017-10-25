---
title: Postcode-updates importeren
description: "Elke maand ontvangt u een postcodebestand met alle postcodemutaties in een maand. Dit postcodebestand kan worden geïmporteerd en kan de relevante gegevens in de tabel **Postcodereeks** bijwerken."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 891257ce2854a6da38377391333258b5d731af02
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-import-post-code-updates"></a>Procedure: Postcode-updates importeren
Elke maand ontvangt u een postcodebestand met alle postcodemutaties in een maand. Dit postcodebestand kan worden geïmporteerd en kan de relevante gegevens in de tabel **Postcodereeks** bijwerken.  
  
### <a name="to-import-the-update-file"></a>Het updatebestand importeren  
  
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Postcode-updates** in en kies vervolgens de gerelateerde koppeling.  
  
2.  Kies in het venster **Postcode-updates** op het tabblad **Acties** in de groep **Functies** de optie **Postcodes-update importeren**.  
  
3.  Geef het pad en de naam op van het postcode-updatebestand en kies vervolgens de knop **OK**. Als u het bestand niet wilt importeren, kiest u de knop **Annuleren** om het venster te sluiten.  
  
 Als geen bestand met een volledige set postcodegegevens is geïmporteerd, verschijnt er een bericht.  
  
 Voordat de postcodes worden bijgewerkt, worden de volgende controles uitgevoerd:  
  
-   Is er al een updatebestand geïmporteerd met een recenter datumveld dan de datum van dit nieuwe updatebestand? Als dat het geval is, wordt het proces gestopt.  
  
-   Is er een lange periode tussen de datum van dit bestand en de waarde in het datumveld van het laatst geïmporteerde bestand? Als dat het geval is, verschijnt er een bericht. U kunt kiezen of u het updatebestand nog steeds wilt importeren.  
  
 Gegevens over de geïmporteerde postcode worden opgeslagen in de tabel Postcode-update logpost.  
  
## <a name="see-also"></a>Zie ook  
 [Nederlandse postcodes](dutch-post-codes.md)   
 Tabel Postcode-update logpost   
 Venster Postcode-updates   
 Tabel Postcodereeks

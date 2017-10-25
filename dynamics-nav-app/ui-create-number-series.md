---
title: 'Procedure: Nummerreeksen maken '
description: Leer hoe u nummerreeksen instelt die unieke ID-codes toewijzen aan rekeningen en documenten in Dynamics NAV.
documentationcenter: 
author: SusanneWindfeldPedersen
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: numbers, numbering
ms.date: 06/02/2017
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 643e3e6a3374a2364f850c9d77ca3f59f01dab61
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-number-series"></a>Procedure: Nummerreeksen maken
Voor elk bedrijf dat u instelt, moet u unieke id-codes toewijzen aan zaken als grootboekrekeningen, klanten- en leveranciersrekeningen, facturen en overige documenten. De nummering is niet alleen belangrijk voor identificatie. Met een goed opgezet nummeringssysteem kan het bedrijf ook beter worden beheerd en geanalyseerd en kan het aantal fouten tijdens gegevensinvoer worden beperkt.

> [!NOTE]  
>   Het wordt aanbevolen om dezelfde nummerreekscodes te gebruiken die worden vermeld in het venster **Nr.-reeksoverzicht** in het voorbeeldbedrijf CRONUS. Codes zoals *I-FACT+* lijken in het begin mogelijk betekenisloos, maar [!INCLUDE[d365fin](includes/d365fin_md.md)] kent een aantal standaardinstellingen die afhankelijk zijn van deze codes.

U maakt een nummeringssysteem door een of meer codes in te stellen voor elk soort hoofdgegevens of document. U kunt bijvoorbeeld een code instellen voor het nummeren van klanten, een andere code voor het nummeren van verkoopfacturen en weer een andere code voor het nummeren van documenten in algemene dagboeken. Nadat u een code hebt ingesteld, moet u minimaal één nummerreeksregel instellen. De nummerreeksregel bevat gegevens, zoals het eerste en laatste nummer in de reeks en de begindatum. U kunt meer dan één nummerreeksregel per nummerreekscode invoeren, met een andere begindatum voor elke regel. De reeks wordt opeenvolgend gebruikt, waarbij elke reeks wordt gestart op de betreffende begindatum.

U configureert normaal gesproken de nummerreeks zodanig dat automatisch het eerstvolgende nummer wordt ingevoegd op nieuwe kaarten of documenten die u maakt. U kunt echter ook een nummerreeks instellen die toestaat dat u handmatig het nieuwe nummer invoert. U geeft dit aan met het selectievakje **Handm. nummering**.

Als u meer dan één nummerreekscode wilt gebruiken voor één soort hoofdgegevens (als u bijvoorbeeld verschillende nummerreeksen voor verschillende artikelcategorieën wilt gebruiken), kunt u relaties tussen nummerreeksen gebruiken.

## <a name="to-create-a-new-number-series"></a>Een nieuwe nummerreeks maken
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Nr.-reeksen** in en klik vervolgens op de gerelateerde koppeling.
2. Kies de actie **Nieuw**.
3. Vul op de nieuwe regel de velden indien nodig in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

**TIP**: Als u handmatige invoer van een nummer op nieuwe kaarten of documenten wilt toestaan, schakelt u het selectievakje **Autom. nummering** uit en schakelt u het selectievakje **Handm. nummering** in.

Wanneer u nu een nieuwe kaart of een document maakt, die is ingesteld om de betreffende nummerreeksen te gebruiken, kunt u handmatig in het veld **Nr.** iedere gewenste waarde invullen.  

## <a name="to-set-up-where-a-number-series-is-used"></a>Instellen waar een nummerreeks wordt gebruikt
In de volgende procedure wordt beschreven hoe u nummerreeksen instelt voor de module Verkoop. De stappen zijn vergelijkbaar voor andere modules.
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Verkopen en Klanten** in en klik vervolgens op de gerelateerde koppeling.
2. Selecteer in het venster **Verkopen en klanten** op het sneltabblad **Nummerreeksen** de gewenste nummerreeksen voor iedere verkoopkaart of -document.

Het geselecteerde nummer wordt nu ingevuld op het veld **Nr.**  op de kaart of het document, afhankelijk van de instellingen die u hebt ingevoerd op de nummerreeksregel.

## <a name="to-create-relationships-between-number-series"></a>Relaties maken tussen nummerreeksen
Als u meerdere nummerreekscodes hebt ingesteld voor hetzelfde soort basisgegevens of transacties, kunt u relaties tussen de codes instellen. Met deze functie kunt u een code kiezen wanneer u een nummer gebruikt.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Nr.-reeksen** in en klik vervolgens op de gerelateerde koppeling.
2. Selecteer de regel met de nummerreeks waarvoor u relaties wilt instellen en kies vervolgens **Relaties**.
3. Geef in het veld **Reeks** de code op voor de nummerreeks die u wilt koppelen aan de reeks die u in stap 2 hebt geselecteerd.
4. Voeg een regel toe voor elke code die u wilt koppelen aan de geselecteerde nummerreeksen.
5. Sluit het venster.

Wanneer u nu iets instelt waarvoor u een nummer nodig hebt, kunt u de relaties gebruiken die u hebt ingesteld om te kiezen tussen de gekoppelde nummerreeksen.

## <a name="see-also"></a>Zie ook
[Instellen van [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  


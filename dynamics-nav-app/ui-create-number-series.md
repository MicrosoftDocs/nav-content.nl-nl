---
title: Nummerreeksen maken
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
ms.openlocfilehash: 22b3bcf71c99e106527d6bfa35478045d29b9629
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="create-number-series"></a>Nummerreeksen maken

Voor elk bedrijf dat u instelt, moet u unieke id-codes toewijzen aan zaken als grootboekrekeningen, klanten- en leveranciersrekeningen, facturen en documenten. De nummering is niet alleen belangrijk voor identificatie. Met een goed opgezet nummeringssysteem kan het bedrijf ook beter worden beheerd en geanalyseerd en kan het aantal fouten tijdens gegevensinvoer worden beperkt.

U kunt een volledig nummeringssysteem instellen met een onbeperkt aantal reeksen. U kunt nummerreeksen gebruiken voor alle soorten documenten en dagboeken alsmede voor hoofdgegevens, zoals klanten, artikelen en verwerkingen.

U kunt het gebruik van nummerreeksen combineren met handmatige nummering.

U maakt een nummeringssysteem door een of meer codes in te stellen voor elk soort hoofdgegevens of document. U kunt bijvoorbeeld een code instellen voor het nummeren van klanten, een andere code voor het nummeren van verkoopfacturen en weer een andere code voor het nummeren van documenten in algemene dagboeken.

Nadat u een code hebt ingesteld, moet u minimaal één nummerreeksregel instellen. De nummerreeksregel bevat gegevens, zoals het eerste en laatste nummer in de reeks en de begindatum. U kunt meer dan één nummerreeksregel per nummerreekscode invoeren, met een andere begindatum voor elke regel. De reeks wordt opeenvolgend gebruikt, waarbij elke reeks wordt gestart op de betreffende begindatum.

Als u meer dan één nummerreekscode wilt gebruiken voor één soort hoofdgegevens (als u bijvoorbeeld verschillende nummerreeksen voor verschillende artikelcategorieën wilt gebruiken), kunt u relaties tussen nummerreeksen gebruiken.

Naast de nummers die u handmatig of via het nummeringssysteem toewijst, worden aan alle transacties (posten) automatisch volgnummers toegewezen. Deze nummers vindt u in het veld **Postnr.** in alle postvensters. U kunt deze nummers niet wijzigen of verwijderen.

## <a name="to-create-relationships-between-number-series"></a>Relaties maken tussen nummerreeksen
Als u meerdere nummerreekscodes hebt ingesteld voor hetzelfde soort basisgegevens of transacties, kunt u relaties tussen de codes instellen. Met deze functie kunt u een code kiezen wanneer u een nummer gebruikt.

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Nr.-reeksen** in en kies vervolgens de gerelateerde koppeling.
2. Selecteer de regel met de nummerreeks waarvoor u relaties wilt instellen en kies vervolgens **Relaties**.
3. Geef in het veld **Reeks** de code op voor de nummerreeks die u wilt koppelen aan de reeks die u in stap 2 hebt geselecteerd.
4. Voeg een regel toe voor elke code die u wilt koppelen aan de geselecteerde nummerreeksen.
5. Sluit het venster.

Wanneer u nu iets instelt waarvoor u een nummer nodig hebt, kunt u de relaties gebruiken die u hebt ingesteld om te kiezen tussen de gekoppelde nummerreeksen.

## <a name="see-also"></a>Zie ook
[Werken met Dynamics NAV](ui-work-product.md)


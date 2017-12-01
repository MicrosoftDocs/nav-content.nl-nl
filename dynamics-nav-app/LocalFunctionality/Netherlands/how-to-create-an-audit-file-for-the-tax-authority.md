---
title: Een auditfile voor de belastingdienst maken
description: Tijdens een controle van de boeken voor een boekjaar kan een belastinginspecteur om gegevens over de basistransacties vanuit het grootboek voor dat boekjaar vragen. Basistransacties worden gewoonlijk via dagboekposten verwerkt.
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
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 3840843555e5d5e5cdd403d025c7953dd2bcf259
ms.contentlocale: nl-nl
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-create-an-audit-file-for-the-tax-authority"></a>Procedure: Een auditfile voor de belastingdienst maken
Tijdens een controle van de boeken voor een boekjaar kan een belastinginspecteur om gegevens over de basistransacties vanuit het grootboek voor dat boekjaar vragen. Basistransacties worden gewoonlijk via dagboekposten verwerkt. Daarom vormen de dagboekposten de basis voor het auditbestand.  

 De belastingdienst stimuleert bedrijven om het auditfile te gebruiken, maar dat is niet verplicht.  

 De auditfile kan tevens worden gebruikt om gegevens uit te wisselen tussen bedrijven. U kunt elke gewenste periode selecteren, maar de begindatum en einddatum van de opgegeven periode moeten in hetzelfde boekjaar liggen.  

## <a name="to-make-an-audit-file"></a>Een auditfile maken  

1.  Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Belastingdienst - Auditfile** in en kies vervolgens de gerelateerde koppeling.  
2.  Vul op het sneltabblad **Opties** de velden in, zoals in de volgende tabel is beschreven.  

    |Veld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Begindatum**|Geef de begindatum of de periode op waarop de gegevens moeten worden gebaseerd.|  
    |**Einddatum**|Geef de einddatum of de periode op waarop de gegevens moeten worden gebaseerd.|  
    |**Beginsaldo uitsluiten**|Geeft op of het auditbestand het beginsaldo moet bevatten van grootboekrekeningen.<br /><br /> Het veld kan worden bewerkt als de begindatum van de periode gelijk is aan de begindatum van een boekjaar.|  

3.  Kies de knop **OK** om het auditbestand te maken. Als u het auditbestand niet wilt maken, kiest u de knop **Annuleren** om het venster te sluiten.  

Wanneer u het rapport uitvoert, moet u de naam en locatie van het geëxporteerde bestand opgeven. De standaardbestandsnaam is **audit.xaf**, maar u kunt dat wijzigen. De bestandsextensie moet .xaf zijn.  

## <a name="see-also"></a>Zie ook  
 [Elektronische btw- en ICP-aangiften](electronic-vat-and-icp-declarations.md)   
 [Procedure: Elektronische btw- en ICP-aangiften verzenden](how-to-submit-electronic-vat-and-icp-declarations.md)


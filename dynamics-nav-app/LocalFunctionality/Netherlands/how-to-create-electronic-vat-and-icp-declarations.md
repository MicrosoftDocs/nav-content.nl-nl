---
title: Elektronische btw- en ICP-aangiften maken
description: Als u elektronische btw- en ICP-aangiften wilt maken, moet u eerst de aangifte instellen met het venster **Elek. aangifte-instellingen**. Vervolgens kunt u ze naar de belastingdienst verzenden.
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
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: a34b50394cec73bc8e0958b5c98d1be3a2d111dd
ms.contentlocale: nl-nl
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-create-electronic-vat-and-icp-declarations"></a>Procedure: Elektronische btw- en ICP-aangiften maken
Als u elektronische btw- en ICP-aangiften wilt maken, moet u eerst de aangifte instellen met het venster **Elek. aangifte-instellingen**. Vervolgens kunt u ze naar de belastingdienst verzenden.  

> [!NOTE]  
>  Als u het veld **Deel van Fiscale eenheid** in het venster **Elek. aangifte-instellingen** hebt geselecteerd, kunt u een elektronische aangifte voor slechts één bedrijf maken. Als u de btw-gegevens van alle dochterondernemingen van een moedermaatschappij wilt combineren, moet u een btw-aangifte op papier opstellen voor elke dochteronderneming en handmatig de totaalbedragen voor de moedermaatschappij berekenen. Deze totaalbedragen van de moedermaatschappij moeten worden ingevoerd op de website van de belastingdienst. U kunt geen belastinggegevens van ICP-aangiften combineren. ICP-aangiften moeten altijd afzonderlijk worden ingediend.  

Als er geen intracommunautaire leveringen zijn geweest in de aangifteperiode, dan wordt er een elektronische ICP-aangifte aangemaakt zonder XML-elementen voor de leveringen. Als u een dergelijke aangifte verzendt, wordt een foutbericht weergegeven.  

## <a name="to-create-an-electronic-vat-or-icp-declaration"></a>Een elektronische btw- of ICP-aangifte maken  

1.  Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Elektronische aangiften** in en kies de gerelateerde koppeling.  
2.  Kies in het venster **Overzicht elektronische aangiften** de actie **Nieuw**.  
3.  Vul in het venster **Elektronische aangiftekaart** op het sneltabblad **Algemeen** de vereiste velden in zoals beschreven in de volgende tabel.  

    |Veld|Description|  
    |-----------------------------------|---------------------------------------|  
    |**Sjabloonnaam**|De naam van de sjabloon die wordt gebruikt om de elektronische aangifte te maken.|  
    |**Aangifte**|De naam van het afschrift dat wordt gebruikt om de elektronische aangifte te maken.|  

6.  Kies de knop **OK**.  

De XML-elementen met de bijbehorende gegevens van de elektronische aangifte worden weergegeven op het sneltabblad **Regels** in het venster **Elektronische aangiftekaart**.  

## <a name="see-also"></a>Zie ook  
 [Elektronische belastingaangiften](electronic-tax-declarations.md)   
 [Elektronische btw- en ICP-aangiften](electronic-vat-and-icp-declarations.md)   
 [Procedure: Btw-categorieën instellen](how-to-set-up-vat-categories.md)


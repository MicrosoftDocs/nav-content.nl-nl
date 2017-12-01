---
title: Responsberichten van de belastingdienst verwerken
description: Als u een elektronische btw- of ICP-aangifte verzendt naar de belastingdienst, wordt de aangifte verwerkt en wordt u in reactie een bericht gestuurd.
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
ms.openlocfilehash: 6a6881ded3bf004b92a63489bc3f17dbb3220beb
ms.contentlocale: nl-nl
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-process-response-messages-from-tax-authorities"></a>Procedure: Responsberichten van de belastingdienst verwerken
Als u een elektronische btw- of ICP-aangifte verzendt naar de belastingdienst, wordt de aangifte verwerkt en wordt u in reactie een bericht gestuurd.  

U kunt de respons in [!INCLUDE[navnow](../../includes/navnow_md.md)] importeren met de batchverwerking **Responsberichten ontvangen**. Het responsbericht bevat de status van de aangifte.  

## <a name="to-import-messages-from-the-tax-authorities-server"></a>Berichten importeren van de server van de belastingdienst  

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Responsberichten elektronische aangiften** in en klik vervolgens op de gerelateerde koppeling.  
2.  Kies de actie **Responsberichten ontvangen**.  
3.  Vul op het sneltabblad **Opties** de velden in, zoals in de volgende tabel is beschreven.  

    |Veld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Wachtwoord versleuteling CA-certificaat**|Het wachtwoord dat is gebruikt wordt om de CA-certificaten te versleutelen.|  
    |**Wachtwoord gebruikerscertificaat**|Het wachtwoord dat gebruikt wordt om de gebruikerscertificaten te versleutelen.|  

4.  Kies de knop **OK**.  

## <a name="to-process-the-response-messages-from-the-tax-authorities"></a>Responsberichten van de belastingdienst verwerken  

1.  Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Responsberichten elektronische aangiften** in en klik vervolgens op de gerelateerde koppeling.  
2.  Kies de actie **Responsberichten verwerken**.  
3.  Selecteer in het venster **Batchverwerking Responsberichten verwerken** op het sneltabblad **Elek. aangifteresponsbericht** de juiste filters.  
4.  Kies de knop **OK**.  

    De verwerkte gegevens over het responsbericht wordt weergegeven in het **Responsberichten elektronische aangiften** in.  

5.  Als u een bericht of bijlage wilt exporteren, kiest u op het tabblad **Responsbericht exporteren** de actie **Responsbericht exporteren**.  

## <a name="see-also"></a>Zie ook  
 [Elektronische btw- en ICP-aangiften](electronic-vat-and-icp-declarations.md)   
 [Procedure: Btw-categorieën instellen:](how-to-set-up-vat-categories.md)   
 [Procedure: Elektronische btw- en ICP-aangiften maken](how-to-create-electronic-vat-and-icp-declarations.md)   
 


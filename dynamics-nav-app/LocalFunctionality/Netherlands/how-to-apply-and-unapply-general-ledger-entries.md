---
title: Grootboekposten vereffenen en de vereffening ervan ongedaan maken
description: Door tijdelijke grootboekposten te vereffenen kunnen bedrijven werken met tijdelijke rekeningen en transferrekeningen in het grootboek. Tijdelijke en transferrekeningen worden gebruikt om tijdelijke posten op te slaan die op verdere verwerking in het grootboek wachten.
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
ms.openlocfilehash: d22556c7fa33cf03eb6a1573378117af68979c4f
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-apply-and-unapply-general-ledger-entries"></a>Procedure: Grootboekposten vereffenen en de vereffening ervan ongedaan maken
Door tijdelijke grootboekposten te vereffenen kunnen bedrijven werken met tijdelijke rekeningen en transferrekeningen in het grootboek. Tijdelijke en transferrekeningen worden gebruikt om tijdelijke posten op te slaan die op verdere verwerking in het grootboek wachten.  
  
 U kunt tijdelijke rekeningen gebruiken voor:  
  
-   Geldtransfers van de ene naar de andere bankrekening.  
  
-   Financiële transactietransfers van het ene systeem naar het andere, waarbij een deel van de gegevens tijdelijk op het oorspronkelijke systeem staat.  
  
-   Transacties waarvoor u een verkoopfactuur hebt verzonden naar een klant maar nog niet de bijbehorende inkoopfactuur van de leverancier hebt ontvangen.  
  
 Nadat de posten zijn verwerkt, kunt u de functie voor postenvereffening gebruiken om de geboekte posten en het boekingsrekeningsoort bij te werken.  
  
 U kunt de vereffening van de vereffende grootboekposten ongedaan maken en vervolgens de gesloten posten openen om wijzigingen aan te brengen.  
  
### <a name="to-apply-general-ledger-entries"></a>Grootboekposten vereffenen  
  
1.  Voer in het tekstvak **Zoeken** **Grootboekjournalen** in en kies vervolgens de gerelateerde koppeling.  
  
2.  Selecteer een grootboekjournaal en kies op het tabblad **Start** in de groep **Verwerken** de optie **Grootboek**.  
  
3.  Kies in het venster **Grootboekposten** op het tabblad **Start** in de groep **Functies** de optie **Posten vereffenen**.  
  
     Alle openstaande posten voor de grootboekrekening worden weergegeven in het venster **Grootboekposten vereffenen**.  
  
    > [!NOTE]  
    >  Standaard wordt het veld **Posten opnemen** ingesteld op **Open**. U kunt de waarde van het veld **Posten opnemen** wijzigen in **Alle** of **Afgesloten**. U kunt alleen grootboekposten vereffenen die **open** zijn.  
  
4.  Selecteer de relevante grootboekpost en kies vervolgens op het tabblad **Navigeren** in de groep **Toepassing** de optie **Vereffenings-id instellen**.  
  
     Het veld **Vereffenings-id** wordt bijgewerkt met de gebruikers-id. Het restbedrag wordt weergegeven in het veld **Saldo** in het venster **Grootboekposten vereffenen**.  
  
5.  Klik op het tabblad **Navigeren** in de groep **Vereffening** op **Vereffening boeken**.  
  
     U kunt de vereffening boeken zelfs wanneer het saldobedrag gelijk is aan 0. Wanneer wordt geboekt, wordt het veld **Restbedrag** als volgt beïnvloed:  
  
    -   Als het veld **Saldo** gelijk is aan 0, wordt het veld **Restbedrag** bij alle grootboekposten op 0 gezet.  
  
    -   Als het veld **Saldo** niet gelijk is aan 0, wordt het bedrag in het veld **Saldo** overgebracht naar het veld **Restbedrag** van de grootboekpost die was geselecteerd toe u de vereffening boekte.  
  
    -   Voor alle overige grootboekposten wordt het veld **Restbedrag** op 0 gezet en worden de velden **Open**, **Afgesloten door volgnr.**, **Afgesloten met bedrag** en **Afgesloten op** bijgewerkt.  
  
    > [!NOTE]  
    >  Wanneer wordt geboekt, worden de grootboekposten die het veld **Vereffenings-id** bijwerken, verwijderd.  
  
6.  Kies de knop **OK**.  
  
### <a name="to-view-the-applied-general-ledger-entries"></a>De vereffende grootboekposten weergeven  
  
1.  Voer in het tekstvak **Zoeken** **Grootboekjournalen** in en kies vervolgens de gerelateerde koppeling.  
  
2.  Selecteer een grootboekjournaal en kies op het tabblad **Start** in de groep **Verwerken** de optie **Grootboek**.  
  
3.  Selecteer de relevante grootboekpost en kies vervolgens op het tabblad **Navigeren** in de groep **Toepassing** de optie **Vereffende posten**.  
  
     U kunt alle vereffende grootboekposten weergeven.  
  
4.  Kies de knop **OK**.  
  
### <a name="to-unapply-general-ledger-entries"></a>De vereffening van grootboekposten ongedaan maken  
  
1.  Voer in het tekstvak **Zoeken** **Grootboekjournalen** in en kies vervolgens de gerelateerde koppeling.  
  
2.  Selecteer een grootboekjournaal en kies op het tabblad **Start** in de groep **Verwerken** de optie **Grootboek**.  
  
3.  Selecteer de grootboekpost waarvan u de vereffening ongedaan wilt maken en kies vervolgens op het tabblad **Navigeren** in de groep **Toepassing** de optie **Vereffening ongedaan maken**.  
  
     De vereffening van de vereffende grootboekposten wordt ongedaan gemaakt.  
  
    > [!NOTE]  
    >  Als een post is vereffend met meer dan één vereffeningspost, moet u de vereffening van de laatste vereffeningspost het eerst ongedaan maken. Standaard wordt de laatste post weergegeven.  
  
4.  Kies de knop **OK**.  
  
## <a name="see-also"></a>Zie ook  
 Grootboekrekening   
 Grootboekpost   
 Grootboekposten

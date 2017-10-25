---
title: Documenten en dagboeken boeken
description: IC-documenten te gebruiken om transacties met uw IC-partners te boeken.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: IC, group, consolidation, affiliate, subsidiary
ms.date: 06/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 176c12271c55936e61235e3a726932aa02b29b74
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-work-with-intercompany-documents-and-journals"></a>Procedure: Werken met intercompany-documenten en -dagboeken
Door middel van intercompany-documenten of -dagboeken kunt u transacties met uw IC-partners boeken. Wanneer u een IC-document of -dagboekregel boekt in uw bedrijf, wordt een corresponderend document of dagboekregel gemaakt in uw IC-outbox, dat/die u kunt overbrengen naar uw partner. Uw partner kan de bijbehorende transactie vervolgens boeken in zijn bedrijf, zonder de gegevens opnieuw te hoeven invoeren.

Bij inkoop- en verkoopdocumenten zorgt de IC-partnercode voor de betrokken klant of leverancier ervoor dat alle gegenereerde orders en facturen die verband houden met transacties met deze bedrijven de bijbehorende documenten aanmaken in het partnerbedrijf, zodat de rekeningen overal sluitend zijn.

Voor IC-diversendagboekregels hoeft u geen rekeningen op te geven voor een aparte reeks boeken, maar geeft u eenvoudigweg de ID van het partnerbedrijf op. Corresponderende IC-grootboekregels worden dan in het partnerbedrijf gemaakt, die resulteren in het sluitend maken van de boeken van beide bedrijven die bij de transactie zijn betrokken.

## <a name="to-fill-in-and-send-an-intercompany-sales-order"></a>Een IC-verkooporder invullen en verzenden
U kunt verkoop- en inkooporders en retourorders verzenden voordat u deze boekt. Facturen en creditnota's kunnen pas worden verzonden nadat u deze hebt geboekt.

In de volgende procedure wordt beschreven hoe u een IC-verkooporder kunt invullen en verzenden. Dezelfde stappen gelden voor IC-inkooporders en -retourorders en voor geboekte IC-facturen en -creditnota's.  

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Verkooporders** in en klik vervolgens op de gerelateerde koppeling.  
2. Kies **Nieuw** om een nieuwe verkooporder te maken. Zie [Procedure: Producten verkopen](sales-how-sell-products.md) voor meer informatie.  
3. Vul indien nodig de velden in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Controleer of de klant een IC-partner is.
5. Als u de verkooporder wilt verzenden voordat u hem boekt, kiest u de actie **IC-verkooporder verzenden**.

> [!NOTE]
> Als u stap 4 uitvoert, wordt de verkooporder naar uw IC-outbox verplaatst van waaruit u hem later kunt verzenden. Zie voor meer informatie [Procedure: De intercompany-inbox en outbox beheren](intercompany-how-manage-intercompany-inbox.md).

## <a name="to-fill-in-and-post-an-intercompany-journal"></a>Een IC-dagboek invullen en boeken
Wanneer u een IC--diversendagboekregel boekt in uw bedrijf, wordt een corresponderende dagboekregel gemaakt in uw IC-outbox, die u kunt overbrengen naar uw partner. Uw partner kan de bijbehorende transactie vervolgens boeken in zijn bedrijf, zonder de gegevens opnieuw te hoeven invoeren.

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **IC-diversendagboeken** in en klik vervolgens op de gerelateerde koppeling.  
2. Open de relevante dagboekbatch. Zie [Werken met diversendagboeken](ui-work-general-journals.md) voor meer informatie.
3. Vul indien nodig de velden in.
4. In het veld **Grootboekrekeningnr. IC-partner** voert u de IC-grootboekrekening in waarop het bedrag wordt geboekt in het bedrijf van uw partner.

    > [!NOTE]
    > Dit veld moet worden ingevuld op een regel met een bankrekening of grootboekrekening in het veld **Rek.-nr.** of in het veld **Tegenrekeningnr.**  
5. Kies de actie **Boeken**.

De betreffende posten worden geboekt in uw bedrijf en een dagboek met de bijbehorende posten wordt gemaakt in uw IC-outbox, die u naar uw partnerbedrijf kunt verzenden. Zie voor meer informatie [Procedure: De intercompany-inbox en outbox beheren](intercompany-how-manage-intercompany-inbox.md). 

## <a name="see-also"></a>Zie ook
[Intercompany-transacties beheren](intercompany-manage.md)  
[Financiën](finance.md)  
[Financiën instellen](finance-setup-finance.md)  
[Werken met diversendagboeken](ui-work-general-journals.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


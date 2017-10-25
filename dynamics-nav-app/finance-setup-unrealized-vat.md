---
title: Ongerealiseerde btw instellen
description: Als u op kas gebaseerde boekhouding gebruikt, kunt u opgeven hoe ongerealiseerde btw voor verkopen en inkopen moet worden verwerkt.
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cash, VAT, unrealized, cash-based
ms.date: 09/08/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: f5786a79e8f12bd86b3d6f7ce53e0c698b19cef4
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---

# <a name="how-to-set-up-unrealized-vat-for-cash-based-accounting"></a>Procedure: Ongerealiseerde btw voor op kas gebaseerde boekhouding instellen
Als u op kas gebaseerde boekhoudingsmethoden gebruikt, kunt u [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)] instellen om ongerealiseerde btw te verwerken.

## <a name="to-use-general-ledger-accounts-for-unrealized-vat"></a>Grootboekrekeningen gebruiken voor ongerealiseerde btw
U kunt ervoor kiezen btw-bedragen te laten berekenen en boeken naar een tijdelijke grootboekrekening wanneer een factuur wordt geboekt. Vervolgens wordt de factuur geboekt naar de juiste grootboekrekening en opgenomen in btw-aangiften wanneer de werkelijke betaling van de factuur is geboekt. Hiervoor moet u eerst de btw-boekingsinstellingen voltooien.

Ga als volgt te werk om rekeningen voor ongerealiseerde btw te gebruiken:
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport") en voer **Grootboekinstellingen** in. 
2. Kies op de pagina **Boekhoudinstellingen** op het sneltabblad **Algemeen** **Meer weergeven** en kies vervolgens het selectievakje **Ongerealiseerde btw**.
3. Sluit de pagina.
4. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport** ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "Pictogram Zoeken naar pagina of rapport") en voer **Btw-boekingsinstellingen** in. 
5. Op de pagina **Btw-boekingsinstellingen** kiest u de btw-boekingsgroep en vervolgens **Bewerken**. 
6. In het veld **Ongerealiseerde btw-soort** kiest u een optie om op te geven hoe u betalingen toewijst aan het factuurbedrag (zonder btw) en het btw-bedrag zelf, en hoe btw-bedragen van de ongerealiseerde btw-rekening moeten worden overgeboekt naar de gerealiseerde rekening. De volgende tabel beschrijft de opties.

| Optie | Omschrijving |
| --- | --- |
| Leeg | Kies deze optie als u de functie voor ongerealiseerde btw niet wilt gebruiken. |
| Percentage | Zowel het btw- als het factuurbedrag worden verrekend met de betalingen in verhouding tot het betalingspercentage van het resterende factuurbedrag. Het betaalde btw-bedrag wordt van de ongerealiseerde btw-rekening overgeboekt naar de gerealiseerde btw-rekening. |
| Eerste | Eerst wordt het btw-bedrag verrekend met de betalingen en dan het factuurbedrag. Het bedrag dat van de ongerealiseerde btw-rekening wordt overgemaakt naar de btw-rekening, is dan gelijk aan het betalingsbedrag totdat de volledige btw is betaald. |
| Laatste | Eerst wordt het factuurbedrag verrekend met de betalingen en dan het btw-bedrag. In dit geval wordt er alleen een bedrag van de ongerealiseerde btw-rekening overgeboekt naar de btw-rekening als het volledige factuurbedrag, exclusief de btw, is betaald. |
| Eerste (Voll. bet.) | Eerst wordt de btw verrekend met betalingen (zoals bij de optie _Eerste_), maar er wordt pas een bedrag naar de btw-rekening overgeboekt als het volledige btw-bedrag is betaald. |
| Laatste (Voll. bet.) | Eerst wordt het factuurbedrag verrekend met betalingen (zoals bij de optie _Laatste_), maar er wordt pas een bedrag naar de btw-rekening overgeboekt als het volledige btw-bedrag is betaald. |

6. Kies in het veld **Ongerealiseerde verkoop-btw-rekening** de rekening voor ongerealiseerde verkoop-btw.

    > [!NOTE]  
>   Het btw-bedrag wordt naar deze rekening geboekt en blijft daar tot de betaling van de klant is geboekt. Daarna wordt het bedrag overgeboekt naar de rekening voor verkoop-btw.
7. Voer in het veld **Ongerealiseerde inkoop-btw-rekening** de grootboekrekening voor ongerealiseerde inkoop-btw in.

    > [!NOTE]  
>   Het btw-bedrag wordt naar deze rekening geboekt en blijft daar tot de betaling van de klant is geboekt. Daarna wordt het bedrag overgeboekt naar de rekening voor verkoop-btw.

## <a name="see-also"></a>Zie ook
[Btw instellen](finance-setup-vat.md)

---
title: Werken met voorraadperioden
description: "U kunt bepalen in welke periode mensen wijzigingen in voorraad kunnen boeken door voorraadperioden te definiëren."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: inventory, periods
ms.date: 08/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 289b12d39c9f67913d862cb3500cccae0b3823d2
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-work-with-inventory-periods"></a>Procedure: werken met voorraadperioden
Een voorraadperiode is een periode waarin gewijzigde voorraadwaarden kunnen worden geboekt. Een voorraadperiode wordt begrensd door een einddatum. Als u een voorraadperiode hebt afgesloten, kunt u geen verwachte of gefactureerde voorraadwaarden vóór de einddatum meer boeken. U kunt geen nieuwe waarden naar de voorraad boeken vóór de einddatum. Als er nog open artikelposten, d.w.z. positieve aantallen die nog niet zijn vereffend met uitgaande transacties, zijn die binnen de afgesloten periode vallen, kunt u de uitgaande aantallen ook nadat de periode is afgesloten nog met deze posten vereffenen.  

In de volgende secties wordt uitgelegd hoe u:  

* Voorraadperioden maken.  
* Voorraadperioden afsluiten.  
* Voorraadperioden opnieuw openen.  

## <a name="to-create-an-inventory-period"></a>Een voorraadperiode maken  
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Voorraadperioden** in en klik vervolgens op de gerelateerde koppeling.  
2. Een nieuwe regel maken.  
3. Voer in het veld **Einddatum** de laatste datum van de voorraadperiode in die u wilt definiëren. Wanneer de periode is afgesloten, kunt u geen voorraadwijzigingen vóór deze datum boeken.  
4. Typ een beschrijvende naam in het veld **Naam**. Kies de knop **Ok**.  

## <a name="closing-inventory-periods"></a>Voorraadperioden afsluiten  
Het veld **Gesloten** geeft aan of de voorraadperiode afgesloten is voor wijzigingen in voorraadwaarden. U kunt dit veld niet bewerken.  

Onder de volgende omstandigheden kunt u iedere voorraadperiode afsluiten:  

* De periode bevat geen openstaande uitgaande artikelposten, dat wil zeggen negatieve voorraad.  
* De kosten van alle artikelen zijn aangepast met gebruik van de batchverwerking **Kostprijs herwaarderen - Artikelposten**.  

Dit betekent dat alle uitgaande transactieaantallen, zoals de aantallen van verkooporders, uitgaande transfers, verkoopfacturen, inkoopretourorders of inkoopcreditnota's, moeten worden vereffend met bestaande aantallen in de voorraad.  

### <a name="to-close-an-inventory-period"></a>Een voorraadperiode afsluiten  
1. Voordat u een voorraadperiode afsluit, voert u de batchverwerking **Kostprijs herwaarderen - Artikelposten** uit, om ervoor te zorgen dat alle kostenherwaarderingen zijn geboekt. Kies op het tabblad **Acties** in de groep **Functies** de optie **Kostprijs herwaarderen - Artikelposten**.  

     Voer de lijst **Voorraadperiode afsluiten - Controle** uit om te zien of er openstaande uitgaande posten voorkomen in de voorraadperiode of artikelen waarvan de kosten nog niet zijn geherwaardeerd.  
2. Kies de actie **Voorraadperiode afsluiten - Controle**.  

     Voer de batchverwerking **Voorraadwaarde boeken** uit om ervoor te zorgen dat alle kosten naar het grootboek zijn geboekt.  
3. Kies de actie **Van Voorraadbeheer naar GB boeken**.  
4. Selecteer in het venster **Voorraadperioden** de voorraadperiode die u wilt sluiten.  
5. Kies de actie **Periode afsluiten**. Wanneer de voorraadperiode eenmaal is afgesloten, kunt u geen voorraadwijzigingen boeken vóór de einddatum. U dient de kosten van alle artikelen te herwaarderen met de batchverwerking **Kostprijs herwaarderen - Artikelposten** voordat u de voorraadperiode afsluit.  
6. Kies de knop **Ja** om te bevestigen dat u de periode wilt afsluiten of kies **Nee** om het afsluiten te annuleren.  
7. De voorraadperiode wordt afgesloten en daarna wordt een bevestigingsbericht weergegeven.  

## <a name="reopening-inventory-periods"></a>Voorraadperioden opnieuw openen  
Nadat u de voorraadperiode hebt afgesloten, kunt u deze niet verwijderen. U kunt de periode echter wel weer opnieuw openen als u boekingen vóór de einddatum van de voorraadperiode wilt toestaan. Wanneer u een periode opnieuw opent, worden alle voorraadperioden met latere einddatums ook weer geopend.  

### <a name="to-reopen-an-inventory-period"></a>Een voorraadperiode opnieuw openen  
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Voorraadperioden** in en klik vervolgens op de gerelateerde koppeling.  
2. Selecteer de voorraadperiode die u opnieuw wilt openen.  
3. Kies de periodeactie **Periode opnieuw openen**. Bevestig dat u de periode opnieuw wilt openen.  
4. Alle voorraadperioden met latere einddatums dan de geselecteerde periode worden eveneens opnieuw geopend.  

## <a name="see-also"></a>Zie ook  
[Ontwerpdetails: Voorraadperioden](design-details-inventory-periods.md)  
[Financiën](finance.md)  
[Voorraad](inventory-manage-inventory.md)  
[Werken met Dynamics NAV](ui-work-product.md)


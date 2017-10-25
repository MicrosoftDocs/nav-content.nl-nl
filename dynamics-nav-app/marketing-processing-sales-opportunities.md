---
title: Verkoopopportunities verwerken in verkoopcycli
description: U kunt verkoopopportunities weergeven sluiten of verwijderen en u kunt ook offertes en verkooporders voor opportunity's maken en een opportunity verplaatsen door de fasen van een verkoopcyclus.
documentationcenter: 
author: jswymer
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 06/06/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 9fe0bd97f7493d9acf4ab99a771fd5f6219027f8
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-process-sales-opportunities"></a>Procedure: Verkoopopportunities verwerken
Nadat u een opportunity hebt gemaakt, zijn er verschillende functies voor het beheren van de opportunity en het verplaatsen ervan naar voltooiing.

## <a name="to-view-opportunities"></a>Opportunities weergeven
De bestaande verkoopopportunities zijn beschikbaar in het venster **Opportunity-overzicht**. Er zijn verschillende manieren om toegang tot dit venster te krijgen om verkoopopportunities te verwerken:

| Opportunities weergeven voor | Dan |
| --- | --- |
| Alle verkopers en contacten |Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Opportunity-overzicht** in en klik vervolgens op de gerelateerde koppeling. |
| Een bepaalde verkoper |Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Verkopers** in en klik vervolgens op de gerelateerde koppeling. Selecteer de verkoper, kies de actie **Opportunities** en kies vervolgens de actie **Overzicht**. |
| Een bepaald contact |Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Contacten** in en klik vervolgens op de gerelateerde koppeling. Selecteer het contact in de lijst en kies vervolgens de actie **Opportunities**. |

Al deze taken openen het venster **Opportunity-overzicht**.

## <a name="to-close-opportunities"></a>Opportunities sluiten
U kunt opportunities afsluiten wanneer de onderhandelingen zijn afgerond. Wanneer u een opportunity afsluit, kunt u opgeven of de opportunity is gewonnen of verloren en de redenen voor het afsluiten. Als u een reden wilt opgeven, moet u codes voor gesloten opportunities instellen.

1. Selecteer in het venster **Opportunity-overzicht** de opportunity en kies de actie **Sluiten**. Het venster **Opportunity afsluiten** wordt geopend.
2. Vul de relevante velden in en kies de knop **OK**.

   De velden **Opportunitycode afsluiten** en **Datum afgesloten** zijn vereiste velden en moeten worden ingevuld voordat u de knop **OK** kunt kiezen.

   In het veld **Opportunitycode afsluiten** kunt u een van de bestaande codes voor het sluiten van opportunities kiezen of een nieuwe code toevoegen. Als u een nieuwe code wilt toevoegen, kiest u in de vervolgkeuzelijst **Selecteren vanuit volledige lijst** en kiest u vervolgens **nieuw**. Vul op de nieuwe, lege regel de velden **Code**, **Soort** en **Omschrijving** in en kies vervolgens de knop **OK**.

## <a name="to-create-quotes-for-opportunities"></a>Offertes maken voor opportunity's
U kunt verkoopoffertes maken voor contactpersonen die niet zijn geregistreerd als klant.

1. Selecteer in het venster **Opportunity-overzicht** de opportunity en kies vervolgens de actie **Verkoopofferte toekennen**. Het venster **Verkoopofferte** wordt geopend.
2. Vul de betreffende velden in.

## <a name="to-create-sales-orders-for-opportunities"></a>Verkooporders voor opportunity's maken
U kunt verkooporders maken van de verkoopoffertes die u hebt gemaakt voor de opportunities. Voordat u verkooporders voor uw contacten kunt maken, moet u het contact eerst als klant maken. Zie voor meer informatie [Een klant, leverancier of bankrekening maken van een contact](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).

1. Zoek in het venster **Opportunity-overzicht** de opportunity waarvoor u een verkoopofferte hebt gemaakt.
2. Kies de actie **Verkoopofferte toekennen**. Het venster **Verkoopofferte** wordt geopend met de verkoopofferte die u aan de opportunity hebt toegewezen.
3. Vul de extra velden in en kies vervolgens de actie **Order maken**.

Wanneer u verkoopopportunities verwerkt, moet u wellicht een offerte maken voor het contact aan wie de opportunity is gekoppeld.

## <a name="to-delete-opportunities"></a>Opportunities verwijderen
U kunt opportunities verwijderen, bijvoorbeeld nadat u een verkoop hebt afgesloten. U kunt echter alleen gesloten opportunities verwijderen. Er zijn twee manieren om afgesloten opportunities te verwijderen. U kunt individuele afgesloten opportunities verwijderen vanuit het venster **Opportunity-overzicht** of u kunt de batchverwerking **Afgesloten opportunities verwijderen** uitvoeren om meerdere opportunities te verwijderen op basis van een opgegeven criterium.

Als u gesloten afgesloten opportunities wilt verwijderen vanuit het venster **Opportunity-overzicht**, selecteert u de opportunity, en kiest u vervolgens de actie **Verwijderen**.

Als u afgesloten opportunities wilt verwijderen met de batchverwerking **Afgesloten opportunities verwijderen**, volgt u deze stappen:

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Opportunity's verwijderen** in en klik vervolgens op de gerelateerde koppeling.
2. Stel in het gedeelte **Opportunity** de filters in die opgeven welke gesloten opportunities moeten worden verwijderd.
3. Kies de knop **Ok**.

Nadat u een opportunity hebt verwijderd, wordt de opportunity verwijderd uit het venster **Opportunity-overzicht**.

## <a name="to-move-an-opportunity-through-sales-cycle-stages"></a>Een opportunity verplaatsen door verkoopcyclifasen
Als een opportunity een verkoopcyclus volgt, kunt u deze voorwaarts of achterwaarts door de verschillende fasen verplaatsen, bijvoorbeeld naar de volgende of vorige fase, en zelfs een fase overslaan.

1. Kies in het venster **Opportunity-overzicht** de actie **Bijwerken**. De wizard **Opportunity bijwerken** wordt geopend.
2. Gebruik het **Actiesoort** om de opportunity door de verkoopcyclusfasen te verplaatsen:
   * **Volgende** verplaatst de opportunity één fase.
   * Met **Overslaan** wordt de opportunity een of meer fasen voorwaarts verplaatst in de verkoopcyclus, wat u opgeeft in het veld **Presentatie**. U kunt alleen fasen overslaan die alleen zijn ingesteld om overslaan toe te staan.
   * **Vorige** verplaatst de opportunity één fase terug.
   * Met **Springen** wordt de opportunity een of meer fasen terug verplaatst in de verkoopcyclus, wat u opgeeft in het veld **Presentatie**.
   * Met **Bijwerken** kunt u informatie wijzigen (bijvoorbeeld om de evaluatie van de slagingskans en de geschatte waarden te wijzigen) zonder te verplaatsen naar een andere fase.
3. Vul de overige velden desgewenst in en kies de knop **OK**.

## <a name="see-also"></a>Zie ook
[Verkoop](sales-manage-sales.md)  
[Contactpersonen maken en beheren](marketing-contacts.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


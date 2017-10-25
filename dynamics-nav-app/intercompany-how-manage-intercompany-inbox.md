---
title: Inkomende en uitgaande IC-transacties verwerken
description: Intercompany-transacties (IC-transacties) die u ontvangt van uw IC-partners worden weergegeven in de IC-inbox, waar u ze handmatig of automatisch verwerkt.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: incoming document
ms.date: 07/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 869dacac09019fda487e8ac18a5c8ff5d0fd17ac
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-manage-the-intercompany-inbox-and-outbox"></a>Procedure: De intercompany-inbox en outbox beheren
Alle IC-transacties die u via elektronische weg ontvangt van uw IC-partners, worden weergegeven in de IC-inbox.  

## <a name="organizing-the-inbox"></a>De IC-inbox ordenen  
 Met de filtervelden boven aan het inboxvenster kunt u bepalen welke transacties worden weergegeven in het venster. Als u bijvoorbeeld alleen transacties wilt weergeven die door een bepaalde partner zijn gemaakt, kunt u filtercriteria invoeren in de filters **Transactiebron** en IC-**partnercode**.  

### <a name="transaction-source"></a>Transactiebron  
Wat u met een transactie kunt doen, hangt af van het volgende:  

- Transactie gemaakt door uw IC-partner  
- Transactie geweigerd door uw IC-partner en aan u geretourneerd  

Met het veld **Transactiebron weergeven** kunt u het venster **IC-inboxtransacties** filteren, zodat maar een van deze soorten transacties wordt weergegeven. U kunt ook filteren op IC-partner of op de inhoud van het veld **Regelactie**.  

#### <a name="created-by-intercompany-partner"></a>Transactie gemaakt door IC-partner  
 Wanneer u een nieuwe transactie ontvangt die door uw partner is gemaakt, kunt u ervoor kiezen:

- De transactie te accepteren  
- De transactie te weigeren (en aan de partner te retourneren)  
- De transactie te annuleren (de transactie verwijderen en niet retourneren aan uw partner)  

#### <a name="returned-from-intercompany-partner"></a>Geretourneerd door IC-partner  
 Als de transactie is geweigerd door uw IC-partner, hebt u geen andere keuze dan de transactie in de inbox te annuleren. Vervolgens moet u correctieregels maken of het dagboek of document in uw bedrijf tegenboeken.  

## <a name="re-creating-inbox-entries"></a>Inboxitems opnieuw maken  
 Als u een transactie in uw inbox hebt geaccepteerd maar het document of dagboek vervolgens hebt verwijderd in plaats van geboekt, kunt u het inboxitem opnieuw maken en het nogmaals accepteren.  

## <a name="getting-an-overview-of-intercompany-transactions-for-a-period"></a>Een overzicht weergeven van IC-transacties voor een bepaalde periode  
 U kunt een overzicht weergeven van alle IC-transacties die u in een bepaalde periode hebt verzonden en ontvangen. In de lijst **IC-transacties** worden alle IC-grootboekposten, klantenposten en leveranciersposten weergegeven.

 > [!NOTE]  
 > Als de IC-partners in dezelfde database zijn opgenomen, worden de transacties verzonden zonder dat een bestand of e-mail nodig is. Zie het veld **Overdrachttype** in het venster **IC-partner**. <br /><br />
In dat geval, kunt u in het systeem instellen om de inbox en de outbox over te slaan, door respectievelijk het selectievakje **Transacties automatisch accepteren** in het venster **IC-partner** en het selectievakje **Transacties automatisch verzenden** in het venster **IC-instellingen** in te schakelen.

## <a name="to-import-intercompany-transactions-from-a-file"></a>IC-transacties importeren uit een bestand  
Als u een IC-partner hebt die zich niet in dezelfde database bevindt als uw bedrijf, kunt u IC-transacties van die partner ophalen in een XML-bestand. Vervolgens moet u de transacties importeren in uw inbox.  

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Bedrijfsgegevens** in en klik vervolgens op de gerelateerde koppeling.
2. Sla het bestand op naar de locatie die u hebt opgegeven in het veld **Details IC-inbox** in het venster **Bedrijfsgegevens**.  
3. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "Zoeken naar pagina of rapport")-pictogram, voer **IC-inboxtransacties** in en klik vervolgens op de gerelateerde koppeling.
4. Kies in het venster **IC-inboxtransacties** de actie **Transactiebestand importeren**.  
5. Selecteer in het venster dat wordt geopend het .xml-bestand dat de transacties bevat en klik vervolgens op **Openen**.  

De transacties worden geïmporteerd in de inbox en u kunt ze nu verwerken.

## <a name="to-process-incoming-intercompany-transactions"></a>Inkomende IC-transacties verwerken  
Wanneer uw IC-partners u IC-transacties toesturen, komen de transacties terecht in uw IC-inbox. U moet elke transactie in uw inbox evalueren en verwerken.  

1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "Zoeken naar pagina of rapport")-pictogram, voer **IC-inboxtransacties** in en klik vervolgens op de gerelateerde koppeling.  
2. Selecteer in het venster **IC-inboxtransacties** een regel en kies een actie om de regel te verwerken, zoals bijvoorbeeld **Goedkeuren**.
3. Vul in het venster **Bewerking IC-inbox voltooien** de velden in met de benodigde gegevens. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Kies de knop **OK**.  

Bij regels die u verwerkt met de actie **Goedkeuren**, worden document- of dagboekregels aangemaakt in uw bedrijf. Open elk document of dagboek, breng de gewenste wijzigingen aan en boek de regels.  

De regels die u verwerkt met de actie **Retour naar partner** worden verplaatst naar de IC-outbox, vanwaar u ze naar uw partner kunt verzenden.

Voor regels die u verwerkt met de actie **Retour door partner** moet u nu een correctie boeken op de oorspronkelijke transactie die u boekte in uw bedrijf.

## <a name="to-process-outgoing-intercompany-transactions"></a>Uitgaande IC-transacties verwerken  
Wanneer u een IC-dagboek of -document boekt of een IC-orderbevestiging verzendt, worden de transacties verzonden naar uw IC-outbox. Als u deze wilt doorsturen naar uw IC-partners, moet u de outbox openen en de transacties verwerken.  

1.  Klik op het pictogram ![Zoeken naar pagina of rapport]pictogram(media/ui-search/search_small.png "Zoeken naar pagina of rapport"), voer **IC-outboxtransacties** in en klik vervolgens op de gerelateerde koppeling.  
2. Selecteer in het venster **IC-outboxtransacties** een regel en kies een actie om de regel te verwerken, zoals bijvoorbeeld **Terug naar inbox**.

Regels die u verwerkt met de actie **Verzenden naar IC-partner** worden verzonden naar de inbox van de betreffende partner.

De regels die u verwerkt met de actie **Terug naar inbox** worden naar de inbox verplaatst, waar u ze kunt goedkeuren om documenten of dagboekregels in uw bedrijf te maken.  

Voor regels die u verwerkt met de actie **Annuleren** moet u nu een correctie boeken op de oorspronkelijke transactie die u boekte in uw bedrijf.  

## <a name="to-recreate-intercompany-inbox-transactions"></a>IC-inboxtransacties opnieuw maken  
Het kan voorkomen dat u een transactie in de inbox of outbox opnieuw wilt maken. Als u een transactie in uw inbox bijvoorbeeld hebt geaccepteerd maar het document of dagboek vervolgens hebt verwijderd in plaats van geboekt, kunt u de inboxpost opnieuw maken en deze nogmaals accepteren.  

In de volgende procedure wordt beschreven hoe u inboxtransacties opnieuw kunt maken. De procedure voor de outbox is hetzelfde.

  1.  Klik op het pictogram ![Zoeken naar pagina of rapport]pictogram(media/ui-search/search_small.png "Zoeken naar pagina of rapport"), voer **Verwerkte IC-inboxtransacties** in en klik vervolgens op de gerelateerde koppeling.  

  2.  Open het venster **Verwerkte IC-inboxtransacties**, selecteer de regel met de transactie die u opnieuw wilt maken in de inbox en selecteer de actie **Inboxtransacties opnieuw maken**.  

## <a name="see-also"></a>Zie ook
[Intercompany-transacties beheren](intercompany-manage.md)  
[Financiën](finance.md)  
[Financiën instellen](finance-setup-finance.md)  
[Werken met diversendagboeken](ui-work-general-journals.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)


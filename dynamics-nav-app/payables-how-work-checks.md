---
title: 'Procedure: Werken met cheques'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 421516a7580a90d6eabc8ecfcc841215839994c9
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-work-with-checks"></a>Procedure: Werken met cheques
Dynamics NAV ondersteunt het elektronisch en handmatig verzenden van cheques. Bij beide methoden wordt het betalingsdagboek gebruikt om cheques te verzenden naar leveranciers. Daarnaast kunt u cheques nietig verklaren en chequeposten weergeven.

Bij het proces voor het uitgeven van cheques worden betalingen voorgesteld, worden posten gemaakt en worden de computercheques afgedrukt.

De printer moet correct zijn ingesteld op het afdrukken van chequeformulieren en u moet bepalen welke indeling wordt gebruikt. Zie voor meer informatie [Procedure: Cheque-indelingen definiëren](finance-setup-how-define-check-layouts.md)

## <a name="to-issue-checks"></a>Cheques uitgeven
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Betalingsdagboeken** in en kies vervolgens de gerelateerde koppeling.
2. Vul het dagboek met relevante betalingen, bijvoorbeeld met behulp van de functie Leveranciersbetalingen voorstellen. Zie voor meer informatie [Procedure: Leveranciersbetalingen voorstellen](payables-how-suggest-vendor-payments.md).
3. Selecteer een van de volgende opties in het veld **Betalingssoort** op dagboekregels voor betalingen die u wilt doen met cheques:

 - **Automatische cheque**: selecteer deze optie als u een cheque wilt afdrukken voor het bedrag op de betalingsdagboekregel. U moet de cheques afdrukken voordat u de dagboekregels kunt boeken. U kunt **Automatische cheque** alleen selecteren als het **Tegenrekeningsoort** of het **Rekeningsoort** **Bankrekening** is.

 - **Handmatige cheque**: selecteer deze optie als u handmatig een cheque hebt gemaakt en er een bijbehorende chequepost moet worden gemaakt voor dit bedrag. Met deze optie kunt u geen cheques afdrukken vanuit Dynamics NAV. U kunt **Handmatige cheque** alleen selecteren als het **Tegenrekeningsoort** of het **Rekeningsoort** **Bankrekening** is.

    **Opmerking**: u moet automatische cheques afdrukken voordat u de gerelateerde dagboekregels boekt.
4. In het geval van automatische cheques kiest u **Cheque afdrukken**.
5. Vul indien nodig de velden in het venster **Cheque** in. Kies een veld om een korte omschrijving van het veld of een koppeling naar meer informatie te lezen.
6. Klik op **Afdrukken**.

**Opmerking**: als u cheques in meerdere valuta's van verschillende bankrekeningen wilt afdrukken, moet u de batchverwerking **Cheque afdrukken** voor elke valuta afzonderlijk uitvoeren en de juiste bankrekening opgeven.

## <a name="to-cancel-printed-checks-that-are-not-posted"></a>Afgedrukte cheques annuleren die niet zijn geboekt
U kunt niet-geboekte cheques annuleren nadat ze zijn afgedrukt door de actie **Ongeldige cheque** in het venster **Betalingsdagboek** te gebruiken.
1. Kies in het venster **Betalingsdagboek** de actie **Ongeldige cheque** en kies vervolgens welke cheques u wilt annuleren.

## <a name="to-void-checks"></a>Cheques nietig verklaren
Wanneer chequebetaling is geboekt, kunt u cheques alleen annuleren (nietig verklaren) vanuit de resulterende bankposten.

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Bankrekeningen** in en kies vervolgens de gerelateerde koppeling.
2. Selecteer de betreffende bankrekening, kies de actie **Bewerken** en kies vervolgens de actie **Chequeposten**.
3. Kies in het venster **Chequeposten** de actie **Ongeldige cheque**.
4. Schakel het selectievakje **Cheque alleen nietig verklaren** in.
5. Kies de knop **OK**.

## <a name="see-also"></a>Zie ook
[Betalingsverplichtingen beheren](payables-manage-payables.md)  
[Bankieren instellen](bank-setup-banking.md)  


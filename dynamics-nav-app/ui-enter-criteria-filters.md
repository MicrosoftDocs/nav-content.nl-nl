---
title: Criteria in filters invoeren
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 8eab393a0a77f9f1595ca1247c7549e68b491cb2
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="entering-criteria-in-filters"></a>Criteria in filters invoeren
Wanneer u naar gegevens, zoals klantnamen, adressen of productgroepen wilt zoeken, voert u criteria in. In zoekcriteria kunt u alle cijfers en letters gebruiken die u normaal in het specifieke veld gebruikt. Daarnaast kunt u speciale symbolen gebruiken om de resultaten verder te filteren.

## <a name="searching-using-the-quick-filter"></a>Zoeken met het Snelfilter
U kunt filters toevoegen aan alle pagina's met het Snelfilter. Het Snelfilter wordt ingeschakeld door het vergrootglaspictogram in de rechterbovenhoek van een pagina te kiezen. Dit type filter wordt gebruikt voor een snelle invoer van criteria.

**Belangrijk**: het Snelfilter biedt eenvoudig toegang om gegevens te filteren door onbewerkte tekst in te voeren, maar het biedt ook veel zoekcriteriaopties. Afhankelijk van of u normale tekst of tekst met symbolen invoert, werkt het snelfilter anders.  
- Als u gewone tekst in de zoekcriteria opgeeft, worden de zoekcriteria geïnterpreteerd als een hoofdletterongevoelige zoekactie die bepaalde tekst bevat.  
- Als u tekst inclusief symbolen in de zoekcriteria opgeeft, worden de zoekcriteria precies zo geïnterpreteerd als u ze hebt ingevoerd en wordt onderscheid gemaakt tussen hoofdletters en kleine letters.

### <a name="quick-filter-criteria"></a>Snelfiltercriteria
<!-- html syntax because symbols conflict with MarkDown syntax -->
<TABLE>
  <TR>
    <TH>Zoekcriteria</TH>
    <TH>Geïnterpreteerd als...</TH>
    <TH>Retourneert...</TH>
  </TR>
  <TR>
    <TD>>man</TD>
    <TD>@*man*</TD>
    <TD>Alle records met de tekst man en ongevoelig voor hoofdletters en kleine letters.</TD>
  </TR>
  <TR>
    <TD>>se</TD>
    <TD>@*se*</TD>
    <TD>Alle records met de tekst se en ongevoelig voor hoofdletters en kleine letters.</TD>
  </TR>
  <TR>
    <TD>>Man*</TD>
    <TD>Begint met Man en is hoofdlettergevoelig.</TD>
    <TD>Alle records die beginnen met de tekst Man.</TD>
  </TR>
  <TR>
    <TD>'man'</TD>
    <TD>Een exacte tekst en gevoelig voor hoofdletters en kleine letters.</TD>
    <TD>Alle records die precies overeenkomen met man.</TD>
  </TR>
  <TR>
    <TD>@*man</TD>
    <TD>Eindigt met en is niet hoofdlettergevoelig.</TD>
    <TD>Alle records die eindigen met man.</TD>
  </TR>
  <TR>
    <TD>@man*</TD>
    <TD>Begint met en is niet hoofdlettergevoelig.</TD>
    <TD>Alle records die beginnen met man.</TD>
  </TR>
</TABLE>

**Opmerking**: u kunt geen jokerteken gebruiken bij het filteren op opsommingvelden, zoals het veld **Status** op verkooporders. Om een filter voor deze veldsoort in te voeren, kunt u de numerieke waarde als een filterparameter invoeren. Bijvoorbeeld: gebruik in het veld **Status** op een verkooporder met de waarden **Open**, **Vrijgegeven**, **Wacht op goedkeuring** en **Wacht op vooruitbetaling** de waarden **0**, **1**, **2** en **3** om voor deze opties te filteren.  

## <a name="see-also"></a>Zie ook
[Werken met Dynamics NAV](ui-work-product.md)


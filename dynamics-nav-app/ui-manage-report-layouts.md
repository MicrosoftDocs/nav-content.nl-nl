---
title: Werken met aangepaste en ingebouwde lay-outs voor rapporten en documenten
description: Gebruik rapportlay-outs om documenten aan te passen, bijvoorbeeld om het lettertype of logo aan te passen of pagina-instellingen of PDF-bestanden die u naar klanten verzendt.
documentationcenter: 
author: SusanneWindfeldPedersen
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customized report, document layout, logo, personalize
ms.date: 03/29/2017
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 11abe8b3375bca1515602143830d4c9963058172
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="managing-report-and-document-layouts"></a>Lay-outs van rapporten en documenten beheren
Een rapportlay-out bepaalt de inhoud en de indeling van het rapport, inclusief welke gegevensvelden van een rapportgegevensset in het rapport worden weergegeven, hoe ze worden gerangschikt, welke tekststijl en afbeeldingen worden gebruikt, enzovoort. Vanuit [!INCLUDE[d365fin](includes/d365fin_md.md)] kunt u bepalen welke lay-out wordt gebruikt in een rapport, een nieuwe lay-out maken of de huidige lay-outs wijzigen.

> [!NOTE]  
>   In [!INCLUDE[d365fin](includes/d365fin_md.md)] omvat de term 'rapport' ook documenten die extern worden verspreid, zoals verkoopfacturen en orderbevestigingen die u aan klanten als pdf-bestanden verzendt.

Met een rapportlay-out wordt met name het volgende ingesteld:

* De label- en gegevensvelden die moeten worden opgenomen uit de gegevensset van het [!INCLUDE[d365fin](includes/d365fin_md.md)]-rapport.
* De tekstindeling, bijvoorbeeld lettertype, -grootte en -kleur.
* Het bedrijfslogo en de positie ervan.
* Algemene pagina-instellingen, zoals marges en achtergrondafbeeldingen.

Een [!INCLUDE[d365fin](includes/d365fin_md.md)]-rapport kan worden ingesteld met meerdere rapportlay-outs, waartussen u indien nodig kunt schakelen. U kunt een van de ingebouwde rapportlay-outs gebruiken of u kunt aangepaste rapportlay-outs maken en ze indien nodig aan uw rapporten toewijzen. Zie voor meer informatie [Procedure: Een aangepaste lay-out voor een rapport of document maken](ui-how-create-custom-report-layout.md).

Er zijn twee soorten rapportlay-outs die u in rapporten kunt gebruiken: Word en RDLC.

## <a name="word-report-layout-overview"></a>Overzicht van de Word-rapportlay-out
Een Word-rapportlay-out wordt gebaseerd op een Word-document (.docx-bestandstype). Met Word-rapportlay-outs kunt u rapportlay-outs ontwerpen door Microsoft Word 2013 of later te gebruiken. Een Word-rapportlay-out bepaalt de inhoud van het rapport: hoe de inhoudelementen worden gerangschikt en hoe ze eruit zien. Een Word-document met een rapportlay-out gebruikt meestal tabellen om inhoud te rangschikken. De cellen kunnen gegevensvelden, tekst of afbeeldingen bevatten.

 ![Voorbeeld van een Word-rapportlay-outdocument voor NAV](media/nav_wordreportlayout_edit_in_word_example.png "NAV_WordReportLayout_Edit_In_Word_Example")  

## <a name="rdlc-layout-overview"></a>Overzicht van de RDLC-lay-out
RDLC-lay-outs zijn gebaseerd op clientrapportdefinitielay-outs (.rdlc- of .rdl-bestandstypen). Deze lay-outs worden gemaakt en gewijzigd vanuit SQL Server Report Builder. Het ontwerpconcept voor RDLC-lay-outs lijkt op Word-lay-outs, waarbij de lay-out de algemene indeling van het rapport definieert en bepaalt welke velden uit de database worden opgenomen. RDLC-lay-outs ontwerpen is geavanceerder dan Word-lay-outs ontwerpen. Zie voor meer informatie [RDLC-rapportlay-outs ontwerpen](https://msdn.microsoft.com/en-us/dynamics-nav/designing-rdlc-report-layouts).

## <a name="built-in-and-custom-report-layouts"></a>Ingebouwde en aangepaste rapportlay-outs
[!INCLUDE[d365fin](includes/d365fin_md.md)] bevat verschillende geïntegreerde lay-outs. Ingebouwde lay-outs zijn vooraf gedefinieerde lay-outs die voor bepaalde rapporten zijn ontworpen. Rapporten in [!INCLUDE[d365fin](includes/d365fin_md.md)] hebben een geïntegreerde lay-out zoals een RDLC-rapportlay-out, Word-rapportlay-outs of in bepaalde gevallen beide. U kunt een geïntegreerde rapportlay-out niet vanuit [!INCLUDE[d365fin](includes/d365fin_md.md)] wijzigen, maar u gebruikt deze als uitgangspunt voor het maken van uw eigen aangepaste rapportlay-outs.

Aangepaste lay-outs zijn rapportlay-outs die u ontwerpt om de weergave van een rapport te wijzigen. U maakt meestal een aangepaste lay-out op basis van een ingebouwde lay-out, maar u kunt ze ook nieuw maken of op basis van een kopie van een bestaande aangepaste lay-out. Met aangepaste lay-outs kunt u meerdere lay-outs voor hetzelfde rapport hebben waartussen u indien nodig kunt schakelen. U kunt bijvoorbeeld verschillende lay-outs voor elk [!INCLUDE[d365fin](includes/d365fin_md.md)]-bedrijf hebben of u kunt verschillende lay-outs voor hetzelfde bedrijf hebben voor bepaalde situaties of gebeurtenissen, zoals een speciale campagne of feestdagen.

## <a name="deciding-whether-to-use-a-word-or-rdlc-report-layout"></a>Besluiten of u een Word- of een RDLC-rapportlay-out wilt gebruiken
Een rapportlay-out kan worden gebaseerd op een Word-document of op een RDLC-bestand. Het besluit om een Word-rapportlay-out of een RDLC-rapportlay-out te gebruiken is afhankelijk van hoe u wilt dat het gegenereerde rapport eruitziet en van uw kennis van Word en SQL Server Report Builder.

De algemene ontwerpconcepten voor Word- en RDLC-lay-outs lijken erg op elkaar. Elk type heeft echter bepaalde ontwerpfuncties die bepalen hoe het gegenereerde rapport eruitziet in [!INCLUDE[d365fin](includes/d365fin_md.md)]. Dit houdt in dat hetzelfde rapport er anders uit kan zien wanneer u de Word-rapportlay-out gebruikt dan wanneer u de RDLC-rapportlay-out gebruikt.

Het proces voor het instellen van Word-rapportlay-outs en RDLC-rapportlay-outs in rapporten is hetzelfde. Het belangrijkste verschil is de manier waarop u de lay-outs wijzigt. Word-rapportlay-outs zijn in het algemeen gemakkelijker te maken en te wijzigen dan RDLC-rapportlay-outs, omdat u Word kunt gebruiken. RDLC-rapportlay-outs worden gewijzigd met SQL Server Report Builder, dat voor geavanceerdere gebruikers is bedoeld.

Zie [Procedure: Wijzigen welke lay-out momenteel in een rapport wordt gebruikt](ui-how-change-layout-currently-used-report.md) voor informatie over het wijzigen van de te gebruiken lay-out.

## <a name="see-also"></a>Zie ook
[Rapport- of documentlay-outs bijwerken](ui-update-report-layouts.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Procedure: Een aangepaste lay-out voor een rapport of document maken en wijzigen](ui-how-create-custom-report-layout.md)  
[Procedure: Een aangepaste lay-out voor een rapport of document importeren en exporteren](ui-how-import-and-export-report-layout.md)  
[Procedure: Documenten per e-mail verzenden](ui-how-send-documents-email.md)  
[Werken met rapporten](ui-work-report.md)  


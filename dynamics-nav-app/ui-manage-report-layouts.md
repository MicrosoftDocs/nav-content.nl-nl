---
title: Rapportlay-outs beheren
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 57cd575c1f72841dae162b077d1f676720ee24e7
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---
    
# <a name="manage-report-layouts"></a>Rapportlay-outs beheren
Een rapportlay-out bepaalt de inhoud en de indeling van het rapport, inclusief welke gegevensvelden van een rapportgegevensset in het rapport worden weergegeven, hoe ze worden gerangschikt, welke tekststijl en afbeeldingen worden gebruikt, enzovoort. Vanuit de clients van Dynamics NAV kunt u bepalen welke lay-out wordt gebruikt in een rapport, kunt u een nieuwe lay-out maken of kunt u de huidige lay-outs wijzigen. 

Met een rapportlay-out wordt met name het volgende ingesteld:

- De label- en gegevensvelden die moeten worden opgenomen uit de gegevensset van het Dynamics NAV-rapport.
- De tekstindeling, bijvoorbeeld lettertype, -grootte en -kleur.
- Het bedrijfslogo en de positie ervan.
- Algemene pagina-instellingen, zoals marges en achtergrondafbeeldingen. 

Een Dynamics NAV-rapport kan worden ingesteld met meerdere rapportlay-outs, waartussen u indien nodig kunt schakelen. U kunt een van de ingebouwde rapportlay-outs gebruiken of u kunt aangepaste rapportlay-outs maken en ze indien nodig aan uw rapporten toewijzen.

Er zijn twee soorten rapportlay-outs die u in rapporten kunt gebruiken: Word en RDLC.

## <a name="word-report-layout-overview"></a>Overzicht van de Word-rapportlay-out
Een Word-rapportlay-out wordt gebaseerd op een Word-document (.docx-bestandstype). Met Word-rapportlay-outs kunt u rapportlay-outs ontwerpen door Microsoft Word 2013 of later te gebruiken. Een Word-rapportlay-out bepaalt de inhoud van het rapport: hoe de inhoudelementen worden gerangschikt en hoe ze eruit zien. Een Word-document met een rapportlay-out gebruikt meestal tabellen om inhoud te rangschikken. De cellen kunnen gegevensvelden, tekst of afbeeldingen bevatten.

## <a name="rdlc-layout-overview"></a>Overzicht van de RDLC-lay-out
RDLC-lay-outs zijn gebaseerd op clientrapportdefinitielay-outs (.rdlc- of .rdl-bestandstypen). Deze lay-outs worden gemaakt en gewijzigd vanuit SQL Server Report Builder. Het ontwerpconcept voor RDLC-lay-outs lijkt op Word-lay-outs, waarbij de lay-out de algemene indeling van het rapport definieert en bepaalt welke velden uit de database worden opgenomen. RDLC-lay-outs ontwerpen is geavanceerder dan Word-lay-outs ontwerpen.

## <a name="built-in-and-custom-report-layouts"></a>Ingebouwde en aangepaste rapportlay-outs
Dynamics NAV bevat verschillende ingebouwde lay-outs. Ingebouwde lay-outs zijn vooraf gedefinieerde lay-outs die voor bepaalde rapporten zijn ontworpen. Rapporten in Dynamics NAV hebben een ingebouwde lay-out zoals een RDLC-rapportlay-out, Word-rapportlay-outs of in bepaalde gevallen beide. U kunt een ingebouwde rapportlay-out niet vanuit Dynamics NAV wijzigen, maar u gebruikt deze als uitgangspunt voor het maken van uw eigen aangepaste rapportlay-outs. 

Aangepaste lay-outs zijn rapportlay-outs die u ontwerpt om de weergave van een rapport te wijzigen. U maakt meestal een aangepaste lay-out op basis van een ingebouwde lay-out, maar u kunt ze ook nieuw maken of op basis van een kopie van een bestaande aangepaste lay-out. Met aangepaste lay-outs kunt u meerdere lay-outs voor hetzelfde rapport hebben waartussen u indien nodig kunt schakelen. U kunt bijvoorbeeld verschillende lay-outs voor elk bedrijf van Dynamics NAV hebben of u kunt verschillende lay-outs voor hetzelfde bedrijf hebben voor bepaalde situaties of gebeurtenissen, zoals een speciale campagne of feestdagen.

## <a name="deciding-whether-to-use-a-word-or-rdlc-report-layout"></a>Besluiten of u een Word- of een RDLC-rapportlay-out wilt gebruiken 
Een rapportlay-out kan worden gebaseerd op een Word-document of op een RDLC-bestand. Het besluit om een Word-rapportlay-out of een RDLC-rapportlay-out te gebruiken is afhankelijk van hoe u wilt dat het gegenereerde rapport eruitziet en van uw kennis van Word en SQL Server Report Builder. 

De algemene ontwerpconcepten voor Word- en RDLC-lay-outs lijken erg op elkaar. Elk type heeft echter bepaalde ontwerpfuncties die bepalen hoe het gegenereerde rapport eruitziet in Dynamics NAV. Dit houdt in dat hetzelfde rapport er anders uit kan zien wanneer u de Word-rapportlay-out gebruikt dan wanneer u de RDLC-rapportlay-out gebruikt.

Het proces voor het instellen van Word-rapportlay-outs en RDLC-rapportlay-outs in rapporten is hetzelfde. Het belangrijkste verschil is de manier waarop u de lay-outs wijzigt. Word-rapportlay-outs zijn in het algemeen gemakkelijker te maken en te wijzigen dan RDLC-rapportlay-outs, omdat u Word kunt gebruiken. RDLC-rapportlay-outs worden gewijzigd met SQL Server Report Builder, dat voor geavanceerdere gebruikers is bedoeld.

Zie [Procedure: Wijzigen welke lay-out momenteel in een rapport wordt gebruikt](ui-how-change-layout-currently-used-report.md) voor informatie over het wijzigen van de te gebruiken lay-out

## <a name="see-also"></a>Zie ook
[Werken met Dynamics NAV](ui-work-product.md)  
[Procedure: Een aangepaste rapportlay-out maken](ui-how-create-custom-report-layout.md)  
[Procedure: Documenten per e-mail verzenden](ui-how-send-documents-email.md)


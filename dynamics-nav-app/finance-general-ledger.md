---
title: Leren over grootboek en COA
description: "Beschrijft het grootboek, het rekeningschema en rekeningcategorieën."
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: analysis, history, track
ms.date: 06/02/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 348a1bcbe6908c7bfd84e99245363e733414aeae
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="understanding-the-general-ledger-and-the-coa"></a>Het grootboek en COA begrijpen
In het grootboek worden uw financiële gegevens opgeslagen en het rekeningschema bevat de rekeningen waarnaar alle grootboekposten worden geboekt. [!INCLUDE[d365fin](includes/d365fin_md.md)] bevat een standaardrekeningschema dat gereed is voor ondersteuning van uw bedrijf.

## <a name="general-ledger-setup-and-general-posting-setup"></a>Grootboekinstellingen en algemene boekingsinstellingen
De instelling van het grootboek bevindt zich in de kern van financiële processen omdat hiermee wordt bepaald hoe u gegevens boekt.  

In het venster **Grootboekinstellingen** geeft u op hoe bepaalde boekhoudkwesties in uw bedrijf worden afgehandeld, zoals:  

* Factuurafrondingsdetails  
* Adresindelingen  
* Financiële rapportage  

In het venster **Boekingsgroepinstelling** geeft u op dezelfde manier op hoe u combinaties van algemene bedrijfsgroepen en algemene productboekingsgroepen wilt instellen. Met boekingsgroepen worden entiteiten zoals klanten, leveranciers, artikelen, resources en verkoop- en inkoopdocumenten aan grootboekrekeningen gekoppeld. U vult een regel in voor elke combinatie van bedrijfs- en productboekingsgroep. Zie [Boekingsgroepinstellingen](finance-posting-groups.md) voor meer informatie.  

## <a name="the-chart-of-accounts"></a>het rekeningschema
In het rekeningschema worden alle grootboekrekeningen weergegeven. In het rekeningschema kunt u onder andere het volgende doen:  

* Rapporten weergeven waarin grootboekposten en saldi worden weergegeven.  
* Sluit uw resultatenrekening.  
* Open de grootboekrekeningkaart om instellingen toe te voegen of te wijzigen.  
* Bekijk een lijst met boekingsgroepen waarmee naar die rekening wordt geboekt.
* Afzonderlijke debet- en creditsaldo's voor één rekening bekijken  

U kunt grootboekrekeningen toevoegen, wijzigen of verwijderen. Om verschillen te voorkomen, kunt u echter geen grootboekrekening verwijderen als deze gegevens worden gebruikt in het rekeningschema.  

## <a name="account-categories"></a>Rekeningcategorieën
U kunt de structuur van uw financiële overzichten personaliseren door grootboekrekeningen toe te wijzen aan rekeningcategorieën.  

Het venster **GB-rekeningcategorieën** toont uw categorieën en subcategorieën en de grootboekrekeningen die eraan zijn toegewezen. U kunt nieuwe subcategorieën maken en die categorieën toewijzen aan bestaande rekeningen.  

U maakt een categoriegroep door andere subcategorieën onder een regel te laten inspringen in het venster **GB-rekeningcategorieën**. Zo wordt het gemakkelijk voor u om een overzicht te krijgen, omdat elke groepering een totaalsaldo weergeeft. U kunt bijvoorbeeld subcategorieën maken voor verschillende soorten activa en vervolgens categoriegroepen maken voor vaste activa versus huidige activa.  

U kunt opgeven of de rekeningen in elke subcategorie moeten worden opgenomen in bepaalde soorten rapporten. De rekeningcategorieën helpen de indeling te definiëren van uw financiële overzichten.  

Het standaardsaldo-overzicht heeft bijvoorbeeld één subcategorie voor Kas onder Huidige activa. Als u wilt dat kleine kas en de betaalrekening worden meegenomen in het saldo-overzicht, kunt u het volgende doen:  

1. Voeg twee nieuwe subcategorieën toe. Een voor kleine kas en een voor uw betaalrekening.  
2. Geef de extra rapportdefinitie **Kasrekeningen** voor deze subcategorieën op.  
3. Laat ze inspringen onder de subcategorie **Kas**.  

De volgende keer dat u rapportageschema's genereert, bevat uw saldo-overzicht een totaalsaldo voor kas en twee regels met saldi voor kleine kas en de betaalrekening.  

## <a name="see-also"></a>Zie ook
[Financiën](finance.md)  
[De rekeningschema's instellen of wijzigen](finance-setup-chart-accounts.md)  
[Bedrijfsinformatie](bi.md)  


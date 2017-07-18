---
title: Het grootboek en het rekeningschema
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 9965ddcad214e97c5e4858824395d6f651b3c003
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="the-general-ledger-and-the-chart-of-accounts"></a>Het grootboek en het rekeningschema
In het grootboek worden uw financiële gegevens opgeslagen en het rekeningschema bevat de rekeningen waarnaar alle grootboekposten worden geboekt. Dynamics NAV bevat een standaardrekeningschema dat gereed is om uw bedrijf te ondersteunen.

## <a name="general-ledger-setup-and-general-posting-setup"></a>Grootboekinstellingen en algemene boekingsinstellingen
In de kern van uw bedrijfsprocessen bevindt zich het grootboek en de configuratie van hoe gegevens worden geboekt naar het grootboek.
In het venster **Grootboekinstellingen** kunt u opgeven hoe bepaalde boekhoudkwesties in uw bedrijf worden afgehandeld. Hieronder vallen factuurafrondingsgegevens, adresnotaties en of u een aanvullende rapportagevaluta wilt gebruiken, bijvoorbeeld.
In het venster **Boekingsgroepinstelling** geeft u op dezelfde manier op hoe u combinaties van algemene bedrijfsgroepen en algemene productboekingsgroepen wilt instellen. U vult een regel in voor elke combinatie van bedrijfs- en productboekingsgroep.  

## <a name="the-chart-of-accounts"></a>het rekeningschema
In het rekeningschema worden alle rekeningen weergegeven. Vanuit het rekeningschema kunt u alle rapporten openen waarin uw grootboekposten en -saldi worden weergegeven, en kunt u de resultatenrekening sluiten. Voor alle rekeningen kunt u de grootboekrekeningkaart openen en instellingen toevoegen of wijzigen. U kunt ook een overzicht bekijken van boekingsgroepen die naar die rekening boeken.  

Dynamics NAV voorkomt dat u een grootboekrekening verwijdert die gegevens bevat die nodig zijn in het rekeningschema.  

## <a name="account-categories"></a>Rekeningcategorieën
Met rekeningcategorieën kunt u grootboekrekeningen toewijzen aan categorieën als een aanpassing van de structuur van uw financiële overzichten.  

Het venster **GB-rekeningcategorieën** toont uw bestaande hoofdcategorieën en subcategorieën en de grootboekrekeningen die u aan elke categorie hebt toegewezen. U kunt nieuwe subcategorieën maken en die categorieën toewijzen aan bestaande rekeningen.  

U kunt de rekeningcategorieën groeperen door afzonderlijke subcategorieën in te laten springen. Zo wordt het gemakkelijk voor u om een overzicht te krijgen, omdat elke groepering een totaalsaldo weergeeft. U kunt bijvoorbeeld een subcategorie maken voor verschillende soorten activa en vervolgens categoriegroepen maken voor vaste activa versus huidige activa, bijvoorbeeld. U maakt een categoriegroep door andere subcategorieën onder een regel te laten inspringen in het venster **GB-rekeningcategorieën**.  

Voor elke subcategorie kunt u opgeven of rekeningen van deze categorie in bepaalde soorten financiële rapporten moeten worden opgenomen. De rekeningcategorieën helpen de indeling te definiëren van uw financiële overzichten. Het standaardsaldo-overzicht heeft bijvoorbeeld één post voor contanten onder activa. Als u wilt dat het saldo-overzicht subposten heeft voor kleine kas en uw betaalrekening, kunt u twee nieuwe subcategorieën toevoegen, de aanvullende rapportdefinitie kasrekeningen voor elke categorie opgeven en ze laten inspringen onder de subcategorie Kas. Wanneer u rapportageschema's hebt gegenereerd op basis van uw wijzigingen, bevat uw volgende saldo-overzicht een totaalsaldo voor kas en twee regels met saldi voor kleine kas en de betaalrekening.     

##<a name="see-also"></a>Zie ook
[Financiën](finance-setup.md)  
[De rekeningschema's instellen of wijzigen](finance-setup-setup-chart-accounts.md)  
[Rapportageschema's](finance-setup-account-schedule.md)  


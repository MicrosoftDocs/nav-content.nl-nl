---
title: Gegevens uit Dynamics GP migreren met de extensie Gegevensmigratie
description: Gebruik de Dynamics GP-extensie Gegevensmigratie om klanten, leveranciers, voorraadartikelen en rekeningen te migreren van Dynamics GP naar Dynamics NAV.
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, import, implement
ms.date: 03/29/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 0156ec040b96f007674161361e4368b81f7c42d9
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="the-dynamics-gp-data-migration-extension-for-dynamics-nav"></a>De gegevensmigratie-extensie Dynamics GP voor Dynamics NAV
Met deze extensie kunt u gemakkelijk klanten, leveranciers, voorraadartikelen en accounts vanuit Dynamics GP naar [!INCLUDE[d365fin](includes/d365fin_md.md)] migreren. Als uw bedrijf momenteel Dynamics GP gebruikt, kunt u de relevante masterrecords exporteren en vervolgens een handleiding voor begeleide instelling openen om de gegevens toe te voegen aan [!INCLUDE[d365fin](includes/d365fin_md.md)]. Zie [Bedrijfsgegevens migreren uit andere financiële systemen](upload-data.md) voor meer informatie.

## <a name="exporting-data-from-dynamics-gp"></a>Gegevens exporteren uit Dynamics GP
U moet gegevens van sommige of alle bestaande klanten, leveranciers, voorraadartikelen en rekeningen naar een bestand geëxporteerd hebben door middel van de Dynamics GP-functionaliteit voor gegevensexport. Voor de doelen in [!INCLUDE[d365fin](includes/d365fin_md.md)] kunt u de volgende soorten gegevens exporteren:

* Rekening  
* Klant  
* Artikel  
* Leverancier  

De extensie Dynamics GP Data Migration wijst automatisch de geëxporteerde gegevens toe, zodat de gegevens snel beschikbaar zijn in uw nieuwe [!INCLUDE[d365fin](includes/d365fin_md.md)]-bedrijf. Tijdens het proces worden ondersteunende configuratiegegevens gemaakt, zoals boekingsgroepen. Voorraadartikelen worden in het systeem ingevoerd met FIFO als methode voor kostenwaardering. Rekeningen worden ingesteld als de hoofdrekeningsegment uit Dynamics GP met dimensies, omdat [!INCLUDE[d365fin](includes/d365fin_long_md.md)] geen rekeningsegmenten kent.

## <a name="see-also"></a>Zie ook
[Bedrijfsgegevens importeren uit andere financiële systemen](upload-data.md)  
[[!INCLUDE[d365fin](includes/d365fin_md.md)] aanpassen met behulp van extensies ](ui-extensions.md)  


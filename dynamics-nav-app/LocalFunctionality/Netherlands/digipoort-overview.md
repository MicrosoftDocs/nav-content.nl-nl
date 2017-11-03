---
title: Overzicht van Digipoort
description: In Nederland gebruikt u Digipoort om periodieke elektronische aangiften te maken voor btw-aangiften en ICP-rapporten in EU-verkooplijstverzendingen. Digipoort is het elektronische postkantoor dat door de Nederlandse overheid voor bedrijven wordt geboden.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: fb1e5528bfd3194f776dbeb1a652b36bf06ede70
ms.contentlocale: nl-nl
ms.lasthandoff: 10/23/2017

---
# <a name="digipoort-overview"></a>Overzicht van Digipoort
In Nederland gebruikt u Digipoort om periodieke elektronische aangiften te maken voor btw-aangiften en ICP-rapporten in EU-verkooplijstverzendingen. Digipoort is het elektronische postkantoor dat door de Nederlandse overheid voor bedrijven wordt geboden. Het bevat de gemeenschappelijke infrastructuur voor de communicatie van gegevens tussen bedrijven en de overheid, inclusief btw-aangiftes. De rapporten hebben de XBRL-indeling.  

Het installatieprogramma van [!INCLUDE[navnow](../../includes/navnow_md.md)] installeert de .dll op de volgende locatie: c:Program Files (x86)Microsoft Dynamics NAV<version>RoleTailored ClientAdd-insMicrosoft.Dynamics.NL.Digipoortservice.dll.  

Het Digipoort-kanaal vervangt de BAPI-methode voor het doen van verzendingen.  

## <a name="certificate-storage"></a>Certificaatopslag  
Als u via Digipoort elektronisch wilt communiceren met de Nederlandse overheid, hebt u twee certificaten nodig (PKIoverheid). U hebt een privécertificaat voor het bedrijf nodig en een openbaar certificaat van de website van de Nederlandse belastingdienst. een privécertificaat voor het bedrijf nodig en een openbaar certificaat van de website van de Nederlandse autoriteiten. U kunt meer specifieke informatie van de website van de Nederlandse belastingdienst krijgen. Zie voor meer informatie de website van de Nederlandse belastingdienst[Logius](https://aansluiten.procesinfrastructuur.nl/site/en/).  

U moet de certificaten importeren die u in het certificaatarchief van Windows hebt ontvangen. Dit is een wijziging van eerdere versies, waarin u certificaten in [!INCLUDE[navnow](../../includes/navnow_md.md)] ontving.  

## <a name="see-also"></a>Zie ook  
[Procedure: Certificaten instellen voor gebruik met Digipoort](how-to-set-up-certificates-for-use-with-digipoort.md)


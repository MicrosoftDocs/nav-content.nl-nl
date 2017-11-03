---
title: Certificaten instellen voor gebruik met Digipoort
description: Informatie over Digipoort-certificaten.
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
ms.openlocfilehash: a27bc10b01315b9f5283a6c21d00356696ffcf44
ms.contentlocale: nl-nl
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-set-up-certificates-for-use-with-digipoort"></a>Procedure: Certificaten instellen voor gebruik met Digipoort
In de volgende procedure wordt ervan uitgegaan dat u de certificaten van de overheid hebt ontvangen. Als dat niet zo is, voert u de volgende stappen uit om de certificaten te krijgen.  

- Verkrijg een PKIoverheid-certificaat voor het bedrijf als u er nog geen hebt. Een overzicht van certificaatproviders vindt u hier: [http://www.logius.nl/producten/toegang/pkioverheid/aansluiten/toegetreden-csps](http://www.logius.nl/producten/toegang/pkioverheid/aansluiten/toegetreden-csps).  

- Verkrijg een **Digipoort Service-certificaat**, dat kan worden verkregen van de website van de Nederlandse belastingdienst: <[https://aansluiten.procesinfrastructuur.nl](https://aansluiten.procesinfrastructuur.nl)>.  

- Registreer een gebruiker van Digipoort, wat hier kan: <[https://aansluiten.procesinfrastructuur.nl/site/registratie/nieuw](https://aansluiten.procesinfrastructuur.nl/site/registratie/nieuw)>.  

Nadat u zich hebt geregistreerd en bij de officiële site hebt aangemeld, kunt u de Digiport-servercertificaten van deze website downloaden: <[https://aansluiten.procesinfrastructuur.nl/site/documentatie/certificaten](https://aansluiten.procesinfrastructuur.nl/site/documentatie/certificaten)>.  

Vervolgens moet u de certificaten installeren. De certificaten moeten op de server worden geïnstalleerd. Later gebruikt u de algemene naam (CN) van de certificaten in [!INCLUDE[navnow](../../includes/navnow_md.md)].  

> [!NOTE]  
>  In de Digipoort-implementatie installeert u certificaten op de server. Gebruikers die moeten kunnen communiceren met de belastingdienst via Digipoort, hebben toegang nodig tot de persoonlijke sleutel van het persoonlijke certificaat op de server.  

## <a name="to-install-the-certificates"></a>De certificaten installeren  

1.  Open de **Windows-certificaatconsole** om de certificaten te importeren die u van de overheid hebt ontvangen. Zie voor meer informatie [Procedure: De certificaatconsole gebruiken](http://social.technet.microsoft.com/wiki/contents/articles/2167.how-to-use-the-certificates-console.aspx).  
2.  Importeer de twee certificaten. Zie voor meer informatie [Een certificaat importeren](http://social.technet.microsoft.com/wiki/contents/articles/2167.how-to-use-the-certificates-console.aspx#To_import_certificates).  

    **Persoonlijk certificaat**  

    1.  Kies in de sectie **Persoonlijk** de actie **Importeren**. Zorg dat u de juiste machtigingen instelt voor de persoonlijke sleutel.  
    2.  Voer de **wizard Certificaat importeren** uit.  

    **Servicecertificaat**  

    1.  Kies in de sectie **Vertrouwde uitgevers** de actie **Importeren**  
    2.  Voer de **wizard Certificaat importeren** uit.  

3.  Verleen leesmachtigingen aan het certificaat voor de gebruiker die de verzending doet.  

    Klik met de rechtermuisknop, kies de actie **Alle taken** en kies vervolgens de actie **Persoonlijke sleutels beheren**. Selecteer de gebruiker en schakel in het vak **Machtigingen** het selectievakje **Lezen toestaan** in.  

4.  Sluit het venster **Console**.  

## <a name="see-also"></a>Zie ook  
 [Overzicht van Digipoort](digipoort-overview.md)


---
title: 'Ontwerpdetails: Artikeltracering en reserveringen'
description: In dit onderwerp worden artikeltracering en -reserveringen, en de concepten hierachter beschreven.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b7d9d4763116bf5db5643af658d06ab4f3c264f3
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-item-tracking-and-reservations"></a>Ontwerpdetails: Artikeltracering en reserveringen
Gelijktijdig gebruik van reserveringen en specifieke artikeltracering is ongebruikelijk, aangezien deze beide een koppeling maken tussen voorziening en vraag. Afgezien van situaties waarin een klant of productieplanner om een specifieke lot verzoekt, is het zelden zinvol voorraadartikelen te reserveren die al artikeltraceringsnummers hebben voor een specifieke toepassing. Hoewel het mogelijk is om artikelen te reserveren die specifieke artikeltracering vereisen, is er speciale functionaliteit nodig om beschikbaarheidsconflicten te voorkomen tussen orderverwerkers die om dezelfde artikelgetraceerde artikelen vragen.  
  
Het concept van late binding zorgt dat een niet-specifieke reservering van een serienummer of lotnummer los gekoppeld blijft totdat wordt geboekt. Wanneer wordt geboekt, kan het reserveringsysteem niet-specifieke reserveringen opnieuw plannen zodat vaste vereffening mogelijk is op basis van het serie- en lotnummer dat werkelijk wordt gepickt. Ondertussen wordt het serie- of lotnummer beschikbaar gemaakt voor specifieke reservering in andere documenten die om bepaalde serie- of lotnummers verzoeken.  
  
Een niet-specifieke reservering is een reservering waarbij het de gebruiker niet uitmaakt welk artikel wordt gepickt. Een specifieke reservering is een reservering waarbij het de gebruiker wel uitmaakt.  
  
> [!NOTE]  
>  De functie voor late binding heeft alleen betrekking op artikelen die zijn ingesteld met specifieke artikeltracering, en geldt alleen voor reserveringen voor voorraad, niet voor inkomende orders voor voorzieningen.  
  
De reservering van artikeltraceringsnummers bestaat uit twee categorieën, zoals wordt getoond in de volgende tabel.  
  
|Reservering|Description|  
|-----------------|---------------------------------------|  
|Specifiek|U selecteert een specifiek serie- of lotnummer als u het voorraadartikel uit een vraag reserveert, zoals een verkooporder.<br /><br /> Dit is een normale reservering. Het is een vaste koppeling tussen vraag en aanbod die beide serie- of lotnummers hebben. **Opmerking:** De vraag omvat serie- of lotnummers. <br /><br /> U wilt bijvoorbeeld een blik blauwe verf uit Lot A reserveren omdat de klant erom vraagt. Een blik blauwe verf uit lot A wordt naar de klant verzonden.|  
|Niet specifiek|U selecteert geen specifiek serie- of lotnummer als u het voorraadartikel uit een vraag reserveert, zoals een verkooporder.<br /><br /> Dit is een status die wordt opgelegd voor een reserveringspost voor serie- of lotnummers die niet specifiek zijn ingeschakeld. **Opmerking:** De vraag omvat geen serie- of lotnummers. <br /><br /> U wilt bijvoorbeeld een blik blauwe verf vanuit een lot reserveren voor uw verkooporder. Een blik blauwe verf met een willekeurig serie- of lotnummer wordt naar de klant verzonden.|  
  
Het belangrijkste verschil tussen specifieke en niet-specifieke reserveringen wordt bepaald door het bestaan van serie- of lotnummers aan de vraagkant, zoals in de volgende tabel wordt getoond.  
  
||||  
|-|-|-|  
||**Voorraad**|**Vraag**|  
|**Specifiek**|Serie- of lotnummer.|Serie- of lotnummer.|  
|**Niet specifiek**|Serie- of lotnummer.|Geen serie- of lotnummer.|  
  
Wanneer u voorraadaantallen reserveert van een uitgaande documentregel voor een artikel waaraan artikeltraceringsnummers zijn toegewezen en dat is ingesteld voor specifieke artikeltracering, wordt in het venster **Reservering** verschillende werkstromen getoond afhankelijk van uw behoefte aan de serie- of lotnummers.  
  
## <a name="specific-reservation"></a>Specifieke reservering  
Als u **Reserveren** op de uitgaande documentregel kiest, wordt een dialoogvenster weergegeven waarin wordt gevraagd of u specifieke serie- of lotnummers wilt reserveren. Als u **Ja** kiest, wordt een lijst weergegeven met alle serie- of lotnummers die op de documentregel zijn toegewezen. Het venster **Reservering** wordt geopend nadat u een van de serie- of lotnummers selecteert, en u kunt vervolgens een van de geselecteerde serie- of lotnummers op de gewone manier reserveren.  
  
Als sommige specifieke artikeltraceringsnummers die u probeert te reserveren, in niet-specifieke reserveringen worden vastgehouden, informeert een bericht onder in het venster **Reservering** u hoeveel van het totaal gereserveerde aantal in niet-specifieke reserveringen wordt vastgehouden en of ze nog beschikbaar zijn.  
  
## <a name="nonspecific-reservation"></a>Niet-specifieke reservering  
Als u **Nee** kiest in het dialoogvenster dat verschijnt, wordt het venster **Reservering** geopend en kunt u reserveren uit alle serie- of lotnummers in voorraad.  
  
Wanneer u een niet-specifieke reservering plaatst voor een artikelgetraceerd artikel, moet het systeem vanwege de structuur van het reserveringsysteem specifieke artikelposten selecteren voor de reservering. Omdat de artikelposten artikeltraceringsnummers hebben, reserveert de reservering indirect specifieke serie- of lotnummers, zelfs wanneer dat niet uw bedoeling was. Om deze situatie te verwerken, probeert het reserveringssysteem niet-specifieke reserveringsposten opnieuw te plannen vóór het boeken.  
  
Het systeem reserveert nog steeds tegen specifieke posten, maar gebruikt wel een procedure voor opnieuw plannen wanneer er een bepaalde vraag voor het lot- of serienummer in de niet-specifieke reservering is. Dit is het geval wanneer u een vraagtransactie, zoals een verkooporder, verbruiksdagboek of transferorder boekt voor het serie- of lotnummer, of wanneer u probeert het serie- of lotnummer specifiek te reserveren. Het systeem plant de reserveringen opnieuw zodat het lot- of serienummer beschikbaar is voor de vraag of specifieke reservering. Hierbij wordt een ander lot- of serienummer in de niet-specifieke reservering geplaatst. Als er onvoldoende aantal in voorraad is, plant het systeem zo veel mogelijk opnieuw en krijgt u een beschikbaarheidsfout als er nog steeds onvoldoende aantal is op het moment van boeken.  
  
> [!NOTE]  
>  Op een niet-specifieke reservering is het lotnummer- of serienummerveld leeg in de reserveringspost die naar de vraag verwijst, zoals de verkoop.  
  
## <a name="reshuffle"></a>Opnieuw plannen  
Wanneer een gebruiker een uitgaand document boekt na het picken van het verkeerde serie- of lotnummer, worden andere niet-specifieke reserveringen opnieuw gepland om het werkelijke serie- of lotnummer aan te geven dat is gepickt. Dit biedt de boekingsengine een vaste vereffening tussen voorziening en vraag.  
  
Voor alle ondersteunde bedrijfsscenario's is opnieuw plannen alleen mogelijk voor positieve artikelposten met reservering en serie- of lotnummers, maar zonder gedefinieerde serie- of lotnummers aan de vraagkant.  
  
## <a name="supported-business-scenarios"></a>Ondersteunde bedrijfsscenario's  
De functie voor late binding ondersteunt de volgende bedrijfsscenario's:  
  
* Een specifiek serienummer of lotnummer invoeren op een uitgaand document met niet-specifieke reservering van een verkeerd serie- of lotnummer.  
* Een specifiek serie- of lotnummer reserveren.  
* Een uitgaand document met niet-specifieke reservering van een serie- of lotnummer boeken.  
  
### <a name="entering-serial-or-lot-numbers-on-an-outbound-document-with-wrong-nonspecific-reservation"></a>Serie- of lotnummers invoeren op een uitgaand document met een verkeerde niet-specifieke reservering  
Dit is de meest gangbare van de drie ondersteunde scenario's. In dit geval zorgt de functie Late binding dat een gebruiker een serie- of lotnummer, dat werkelijk wordt gepickt, kan invoeren op een uitgaand document dat al een niet-specifieke reservering van een ander serie- of lotnummer heeft.  
  
Dit is bijvoorbeeld nodig wanneer een orderverwerker eerst een niet-specifieke reservering van een serie- of lotnummer heeft gemaakt. Later, wanneer het artikel werkelijk wordt gepickt uit voorraad, moet het gepickte serie- of lotnummer op de order worden ingevoerd voordat deze wordt geboekt. De niet-specifieke reservering wordt bij het boeken opnieuw gepland om te zorgen dat het gepickte serie- of lotnummer kan worden ingevoerd zonder de reservering te verliezen en te zorgen dat het gepickte serie- of lotnummer volledig kan worden vereffend en geboekt.  
  
### <a name="reserve-specific-serial-or-lot-numbers"></a>Specifieke serie- of lotnummers reserveren  
In dit bedrijfsscenario zorgt de functie Late binding dat een gebruiker die probeert een bepaald serie- of lotnummer te reserveren dat op het moment niet-specifiek is gereserveerd, dat kan doen. Een niet-specifieke reservering wordt opnieuw gepland op het moment van reservering om het serie- of lotnummer voor de specifieke aanvraag vrij te geven.  
  
Het opnieuw plannen wordt automatisch uitgevoerd, maar er wordt ingesloten Help weergegeven onder in het venster **Reservering** met de volgende tekst:  
  
**XX van het totale gereserveerde aantal zijn niet-specifiek en kunnen beschikbaar zijn.**  
  
Daarnaast toont het veld **Niet-specifiek gereserveerd aantal** hoeveel reserveringsposten niet-specifiek zijn. Standaard is dit veld niet zichtbaar voor gebruikers.  
  
### <a name="posting-an-outbound-document-with-nonspecific-reservation-of-serial-or-lot-numbers"></a>Een uitgaand document met niet-specifieke reservering van serie- of lotnummers boeken.  
Dit bedrijfsscenario wordt ondersteund met de functie voor late binding die zorgt voor vaste vereffening en het boeken van uitgaande posten van wat werkelijk is gepickt, door een andere, niet-specifieke reservering van een serie- of lotnummer opnieuw te plannen. Als opnieuw plannen niet mogelijk is, wordt het volgende standaardfoutbericht weergegeven wanneer de gebruiker probeert de verzending boeken:  
  
**Artikel XX kan niet volledig worden vereffend.**  
  
## <a name="see-also"></a>Zie ook  
[Ontwerpdetails: Artikeltracering](design-details-item-tracking.md)

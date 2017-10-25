---
title: Een service voor documentuitwisseling instellen
description: U gebruikt een externe serviceprovider om elektronische documenten uit te wisselen met uw handelspartners.
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/18/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3f5fe8fc4c14e63b54ee0dce34278f2f13535265
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-a-document-exchange-service"></a>Procedure: Een service voor documentuitwisseling instellen
U gebruikt een externe serviceprovider om elektronische documenten uit te wisselen met uw handelspartners. Zie [Gegevens elektronische uitwisselen](across-data-exchange.md) voor meer informatie.  

## <a name="to-set-up-a-document-exchange-service"></a>Een service voor documentuitwisseling instellen  
1. Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Instellingen service doc.uitw.** in en klik op de gerelateerde koppeling.  
2. Vul de velden in zoals beschreven in de volgende tabel.  

    |Veld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Gebruikersagent**|Voer elke willekeurige tekst in die kan worden gebruikt om uw bedrijf te identificeren in processen voor documentuitwisseling.|  
    |**Tenant-id doc.uitw.**|Voer de tenant in de service voor documentuitwisseling in die uw bedrijf vertegenwoordigt. Deze wordt geleverd door de aanbieder van de service voor documentuitwisseling.|  
    |**Ingeschakeld**|Geef op of de service is ingeschakeld. **Opmerking:** zodra u de service inschakelt, worden ten minste twee taakwachtrijposten gemaakt om het verkeer van elektronische documenten naar en vanuit [!INCLUDE[d365fin](includes/d365fin_md.md)] te verwerken. Wanneer u de service uitschakelt, worden de taakwachtrijposten verwijderd.|  
    |**Registratie-URL**|Geef de webpagina op waarop u zich aanmeldt voor de service voor documentuitwisseling.|  
    |**Service-URL**|Geef het adres op van de service voor documentuitwisseling die wordt aangeroepen wanneer u elektronische documenten verzendt en ontvangt.|  
    |**Aanmelden**|Geef de aanmeldpagina op voor de service voor documentuitwisseling. Dit is de pagina waarop u de gebruikersnaam en het wachtwoord van uw bedrijf invoert om aan te melden bij de service.|  
    |**Consumentsleutel**|Voer de 3 legged sleutel voor OAuth voor de consumentsleutel in. Deze wordt geleverd door de aanbieder van de service voor documentuitwisseling.|  
    |**Consumentgeheimsleutel**|Voer het geheim in dat de consumentsleutel beveiligt. Deze wordt geleverd door de aanbieder van de service voor documentuitwisseling.|  
    |**Token**|Voer de 3 legged sleutel voor OAuth voor het token in. Deze wordt geleverd door de aanbieder van de service voor documentuitwisseling.|  
    |**Tokengeheim**|Voer het geheim in dat het token beveiligt. Deze wordt geleverd door de aanbieder van de service voor documentuitwisseling.|  

> [!NOTE]  
>  We raden u aan de aanmeldgegevens te beveiligen die u invoert in het venster **Instellingen van VAN-service**. U kunt gegevens op de server versleutelen door nieuwe encryptiesleutels te genereren of bestaande sleutels te importeren die u inschakelt op de serverinstantie die verbinding maakt met de database. Dit wordt in de volgende procedure beschreven.  

## <a name="to-encrypt-your-logon-information"></a>Uw aanmeldgegevens versleutelen  
1. Kies in het venster **Instellingen van VAN-service** de actie **Versleutelingsbeheer**.  
2. Schakel in het venster **Beheer gegevensversleuteling** versleuteling van uw gegevens in. <!--For more information, see [Manage Data Encryption](../manage-data-encryption.md).-->  

## <a name="see-also"></a>Zie ook  
[Gegevensuitwisseling instellen](across-set-up-data-exchange.md)  
[Gegevens elektronisch uitwisselen](across-data-exchange.md)


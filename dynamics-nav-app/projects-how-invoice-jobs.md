---
title: 'Procedure: Projecten factureren'
author: SorenGP
ms.custom: na
ms.date: 11/01/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: c0dcce83dfba30af38f33a6bf814b15862d5fc19
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-invoice-jobs"></a>Procedure: Projecten factureren
Tijdens het project kunnen projectkosten van resourceverbruik, materialen en aan het project gerelateerde inkopen, zich ophopen. Naarmate het project vordert, worden deze transacties geboekt in het projectdagboek. Het is van belang dat alle kosten worden vastgelegd in het projectdagboek voordat u het project aan de klant factureert.

U kunt het hele project factureren vanuit het venster **Projecttaakregels** of alleen de geselecteerde factureerbare regels factureren vanuit het venster **Planningsregels**. Facturering kan plaatsvinden nadat het project is voltooid of op bepaalde intervallen tijdens de voortgang van het project op basis van een factureringsschema.

**Opmerking**: als u **Factureerbaar** selecteert in het veld **Regelsoort project** in de inkoopdocumenten voor aan het project gerelateerde inkopen, worden projectplanningsregels gemaakt die gereed zijn om te worden gefactureerd aan de klant. Zie [Procedure: Projectvoorraden beheren](projects-how-manage-project-supplies.md) voor meer informatie.

## <a name="to-create-and-post-a-job-sales-invoice"></a>Een projectverkoopfactuur maken en boeken  
U kunt een factuur maken voor een project of voor één of meer projecttaken voor een klant, wanneer ofwel het werk dat moet worden gefactureerd voltooid is ofwel de datum voor facturering op basis van een factureringsschema is bereikt.

Vanuit het venster **Projecten** kunt u een klant factureren door het project te selecteren en vervolgens de actie **Projectverkoopfactuur maken** te kiezen. In de volgende procedure wordt beschreven hoe u een batchverwerking gebruikt om meerdere projecten te factureren.  

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Verkoopfactuur project maken** in en kies vervolgens de gerelateerde koppeling.  
2. Vul indien nodig de velden in. Kies een veld om een korte omschrijving van het veld of een koppeling naar meer informatie te lezen.
3. Stel filters in als u de projecten wilt beperken die door de batchverwerking worden verwerkt.
3. Kies de knop **OK** om de facturen te maken.  

## <a name="to-create-multiple-job-sales-invoices-from-job-planning-lines"></a>Meerdere projectverkoopfacturen maken vanuit projectplanningsregels  
U kunt een factuur maken vanuit een projectplanningsregel en op dat moment de hoeveelheid van het artikel, resource of grootboekrekening die u wilt factureren, aangeven.

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Projecten** in en kies vervolgens de gerelateerde koppeling.
2. Open het betreffende project.
3. Selecteer een projecttaak waarvoor **Boeking** de **projecttaaksoort** is, en kies vervolgens de actie **Projectplanningsregels**.  
4. Voer op een projectplanningsregel in het veld **Aantal te verplaatsen naar factuur** de hoeveelheid van het artikel, de resource en het soort grootboekrekening dat u wilt factureren in.  
5. Kies de actie **Verkoopfactuur maken**.
6. Voer in het venster **Verkoopfactuur project maken** de boekingsdatum in en of u een nieuwe factuur wilt maken of toevoegen aan deze factuur of aan een bestaande factuur.
7. Kies de knop **Ok**.

    Op de projectplanningsregel, in het veld **Aantal overgebracht naar factuur** ziet u de hoeveelheid.

8. Kies in het venster **Projectplanningsregels** de actie **Verkoopfacturen/-creditnota's**.

    Het venster **Verkoopfactuur** wordt geopend met het aantal dat u naar de factuur hebt verzonden.  
9. Breng eventuele aanvullende wijzigingen aan en kies vervolgens de actie **Boeken**.

**Opmerking**: de bovengenoemde procedure is soortgelijk voor het maken, controleren en boeken van een aan een project gerelateerde verkoopcreditnota.

## <a name="to-calculate-and-post-job-completion-entries"></a>Projectvoltooiingsposten berekenen en boeken  
Wanneer u alle activiteiten voor een project hebt uitgevoerd, waaronder gebruiksboekingen en -facturering, moet u het project bijwerken om de **Status** in te stellen op **Voltooid**. Vervolgens moet u eventueel OHW tegenboeken dat naar het grootboek is geboekt.

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Projecten** in en kies vervolgens de gerelateerde koppeling.  
2. Selecteer een open project en kies vervolgens de actie **Bewerken**.
3. Selecteer in het veld **Status** de optie **Voltooid**.
4. Volg de hulpstappen om OHW te berekenen en te boeken. Of volg stap 5 en 6 om dit handmatig te doen.  
5. Kies de actie **OHW berekenen**.
6. Vul in het venster **OHW voor project berekenen** indien nodig de velden in.  

     De OHW-posten voor het project die worden gemaakt door het uitvoeren van de batchverwerking, hebben nu een vinkje in het selectievak **Project voltooid** om aan te geven dat het voltooiingsposten zijn.  

7. Kies de actie **Project-OHW naar GB boeken**.
8. Vul in het venster **Project-OHW naar GB boeken** indien nodig de velden in.  

     De OHW-grootboekposten voor het project die worden gemaakt door het uitvoeren van de batchverwerking hebben nu een vinkje in het selectievak **Project voltooid** om aan te geven dat het voltooide posten zijn.

## <a name="see-also"></a>Zie ook
[Projecten beheren](projects-manage-projects.md)  
[Financiën](finance-setup.md)  
[Inkoop beheren](purchasing-manage-purchasing.md)         
[Verkoop beheren](sales-manage-sales.md)      
[Werken met Dynamics NAV](ui-work-product.md)  


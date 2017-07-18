---
title: Sales tax en belastinggroepen in de VS en Canada
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
ms.openlocfilehash: f70a191fc8392bf1685c08c7e905ac96ba7ed069
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="sales-tax-and-tax-groups-in-the-us-and-canada"></a>Sales tax en belastinggroepen in de VS en Canada
Wanneer u voor het eerst gaat werken met project Dynamics NAV, kunt u een handleiding voor begeleide instelling uitvoeren om snel en gemakkelijk btw-gegevens voor uw bedrijf en optioneel voor uw klanten en leveranciers in te stellen. In enkele minuten bent u gereed om verkoopdocumenten en inkoopdocumenten te maken waarvoor de btw correct is berekend.
Als u naar het lege Mijn bedrijf gaat, is het raadzaam dat u elke handleiding voor begeleide instelling gaat gebruiken, inclusief de handleiding voor btw. Als u btw liever zelf instelt, wordt in dit artikel uitgelegd waarmee u rekening moet houden.  

## <a name="tax-groups-tax-areas-and-tax-jurisdictions"></a>Belastinggroepen, belastinggebieden en belastingjurisdicties
In Dynamics NAV staat een belastinggroep voor een groep voorraadartikelen of resources waarop identieke belastingvoorwaarden van toepassing zijn. U kunt bijvoorbeeld een belastinggroep instellen voor belastbare artikelen en een andere belastinggroep voor niet-belastbare artikelen. U moet belastinggroepscodes toewijzen aan voorraadartikelen en grootboekrekeningen. Op dezelfde manier moet u belastinggebiedcodes toewijzen aan klanten, locaties en aan uw eigen bedrijfsinstellingen. De handleiding voor begeleide instelling helpt u hierbij.  

Elk belastinggebied is een groepering van btw-jurisdicties die zijn gebaseerd op een bepaalde geografische locatie. Het belastinggebied Miami, Florida, bevat bijvoorbeeld drie btw-jurisdicties: plaats (Miami) county (Dade) en provincie (Florida). Dynamics NAV bevat een beperkte set belastinggebieden met een standaardconfiguratie, maar u kunt deze wijzigen en nieuwe belastinggebieden toevoegen.  

Als u de tax area's en belastingjurisdicties instelt, moet u ervoor zorgen dat u de velden correct invult. In de Verenigde Staten kunnen staten, county's, steden en districten btw heffen. In Canada kan de federale overheid en de provincies btw heffen. Bedrijven innen btw en dragen deze af aan overheidsinstanties voor producten die zijn verkocht aan eindgebruikers. Btw kan ook worden berekend over bestaande btw. Belasting kan bijvoorbeeld worden berekend over een verkoopfactuurbedrag dat reeds de belasting van andere jurisdicties bevat.  

In Canada moeten belastingbedragen gedetailleerd worden beschreven in documenten voor elke belastingjurisdictie. Maximaal vier jurisdicties kunnen worden weergegeven in een document en jurisdicties met dezelfde afdrukvolgorde worden gecombineerd wanneer ze worden afgedrukt.

## <a name="tax-details"></a>Belastingdetails
In het venster **Belastingdetails** worden verschillende combinaties weergegeven van btw-jurisdicties en btw-groepen om btw-tarieven in te stellen. Voor elke belastingjurisdictie is het raadzaam dat u één belastinggroep instelt voor normale btw, een andere belastinggroep voor artikelen of services die niet worden belast en een extra belastinggroep voor elk type artikel of service met een ander btw-tarief in die jurisdictie.  

Wanneer u in de Verenigde Staten verkoopt aan een klant op een locatie waar u geen *situs* hebt, of een juridische locatie in die provincie, int u geen btw. Voor locaties waarin u geen situs hebt, moet u ervoor zorgen dat de beiden velden **Belasting onder minimum** en **Belasting boven maximum** 0,00 zijn.  

## <a name="see-also"></a>Zie ook
[Financiën](finance-setup.md)  
[Financiering instellen](finance-setup-setup-finance-setup.md)  
[Sales tax en goederen en services in Canada](ca-finance-setup-tax.md)  
[Btw-instellingen gemakkelijk gemaakt](https://madeira.microsoft.com/en-us/blog/sales-tax-setup-made-easy)  


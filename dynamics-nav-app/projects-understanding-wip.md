---
title: OHW-methoden
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
ms.openlocfilehash: f21357897dd730d96db7abab469d5958c6fe117c
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="understanding-wip-methods"></a>OHW-methoden

Dynamics NAV ondersteunt de volgende methoden om de waarde van onderhanden werk te berekenen en vast te leggen.

|OHW-methode |Berekeningsformule |Omschrijving van berekening|
|-----------|--------------------|-----------------------|
|Kostenwaarde|Verantwoorde omzet = Factureerbaar (gefactureerde prijs)<br /><br /> Geschatte totale kostprijs = Factureerbaar (totale prijs) x Budgetkostenverhouding<br /><br /> OHW-kosten = \(Voltooiingspercentage - Gefactureerd %\) x Geschatte totale kosten<br /><br /> Voltooiingspercentage = Gebruik (totale kostprijs) / Budget (totale kostprijs)<br /> Gefactureerd % = Factureerbaar (gefactureerde prijs)<br /><br /> Factureerbare verantwoorde kosten (totale kosten) = Gebruik (totale kosten) - OHW|Het berekenen van de kostenwaarde wordt gestart door de waarde te berekenen van wat er is aangeleverd, door een deel van de geschatte totale kosten op basis van percentage voltooid te nemen. De gefactureerde kosten worden afgetrokken door een deel van de geschatte totale kosten op basis van het gefactureerde percentage te nemen.<br /><br /> Voor deze berekening moeten de factureerbare totale prijs, de totale budgetprijs en de totale budgetkosten correct worden ingevoerd voor het hele project.|
|Kosten van verkoop|Verantwoorde omzet = Factureerbaar (gefactureerde prijs)<br /><br /> Verantwoorde kosten = Budget (totale kostprijs) x Gefactureerd percentage<br /><br /> Gefactureerd % = Factureerbaar (gefactureerde prijs) / Factureerbaar (totale prijs)<br /><br /> \(Gefactureerd % is een kolom op projecttaakregels\)<br /><br /> OHW-kosten = Gebruik (totale kosten) - Verantwoorde kosten|Het berekenen van de kosten van de verkoopprijs wordt gestart door de verantwoorde kosten te berekenen. Kosten worden proportioneel verantwoord op basis van totale budgetkosten.<br /><br /> Voor deze berekening moeten de factureerbare totale prijs en de totale budgetkosten correct worden ingevoerd voor het hele project.|
|Verkoopwaarde|Verantwoorde kosten = Gebruik (totale kosten)<br /><br /> Verantwoorde omzet = Gebruik (totale verkoopprijs) x Verwachten factuurverhouding<br /><br /> Kosten-recovery % = Factureerbaar (totale prijs) / Budget (totale prijs)<br /><br /> OHW-omzet = Verantwoorde omzet - Factureerbaar (gefactureerde prijs)|Bij het berekenen van de verkoopprijs wordt de omzet proportioneel verantwoord op basis van de totale kosten van het gebruik en de verwachte kosten van de recovery-verhouding.<br /><br /> Voor deze berekening moeten de factureerbare kostprijs en de totale budgetprijs correct worden ingevoerd voor het hele project.|
|Percentage van voltooiing|Verantwoorde kosten = Gebruik (totale kosten)<br /><br /> Verantwoorde omzet = Factureerbaar (totale prijs) x Voltooiingspercentage<br /><br /> Voltooiingspercentage = Gebruik (totale kostprijs) / Budget (totale kostprijs)<br /><br /> \(Wordt 'Taakvoltooing %' genoemd op projecttaakregels\)<br /> OHW-omzet = Verantwoorde omzet - Factureerbaar (gefactureerde prijs)|Bij het berekenen van het voltooiingspercentage worden inkomsten proportioneel verantwoord op basis van het percentage voltooid, dat wil zeggen de totale kosten van het gebruik versus de budgetkosten.<br /><br /> Voor deze berekening moeten de factureerbare totale prijs en de totale budgetkosten correct worden ingevoerd voor het hele project.|
|Voltooid contract|OHW-bedrag = Totale OHW-kosten = Gebruik \(totale kostprijs\)<br /><br /> Omzet OHW = Factureerbaar \(gefactureerde prijs\)|Bij Contract voltooid worden de inkomsten en de kosten pas verantwoord als het project is voltooid. U kunt hiervoor kiezen als de geschatte kosten en inkomsten van het project nog niet zeker zijn.<br /><br /> Al het gebruik wordt op de rekening OHW-kosten \(activum\) geboekt, terwijl alle gefactureerde omzet op de rekening gefactureerde omzet OHW \(passief\) wordt geboekt totdat het project is voltooid.|

## <a name="see-also"></a>Zie ook
[Projecten beheren](projects-manage-projects.md)  
[Financiën](finance-setup.md)  
[Inkoop beheren](purchasing-manage-purchasing.md)         
[Verkoop beheren](sales-manage-sales.md)      
[Werken met Dynamics NAV](ui-work-product.md)  


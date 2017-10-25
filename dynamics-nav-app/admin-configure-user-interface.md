---
title: Het configureren van de gebruikersinterface voor gebruikers
description: Als beheerder configureert u de standaardgebruikersinterfaces van het bedrijf door pagina-indelingen aan te passen voor verschillende gebruikersprofielen in het bedrijf.
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize pages, configure user interface, customize UI
ms.date: 07/01/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7ba3d45a856eb38fe99fc5012b4e2f2d8609f9ce
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="configuring-the-user-interface-ui-for-users"></a>Het configureren van de gebruikersinterface voor gebruikers
Als beheerder configureert u de standaardgebruikersinterfaces van het bedrijf door pagina-indelingen aan te passen voor verschillende gebruikersprofielen in het bedrijf. Om dit werk uit te voeren, moet u een beheerder zijn met de machtigingenset SUPER. Bovendien moeten profielen worden ingesteld en moeten er de juiste gebruikers aan worden toegewezen. Zie [Gebruikers, profielen en rolcentra beheren](admin-users-profiles-roles.md) voor meer informatie.  
  
U configureert de gebruikersinterface voor meerdere gebruikers door pagina's aan te passen voor een bepaald profiel waaraan de gebruikers zijn toegewezen. Gebruik hiervoor [!INCLUDE[nav_windows](includes/nav_windows_md.md)] en door het doorvoeren van aanpassingen op dezelfde manier waarop individuele gebruikers hun eigen werkruimten aan hun persoonlijke voorkeuren aanpassen, met behulp van de functie **Aanpassen**. Het verschil is dat u [!INCLUDE[nav_windows](includes/nav_windows_md.md)] in de configuratiemodus opent. Veelvoorkomende aanpassingen omvatten welke acties moeten worden opgenomen op het lint, hoe velden op sneltabbladen of in feitenblokken worden geplaatst en welke menu-items worden opgenomen in het navigatiedeelvenster. 

> [!TIP]  
>  Een snelle manier om configuraties voor de gebruikersinterface voor een profiel te implementeren is als u al een geconfigureerd profiel in een andere [!INCLUDE[d365fin](includes/d365fin_md.md)]-database hebt. U kunt dat profiel exporteren en vervolgens importeren in de huidige database. Zie [Profielen exporteren en importeren](admin-profiles.md#ExportImportProfile).  
  
## <a name="general-information"></a>Algemene informatie
Houd rekening met het volgende voordat u de gebruikersinterface gaat configureren:
-   Voordat u begint de gebruikersinterface te configureren, kan de toepassing zijn geconfigureerd om gebruikersinterface-elementen weer te geven en te verbergen (zoals velden, sneltabbladen en feitenblokken) op basis van licenties of machtigingen van de gebruiker. Zie voor meer informatie over hoe u dit moet doen [Elementen uit de gebruikersinterface verwijderen op basis van machtigingen](https://msdn.microsoft.com/en-us/dynamics-nav/removing-elements-from-the-user-interface-according-to-permissions).

    Om het effect te zien van de optie Verwijdering UI-elementen, kunt u zich als testgebruiker aanmelden met de machtigingenset van het profiel dat u configureert. De reden is dat u als beheerder de machtigingenset SUPER hebt en u daarom niet de resulterende gebruikersinterface kunt controleren tijdens uw eigen aanmelding.    
-   Wanneer u wijzigingen aanbrengt in de gebruikersinterfaceconfiguratie voor een pagina die een gebruiker heeft gepersonaliseerd, blijft de gebruikersinterfacepersonalisatie van de gebruiker behouden en wordt deze niet overschreven door de nieuwe paginaconfiguratie. Wanneer u de UI-configuratie annuleert van een pagina die een gebruiker sindsdien heeft gepersonaliseerd, wordt de UI-personalisatie van de gebruiker ook niet geannuleerd.
-   De enige situatie waarin de UI-configuratie de aangepaste UI overschrijft, is wanneer een UI-element wordt verwijderd door de configuratie. Als de beheerder bijvoorbeeld een veld verwijdert dat de gebruiker heeft hernoemd of verplaatst, wordt het veld toch verwijderd uit de gebruikersinterface van de gebruiker.
-   U kunt gebruikersinterfaceconfiguraties van dezelfde pagina vastleggen op basis van verschillende toegangspunten naar de pagina. Het venster **Verkooporders** kan bijvoorbeeld worden aangepast zodat het er anders uitziet wanneer het wordt geopend vanuit het venster **Klantkaart** dan wanneer het wordt geopend vanuit het Rolcentrum **Verkooporderverwerker**. Het punt van waaruit u de pagina opent die moet worden aangepast, wordt vastgelegd in die specifieke pagina-aanpassing. Er kunnen meerdere pagina-aanpassingsrecords in de database zijn, zoals u kunt zien in het venster **Profielconfiguratie verwijderen**.  
-   In tegenstelling tot wanneer gebruikers de grootte van vensters of de breedte van kolommen op hun eigen computer wijzigen, worden dergelijke wijzigingen in de basisweergave die u tijdens de configuratie van de gebruikersinterface voor een profiel maakt, niet opgeslagen in het profiel en zijn niet beschikbaar voor gebruikers die aan het profiel zijn toegewezen. Elementaire weergavewijzigingen zijn computerspecifiek.   

## <a name="configure-a-profile-with-the-includenavwindowsincludesnavwindowsmdmd-in-configuration-mode"></a>Een profiel configureren met [!INCLUDE[nav_windows](includes/nav_windows_md.md)] in de configuratiemodus
1.  Open een opdrachtprompt en typ de volgende opdracht om naar de installatiemap van [!INCLUDE[nav_windows](includes/nav_windows_md.md)] te gaan. Voorbeeld:  
  
    ```  
    cd C:\Program Files\(x86)\Microsoft Dynamics NAV\110\RoleTailored Client  
    ```  
  
2.  Typ de volgende opdracht om [!INCLUDE[nav_windows](includes/nav_windows_md.md)] in de configuratiemodus te starten voor een bepaald profiel:  
  
    ```  
    Microsoft.Dynamics.Nav.Client.exe -configure -profile:"profileid"  
    ```  
  
     Vervang **profileid** door de naam van het profiel dat u wilt configureren.  
  
     Als u bijvoorbeeld het profiel Administrateur wilt configureren, gebruikt u deze opdracht:  
  
    ```  
    Microsoft.Dynamics.Nav.Client.exe -configure -profile:"Accounting Manager"  
    ``` 

3. U kunt nu beginnen met het configureren van de gebruikersinterface. Dit gaat op dezelfde manier in zijn werk als afzonderlijke gebruikers die hun eigen werkruimten aanpassen. Zie [Uw werkruimte personaliseren in [!INCLUDE[nav_windows](includes/nav_windows_md.md)]](ui-personalization-windows-client.md). 

## <a name="cancel-ui-configuration"></a>Gebruikersinterfaceconfiguratie annuleren
U kunt UI-aanpassingen die u in de configuratie voor een profiel hebt aangebracht, op drie manieren annuleren:  
  
-   Annuleer alle UI-aanpassing die u voor een profiel hebt aangebracht met de knop **Geconfigureerde pagina's wissen** in het venster **Profielkaart**.  
  
-   Annuleer UI-aanpassing die u voor specifieke pagina's voor een profiel hebt aangebracht door rijen te verwijderen in het venster **Profielconfiguratie verwijderen**.  
  
-   Annuleer UI-aanpassing die u voor een bepaald UI-gebied voor een bepaalde pagina voor een profiel hebt aangebracht met de knop **Standaardwaarden herstellen** in het venster **Aanpassen**.  
  
### <a name="general-information"></a>Algemene informatie  
-   Gebruikers kunnen UI-aanpassingen onder hun eigen gebruikersaanmelding maken om hun gebruikersinterface persoonlijker te maken. Wanneer u de UI-configuratie annuleert van een pagina die een gebruiker sindsdien heeft gepersonaliseerd, wordt de UI-personalisatie van de gebruiker niet geannuleerd. Wanneer u een nieuwe UI-configuratie maakt voor een pagina die een gebruiker heeft gepersonaliseerd, blijft de UI-personalisatie van de gebruiker behouden en wordt deze niet overschreven door de nieuwe paginaconfiguratie.  

    De enige situatie waarin de UI-configuratie de aangepaste UI overschrijft, is wanneer een UI-element wordt verwijderd door de configuratie. Als de beheerder bijvoorbeeld een veld verwijdert dat de gebruiker heeft hernoemd of verplaatst, wordt het veld toch verwijderd uit de gebruikersinterface van de gebruiker.  
  
-   In het venster **Pers. gebruikersinstellingen verwijderen** en met de knop **Standaardwaarden herstellen** in het venster **Aanpassen** kunnen gebruikers UI-aanpassing annuleren die ze in pagina's hebben aangebracht onder hun eigen gebruikersaanmelding. Wanneer ze dit doen, wordt de indeling van deze pagina's opnieuw ingesteld op alle UI-aanpassingen die de beheerder heeft geconfigureerd voor het profiel. Als het profiel niet is geconfigureerd, wordt de indeling van de pagina's van de gebruiker opnieuw ingesteld op de standaardprofielconfiguratie. Zie [Personalisatie annuleren](ui-personalization-windows-client.md#CancelPersonalization) voor meer informatie over hoe gebruikers aanpassingen kunnen annuleren.
  
### <a name="to-cancel-all-ui-customization-that-you-have-made-for-a-profile"></a>Alle aanpassingen van de gebruikersinterface annuleren die u hebt gemaakt voor een profiel  
  
1.  Voer in het tekstvak **Zoeken** **Profielen** in en kies vervolgens de gerelateerde koppeling.  
  
2.  Selecteer het profiel waarvoor u alle aanpassingen van de gebruikersinterface wilt annuleren en kies op het tabblad **Start** in de groep **Beheren** de optie **Bewerken**.  
  
3.  Kies in het venster **Profielkaart** op het tabblad **Acties** in de groep **Functies** de optie **Geconfigureerde pagina's wissen**.  
  
> [!NOTE]  
>  Alle gebruikersinterfaceaanpassingen voor het profiel, zowel geïnstalleerd met de toepassing als aangebracht door de beheerder, worden geannuleerd. Er zijn geen voor het profiel specifieke pagina-indelingen meer in de database.  
  
### <a name="to-cancel-ui-customization-that-you-have-made-for-specific-page-for-a-profile"></a>Aanpassingen van de gebruikersinterface annuleren die u hebt gemaakt voor een specifieke pagina voor een profiel  
  
1.  Voer in het vak **Zoeken** de tekst **Profielconfiguratie verwijderen** in en kies vervolgens de gerelateerde koppeling.  
  
2.  Selecteer de profiel-/paginacombinatie waarvoor u de aanpassing van de gebruikersinterface wilt annuleren en kies op het tabblad **Start** in de groep **Beheren** de optie **Verwijderen**.  
  
    > [!IMPORTANT]  
    >  Als u verschillende UI-aanpassingen van dezelfde pagina hebt geconfigureerd in verschillende navigatiepaden naar de pagina, wordt elke pagina-aanpassing in het venster **Profielconfiguratie verwijderen** met dezelfde gegevens weergegeven. Er is geen informatie om te bepalen welke rij betrekking heeft op welk navigatiepad. U moet daarom of rijen één voor één verwijderen, gevolgd door een visuele controle van de pagina, of u kunt alle rijen verwijderen met UI-aanpassingen voor het profiel/de pagina.
    >    
    >  Alle UI-aanpassing voor de pagina voor het profiel die u ooit in de installatie hebt aangebracht, of sinds u voor het laatst het venster **Profielconfiguratie verwijderen** hebt gebruikt, wordt geannuleerd. De indeling van de pagina wordt hersteld naar de standaardindeling van het paginaobject.  
  
### <a name="to-cancel-ui-customization-that-you-have-made-for-a-specific-ui-area-for-a-specific-page-for-a-profile"></a>Aanpassingen van de gebruikersinterface annuleren die u hebt gemaakt voor een specifiek UI-gebied voor een specifieke pagina voor een profiel  
  
U kunt wijzigingen ongedaan maken voor individuele UI-gebieden, zoals een lint, met de knop **Standaardwaarden herstellen** in het venster **Aanpassen**. U kunt ook alle UI-veranderingen die u voor een profiel hebt aangebracht, ongedaan maken met behulp van het venster **Profielconfiguratie verwijderen**.  
  
De aanpassing van de gebruikersinterface voor het profiel van het betreffende UI-gebied op de specifieke pagina wordt geannuleerd. De indeling van het gebruikersinterfacegebied (UI-gebied) op de pagina wordt hersteld naar de standaardconfiguratie voor uw profiel, zoals ingesteld door de beheerder of zoals geïnstalleerd met de toepassing.  
  
## <a name="see-also"></a>Zie ook  
[Aanpassen [!INCLUDE[navnow_md](includes/navnow_md.md)]](ui-customizing-overview.md)   

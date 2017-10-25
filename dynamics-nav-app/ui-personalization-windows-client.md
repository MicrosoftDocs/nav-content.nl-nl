---
title: Het personaliseren van pagina's in de Dynamics Windows-client
description: Meer informatie over hoe u de gebruikersinterface kunt aanpassen aan uw manier van werken.
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 07/26/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 12aee74950066647f61639ec88c47e9be3c2f172
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="personalizing-your-workspace-in-the-dynamics-windows-client"></a>Uw werkruimte personaliseren met behulp van de Dynamics Windows-client
U kunt uw werkruimte aanpassen aan uw werk- en persoonlijke voorkeuren, door pagina's te wijzigen zodat deze alleen de gegevens weergeven die u nodig hebt en waar u die nodig hebt. De personalisatiewijzigingen die u maakt, hebben alleen effect op wat u ziet, niet wat andere gebruikers kunnen zien. U kunt veel onderdelen van de gebruikersinterface (UI) aanpassen, zoals welke acties moeten worden opgenomen op het lint, hoe velden op sneltabbladen of in feitenblokken worden geplaatst en welke menu-items worden opgenomen in het navigatiedeelvenster.

> [!NOTE]  
> U kunt ook pagina´s ook personaliseren met behulp van [!INCLUDE[nav_web_md](includes/nav_web_md.md)]. Zie [Overzicht personalisatie](ui-personalization-overview.md) voor meer informatie over hoe dit werk voor de twee clients.
 
## <a name="how-to-personalize-your-workspace"></a>Uw werkruimte personaliseren
De meeste taken voor het personaliseren van uw werk doet u met de functie **Aanpassen**, die vanaf bijna alle pagina´s kan worden gebruikt door het volgende te doen:

1.  Open de pagina die u wilt personaliseren.
2.  Selecteer linksboven het menu **Toepassing** ![knop van menu Toepassing op menubalk](media/applicationmenuicon.png "ApplicationMenuIcon")-pictogram, selecteer **Aanpassen** en selecteer een van de volgende aanpassingsopties.

Er zijn ook een aantal basiswijzigingen in de gebruikersinterface, zoals het aanpassen van de grootte van elk venster of het verbreden van de kolommen, dat u direct op de pagina, buiten de optie **Aanpassen** uitvoert.

## <a name="general-information"></a>Algemene informatie
Bij het aanpassen van de gebruikersinterface, moet het volgende in gedachte houden: 

-   U kunt meerdere aanpassingen van dezelfde pagina vastleggen op basis van verschillende toegangspunten naar de pagina. Het venster Verkooporders kan bijvoorbeeld worden aangepast zodat het er anders uitziet wanneer het wordt geopend vanuit het venster Klantkaart dan wanneer het wordt geopend vanuit het Rolcentrum Verkooporderverwerker. Het punt van waaruit u de pagina opent die moet worden aangepast, wordt vastgelegd in die specifieke pagina-aanpassing. Er kunnen meerdere pagina-aanpassingsrecords in de database zijn, zoals u kunt zien in het venster **Pers. gebruikersinstellingen verwijderen**.

-   De toepassing kan zijn geconfigureerd om gebruikersinterface-elementen weer te geven en te verbergen (zoals velden, sneltabbladen en feitenblokken) op basis van uw licenties of machtigingen. U kunt alleen elementvelden zien en aanpassen waarvoor u gemachtigd bent.

## <a name="customize-ribbons"></a>Lintsn aanpassen
Het lint biedt toegang tot diverse acties. U kunt het lint aanpassen om werkprocessen en voorkeuren te optimaliseren. Als u bijvoorbeeld vaak het venster **Afmetingen** gebruikt, kunt u de actie **Afmetingen** toevoegen aan de actiegroep **Verwerken**. U kunt ook acties die u nooit gebruikt, verwijderen voor een beter overzicht.  
  
U kunt de volgende taken uitvoeren om linten op pagina's aan te passen:  
  
-   Toevoegen, hernoemen of verwijderen van tabbladen, groepen, acties en menu's.  
-   De volgorde van acties wijzigen.  
-   Het lint op de standaardinstelling herstellen.  
  
### <a name="to-customize-a-ribbon"></a>U kunt een lint als volgt aanpassen
1. Open de pagina die u wilt wijzigen.
2. Kies linksboven het menu **Toepassing** ![knop van menu Toepassing op menubalk](media/applicationmenuicon.png "ApplicationMenuIcon")-pictogram, selecteer  **Aanpassen** en kies vervolgens **Lint aanpassen**.

Het dialoogvenster **Acties in het lint ordenen** is onderverdeeld in twee deelvensters. Het deelvenster **Beschikbare acties** bevat alle acties die u aan de pagina kunt toevoegen. Het deelvenster **Acties in deze volgorde weergeven** geeft de structuur weer van alle acties die momenteel op de pagina worden weergegeven.

-   Items op het niveau van de hoofdmap bepalen de tabbladen.

    -   Items op het tweede niveau bepalen een groep op een tabblad.

        -   Items op het derde niveau bepalen een menu met acties in een groep

### <a name="add-a-group"></a>Groep toevoegen
Selecteer het tabblad waaronder u de groep hebben wilt, en selecteer **Groep maken** U kunt geen groep onder een menu toevoegen.

### <a name="add-a-menu"></a>Een menu toevoegen
Selecteer de groep waaronder u het menu hebben wilt, en selecteer **Menu maken**. U kunt een menu alleen aan een groep of een ander menu toevoegen. 

#### <a name="add-an-action"></a>Actie toevoegen
Selecteer het in het deelvenster **Beschikbare acties**, kies **Toevoegen** om het toe te voegen aan het deelvenster **Acties in deze volgorde weergeven**, en gebruik vervolgens de knoppen **Omhoog** en **Omlaag** om deze te plaatsen waar u ze hebben wilt.

U kunt geen actie aan een tabblad toevoegen; alleen aan een groep of menu.

###  <a name="limitations-and-recommendations"></a>Beperkingen en aanbevelingen 
Houd de volgende beperkingen in gedachten als u het lint aanpast:  
  
-   De systeemtabbladen of groepen zoals **Start** of **Nieuw** kunnen niet worden verplaatst of hernoemd. De positie van sommige groepen, zoals **Nieuw document** staat vast.  
-   Acties of groepen met dynamische zichtbaarheid kunnen niet worden toegevoegd of verwijderd. 
-   U kunt alleen menu's binnen groepen maken, niet binnen tabbladen.  
-   U kunt een menu binnen een ander menu nesten, maar dit wordt niet aangeraden.  
-   Als groepen en acties onverwacht gedrag na aanpassing van het lint, doet u het volgende:  
    
    1.  Maak de groep waar het probleem is opgetreden, leeg maar verwijder de groep niet.  
    2.  Sluit het venster met de knop **OK**.  
    3.  Open het dialoogvenster opnieuw en voeg de acties opnieuw aan de groep toe.  

> [!IMPORTANT]  
>  Eventuele aanpassing waardoor het lint wordt gewijzigd, kan van invloed zijn op de begeleiding die wordt verschaft in de [!INCLUDE[navnow_md](includes/navnow_md.md)] Help, omdat navigatiestappen in de Help kunnen verwijzen naar een andere lintindeling.

## <a name="customize-fasttabs"></a>Sneltabbladen aanpassen
Sneltabbladen helpen u gegevens over pagina's te ordenen in eenvoudige, beheerbare groepen. U kunt sneltabbladen op pagina's aanpassen zodat ze uw workflow ondersteunen. U wilt bijvoorbeeld specifieke velden op sneltabbladen weergeven of verbergen. Ook kunt u de belangrijkste velden in de kopteksten van de sneltabbladen laten weergeven wanneer die overzichten worden samengevouwen.  

### <a name="to-customize-a-fasttab"></a>Een sneltabblad aanpassen  
  
1.  Open de pagina die u wilt wijzigen.
2.  Kies het menu **Toepassing** ![knop van menu Toepassing op menubalk](media/applicationmenuicon.png "ApplicationMenuIcon")-pictogram, selecteer **Aanpassen** en kies vervolgens **Deze pagina aanpassen**.  
3.  Kies in het dialoogvenster **<Page Name> aanpassen** de optie **Sneltabbladen**.  
  
### <a name="add-move-or-remove-fasttabs"></a>Sneltabbladen toevoegen, verplaatsen of verwijderen
Het vak **Sneltabbladen in deze volgorde weergeven** bevat de sneltabbladen die zich momenteel op de pagina bevinden, en de volgorde waarin deze worden weergegeven. Gebruik **Toevoegen**, **Verwijderen** en de knoppen **Omhoog** en **Omlaag** om de wijzigingen aan te brengen.

### <a name="show-and-hide-fields-on-fasttabs"></a>Velden op de sneltabbladen weergeven en verbergen
Selecteer in de lijst **Sneltabbladen in deze volgorde weergeven** het sneltabblad dat u wilt aanpassen, en klik vervolgens op **Sneltabblad aanpassen**. Gebruik de knoppen om de velden aan te passen die u wilt weergeven en de volgorde ervan op de pagina.

Stel het **belang** als volgt in:
-   Als u het veld in de kop van het sneltabblad wilt weergeven als dit is samengevouwen, stelt u dit in op **Gepromoveerd**.
- Als u het veld wilt verbergen tenzij de gebruiker de actie **Meer velden weergeven** op het sneltabblad kiest, stelt u het in op **Aanvullend**.
-   **Standaard** is de standaard of de normale instelling.

### <a name="set-up-field-for-quick-entry"></a>Veld Instellingen voor snelle invoer 
Selecteer het selectievakje **Snelinvoer** als u het veld aan het overzicht met snelinvoer wilt toevoegen. Als u op de pagina werkt en op de Enter-toets drukt in een veld, springt de aanwijzer naar het volgende veld dat is ingesteld als een veld voor snelinvoer. 

## <a name="customize-factboxes"></a>Feitenblokken aanpassen
U kunt feitenblokken gebruiken om informatie te bekijken over de record die u in de lijst hebt geselecteerd of op een taakpagina hebt geopend. U kun de feitenblokken selecteren die u in het feitenblokdeelvenster wilt laten weergeven. U kunt de feitenblokken zodanig aanpassen dat alleen de velden worden weergegeven die u wilt weergeven.  
  
### <a name="to-show-or-hide-the-factbox-pane"></a>Het deelvenster Feitenblok weergeven of verbergen
Feitenblokken bevinden zich in het feitenblokdeelvenster, en kunt u kiezen om op paginabasis te bekijken of te verbergen. Zo kunt u eenvoudig meerdere feitenblokken gelijktijdig verbergen zonder dat u ze afzonderlijk hoeft te verwijderen. 

1.  Open de pagina die u wilt wijzigen. 
2.  Kies het menu **Toepassing** ![knop van menu Toepassing op menubalk](media/applicationmenuicon.png "ApplicationMenuIcon")-pictogram, selecteer **Aanpassen** en kies vervolgens **Feitenblokken**. Als het selectievakje is ingeschakeld, wordt het deelvenster Feitenblok weergegeven.  

### <a name="to-customize-the-factbox-pane"></a>Het feitenblokdeelvenster aanpassen  
1.  Open de pagina die u wilt wijzigen. 
2.  Kies het menu **Toepassing** ![knop van menu Toepassing op menubalk](media/applicationmenuicon.png "ApplicationMenuIcon")-pictogram, selecteer **Aanpassen** en kies vervolgens **Feitenblokken kiezen**.  
    
### <a name="add-a-factbox"></a>Een feitenblok toevoegen  
  
Selecteer het feitenblok dat u wilt toevoegen aan het feitenblokdeelvenster in het vak **Beschikbare feitenblokken** en kies de knop **Toevoegen**.  
  
### <a name="remove-a-factbox"></a>Een feitenblok verwijderen  
  
Selecteer in het vak **Feitenblokken in deze volgorde weergeven** de feitenblokken en klik vervolgens op de knop **Verwijderen**.   
  
### <a name="change-the-order-of-the-factboxes"></a>De volgorde van de feitenblokken wijzigen  
  
Selecteer het feitenblok dat u wilt verplaatsen, in het vak **Feitenblokken in deze volgorde weergeven** en kies vervolgens **Omhoog** of **Omlaag** totdat het feitenblok op de gewenste plaats staat.  
  
### <a name="change-the-fields-in-a-factbox"></a>De velden in een feitenblok wijzigen  
  
1.  Selecteer in het vak **Feitenblokken in deze volgorde weergeven** het feitenblok en klik vervolgens op de knop **Onderdeel aanpassen**.  
  
2.   Het vak **Beschikbare velden** bevat alle velden waaruit u kunt kiezen. Het vak **Weergegeven velden** bevat alle velden die momenteel in het feitenblok worden weergegeven. Gebruik de knoppen om de velden toe te voegen, te verwijderen en te verplaatsen.   


## <a name="customize-columns-in-a-list-or-on-document-lines"></a>Kolommen in een lijst of op documentregels aanpassen
Als u een beter overzicht van de benodigde gegevens wilt krijgen, kunt u lijstpagina's en kaartpagina's aanpassen door kolommen in de rasters toe te voegen of te verwijderen, kolommen opnieuw te rangschikken en een bevroren deelvenster toe te voegen.  
  
### <a name="to-add-remove-and-arrange-columns"></a>Kolommen toevoegen, verwijderen en ordenen  
  
1.  U kunt kolommen toevoegen, verwijderen of opnieuw rangschikken op twee manieren:

    -   Kies het menu **Toepassing** ![knop van menu Toepassing op menubalk](media/applicationmenuicon.png "ApplicationMenuIcon")-pictogram, selecteer **Aanpassen** en kies vervolgens **Kolommen kiezen**.
    -   Klik met de rechtermuisknop op een kolomkop en klik op **Kolommen kiezen**.

2.  Het dialoogvenster **Kiezen welke kolommen worden weergegeven in de lijst** bevat het deelvenster **Beschikbare kolommen** de kolommen die verborgen zijn. Het deelvenster **Kolommen in deze volgorde weergeven** bevat kolommen die worden weergegeven. Gebruik de knoppen **Toevoegen** en **Verwijderen** om kolommen naar een ander veld te verplaatsen. Gebruik de knoppen **Omhoog** en **Omlaag** om de kolommen te positioneren. 

>[!TIP]
>Selecteer het selectievakje **Snelinvoer** als u het veld aan het overzicht met snelinvoer wilt toevoegen. Als u op de pagina werkt en op de Enter-toets drukt in een veld, springt de aanwijzer naar het volgende veld dat is ingesteld als een veld voor snelinvoer. 

### <a name="to-set-the-freeze-pane"></a>Bevroren deelvenster instellen
Een overzicht kan veel kolommen bevatten, die u kunnen dwingen horizontaal te schuiven om alle kolommen te zien. Er zijn mogelijk een aantal kolommen die u altijd wilt weergeven zelfs als u schuift. Als u dit wilt, kunt u een verticaal bevroren deelvenster toevoegen om ervoor te zorgen dat sommige kolommen niet verschuiven. Zo kunt u ervoor zorgen dat alleen minder belangrijke kolommen verschuiven als u schuift.

Als u het bevroren deelvenster wilt instellen, selecteert u de kolom waarna u wilt dat het bevroren paneel begint en kiest u **Bevroren deelvenster toevoegen**.

## <a name="customizing-the-navigation-pane"></a>Het navigatiedeelvenster aanpassen
In het navigatiedeelvenster wordt een menu met koppelingen naar verschillende overzichtpagina's weergegeven. De koppelingen zijn gegroepeerd op knoppen op hoofdniveau. 

### <a name="to-customize-the-navigation-pane"></a>Het navigatiedeelvenster aanpassen  
  
Kies het menu **Toepassing** ![knop van menu Toepassing op menubalk](media/applicationmenuicon.png "ApplicationMenuIcon")-pictogram, selecteer **Aanpassen** en kies vervolgens **Navigatiedeelvenster aanpassen**.  
  
### <a name="rename-or-rearrange-buttons-in-the-navigation-pane"></a>Knoppen in het navigatiedeelvenster hernoemen of opnieuw rangschikken  
Selecteer in het linkerdeelvenster van het dialoogvenster **Navigatiedeelvenster aanpassen** die knop die u wilt verplaatsen, verwijderen of waarvan u de naam wilt wijzigen, en klik vervolgens op de relevante knop in het midden van het venster.

U kunt de knop **Start** niet verplaatsen, anders noemen of verwijderen. De knop **Afdelingen** kan worden verwijderd uit het navigatiedeelvenster, maar kan niet worden hernoemd of verplaatst. 
  
### <a name="add-a-new-menu-button"></a>Een nieuwe menuknop maken 
U kunt een nieuwe knop op hoofdniveau maken en vervolgens een menu met koppelingen toevoegen op de knop om verschillende pagina's te openen

1. Klik in het dialoogvenster **Navigatiedeelvenster aanpassen** op **Nieuw** en typ vervolgens een naam in het veld **Naam**.
2.  Kies de knop **OK**.

Nu kunt u koppelingen aan de knop toevoegen.  
  
### <a name="add-a-link-to-a-button"></a>Een koppeling toevoegen aan een knop   
Als u een lijst, zoals een lijst met verkooporders, mag bekijken, kunt u een koppeling naar de lijst vanaf een knop in het navigatiedeelvenster toevoegen.  
  
1.  Selecteer in het dialoogvenster **Navigatiedeelvenster aanpassen** in het veld **Knoppen in het navigatiedeelvenster** het menu waaraan u de koppeling wilt toevoegen.  
  
2.  Kies de knop **Toevoegen**.  
  
3.  Ga naar de koppeling die u wilt toevoegen, en klik op **OK**.  
> [!TIP]
> Als u een koppeling op een van de pagina's **Kostenplaatsen** vindt, kunt u die koppeling ook aan het navigatiedeelvenster toevoegen. Zie het gedeelte Een koppeling vanuit kostenplaatsen aan uw rolcentrum toevoegen voor meer informatie.  
  
### <a name="move-or-copy-a-link-from-one-button-to-another"></a>Een koppeling van de ene naar de andere knop kopiëren of verplaatsen  
  
1.  Selecteer in het dialoogvenster **Navigatiedeelvenster aanpassen** in het veld **Knoppen in het navigatiedeelvenster** het menu waarin de koppeling staat.  
  
2.  Selecteer in het deelvenster **Lijsten** de koppeling die u wilt verplaatsen, en klik op **Verplaatsen naar** of **Kopiëren naar**  
  
3.  Selecteer de navigatieknop waaraan u de koppeling wilt toevoegen, en klik op **OK**.  
  
### <a name="rearrange-the-order-of-a-links-under-a-button"></a>Herschik de volgorde van koppelingen op een knop  
  
1.  Selecteer in het deelvenster **Lijsten** de koppeling die u wilt verplaatsen.  
  
2.  Verplaats de koppeling met de knop **Omhoog** of **Omlaag**.

## <a name="adding-department-links-to-the-role-center"></a>Koppelingen van kostenplaatsen toevoegen aan het rolcentrum
Er kan soms een koppeling op een pagina **Kostenplaatsen** staan die u graag aan uw rolcentrum zou willen toevoegen om er eenvoudiger toegang tot te krijgen. Waar u de koppeling in het rolcentrum kunt plaatsen, hangt af van de categorie van de koppeling op de pagina **Afdelingen**.

In de volgende tabel wordt een beschrijving gegeven van de typen koppelingen in elke categorie op de pagina's **Kostenplaatsen** en waar u die koppelingen in uw rolcentrum kunt toevoegen.  
  
|**Categorie**|**Bevat**|**Koppeling toevoegen aan**|  
|------------------|------------------|---------------------|  
|Lijsten|Lijstpagina's|De knop **Startpagina** in het navigatiedeelvenster|  
|Taken|Taakpagina's, batchtaken, werkbladen, journalen|Het tabblad **Acties** in het lint|  
|Rapporten en analyse|Lijsten, batchtaken, matrixvensters|Het tabblad **Rapporten** in het lint|  
|Documenten|Documenten, zoals facturen en herinneringen|**Rapporten** in het lint|  
|Archief/Historie|Geboekte/voltooide documenten, registers|De knop **Startpagina** in het navigatiedeelvenster|  
|Beheer|Vensters met instellingen|Het tabblad **Acties** in het lint|  
  
### <a name="to-copy-department-links-to-your-role-center"></a>Koppelingen van kostenplaatsen kopiëren naar uw rolcentrum  
  
1.  Open de pagina **Afdelingen**.  
  
2.  Klik met de rechtermuisknop op de koppeling en klik op een van de opties (slechts een van deze opties is beschikbaar).  
  
    |**Selecteren**|**Koppeling toevoegen aan**|  
    |----------------|----------------------------|  
    |**Toevoegen aan navigatiedeelvenster**|De knop **Startpagina** in het navigatiedeelvenster van uw rolcentrum.|  
    |**Toevoegen aan acties op lint in rolcentrum**|Het menu **Acties** op het lint in uw rolcentrum|  
    |**Toevoegen aan lijsten op lint in rolcentrum**|Het menu **Lijsten** op het lint in uw rolcentrum|  
  
3.  Bevestig het bericht dat verschijnt.  
  
 De nieuwe koppeling wordt nu weergegeven in het menu waaraan u deze hebt toegevoegd. Misschien wilt u de koppeling naar een andere positie in het menu verplaatsen. Als u bijvoorbeeld een koppeling hebt toegevoegd aan het navigatiedeelvenster, verschijnt deze op het menu **Startpagina**, maar u kunt dit verplaatsen naar een ander menu in het navigatiedeelvenster. Zie voor meer informatie het gedeelte Het navigatiedeelvenster aanpassen. 

## <a name="adding-charts-to-role-centers-and-list-pages"></a>Grafieken toevoegen aan de rolcentra en lijstpagina's
Wanneer u complexe informatie hebt, wilt u misschien een visuele weergave van de gegevens zien om de weergave van trends en het nemen van beslissingen te vergemakkelijken. Misschien wilt u de saldi per bankrekening voor uw bedrijf controleren in een grafiek. U gebruikt het diagramvenster om gegevens visueel weer te geven vanuit een lijst op de volgende typen pagina's:  
  
-   In uw Rolcentrum, waar u een keuze kunt maken uit vooraf gedefinieerde algemene diagrammen.  
  
-   Op een lijstpagina waar u kunt kiezen om een lijst als een diagram weer te geven.  
  
### <a name="to-add-a-generic-chart-to-your-role-center"></a>Een algemeen diagram aan uw Rolcentrum toevoegen  
  
1.  Kies in uw rolcentrum het menu **Toepassing** ![knop van menu Toepassing op menubalk](media/applicationmenuicon.png "ApplicationMenuIcon")-pictogram, selecteer  **Aanpassen** en kies vervolgens **Deze pagina aanpassen**.  
  
2.  Selecteer in het venster **Het rolcentrum aanpassen** in het veld **Beschikbare onderdelen** de optie **Diagramonderdeel** en klik op **Toevoegen**.  
  
3.  Gebruik de knoppen **Omhoog**, **Omlaag**, **Naar links** en **Naar rechts** om het diagramonderdeel op uw rolcentrum te plaatsen.  
  
4.  Selecteer het grafiekdeel, kies **Onderdeel aanpassen**.  
  
5.  Selecteer in het venster **Diagram aanpassen** het vooraf ingestelde diagram dat u wilt weergeven en klik op **OK**.  
  
### <a name="to-view-a-list-as-a-chart"></a>Een lijst weergeven als een diagram  
  
1.  Selecteer op de lijstpagina de actie **Als diagram weergeven**.  
  
2.  Selecteer een eenheid en een dimensie om een aangepaste grafiek te maken. Selecteer een secundaire dimensie voor meer informatie. U kunt bijvoorbeeld een eenvoudige staafdiagram maken door een dimensie voor de X-as en de dimensie **Aantal dimensies** voor de Y-as te selecteren.  
  
> [!NOTE]  
>  Het diagramdeelvenster is standaard verborgen omdat dit de prestaties nadelig kan beïnvloeden. De grafiek moet alleen worden weergegeven wanneer u de informatie nodig hebt.  
    
## <a name="handling-external-files-and-automation-objects"></a>Extern bestanden en automatiseringsobjecten afhandelen
Wanneer [!INCLUDE[navnow_md](includes/navnow_md.md)] een extern bestand ontvangt, wordt een dialoogvenster weergegeven. Naast het selecteren wat er met het bestand moet gebeuren kunt u beslissen hoe dat bestandstype de volgende keer dat het wordt ontvangen, moet worden behandeld.  
  
Wanneer [!INCLUDE[navnow_md](includes/navnow_md.md)] een automatiseringsobject moet uitvoeren, wordt een dialoogvenster weergegeven. U kunt bepalen of dat soort object altijd of nooit moet worden uitgevoerd.  
  
### <a name="to-specify-how-to-handle-external-files"></a>Opgeven hoe externe bestanden worden verwerkt  
  
1.  Wanneer een dialoogvenster wordt weergegeven, schakelt u het selectievakje **Altijd waarschuwen voordat dit soort bestanden wordt geopend** uit als u wilt dat [!INCLUDE[navnow_md](includes/navnow_md.md)] de optie onthoudt die u in stap 2 selecteert. De volgende keer dat het bestandsoort moet worden verwerkt, wordt geen dialoogvenster weergegeven en wordt het bestand behandeld als in stap 2.  
  
     U kunt ook het selectievakje **Altijd waarschuwen voordat dit soort bestanden wordt geopend** inschakelen om altijd het dialoogvenster weer te geven wanneer dit bestandstype wordt ontvangen.  
  
2.  Selecteer **Openen**, **Opslaan** of **Annuleren**. Het bestand worden verwerkt op basis van uw selectie.  
  
### <a name="to-specify-how-to-handle-automation-objects"></a>Opgeven hoe automatiseringsobjecten worden verwerkt  
  
Wanneer het dialoogvenster wordt weergegeven, schakelt u het selectievakje **Altijd toestaan** in als u wilt dat [!INCLUDE[navnow_md](includes/navnow_md.md)] dit soort automatiseringsobject altijd uitvoert. De volgende keer dat het type automatiseringsobject nodig is om te worden uitgevoerd, wordt het dialoogvenster niet weergegeven en wordt het automatiseringsobject direct uitgevoerd.  
  
U kunt ook het selectievakje **Nooit toestaan** inschakelen. De volgende keer dat het type automatiseringsobject nodig is om te worden uitgevoerd, wordt het dialoogvenster niet weergegeven en wordt het automatiseringsobject niet uitgevoerd.  

## <a name="CancelPersonalization"></a>Personalisatie annuleren
Het annuleren van personalisatie kan in twee categorieën worden onderverdeeld:

-   Wijzigingen annuleren die u met de functie **Aanpassen** hebt gemaakt.
-   Annuleren van basiswijzigingen in de gebruikersinterface. 

### <a name="cancel-customization"></a>Aanpassing annuleren
Als u alle UI-aanpassing wilt annuleren die u ooit voor een pagina hebt aangebracht onder uw huidige gebruikersaanmelding of sinds u voor het laatst UI-aanpassingen hebt geannuleerd, kunt u het venster **Pers. gebruikersinstellingen verwijderen** gebruiken. De indeling van de pagina waarvoor u persoonlijke aanpassingen verwijdert, wordt vervolgens hersteld naar de standaardconfiguratie voor uw profiel.  
  
Als u slechts UI-aanpassingen wilt annuleren die u in een bepaald UI-gebied op een pagina hebt aangebracht, zoals het lint, kunt u de knop **Standaardwaarden herstellen** in het venster **Aanpassen** gebruiken. De indeling van het specifieke UI-gebied op die pagina wordt vervolgens hersteld naar de standaardconfiguratie voor uw profiel.  
  
#### <a name="to-cancel-all-ui-customization-that-you-have-made-to-a-page"></a>Alle aanpassingen van de gebruikersinterface annuleren die u hebt gemaakt voor een pagina  
  
1.  Typ in het tekstvak **Zoeken** de tekst **Pers. gebruikersinstellingen verwijderen** en kies vervolgens de gerelateerde koppeling.  
  
2.  Selecteer de pagina waarvoor u de aanpassing van de gebruikersinterface wilt annuleren en kies op het tabblad **Start** in de groep **Weergeven** de optie **Verwijderen**.  
  
> [!NOTE]  
>  Alle UI-aanpassing van de pagina die u ooit hebt aangebracht onder uw huidige gebruikersaanmelding of sinds u voor het laatst het venster **Pers. gebruikersinstellingen verwijderen** hebt gebruikt, wordt geannuleerd. De indeling van de pagina wordt hersteld naar de standaardconfiguratie voor uw profiel, zoals geconfigureerd door de beheerder of zoals geïnstalleerd met Microsoft Dynamics NAV.  
  
#### <a name="to-cancel-ui-customization-that-you-have-made-to-a-ui-area-on-a-page"></a>Aanpassingen van de gebruikersinterface annuleren die u hebt gemaakt voor een UI-gebied op een pagina  
  
1.  Vanaf de pagina waar u een gebruikersinterfacegebied hebt aangepast, zoals het lint, kiest u in het menu **Toepassing** ![ knop van menu Toepassing op menubalk](media/applicationmenuicon.png "ApplicationMenuIcon")-pictogram, selecteer **Aanpassen** en kiest u vervolgens **Aanpassen<UI area>**.  
  
2.  Kies onder in het venster **Aanpassen** de knop **Standaardwaarden herstellen**.  
  
> [!NOTE]  
>  Alle aanpassing van het UI-gebied die u ooit voor de pagina hebt aangebracht onder uw huidige gebruikersaanmelding, of sinds u voor het laatst de knop **Standaardwaarden herstellen** hebt gebruikt, wordt geannuleerd. De indeling van het UI-gebied op de pagina wordt hersteld naar de standaardconfiguratie voor uw profiel, zoals geconfigureerd door de beheerder of zoals geïnstalleerd met Microsoft Dynamics NAV.

### <a name="cancel-basic-ui-changes"></a>Annuleren van basiswijzigingen in de gebruikersinterface
U kunt algemene wijzigingen in de gebruikersinterface annuleren door het venster **Door de gebruiker gedefinieerde instellingen opnieuw instellen** te openen vanuit het rolcentrum.  
  
De basiswijzigingen in de gebruikersinterface omvat zaken als:
 -  Het wijzigen van de grootte en positie van een venster.
 -  Het wijzigen van de breedte van een kolom
 -  De hoogte van kolomkoppen wijzigen.
 -  Het sorteren van kolommen in een lijst.
 -  Het weergeven van lijsten als diagram.
 -  Opgeven hoe externe bestanden en automatiseringsobjecten worden afgehandeld.  
 
#### <a name="to-cancel-basic-ui-changes"></a>Annuleren van basiswijzigingen in de gebruikersinterface
  
1.  Ga naar uw rolcentrum.  
  
     Kies in het menu **Toepassing** menu ![knop van menu Toepassing op menubalk](media/applicationmenuicon.png "ApplicationMenuIcon") de optie **Aanpassen** en kies vervolgens **Door de gebruiker gedefinieerde instellingen opnieuw instellen**.  
  
2.  Kies de knop **Gebruikersinterface-instellingen opnieuw instellen**. Of kies de knop **Alles opnieuw instellen** om ook uw beslissingen voor het verwerken van bestanden en automatiseringsobjecten te annuleren.  
  
 Alle elementaire UI-wijzigingen die u ooit onder uw huidige gebruikersaanmelding hebt aangebracht in [!INCLUDE[navnow_md](includes/navnow_md.md)], of sinds u voor het laatst de knop **Gebruikersinterface-instellingen opnieuw instellen** hebt gekozen, worden geannuleerd. De gebruikersinterface wordt hersteld naar de standaardconfiguratie voor uw profiel.  
  
#### <a name="to-cancel-your-decision-for-running-or-saving-external-files"></a>Uw beslissing annuleren voor het uitvoeren of opslaan van externe bestanden  
  
1.  Ga naar uw rolcentrum.  
  
     Kies in het menu **Toepassing** menu ![knop van menu Toepassing op menubalk](media/applicationmenuicon.png "ApplicationMenuIcon") de optie **Aanpassen** en kies vervolgens **Door de gebruiker gedefinieerde instellingen opnieuw instellen**.  
  
2.  Kies de knop **Actie voor bestandsafhandeling opnieuw instellen**. Of kies de knop **Alles opnieuw instellen** om ook uw weergavewijzigingen en beslissingen voor het verwerken van automatiseringsobjecten te annuleren.  
  
 Alle beslissingen over standaardverwerking van bestandstypen die u ooit onder uw huidige gebruikeraanmelding hebt genomen, of sinds u voor het laatst de knop **Client-bestandstoegang** hebt gekozen, worden geannuleerd en opnieuw ingesteld op de standaardconfiguratie voor uw profiel. De volgende keer dat [!INCLUDE[navnow_md](includes/navnow_md.md)] een willekeurig soort extern bestand ontvangt, wordt een dialoogvenster weergegeven met de opties **Opslaan**, **Uitvoeren** en **Annuleren**.  
  
### <a name="to-cancel-your-decision-for-handling-automation-objects"></a>Uw beslissing annuleren voor de verwerking van automatiseringsobjecten  
  
1.  Ga naar uw rolcentrum.  
  
     Kies in het menu **Toepassing** menu ![knop van menu Toepassing op menubalk](media/applicationmenuicon.png "ApplicationMenuIcon") de optie **Aanpassen** en kies vervolgens **Door de gebruiker gedefinieerde instellingen opnieuw instellen**.  
  
2.  Kies de knop **Automatiseringsacties opnieuw instellen**. Of kies de knop **Alles opnieuw instellen** om ook uw weergavewijzigingen en beslissingen voor het uitvoeren of opslaan van externe bestanden te annuleren.  
  
 Alle beslissingen over hoe automatiseringsobjecten worden uitgevoerd die u ooit onder uw huidige gebruikersaanmelding hebt genomen, of sinds u voor het laatst de knop **Gebruikersinterface-instellingen opnieuw instellen** hebt gekozen, worden geannuleerd. Het bestandsverwerkinggedrag wordt hersteld naar de standaardconfiguratie voor uw profiel. De volgende keer dat [!INCLUDE[navnow_md](includes/navnow_md.md)] een willekeurig soort automatiseringsobject moet uitvoeren, wordt een dialoogvenster weergegeven met de opties **Altijd toestaan** en **Nooit toestaan**.    

<!--Use the following table to get more information about customizing the different elements of the UI.

| To | See |
| --- | --- |
| Change which actions to show on the ribbon and how the actions are grouped. |[How to: Customize FastTabs](purchasing-how-record-purchases.md) |
|Change which FastTabs to show and which fields to include on the FastTabs.|[How to: Request Quotes](purchasing-how-request-quotes.md)|
|Add, remove, or arrange columns in a list or document-lines that represent fields in the underlying tables. |[ How to: Add or Remove Columns in a List or on Document Lines](purchasing-how-purchase-products-sale.md) |
| Rename or rearrange buttons, create a new menu button, add a link to a menu, or rearrange the order of a menu. |[ How to: Customize the Navigation Pane](purchasing-how-correct-cancel-unpaid-purchase-invoices.md) |
| Add a link from a department page to your Role Center. |[How to: Process Purchase Returns or Cancellations](purchasing-how-register-new-vendors.md) |
|Add a chart to your Role Center or to a list page.|[How to: Combine Receipts on a Single Invoice](purchasing-how-to-combine-receipts.md)|
| Unod personalization that you have made to your user interface, either for a specific area on a page, such as a ribbon, or for the whole page.|[How to: Cancel Personalization](ui-customization-cancel.md)|
-->


## <a name="see-also"></a>Zie ook
[Uw werkruimte personaliseren met behulp van de Dynamics Web-client](ui-personalization-user.md)  
[Overzicht personalisatie](ui-personalization-overview.md)  




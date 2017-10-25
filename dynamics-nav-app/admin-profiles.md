---
title: Profielen en rolcentra beheren
description: Meer informatie over het beheer van gebruikers en rolcentra in Dynamics NAV.
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: profiles, roles, role centers, user roles
ms.date: 09/01/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: cd60cbc206b8e2cd6665b98ee49a5dc10c50fe08
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="managing-profiles-and-role-centers"></a>Profielen en rolcentra beheren
Profielen zijn verzamelingen [!INCLUDE[navnow_md](includes/navnow_md.md)]-gebruikers die hetzelfde rolcentrum delen. Een rolcentrum is een soort pagina waarop u de verschillende onderdelen kunt plaatsen. Elk deel is een container waarin u andere pagina's of vooraf gedefinieerde systeemdelen kunt hosten, zoals Outlook-onderdelen voor het toevoegen van taken, meldingen of notities.  

## <a name="about-profiles-and-role-centers"></a>Over gebruikers en rolcentra
U gebruikt profielen om gebruikers aan rolcentra te koppelen. Het rolcentrum is de startpagina voor alle gebruikers van een profiel, en is geconfigureerd om de taken en prioriteiten voor gebruikers van het profiel weer te geven. Het rolcentrum Orderverwerker is bijvoorbeeld geconfigureerd voor de taken en prioriteiten van een orderverwerker. Het rolcentrum biedt eenvoudig toegang tot informatie die gebruikers nodig hebben om hun dagelijkse werk te doen. Het rolcentrum bepaalt bijvoorbeeld de indicatiestapels, of de tegel, die worden weergeven wanneer gebruikers zich voor het eerst aanmelden, evenals de koppelingen van de navigatiepagina.

Het gebruikte profiel wordt weergegeven in de koptekst van het hoofdgebied van het rolcentrum. Een beheerder kan dit rolcentrum aan de behoeften van een specifieke rol in een bepaald bedrijf aanpassen. Het rolcentrum Orderverwerker kan vervolgens op één computer verder worden aangepast aan de behoeften van een persoon die de taak uitvoert als een orderverwerker. Deze persoon kan het rolcentrum personaliseren door query's op te slaan, filters toe te voegen en velden toe te voegen of te verwijderen.

Net als rolcentra komen profielen overeen met de functies en verantwoordelijkheden in uw organisatie. [!INCLUDE[navnow_md](includes/navnow_md.md)] biedt een reeks standaardprofielen die elk corresponderen met en zijn gekoppeld aan een rolcentrum. Beheerders kunnen bestaande profielen aanpassen of nieuwe profielen maken.  
  
> [!NOTE]  
>  : Profielen zijn niet expliciet gekoppeld aan de functies en machtigingen die het beveiligingssysteem uitmaken, maar profielgebruikers hebben machtigingen nodig die overeenkomen met hun functies in het beveiligingssysteem. Zie [Beveiliging in de omgeving van de rolgerichte client](http://go.microsoft.com/fwlink?LinkId=147633) in de MSDN-bibliotheek voor meer informatie. 

## <a name="to-create-a-profile"></a>Een profiel maken
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Profielen** in en klik vervolgens op de gerelateerde koppeling.  
  
2.  Klik op het lint op **Nieuw** om het venster **Nieuwe profielkaart** te openen.  
  
3.  Voer in het veld **Profiel-ID** een naam in die de beoogde rol van de gebruiker beschrijft.  
  
4.  Voer in het veld **Beschrijving** een beschrijving in van de profiel-id in, bijvoorbeeld **Orderverwerker**.  
  
5.  Stel het veld **Rolcentrum-id** in op het rolcentrum dat u aan het profiel wilt toewijzen.  
  
6.  Schakel het selectievakje **Standaardrolcentrum** in om dit rolcentrum als standaard voor het profiel in te stellen.  
  
7.  Kies de knop **OK**. .  
  
De procedure voor het wijzigen van een bestaand profiel is hetzelfde, behalve dat u een bestaand profiel selecteert op de profielpagina in plaats van te klikken op **nieuw**.  


##<a name="copying-a-profile"></a>Een profiel kopiëren 
Een profiel kopiëren kan u tijd besparen als u dezelfde instellingen voor een profiel wilt gebruiken en u slechts enkele instellingen wilt wijzigen.

1.  Open het profiel dat u wilt kopiëren en kies vervolgens de actie **Profiel kopiëren**.

2.  Voer in het veld **Nieuwe profiel-id** een naam in voor het profiel dat u wilt kopiëren. 

3.  Stel het veld **Nieuw profielbereik** op een van de volgende waarden in:

    - **Systeem** om het profiel voor de nieuwe tenantdatabases beschikbaar te maken die de toepassing gebruikt.
    - **Tenant** om het nieuwe profiel alleen voor de huidige tenantdatabase beschikbaar te maken. 
4. Kies de knop **OK** als u gereed bent.

## <a name="ExportImportProfile"></a>Profielen importeren en exporteren

U kunt profielen als XML-bestanden van en naar een [!INCLUDE[d365fin](includes/d365fin_md.md)] database exporteren en importeren. Het exporteren en importeren van een profiel kan u tijd besparen als u de gebruikersinterface configureert, omdat u een bestaande profielconfiguratie opnieuw gebruikt in plaats van dat een profiel helemaal vanaf het begin moet worden geconfigureerd. Als u een profiel hebt dat in een [!INCLUDE[d365fin](includes/d365fin_md.md)] database is geconfigureerd en u alle of een aantal van dezelfde profielconfiguraties in een andere database opnieuw wilt gebruiken, kunt u het profiel naar een XML-bestand exporteren. Vervolgens kunt u het XML-profielbestand in een andere database importeren.

-   Als u een profiel wilt exporteren, gaat u naar de pagina **Profielen exporteren**, selecteert u het profiel in de lijst en kiest u de actie **Exporteren**. Sla het XML-bestand op op een locatie op uw computer of netwerk. 
  
-   Als u een profiel wilt importeren, gaat u naar de pagina **Profielen importeren**, selecteert u het XML-profielbestand en kiest u de knop **OK**. 

    > [!NOTE]  
    >  U kunt geen profiel importeren dat al bestaat in de database, zelfs als het XML-bestand anders is genoemd of andere inhoud heeft. U moet het bestaande profiel verwijderen voordat u het nieuwe profiel kunt importeren. 



## <a name="see-also"></a>Zie ook  
[Procedure: Gebruikers en machtigingen beheren](ui-how-users-permissions.md)  
[De gebruikersinterface aanpassen](ui-customizing-overview.md)   
<!--[Security Overview](../Security%20Overview.md)-->


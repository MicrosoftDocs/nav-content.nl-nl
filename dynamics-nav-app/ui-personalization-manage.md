---
title: Personalisaties beheren als beheerder
description: Meer informatie over hoe u de gebruikersinterface kunt aanpassen aan uw manier van werken.
documentationcenter: 
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
ms.openlocfilehash: e3d088c35efca4d62b7db1f0d44d5ef2958317d4
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="managing-personalization-as-an-administrator"></a>Personalisaties beheren als beheerder
Gebruikers kunnen hun werkruimte aan hun eigen voorkeuren aanpassen. Als beheerder kunt u personalisaties bewaken en beheren door voor gebruikers de mogelijkheid uit te schakelen om pagina´s te personaliseren, en door alle personalisaties die door gebruikers zijn gemaakt, te wissen.

## <a name="disable-personalization-for-a-profile"></a>Personalisatie uitschakelen voor een profiel
U kunt voorkomen dat alle gebruikers die tot een bepaald profiel behoren, in staat zijn hun pagina's te personaliseren.
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Profielen** in en klik vervolgens op de gerelateerde koppeling.
2.  Selecteer in de lijst het profiel dat u wilt wijzigen.
3.  Selecteer het selectievakje **Personalisering deactiveren** en kies vervolgens de knop **OK**.

## <a name="clear-user-personalizations"></a>Gebruikerspersonalisaties wissen

Door paginapersonalisaties te wissen wordt de pagina teruggezet naar de oorspronkelijke layout die deze had voordat de personalisatie werd doorgevoerd. Er zijn twee manieren om de personalisaties te wissen die door gebruikers aan pagina's zijn aangebracht: met de pagina **Pers. gebruikersinstellingen verwijderen** en met de pagina **Gebruikerspersonalisatiekaart**.

### <a name="clear-user-personalizations-by-using-the-delete-user-personalization-page"></a>Personalisaties wissen met de pagina Pers. gebruikersinstellingen verwijderen.

Met de pagina **Pers. gebruikersinstellingen verwijderen** kunt u personalisaties per pagina, per gebruiker wissen.

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Pers. gebruikersinstellingen verwijderen** in en klik vervolgens op de gerelateerde koppeling.

    De pagina bevat alle pagina's die zijn gepersonaliseerd en gebruiker waartoe ze behoren.

    >[!NOTE]
    > Een vinkje in de kolom **Oude persoonlijke instellingen** is geeft aan dat de personalisatie uitsluitend is gedaan met behulp van [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] en/of met [!INCLUDE[nav_web_md](includes/nav_web_md.md)] vóór [!INCLUDE[navnow_md](includes/navnow_md.md)]. Gebruikers die proberen deze pagina's te personaliseren met behulp van [!INCLUDE[nav_web_md](includes/nav_web_md.md)] zijn hiertoe niet in staat omdat de pagina´s voor hen zijn vergrendeld totdat ze ervoor kiezen de pagina te ontgrendelen. Zie [Waarom is de pagina vergrendeld voor personaliseren?](ui-personalization-locked.md) voor meer informatie. Voor meer informatie over personalisaties in [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] en [!INCLUDE[nav_web_md](includes/nav_web_md.md)] zie [Werken met personalisatie tussen de Dynamics NAV Windows- en de webclient](ui-personalization-overview.md#PersonalizationWinWeb).

2. Selecteer het gegeven dat u wilt verwijderen en kies de actie **Verwijderen**.

    De gebruiker ziet de wijzigingen de volgende keer dat hij of zij zich aanmeldt.

### <a name="clear-user-personalizations-by-using-the-user-personalization-card-page"></a>Personalisaties wissen met de pagina Gebruikerspersonalisatiekaart.

Met de pagina **Gebruikerspersonalisatiekaart** kunt u de personalisaties op alle pagina´s voor een bepaalde gebruiker wissen. Hiervoor hebt u schrijfmachtiging nodig voor tabel 2000000072 **Profiel**.

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Gebruikerspersonalisatie** in en klik vervolgens op de gerelateerde koppeling.

    De pagina **Gebruikerspersonalisatie** bevat alle gebruikers waarvoor mogelijk gepersonaliseerde pagina's voorkomen. Als u een gebruikers-ID niet kunt vinden in de lijst, bestaan er geen gepersonaliseerde pagina´s voor.

2. Selecteer de gebruiker in de lijst en kies vervolgens de actie **Bewerken**.

3.  Op het tabblad **Acties** kiest **Aangepaste pagina's wissen**.

    De gebruiker ziet de wijzigingen de volgende keer dat hij of zij zich aanmeldt.

## <a name="see-also"></a>Zie ook
[Overzicht personalisatie](ui-personalization-overview.md)  
[Het personaliseren van uw werkruimte](ui-personalization-user.md)  
[Werken met [!INCLUDE[navnow_md](includes/navnow_md.md)]](ui-work-product.md)  
[Procedure: Het rolcentrum wijzigen](change-role.md)  

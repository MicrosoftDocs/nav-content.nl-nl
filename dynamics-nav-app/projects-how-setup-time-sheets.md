---
title: 'Procedure: Urenstaten instellen'
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
ms.openlocfilehash: 6cbacce79ce185d6ed00ea8383259d1b28f9e11b
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-time-sheets"></a>Procedure: urenstaten instellen
Urenstaten in Dynamics NAV verwerken tijdregistraties in wekelijkse termijnen van zeven dagen. U gebruikt ze om de tijd te volgen die aan projecten wordt besteed en u kunt ze gebruiken om eenvoudige registratie van resourcetijd vast te leggen. Voordat u urenstaten kunt gebruiken, moet u opgeven hoe u wilt dat ze worden ingesteld en geconfigureerd.

Nadat u hebt ingesteld hoe uw organisatie urenstaten gaat gebruiken, kunt u opgeven of en hoe urenstaten worden goedgekeurd. Afhankelijk van de wensen van uw organisatie kunt u het volgende aangeven:

- Een of meer gebruikers als urenstatenbeheerders en fiatteurs voor alle urenstaten.
- Een urenstaatgoedkeurder voor elke resource.

Wanneer u urenstaten hebt ingesteld, kunt u urenstaten maken voor resources, ze toewijzen een projectplanningsregels en urenstaatregels boeken. Zie [Procedure: Urenstaten gebruiken](projects-how-use-time-sheets.md) voor meer informatie.

## <a name="to-set-up-general-information-for-time-sheets"></a>Algemene informatie instellen voor urenstaten  

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Resource-instellingen** in en kies vervolgens de gerelateerde koppeling.  
2. Vul indien nodig de velden in. Kies een veld om een korte omschrijving van het veld of een koppeling naar meer informatie te lezen.
3. Selecteer voor het veld **Urenstaat op taakgoedkeuring** een van de volgende opties.

|Optie |Omschrijving|
|---|---|
|**Nooit**|De gebruiker in het veld **Gebruikers-id van fiatteur van urenstaat** op de resourcekaart keurt de urenstaat goed.|
|**Altijd**|De gebruiker in het veld **Verantwoordelijke** op de projectkaart keurt de urenstaat goed.|
|**Alleen machine**´|Als de urenstaat van een machine is gekoppeld aan een project, keurt de gebruiker in het veld **Verantwoordelijke** op de projectkaart de urenstaat goed. Als de urenstaat van een machine is gekoppeld aan een resource, keurt de gebruiker in het veld **Gebruikers-id van fiatteur van urenstaat** op de resourcekaart de urenstaat goed.

## <a name="to-assign-a-time-sheet-administrator"></a>Een beheerder van urenstaten toewijzen  

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Gebruikersinstellingen** in en kies vervolgens de gerelateerde koppeling.  
2.  Voeg een nieuwe gebruiker toe als de lijst met gebruikers niet de persoon bevat die de beheerder van urenstaten moet zijn. Neem contact op met uw beheerder voor meer informatie.  
3. Selecteer een gebruiker als beheerder van urenstaten en selecteer vervolgens het selectievakje **Urenstaat-admin** .  

**Tip**: het is raadzaam dat u slechts één gebruiker als beheerder van urenstaten van een bedrijf aanwijst. In de volgende procedure stelt u een urenstaateigenaar en fiatteur in waarbij de urenstaatfiatteur voor elke resource wordt toegewezen.  

## <a name="to-assign-a-time-sheets-owner-and-approver"></a>Een urenstaateigenaar en -fiatteur toewijzen  

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Resources** in en kies vervolgens de gerelateerde koppeling.
2. Selecteer de resource waarvoor u de mogelijkheid wilt instellen om urenstaten te gebruiken, en schakel vervolgens het selectievakje **Urenstaat gebruiken** in.  
3. Voer in het veld **Gebruikers-id van eigenaar van urenstaat** de id in van de eigenaar van de urenstaat. De eigenaar kan tijdsgebruik op een urenstaat invoeren en indienen voor goedkeuring. Als de resource een persoon, is die persoon in het algemeen ook de eigenaar.  
4. Voer in het veld **Gebruikers-id van fiatteur van urenstaat** de id in van de fiatteur van de urenstaat. De goedkeurder kan goedkeuren, weigeren of een urenstaat opnieuw openen.  

**Opmerking**: u kunt de id van de urenstaatfiatteur niet wijzigen als er urenstaten zijn die nog niet zijn verwerkt en die de status **Verstuurd** of **Open** hebben.

## <a name="see-also"></a>Zie ook
[Projectbeheer instellen](projects-setup-projects.md)  
[Projecten beheren](projects-manage-projects.md)  
[Financiën](finance-setup.md)  
[Inkoop beheren](purchasing-manage-purchasing.md)         
[Verkoop beheren](sales-manage-sales.md)      
[Werken met Dynamics NAV](ui-work-product.md)  


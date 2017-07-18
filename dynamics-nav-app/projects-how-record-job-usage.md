---
title: 'Procedure: Gebruik voor projecten vastleggen'
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
ms.openlocfilehash: 86cc31ea9c117700d2905dd6b8c4bd88eb0f9854
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

#<a name="how-to-record-usage-for-jobs"></a>Procedure: Gebruik voor projecten vastleggen
In het venster **Projectplanningsregels** kunt u het gebruik bekijken en vastleggen voor verschillende delen van uw project. Het gebruik wordt automatisch bijgewerkt wanneer u gegevens wijzigt en uitwisselt tussen projecten en projectdagboeken of projectfacturen. Hiervoor moet u een project hebt ingesteld zodat **Gebruikslink toepassen** is ingeschakeld. Zie [Procedure: Projecten instellen](projects-how-setup-jobs.md) voor meer informatie.  

Zo kunt u bijvoorbeeld voor planningsregels van het soort **Budget** de hoeveelheid van een resource invoeren en aangeven welke hoeveelheid moet worden overgebracht naar het projectdagboek. Als het soort van de planningsregel **Factureerbaar** is, kunt u de hoeveelheid van de resource invoeren en aangeven welke hoeveelheid moet worden overgebracht naar een factuur. Door de hoeveelheid die is doorgegeven aan het dagboek of de factuur te vergelijken met het resterend aantal, kunt u snel informatie over het gebruik bekijken.

In de volgende procedures wordt beschreven hoe u werkelijke (factureerbare) of gebudgetteerde projectprijzen en -kosten vastlegt. Voor informatie over het inschatten van gebudgetteerde waarde tijdens planning raadpleegt u [Procedure: Projectbudgetten beheren](projects-how-manage-budgets.md).

## <a name="to-record-usage-for-a-job-planning-line-of-type-budget"></a>Gebruik vastleggen voor een projectplanningsregel van het soort Budget

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Projecten** in en kies vervolgens de gerelateerde koppeling.  
2. Selecteer het betreffende project en kies vervolgens de actie **Projectplanningsregels**.
3. Selecteer een projectplanningsregel van het soort **Budget** of het soort **Budget en factureerbaar** waarvoor u gebruik wilt vastleggen.
4. In het veld **Aantal te verplaatsen naar dagboek** voert u het aantal in dat u wilt overbrengen. De standaardhoeveelheid is de waarde die u invoert in het veld **Aantal**.

    Het **Resterend aantal** bevat het resterende aantal om het project te voltooien en dat moet worden overgebracht naar het dagboek.  

5. Kies de actie **Projectdagboekregels maken**.
6. Vul in het venster **Projectplanningsregel taakoverdracht** de benodigde velden in. Kies een veld om een korte omschrijving van het veld of een koppeling naar meer informatie te lezen.
7. Kies de actie **Projectdagboek openen**.  
8. Selecteer in het venster **Projectdagboek** de relevante regel en kies vervolgens de actie **Boeken**.
9. Bekijk in het venster **Projectplanningsregels** het vastgelegde gebruik door te kijken naar de velden **Aantal**, **Resterend aantal** en **Aantal te verplaatsen naar dagboek**.  
10. Herhaal stap 3 tot en met 8 om aanvullend gebruik vast te leggen.  

## <a name="to-record-usage-for-a-job-planning-line-of-type-billable"></a>Gebruik vastleggen voor een projectplanningsregel van het soort Factureerbaar  
In de volgende taak kunt u eveneens gebruik bijhouden, maar dan voor een projectplanningsregel van het soort **Factureerbaar**. Meestal factuurt u in dit geval uw gebruik, maar u kunt het ook overbrengen naar een dagboek. Wanneer u dat echter doet, wordt een projectplanningsregel van het type **Budget** gemaakt voor afstemming met de factureerbare regel. Zie [Procedure: Projectbudgetten beheren](projects-how-manage-budgets.md) voor meer informatie.

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Projecten** in en kies vervolgens de gerelateerde koppeling.
2. Selecteer het betreffende project en kies vervolgens de actie **Projectplanningsregels**.  
3. Selecteer een projectplanningsregel van het soort **Factureerbaar** waarvoor u gebruik wilt vastleggen.
4. Voer in het veld **Aantal te verplaatsen naar factuur** het aantal in dat u wilt overbrengen. De standaardhoeveelheid is de waarde die u invoert in het veld **Aantal**.

    Het **Te factureren aantal** bevat het resterende aantal om het project te voltooien en dat moet worden gefactureerd.  

5. Kies de actie **Verkoopfactuur maken**.
6. Vul in het venster **Project - Naar verkoopfactuur overbrengen** desgewenst de velden in en kies vervolgens de knop **OK**.
7. Selecteer in het venster **Projectplanningsregels** de relevante regel en kies vervolgens de actie **Boeken**.
8. Bekijk het vastgelegde gebruik door te kijken naar de velden **Aantal**, **Te factureren aantal**, **Aantal te verplaatsen naar factuur** en, als de verkoopfactuur is geboekt, **Aantal gefactureerd**.
9. Herhaal stap 3 tot en met 8 om aanvullend gebruik vast te leggen.  
10. Als u een gerelateerde, geboekte verkoopfactuur wilt bekijken, kiest u de actie **Verkoopfacturen/-creditnota's**.  
11. Selecteer in het venster **Projectfacturen** de relevante factuur en kies vervolgens de actie **Verkoopfactuur/creditnota openen**.         

## <a name="to-create-job-journal-lines-from-job-planning-lines"></a>Projectdagboekregels maken uit projectplanningsregels  
Wanneer u klaar bent om financiële gegevens voor projecten te boeken, moet u projectdagboekregels maken die u kunt boeken.

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Projecten** in en kies vervolgens de gerelateerde koppeling.  
2. Selecteer een relevant open project en kies vervolgens de actie **Projectplanningsregels**.  
3. Voer in het venster **Projectplanningsregels** op een relevante projectplanningsregel in het veld **Aant. te verplaatsen naar dagboek** het aantal in dat u wilt verplaatsen naar een projectdagboek.  
4. Kies de actie **Projectdagboekregels maken**.
5. Vul in het venster **Projectplanningsregel taakoverdracht** de benodigde velden in.  
6. Kies de knop **Ok**. Er worden dagboekregels gemaakt.
7. Controleer de overdracht door de relevante projectdagboekbatch te openen en de posten te controleren.  
8. Wanneer de projectdagboekregels zijn voltooid, kiest u de actie **Boeken**.  

## <a name="to-create-job-journal-lines-manually"></a>Handmatig projectdagboekregels maken  

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Projectdagboeken** in en kies vervolgens de gerelateerde koppeling.  
2. Kies in het veld **Batchnaam** een relevante projectdagboekbatch.  
3. Voer op een nieuwe regel documentnummer, projectnummer, projecttaaknummer, soort en aantal van het verbruikte soort in.  
4. Wanneer de projectdagboekregels zijn voltooid, kiest u de actie **Boeken**.  

## <a name="to-review-planning-lines-for-a-job-ledger-entry"></a>Planningsregels voor een projectpost controleren  
Nadat u projectdagboekregels hebt geboekt, kunt u de planningsregels zien die zijn gekoppeld aan de projectdagboekposten die zijn geboekt.

**Opmerking**: hiertoe moet het selectievakje **Gebruikslink toepassen** zijn ingeschakeld voor het project of de standaardinstelling voor alle projecten in uw organisatie zijn. Zie [Procedure: Projecten instellen](projects-how-setup-jobs.md) voor meer informatie.  

1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Projectdagboeken** in en kies vervolgens de gerelateerde koppeling.  
2. Selecteer een relevant projectdagboek en kies vervolgens de actie **Posten**.  
3. Kies in het venster **Projectposten** de actie **Gekoppelde projectplanningsregels weergeven**.

## <a name="see-also"></a>Zie ook
[Projecten beheren](projects-manage-projects.md)  
[Financiën](finance-setup.md)  
[Inkoop beheren](purchasing-manage-purchasing.md)         
[Verkoop beheren](sales-manage-sales.md)      
[Werken met Dynamics NAV](ui-work-product.md)  


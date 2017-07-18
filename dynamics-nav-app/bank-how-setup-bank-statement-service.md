---
title: 'Procedure: De service Envestnet Yodlee Bank Feeds instellen'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 270568214afd2ca8af15f0fa7640337c77ec2f1e
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-the-envestnet-yodlee-bank-feeds-service"></a>Procedure: De service Envestnet Yodlee Bank Feeds instellen
U kunt elektronische bankafschriften van uw bank importeren om snel het venster **Betalingsreconciliatiedagboek** in te vullen, zodat u betalingen kunt vereffenen en de bankrekening kunt reconciliëren. Zie voor meer informatie [Betalingen automatisch vereffenen en bankrekeningen reconciliëren](receivables-apply-payments-auto-reconcile-bank-accounts.md).

**Opmerking**: de Envestnet Yodlee Bank Feeds-service of de bankfeedservice van een andere provider is mogelijk niet beschikbaar in uw systeem. Neem contact op met uw Microsoft-partner als u een bankfeedservice wilt gebruiken om bankafschriften te importeren.

Wanneer u de bankfeedservice hebt ingeschakeld, moet u de betreffende bankrekening koppelen aan de online bankrekening waar de feed vandaan zal komen. U koppelt bankrekeningen aan online bankrekeningen in de volgende scenario's:

- Er bestaat geen bankrekening in Dynamics NAV voor uw online bankrekening. Daarom kunt u de bankrekening maken door te koppelen vanuit de online bankrekening.
- Er bestaat een bankrekening in Dynamics NAV die u aan een online bankrekening wilt koppelen.
- Een gekoppelde bankrekening moet worden ontkoppeld omdat u de bankfeedservice niet meer voor de rekening wilt gebruiken.
- Online bankrekeningen zijn gewijzigd en u wilt de informatie over bankrekeningen bijwerken in Dynamics NAV.

Als de bankfeedservice is ingeschakeld, kunt u een bankrekening instellen om elke twee uur automatisch nieuwe bankafschriften te importeren in het venster **Betalingsreconciliatiedagboek**. Transacties voor betalingen die reeds zijn geboekt als vereffend en/of gereconcilieerd in het venster **Betalingsreconciliatiedagboek**, worden niet geïmporteerd. Zie voor meer informatie het gedeelte “Automatische import van bankafschriften inschakelen”.

**Opmerking**: als u de begeleide instelling Bedrijf instellen gebruikt, worden sommige stappen in de volgende procedures automatisch uitgevoerd wanneer u de instelling van de bedrijfsbankrekening uitvoert. Zie voor meer informatie [Welkom bij Dynamics NAV](across-get-started.md).

## <a name="to-enable-the-bank-feed-service"></a>De bankfeedservice inschakelen
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Bankrekeningen** in en kies vervolgens de gerelateerde koppeling.
2. Open de bankrekening die u voor de bankfeedservice wilt gebruiken.
3. Selecteer in het venster **Bankrekening** in het veld **Importindeling van bankafschrift** YODLEEBANKFEED.  

De bankfeedservice wordt ingeschakeld als u een bankrekening koppelt aan de gerelateerde online bankrekening. Zie de volgende procedure.  

## <a name="to-create-a-new-linked-bank-account"></a>Een nieuwe gekoppelde bankrekening maken
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Bankrekeningen** in en kies vervolgens de gerelateerde koppeling.
2. Selecteer de betreffende bankrekening en kies vervolgens **Nieuwe gekoppelde bankrekening maken**. Het venster **Bankrekening koppelen** opent na een aantal ogenblikken.

    **Opmerking**: dit venster bevat de werkelijke webpagina van de bankfeedservice van Envestnet Yodlee. De terminologie en functionaliteit in het venster komen mogelijk niet overeen met de instructies in dit onderwerp.  
3. Gebruik in het venster **Koppeling aan online bankrekening** in het deelvenster **Rekening koppelen** de zoekfunctie om de bank te zoeken waar u een of meer online bankrekeningen hebt.
4. Kies de banknaam. Het deelvenster **Aanmelden** wordt geopend.
5. Voer de gebruikersnaam en het wachtwoord in die u gebruikt om u aan te melden bij de online bank en kies vervolgens de knop **Volgende**.  
6. De bankfeedservice treft voorbereidingen om de eerste online bankrekening bij de opgegeven bank te koppelen aan een nieuwe bankrekening in Dynamics NAV.

    **Opmerking**: als u meer dan één online bankrekening bij de bank hebt, moet u extra bankrekeningen maken in Dynamics NAV voor die extra online bankrekeningen. Zie stap 8 t/m 10.

    Wanneer het proces probleemloos is voltooid, wordt de naam van de bank weergegeven in het deelvenster **Mijn rekeningen** op het tabblad **Gekoppeld**. Het nummer tussen haakjes geeft aan hoeveel online bankrekeningen zijn gekoppeld.
7. Kies de knop **Ok**.

    Als slechts één online bankrekening is gekoppeld, wordt het venster **Bankrekeningkaart** geopend voor een nieuwe bankrekening en vooraf ingevuld met de naam van de online bankrekening. In dit geval is de koppeling van de bankrekening voltooid. Alleen de bankrekening hoeft nog te worden ingesteld. Zie voor meer informatie [Procedure: Bankrekeningen instellen](bank-how-setup-bank-accounts.md).

    Als meerdere online bankrekeningen zijn gekoppeld, wordt het venster **Bankrekening koppelen** geopend met de aanvullende online bankrekeningen die nog niet zijn gekoppeld aan bankrekeningen in Dynamics NAV. In dat geval volgt u de volgende stap.  
8. Selecteer in het venster **Bankrekening koppelen** de regel voor een online bankrekening en kies vervolgens de actie **Koppelen aan nieuwe bankrekening**.

    Het venster **Bankrekeningkaart** voor een nieuwe bankrekening wordt geopend, vooraf ingevuld met de naam van de online bankrekening.

    Als er al een bankrekening bestaat in Dynamics NAV die u wilt koppelen aan de extra online de bankrekening, voert u de volgende stap uit.  
9. Selecteer in het venster **Bankrekening koppelen** de regel voor een online bankrekening en kies vervolgens de actie **Koppelen aan bestaande bankrekening**.
10. Selecteer in het venster **Bankenoverzicht** de bankrekening waarmee u wilt koppelen, en kies vervolgens de knop **OK**.

## <a name="to-link-a-bank-account-to-an-online-bank-account"></a>Een bankrekening koppelen aan een online bankrekening
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Bankrekeningen** in en kies vervolgens de gerelateerde koppeling.
2. Selecteer de regel voor een bankrekening die niet is gekoppeld aan een online bankrekening, en kies vervolgens de actie **Koppelen aan online bankrekening**. Het venster **Koppeling aan online bankrekening** wordt geopend met de naam van de bank al ingevuld in het deelvenster **Rekening koppelen**.
3. Kies de banknaam. Het deelvenster **Aanmelden** wordt geopend.
4. Voer de gebruikersnaam en het wachtwoord in die u gebruikt om u aan te melden bij de online bank en kies vervolgens de knop **Volgende**.

    De bankfeedservice treft voorbereidingen om uw bankrekening in Dynamics NAV te koppelen aan de gerelateerde online bankrekening.

    Wanneer het proces probleemloos is voltooid, wordt de naam van de bank weergegeven in het deelvenster **Mijn rekeningen** op het tabblad **Gekoppeld**. Als de bank meerdere bankrekeningen heeft, wordt alleen de bankrekening gekoppeld die u in stap 2 hebt geselecteerd.
5. Kies de knop **Ok**.

In het venster **Bankenoverzicht** is het selectievakje **Gekoppeld** ingeschakeld.

## <a name="to-unlink-a-bank-account"></a>Een bankrekening ontkoppelen
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Bankrekeningen** in en kies vervolgens de gerelateerde koppeling.  
2. Selecteer de regel voor een gekoppelde bankrekening die u wilt ontkoppelen van de gerelateerde online bankrekening, en kies de actie **Online bankrekening ontkoppelen**.

**Opmerking**: als u **Ja** kiest in het bevestigingsdialoogvenster, wordt de koppeling met de online bankrekening verwijderd en worden de logdetails gewist. Om de bankrekening weer te koppelen aan de online bankrekening, moet u zich weer aanmelden bij de bank. Zie voor meer informatie het gedeelte “Een bankrekening koppelen aan een online bankrekening“.

## <a name="to-update-bank-account-linking"></a>Koppeling aan bankrekening bijwerken
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Bankrekeningen** in en kies vervolgens de gerelateerde koppeling.
2. Selecteer de betreffende bankrekening en kies vervolgens de actie **Koppeling aan bankrekening bijwerken**.

Als er problemen voor de gekoppelde bankrekeningen zijn in het venster **Bankenoverzicht**, wordt het venster **Bankrekening koppelen** geopend, waarin wordt aangegeven welke bankrekeningen problemen hebben. Problemen kunnen het beste worden opgelost door de online bankrekening te ontkoppelen en de koppeling vervolgens opnieuw te maken. Zie voor meer informatie het gedeelte “Een bankrekening koppelen aan een online bankrekening“.

## <a name="to-enable-automatic-import-of-bank-statements"></a>Automatisch importeren van bankafschriften inschakelen
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Bankrekeningen** in en kies vervolgens de gerelateerde koppeling.
2. Selecteer de regel voor een gekoppelde bankrekening, en kies vervolgens de actie **Instelling van automatische import van bankafschriften**.
3. Geef in het venster **Instelling van automatische import van bankafschriften** in het veld **Aantal opgenomen dagen** op hoe ver in het verleden u banktransacties wilt ophalen.

    **Opmerking**: u wordt aangeraden deze waarde in te stellen op 7 dagen of meer.
4. Schakel het selectievakje **Ingeschakeld** in.  
Het venster **Betalingsreconciliatiedagboek** wordt nu elk uur gevuld met nieuwe betalingen die worden gedaan op de online bankrekening.

**Opmerking**: transacties voor betalingen die reeds zijn geboekt als vereffend en/of gereconcilieerd in het venster **Betalingsreconciliatiedagboek**, worden niet geïmporteerd.

## <a name="see-also"></a>Zie ook  
[Bankieren instellen](bank-setup-banking.md)  
[Bankrekeningen beheren.](bank-manage-bank-accounts.md)  
[Betalingen automatisch vereffenen en bankrekeningen reconciliëren](receivables-apply-payments-auto-reconcile-bank-accounts.md)  
[Dynamics NAV aanpassen met extensies](ui-extensions.md)


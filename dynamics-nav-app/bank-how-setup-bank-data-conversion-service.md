---
title: 'Procedure: Conversieservice voor bankgegevens instellen'
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
ms.openlocfilehash: 801e2abee52ec9804028a797e4f330b5e080549a
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-the-bank-data-conversion-service"></a>Procedure: Conversieservice voor bankgegevens instellen
U kunt betalingsregels uit het venster **Betalingsdagboek** exporteren naar een gegevensstroom die u vervolgens uploadt naar uw bank voor automatische verwerking, zodat u geen afzonderlijke elektronische betalingen hoeft te doen. Zie voor meer informatie [Procedure: Betalingen naar een bankbestand exporteren](payables-how-export-payments-bank-file.md).

Een algemene provider van services om betalingsgegevens naar elke willekeurige gegevensindeling te converteren die uw bank vereist, is verbonden en gereed om te worden ingeschakeld in Dynamics NAV.

Als alternatief voor de gegevensfeedservice van de Envestnet Bank kunt u ook de service voor conversie van bankgegevens gebruiken om een bankafschriftbestand dat u van uw bank ontvangt, te laten converteren naar een gegevensstroom die u kunt importeren in Dynamics NAV. Zie voor meer informatie [Procedure: Betalingen automatisch vereffenen en bankrekeningen reconciliëren](receivables-apply-payments-auto-reconcile-bank-accounts.md).

**Opmerking**: de conversieservice voor bankgegevens kan een limiet aan het aantal regels opleggen dat in één bestand mag worden geëxporteerd. Er wordt een foutbericht gestuurd als de limiet wordt overschreden. Het wordt aangeraden dat bankafschriftbestanden de 1000 regels niet overschrijden omdat de verwerkingstijd in de conversieservice van de bankgegevens anders beduidend kan toenemen.

## <a name="to-sign-your-company-up-for-the-bank-data-conversion-service"></a>Uw bedrijf aanmelden voor de conversieservice van bankgegevens
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Instelling gegevensconv.service bank** in en kies vervolgens de gerelateerde koppeling.  
2. Het venster **Instelling gegevensconv.service bank** wordt geopend met drie vooraf ingevulde velden met relevante URL's van de provider van de conversieservice voor bankgegevens.

    **Opmerking**: in de demodatabase CRONUS International Ltd. worden de velden Gebruikersnaam en Wachtwoord vooraf ingevuld met demoaanmeldgegevens, die u vervangt door de werkelijke gegevens van uw bedrijf wanneer u zich aanmeldt bij de conversieservice voor bankgegevens.
3. Kies in het veld **Inschrijvings-URL** de browserknop om de aanmeldingspagina van de serviceprovider te openen.  
4. Voer op de inschrijvingspagina van de serviceprovider van bankgegevens de gebruikersnaam en het wachtwoord in van het abonnement van uw bedrijf op de service en voltooi vervolgens het aanmeldingsproces volgens de instructies van de serviceprovider.

    Uw bedrijf is nu aangemeld voor de conversieservice van bankgegevens. Ga door met het invoeren van de gebruikersnaam en het wachtwoord dat u voor de service hebt opgegeven in de gerelateerde instellingsvelden in Dynamics NAV.
5. Voer in het venster **Instelling gegevensconv.service bank** in het veld **Naam** dezelfde waarde in die u in stap 4 als aanmeldnaam op de pagina van de serviceprovider hebt ingevoerd.
6. Voer in het veld **Wachtwoord** dezelfde waarde in die u in stap 4 in het veld **Wachtwoord** op de pagina van de serviceprovider hebt ingevoerd.

## <a name="to-encrypt-your-login-information"></a>Uw aanmeldgegevens versleutelen
We raden u aan de aanmeldgegevens te beveiligen die u invoert in het venster **Instelling gegevensconv.service bank**. U kunt gegevens op de Dynamics NAV-server versleutelen door nieuwe encryptiesleutels te genereren of bestaande sleutels te importeren die u inschakelt op de Dynamics NAV-serverinstantie die verbinding maakt met de database.

1. Kies in het venster **Instelling gegevensconv.service bank** de actie **Versleutelingsbeheer**.
2. Schakel in het venster **Beheer gegevensversleuteling** versleuteling van uw gegevens in.

##<a name="to-view-or-update-the-list-of-currently-supported-bank-data-formats"></a>De lijst met momenteel ondersteunde bankgegevensindelingen weergeven of bijwerken
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Instelling gegevensconv.service bank** in en kies vervolgens de gerelateerde koppeling.
2. Kies in het venster **Instelling gegevensconv.service bank** de actie **Banknaam - Gegevensconversielijst** om de lijst met banknamen te openen die bankgegevensindelingen vertegenwoordigen die door de conversieservice worden ondersteund.
3. Kies op de pagina **Banknaam - Gegevensconversielijst** de actie **Banknaamlijst bijwerken**.

De lijst met bankgegevensindelingen die door de conversieservice voor bankgegevens worden ondersteund, wordt nu bijgewerkt. Dit is de lijst met banknamen, gefilterd op land/regio, die u kunt selecteren vanuit het veld **Banknaam - Gegevensconversie** in het venster **Bankrekeningkaart**.

**Opmerking**: de bijwerking van ondersteunde bankgegevensindelingen treedt ook op wanneer u een waarde selecteert of invoert in het veld **Banknaam - Gegevensconversie** voor de bankrekening.

U bent nu aangemeld voor de conversieservice van bankgegevens. Ga verder om de inschrijvingsinformatie door te voeren voor elke bankrekening die de service zal gebruiken.

## <a name="to-set-up-bank-accounts-to-use-the-bank-data-conversion-service"></a>Bankrekeningen instellen om de conversieservice van bankgegevens gebruiken
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Bankrekeningen** in en kies vervolgens de gerelateerde koppeling.
2. Open de kaart voor een bankrekening die u gaat exporteren of importeer bankbestanden met de conversieservice voor bankgegevens.
3. Kies op het sneltabblad **Transfer** in het veld **Exportindeling betaling** **Conversieservice voor bankgegevens - Krediettransfer** om betalingexport in te stellen.
4. Typ of selecteer in het veld **Banknaam - Gegevensconversie** de naam van de gegevensindeling van de bankrekening waarvoor u zich in stap 4 hebt aangemeld in het gedeelte “Aanmelden voor de conversieservice van bankgegevens”.
5. Herhaal stap 1 t/m 4 voor andere bankrekeningen die de conversieservice voor bankgegevens zullen gebruiken.

## <a name="see-also"></a>Zie ook  
[Bankieren instellen](bank-setup-banking.md)  
[Bankrekeningen beheren.](bank-manage-bank-accounts.md)


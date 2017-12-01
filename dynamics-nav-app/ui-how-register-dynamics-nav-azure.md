---
title: 'Procedure: Dynamics NAV registreren in Azure Management Portal'
author: edupont04
manager: edupont
ms.author: edupont
ms.custom: na
ms.date: 11/15/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: d41b96ab5807402a342991d5c5bc2d672db09e2f
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-register-dynamics-nav-in-the-azure-management-portal"></a>Procedure: Dynamics NAV registreren in Azure Management Portal
Als u services wilt gebruiken die gebaseerd zijn op Microsoft Azure, moet u uw Dynamics NAV registreren in Azure Management Portal. De extensie [Verkoop- en voorraadprognose](ui-extensions-sales-forecast.md) vereist bijvoorbeeld dat u een API-sleutel en een API-URI opgeeft, en andere services vereisen soortgelijke gegevens. Waar vindt u deze gegevens?

U kunt de gids **Azure Management Portal instellen** gebruiken om Dynamics NAV te registreren in Azure Management Portal en de gegevens die u nodig hebt, ophalen om services zoals de extensie Verkoop- en voorraadprognose, Power BI, Office 365 enzovoort te kunnen gebruiken. U hoeft slechts eenmaal bij Azure Management Portal te registreren en u moet een beheerder of supergebruiker in Dynamics NAV zijn.

De reden voor registratie is dat Dynamics NAV en de service waarmee u verbinding wilt maken, de Azure AD-gegevens (Azure Active Directory) van elkaar moeten weten.

## <a name="to-register-dynamics-nav-in-the-azure-management-portal"></a>Dynamics NAV registreren in Azure Management Portal
1. Meld u weer aan bij Azure Management Portal op [https://portal.azure.com](https://portal.azure.com). Als u niet bekend bent met Azure Management Portal, kunt u richtlijnen vinden in de [Azure-documentatiebibliotheek](https://azure.microsoft.com/en-us/documentation/articles).
2. Kies in het linkernavigatievenster **Meer services** en kies vervolgens **App-registraties**.
3. Kies in het bovenste menu **Toevoegen** en vul vervolgens in het **paneel Maken** de velden in met de volgende gegevens:
    - **Naam**: geef een naam op voor uw Dynamics NAV-oplossing, zoals *Dynamics NAV*.
    - **Type toepassing**: kies **Webapp*/API**.
    - **Aanmeldings-URL**: voer de URL in voor uw Dynamics NAV-browserclient, zoals *https://MyServer:8080/DynamicsNAV/WebClient/OAuthLanding.htm*.
        Het bestand OAuthLanding.htm is een bestand dat helpt bij het beheren van de uitwisseling van gegevens tussen Dynamics NAV en andere services, met behulp van Azure AD.
4. Kies de knop **Maken**.
    Hierdoor wordt Dynamics NAV toegevoegd aan het paneel **App-registraties**, zodat u er nu instellingen aan kunt toevoegen.
5. Kies uw nieuwe app in de **lijst App-registraties**. Als hierdoor het paneel **Instellingen** niet wordt geopend, zou u een actie moeten zien om **Instellingen**** te openen.
6. Kies in het paneel **Instellingen** in het gedeelte **API-toegang** **Sleutels**.
7. Geef in het paneel **Sleutels** een beschrijving op en wanneer u wilt dat de sleutel verloopt, en kies vervolgens **Opslaan**.
8. Kopieer de gegenereerde sleutel naar een tijdelijke locatie. U hebt deze in de volgende procedure nodig.
9. Kies in het gedeelte **API-toegang** **Vereiste machtigingen**.
    - Voeg gedelegeerde machtigingen toe om alle rapporten in de Power BI-service te zien
    - Voeg gedelegeerde machtigingen toe om u aan te melden en het gebruikersprofiel te lezen voor Windows Azure Active Directory
    - Herhaal dit voor andere services waaraan u toegang wilt verlenen tot uw Dynamics NAV
10. Sluit het paneel **Instellingen** en kopieer vervolgens in het paneel **Hoofdzaken** de waarde van de **Toepassings-ID** naar een tijdelijke locatie.

U hebt nu Dynamics NAV in uw Azure Management Portal geregistreerd en u hebt toegang verleend tot de relevante services, en u hebt de gegevens opgehaald die u nodig hebt in Dynamics NAV.  

## <a name="to-add-the-information-to-dynamics-nav"></a>De gegevens toevoegen aan Dynamics NAV
1. Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Wizard Instelling van Azure AD-toepassing** in en kies de gerelateerde koppeling.
2. Kies **Volgende** in de wizard.
3. Geef in het veld **Client-id** de inhoud op die u eerder hebt gekopieerd uit het veld **Toepassings-id**.
4. Geef in het veld **Geheime sleutel** de inhoud op die u eerder hebt gekopieerd uit het veld **Sleutels**.
5. Kies **Volgende**. Tenzij u een foutbericht ziet, bent u nu klaar.

Uw Dynamics NAV is geregistreerd en gereed om verbinding te maken met services zoals Cortana Intelligence en Power BI.

## <a name="see-also"></a>Zie ook
[Verkoop- en voorraadprognose](ui-extensions-sales-forecast.md)  
[UwDynamics NAV](setup.md) instellen  


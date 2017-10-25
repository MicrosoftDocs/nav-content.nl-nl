---
title: Uw externe accountant toevoegen aan uw Dynamics NAV
description: Leer hoe u uw externe accountant kunt uitnodigen voor uw Dynamics NAV.
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting
ms.date: 09/05/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 856a95b929ca4fc419178c180bb8138e7f37ab61
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="inviting-your-external-accountant-to-your-included365finincludesd365finmdmd"></a>Uw externe accountant uitnodigen voor uw [!INCLUDE[d365fin](includes/d365fin_md.md)]
Als u een externe auditor gebruikt om uw boeken en financiële rapportage beheren, kunt u deze uitnodigen voor uw [!INCLUDE[d365fin](includes/d365fin_md.md)], zodat hij of zij met u kan werken aan uw fiscale gegevens.

Als de accountant toegang heeft gekregen tot uw [!INCLUDE[d365fin](includes/d365fin_md.md)], kan hij of zij het rolcentrum **Accountant** gebruiken, dat eenvoudig toegang tot de meest relevante vensters voor hun werk biedt.  

## <a name="invite-your-accountant-to-your-included365finincludesd365finmdmd"></a>Uw accountant uitnodigen voor uw [!INCLUDE[d365fin](includes/d365fin_md.md)]
In de laatste versie van [!INCLUDE[d365fin](includes/d365fin_md.md)] hebben we het voor u eenvoudig gemaakt om uw externe accountant uit te nodigen. Open gewoon het venster **Gebruikers** en kies de actie **Externe accountant uitnodigen** op het lint. Er wordt een e-mail voor u gemaakt. Voeg het werke-mailadres van uw accountant eraan toe en verzend de uitnodiging.  

![Uw accountant uitnodigen](./media/finance-invite-accountant/invite-accountant.png)

> [!TIP]  
>  Dit vereist dat u SMTP-e-mail hebt ingesteld. U kunt dit zelf doen of uw [!INCLUDE[d365fin](includes/d365fin_md.md)]-partner vragen. Daarnaast moet u als gebruikersbeheerder zijn aangemeld bij [!INCLUDE[d365fin](includes/d365fin_md.md)], niet als bedrijfeigenaar of een andere gebruiker.  

### <a name="separate-license"></a>Afzonderlijke licentie
Achter de schermen wordt de accountant toegevoegd aan uw Active Directory-tenant. Uw beheerder kan controleren of de accountant de uitnodiging accepteert en de juiste licentie toegewezen krijgt. De stappen hiervoor zijn afhankelijk van het soort rekening in dat u hebt gebruikt toen u zich aanmeldde bij [!INCLUDE[d365fin](includes/d365fin_md.md)]. Dit onderwerp is gebaseerd op het gebruik van een Office 365-account dat Microsoft Azure Active Directory gebruikt.  

Als u uw abonnement op [!INCLUDE[d365fin](includes/d365fin_md.md)] hebt geactiveerd en het evaluatiebedrijf niet meer gebruikt, hebt u een Azure Active Directory-tenant. De beheerder of [!INCLUDE[d365fin](includes/d365fin_md.md)]-partner beheert deze tenant in de [Azure-portal](https://portal.azure.com). Hier worden nieuwe gebruikers en toegevoegd en licenties toegepast en verwijderd. Zie voor meer informatie het [Microsoft Azure-portal - overzicht](https://docs.microsoft.com/en-us/azure/azure-portal-overview).  

Een van de licentiesoorten voor [!INCLUDE[d365fin](includes/d365fin_md.md)] is de *Externe accountant*-licentie. Dit licentiesoort is bedoeld voor gebruik door gebruikers zoals externe accountants. Dit betekent dat u geen extra seat in uw huidige Active Directory hoeft te kopen of een van uw bestaande [!INCLUDE[d365fin](includes/d365fin_md.md)]-gebruikersaccounts voor uw externe accountant hoeft te gebruiken. Als uw huidige Office 365-abonnement bijvoorbeeld 10 gebruikers bevat voor [!INCLUDE[d365fin](includes/d365fin_md.md)] en u momenteel 10 *Volwaardige gebruiker*-licenties gebruikt, kan uw beheerder gewoon uw externe accountant als gastgebruiker toevoegen in de Azure-portal en aan deze gebruiker zonder extra kosten de *Externe accountant*-licentie toewijzen. U kunt echter maar één gebruiker met de *Externe accountant*-licentie hebben. Als u meer gebruikers wilt toevoegen, moet u uw Office 365-abonnement bijwerken.  

## <a name="see-also"></a>Zie ook
[Financiën](finance.md)  
[Procedure: E-mail handmatig instellen of de begeleide instelling gebruiken](madeira-how-setup-email.md)  
[Accountantervaringen binnen Dynamics NAV](finance-accounting.md)  
[Dynamics NAV for Accountants op Microsoft.com](https://www.microsoft.com/en-us/dynamics365/financial-insights-for-accountants)  


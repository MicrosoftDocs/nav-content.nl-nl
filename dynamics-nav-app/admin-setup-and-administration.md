---
title: Beheertaken in Dynamics NAV
description: Sommige taken in [!INCLUDE[d365fin](includes/d365fin_md.md)] moeten centraal worden beheerd en ingesteld. Zie om welke taken het gaat en wat u hiermee doet.
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/01/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 3ddb647d28a4065be248a265316b38e8d37d28c2
ms.contentlocale: nl-nl
ms.lasthandoff: 12/01/2017

---
# <a name="setup-and-administration-in-dynamics-nav"></a><span data-ttu-id="87686-104">Installatie en beheer in Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="87686-104">Setup and Administration in Dynamics NAV</span></span>
<span data-ttu-id="87686-105">Centrale beheertaken worden meestal uitgevoerd door één rol in het bedrijf.</span><span class="sxs-lookup"><span data-stu-id="87686-105">Central administration tasks are usually performed by one role in the company.</span></span> <span data-ttu-id="87686-106">De omvang van deze taken kan afhangen van de bedrijfsgrootte en de functieverantwoordelijkheden van de beheerder.</span><span class="sxs-lookup"><span data-stu-id="87686-106">The scope of these tasks can depend on the company's size and the administrator's job responsibilities.</span></span> <span data-ttu-id="87686-107">Deze taken kunnen het beheer van databasesynchronisatie van verwerkings- en e-mailwachtrijen, instellen van gebruikers, aanpassen van de gebruikersinterface en het beheer van encryptiesleutels zijn.</span><span class="sxs-lookup"><span data-stu-id="87686-107">These tasks can include managing database synchronization of job and email queues, setting up users, customizing the user interface, and managing encryption keys.</span></span>  

<span data-ttu-id="87686-108">Voor het succes van nieuwe zakelijke software is het van belang dat vanaf het begin de juiste instellingswaarden worden ingevoerd.</span><span class="sxs-lookup"><span data-stu-id="87686-108">Entering the correct setup values from the start is important to the success of any new business software.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="87686-109"> bevat een aantal begeleide instellingen waarmee u hoofdgegevens kunt instellen.</span><span class="sxs-lookup"><span data-stu-id="87686-109"> includes a number of setup guides that help you set up core data.</span></span> <span data-ttu-id="87686-110">Zie voor meer informatie [Dynamics NAV](setup.md) instellen.</span><span class="sxs-lookup"><span data-stu-id="87686-110">For more information, see [Setting Up Dynamics NAV](setup.md).</span></span>

<!--Whether you use [!INCLUDE[rim](../../includes/rim_md.md)] to implement setup values or you manually enter them in the new company, you can support your setup decisions with some general recommendations for selected setup fields that are known to potentially cause the solution to be inefficient if defined incorrectly.-->  

<span data-ttu-id="87686-111">Een supergebruiker of gebruiker kan het kader voor gegevensuitwisseling instellen zodat gebruikers gegevens in bank- en salarisbestanden kunnen importeren en exporteren. bijvoorbeeld voor verschillende processen in kasbeheer.</span><span class="sxs-lookup"><span data-stu-id="87686-111">A super user or an administrator can set up the Data Exchange Framework to enable users to export and import data in bank and payroll files, for example for various cash management processes.</span></span>  

<span data-ttu-id="87686-112">In de volgende tabel wordt een reeks taken beschreven, met koppelingen naar de beschrijvende onderwerpen.</span><span class="sxs-lookup"><span data-stu-id="87686-112">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="87686-113">**Als u dit wilt doen**</span><span class="sxs-lookup"><span data-stu-id="87686-113">**To**</span></span>|<span data-ttu-id="87686-114">**Zie**</span><span class="sxs-lookup"><span data-stu-id="87686-114">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="87686-115">Gebruikers toevoegen, machtigingen en de toegang tot gegevens beheren en rollen toewijzen.</span><span class="sxs-lookup"><span data-stu-id="87686-115">Add users, manage permissions and access to data, assign roles.</span></span>|[<span data-ttu-id="87686-116">Gebruikers, profielen en rolcentra in Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="87686-116">Users, Profiles, and Role Centers in Dynamics NAV</span></span>](admin-users-profiles-roles.md)|  
|<span data-ttu-id="87686-117">Alle rechtstreekse wijzigingen bijhouden die gebruikers aanbrengen in databasegegevens, zodat de herkomst van fouten en wijzigingen in gegevens kan worden vastgesteld.</span><span class="sxs-lookup"><span data-stu-id="87686-117">Track all direct modifications that users make to data in the database to identify the origin of errors and data changes.</span></span>|[<span data-ttu-id="87686-118">Wijzigingen registreren in Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="87686-118">Logging Changes in Dynamics NAV</span></span>](across-log-changes.md)|  
|<span data-ttu-id="87686-119">Steun uw instellingsbeslissingen met aanbevelingen voor geselecteerde velden waarvan bekend is dat ze mogelijkerwijs de oplossing inefficiënt maken wanneer ze onjuist zijn ingesteld</span><span class="sxs-lookup"><span data-stu-id="87686-119">Support your setup decisions with recommendations for selected fields that are known to potentially cause the solution to be inefficient if set up incorrectly</span></span>|[<span data-ttu-id="87686-120">Complexe toepassingsgebieden instellen met aanbevolen procedures</span><span class="sxs-lookup"><span data-stu-id="87686-120">Set Up Complex Application Areas Using Best Practices</span></span>](set-up-complex-application-areas-using-best-practices.md)|  
|<span data-ttu-id="87686-121">Stel pagina's, code-units en query's open als webservices.</span><span class="sxs-lookup"><span data-stu-id="87686-121">Expose pages, codeunits, and queries as web services.</span></span>|[<span data-ttu-id="87686-122">Procedure: Een webservice publiceren</span><span class="sxs-lookup"><span data-stu-id="87686-122">How to: Publish a Web Service</span></span>](across-how-publish-web-service.md)|  
|<span data-ttu-id="87686-123">Stel een SMTP-server in om communicatie per e-mail in en vanuit Dynamics NAV in te stellen.</span><span class="sxs-lookup"><span data-stu-id="87686-123">Set up an SMTP server to enable e-mail communication in and out of Dynamics NAV</span></span>| [<span data-ttu-id="87686-124">Procedure: E-mail handmatig instellen of de begeleide instelling gebruiken</span><span class="sxs-lookup"><span data-stu-id="87686-124">How to: Set Up Email Manually or Using the Assisted Setup</span></span>](madeira-how-setup-email.md)|  
|<span data-ttu-id="87686-125">Eenmalige of periodieke verzoeken voor het uitvoeren van rapporten of code-units invoeren.</span><span class="sxs-lookup"><span data-stu-id="87686-125">Enter single or recurring requests to run reports or codeunits.</span></span>|[<span data-ttu-id="87686-126">Gebruik van taakwachtrijen om taken te plannen</span><span class="sxs-lookup"><span data-stu-id="87686-126">Use Job Queues to Schedule Tasks</span></span>](admin-job-queues-schedule-tasks.md)|  
|<span data-ttu-id="87686-127">Documenten beheren, verwijderen of comprimeren</span><span class="sxs-lookup"><span data-stu-id="87686-127">Manage, delete, or compress documents</span></span>|[<span data-ttu-id="87686-128">Documenten beheren</span><span class="sxs-lookup"><span data-stu-id="87686-128">Manage Documents</span></span>](admin-manage-documents.md)|  

## <a name="see-also"></a><span data-ttu-id="87686-129">Zie ook</span><span class="sxs-lookup"><span data-stu-id="87686-129">See Also</span></span>
[<span data-ttu-id="87686-130">Overzicht van bedrijffunctionaliteit</span><span class="sxs-lookup"><span data-stu-id="87686-130">Overview of Business Functionality</span></span>](madeira-business-functionality.md)  
[<span data-ttu-id="87686-131">Algemene bedrijfsfunctionaliteit</span><span class="sxs-lookup"><span data-stu-id="87686-131">General Business Functionality</span></span>](ui-across-business-areas.md)  
<span data-ttu-id="87686-132">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="87686-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
<span data-ttu-id="87686-133">[Welkom bij [!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="87686-133">[Welcome to [!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)</span></span>  


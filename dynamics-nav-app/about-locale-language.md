---
title: Meerdere talen en lokalisatie
description: "Leer hoe taal en landinstellingen uw ervaring in Dynamics NAV beïnvloeden."
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: language, locale, localization, culture
ms.date: 09/01/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 57787e98f1d845ab3edeb945be5e00750d7c9ae8
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="language-and-locale"></a><span data-ttu-id="dae96-103">Taal en landinstellingen</span><span class="sxs-lookup"><span data-stu-id="dae96-103">Language and Locale</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="dae96-104"> wordt ondersteund in een aantal markten en is beschikbaar in de talen die nodig zijn voor die markten.</span><span class="sxs-lookup"><span data-stu-id="dae96-104"> is supported in a number of markets and available in the languages that those markets require.</span></span> <span data-ttu-id="dae96-105">Dit is een resultaat van de ondersteuning voor meerdere talen tijdens runtime in combinatie met ondersteuning voor wettelijke vereisten in de ondersteunde markten.</span><span class="sxs-lookup"><span data-stu-id="dae96-105">This is a result of support for multiple languages at runtime in combination with support for legal requirements in the supported markets.</span></span> <span data-ttu-id="dae96-106">Dit betekent dat [!INCLUDE[d365fin](includes/d365fin_md.md)] in verschillende talen kan worden weergegeven.</span><span class="sxs-lookup"><span data-stu-id="dae96-106">This means that [!INCLUDE[d365fin](includes/d365fin_md.md)] can present itself in different languages.</span></span> <span data-ttu-id="dae96-107">U kunt de taal wijzigen die wordt gebruikt om teksten weer te geven. Deze wijziging wordt doorgevoerd zodra u automatisch bent afgemeld en weer aangemeld.</span><span class="sxs-lookup"><span data-stu-id="dae96-107">You can change the language that is used to display texts, and the change is immediate, once you have been automatically signed out and in again.</span></span> <span data-ttu-id="dae96-108">De instelling geldt alleen voor u, niet voor anderen in uw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="dae96-108">The setting applies to you and not to everyone else in your company.</span></span>  

<span data-ttu-id="dae96-109">Als u Canadees bent, kunt u de gebruikersinterface bijvoorbeeld in het Engels en Frans bekijken, maar in alle andere aspecten is het nog de Canadese versie van [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="dae96-109">For example, if you are Canadian, you can see the user interface in English and in French, but it is still the Canadian version of [!INCLUDE[d365fin](includes/d365fin_md.md)] in all other aspects.</span></span> <span data-ttu-id="dae96-110">In het Verenigd Koninkrijk wordt bijvoorbeeld een andere versie van [!INCLUDE[d365fin](includes/d365fin_md.md)] gebruikt.</span><span class="sxs-lookup"><span data-stu-id="dae96-110">It is not the same as, say, [!INCLUDE[d365fin](includes/d365fin_md.md)] in the United Kingdom.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="dae96-111">Het wijzigen van de taal wordt momenteel niet ondersteund in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="dae96-111">Changing the language is currently not supported in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

<span data-ttu-id="dae96-112">Deze meertalige functionaliteit heeft geen invloed op de taal waarin de toepassingsgegevens zijn opgeslagen.</span><span class="sxs-lookup"><span data-stu-id="dae96-112">Changing the texts that are stored as application data is not part of the multilanguage capability.</span></span> <span data-ttu-id="dae96-113">De taal van deze gegevens wordt bestuurd door het toepassingsontwerp.</span><span class="sxs-lookup"><span data-stu-id="dae96-113">This is an application design issue.</span></span> <span data-ttu-id="dae96-114">De namen van artikelen in de voorraad en de opmerkingen voor een klant zijn voorbeelden van dergelijke tekst.</span><span class="sxs-lookup"><span data-stu-id="dae96-114">Examples of such texts are the names of items in the inventory or the comments for a customer.</span></span> <span data-ttu-id="dae96-115">Deze tekst wordt dus niet vertaald.</span><span class="sxs-lookup"><span data-stu-id="dae96-115">In other words, these types of text are not translated.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="dae96-116">In [!INCLUDE[d365fin](includes/d365fin_md.md)] wordt slechts één tekenset voor gegevens ondersteund.</span><span class="sxs-lookup"><span data-stu-id="dae96-116">[!INCLUDE[d365fin](includes/d365fin_md.md)] only supports a single character set for data.</span></span> <span data-ttu-id="dae96-117">Daarom worden bepaalde tekens mogelijk niet ondersteund in uw tenant en kunnen er problemen optreden wanneer u gegevens ophaalt die zijn ingevoerd met een andere tekenset.</span><span class="sxs-lookup"><span data-stu-id="dae96-117">Therefore some characters may not be supported in your tenant, and you may experience problems when retrieving data that was entered using a different character set.</span></span> <span data-ttu-id="dae96-118">Uw tenant ondersteunt bijvoorbeeld alleen Engelse en Russische tekens en u voert gegevens in een andere taal in. De gegevens worden dan mogelijk niet juist opgeslagen.</span><span class="sxs-lookup"><span data-stu-id="dae96-118">For instance, your tenant may support only English and Russian characters and if you enter data in a different language, it may not be stored correctly.</span></span> <span data-ttu-id="dae96-119">Neem contact op met de systeembeheerder om te informeren welke talen precies worden ondersteund voor uw versie van [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="dae96-119">You should contact your system administrator to make sure you understand which languages are supported for your [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

## <a name="changing-the-locale"></a><span data-ttu-id="dae96-120">De landinstellingen wijzigen</span><span class="sxs-lookup"><span data-stu-id="dae96-120">Changing the Locale</span></span>
<span data-ttu-id="dae96-121">Landinstellingen zijn iets anders dan de taal en wettelijke vereisten in lokale markten.</span><span class="sxs-lookup"><span data-stu-id="dae96-121">Locale is different from both language and legal requirements in local markets.</span></span> <span data-ttu-id="dae96-122">De landinstellingen bepalen hoe uw gegevens worden weergegeven, bijvoorbeeld welke scheidingstekens worden gebruikt, of een tekst links of rechts wordt uitgelijnd en bepaalde andere instellingen.</span><span class="sxs-lookup"><span data-stu-id="dae96-122">Locale determines how your data presents itself in terms of comma separator, aligned to the left or to the right, and certain other settings.</span></span> <span data-ttu-id="dae96-123">De landinstellingen bepalen ook enkele systeemelementen in de browser, zoals de actie om een nieuw artikel in een lijst te maken.</span><span class="sxs-lookup"><span data-stu-id="dae96-123">The locale also determines some of the system elements in the browser, such as the action to create a new item in a list, for example.</span></span>  

<span data-ttu-id="dae96-124">U kunt de landinstellingen wijzigen op het browsertabblad dat u gebruikt om te werken in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="dae96-124">You can change the locale in the browser tab that you are using to work in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="dae96-125">De wijziging geldt alleen voor u, niet voor de andere gebruikers in uw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="dae96-125">the change applies only to you and not to the other users in your company.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="dae96-126">Wanneer u de landinstellingen wilt wijzigen, wordt er een lange lijst met talen en landinstellingen weergegeven.</span><span class="sxs-lookup"><span data-stu-id="dae96-126">When you change the locale, you will see a long list of languages and locales.</span></span> <span data-ttu-id="dae96-127">In dat geval worden echter alleen de lokale landinstellingen gebruikt in de huidige versie van [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="dae96-127">However, only the locale setting is used in the current version of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

<span data-ttu-id="dae96-128">U wijzigt de landinstellingen in het venster **Mijn instellingen**.</span><span class="sxs-lookup"><span data-stu-id="dae96-128">To change the locale, go to the **My Settings** window.</span></span> <span data-ttu-id="dae96-129">Zie voor meer informatie [Basisinstellingen wijzigen](ui-change-basic-settings.md).</span><span class="sxs-lookup"><span data-stu-id="dae96-129">For more information, see [Changing Basic Settings](ui-change-basic-settings.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="dae96-130">Zie ook</span><span class="sxs-lookup"><span data-stu-id="dae96-130">See Also</span></span>  
[<span data-ttu-id="dae96-131">Talen van de documenten</span><span class="sxs-lookup"><span data-stu-id="dae96-131">Languages of the Docs</span></span>](about-languages.md)  
[<span data-ttu-id="dae96-132">Basisinstellingen wijzigen</span><span class="sxs-lookup"><span data-stu-id="dae96-132">Changing Basic Settings</span></span>](ui-change-basic-settings.md)  
<span data-ttu-id="dae96-133">[Welkom bij [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="dae96-133">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span></span>  

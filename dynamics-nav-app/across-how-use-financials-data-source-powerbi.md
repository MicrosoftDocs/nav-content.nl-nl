---
title: Met Dynamics NAV een Power BI-gegevensbron maken
description: U kunt uw Dynamics NAV-gegevens als gegevensbron in Power BI beschikbaar maken en krachtige rapporten maken van de status van uw bedrijf.
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: business intelligence, KPI, Odata, Power App, SOAP, analysis
ms.date: 06/06/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b1beb7286eb221e5df3e7d5b2050ddcb389a0a07
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="using-included365finincludesd365finmdmd-as-a-power-bi-data-source"></a><span data-ttu-id="4f14a-103">[!INCLUDE[d365fin](includes/d365fin_md.md)] gebruiken als een Power BI-gegevensbron</span><span class="sxs-lookup"><span data-stu-id="4f14a-103">Using [!INCLUDE[d365fin](includes/d365fin_md.md)] as a Power BI Data Source</span></span>
<span data-ttu-id="4f14a-104">U kunt uw [!INCLUDE[d365fin](includes/d365fin_md.md)]-gegevens als gegevensbron in Power BI beschikbaar maken en krachtige rapporten maken van de status van uw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="4f14a-104">You can make your [!INCLUDE[d365fin](includes/d365fin_md.md)] data available as a data source in Power BI and build powerful reports of the state of your business.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="4f14a-105">U moet een geldig account bij [!INCLUDE[d365fin](includes/d365fin_md.md)] en Power BI hebben.</span><span class="sxs-lookup"><span data-stu-id="4f14a-105">You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with Power BI.</span></span> <span data-ttu-id="4f14a-106">Ook moet u [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/) downloaden.</span><span class="sxs-lookup"><span data-stu-id="4f14a-106">Also, you must download [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/).</span></span>  

## <a name="to-add-included365finincludesd365finmdmd-as-a-data-source-in-power-bi-desktop"></a><span data-ttu-id="4f14a-107">[!INCLUDE[d365fin](includes/d365fin_md.md)] als gegevensbron in Power BI Desktop toevoegen</span><span class="sxs-lookup"><span data-stu-id="4f14a-107">To add [!INCLUDE[d365fin](includes/d365fin_md.md)] as a data source in Power BI Desktop</span></span>
1. <span data-ttu-id="4f14a-108">Kies in Power BI Desktop in het linkernavigatievenster **Gegevens ophalen**.</span><span class="sxs-lookup"><span data-stu-id="4f14a-108">In Power BI Desktop, in the left navigation pane, choose **Get Data**.</span></span>
2. <span data-ttu-id="4f14a-109">Kies in het venster **Gegevens ophalen** achtereenvolgens **Online Services**, **Dynamics NAV** en de knop **Verbinden**.</span><span class="sxs-lookup"><span data-stu-id="4f14a-109">In the **Get Data** window, choose **Online Services**, choose **Dynamics NAV**, and then choose the **Connect** button.</span></span>

   <span data-ttu-id="4f14a-110">Power BI geeft een wizard weer die u in het verbindingsproces begeleidt.</span><span class="sxs-lookup"><span data-stu-id="4f14a-110">Power BI displays a wizard that will guide you though the connection process.</span></span> <span data-ttu-id="4f14a-111">De eerste stap bestaat eruit een OData-URL in te voeren en de bedrijfsnaam die aan uw [!INCLUDE[d365fin](includes/d365fin_md.md)]-account is gekoppeld.</span><span class="sxs-lookup"><span data-stu-id="4f14a-111">The first step will be to enter an OData URL and the company name that is associated with your [!INCLUDE[d365fin](includes/d365fin_md.md)] account.</span></span>  

   <span data-ttu-id="4f14a-112">Voor de *OData-URL* kunt u de URL van OData V4 kopiëren van een van de webservices die worden weergegeven op de pagina **Webservices** in [!INCLUDE[d365fin](includes/d365fin_md.md)], zoals `https://mycompany.financials.dynamics.com:7048/MS/ODataV4/`.</span><span class="sxs-lookup"><span data-stu-id="4f14a-112">For the *OData URL*, you can copy the OData V4 URL of any of the web services that are listed in the **Web Services** page in [!INCLUDE[d365fin](includes/d365fin_md.md)], such as `https://mycompany.financials.dynamics.com:7048/MS/ODataV4/`.</span></span>  

   <span data-ttu-id="4f14a-113">Voor *Bedrijfsnaam* gebruikt u de naam van het veld **Naam** in het venster **Bedrijfsgegevens** in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="4f14a-113">For the *Company Name*, use the name that is shown in the **Name** field in the **Company Information** window in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="4f14a-114">Als [!INCLUDE[d365fin](includes/d365fin_md.md)] meerdere bedrijven bevat, kies u de relevante bedrijfsnaam in de lijst van het venster **Bedrijven**.</span><span class="sxs-lookup"><span data-stu-id="4f14a-114">If your [!INCLUDE[d365fin](includes/d365fin_md.md)] contains multiple companies, choose the relevant company name from the list in the **Companies** window.</span></span> <span data-ttu-id="4f14a-115">In beide gevallen moet u ervoor zorgen dat de naam die u in de Power BI-wizard opgeeft, exact overeenkomt met de tekst die in [!INCLUDE[d365fin](includes/d365fin_md.md)] wordt weergegeven, zoals `My Company`.</span><span class="sxs-lookup"><span data-stu-id="4f14a-115">In both cases, make sure that the name that you specify in the Power BI wizard matches exactly the text shown in [!INCLUDE[d365fin](includes/d365fin_md.md)], such as `My Company`.</span></span>
3. <span data-ttu-id="4f14a-116">Klik op OK nadat u de gegevens hebt ingevoerd.</span><span class="sxs-lookup"><span data-stu-id="4f14a-116">Once you have entered the information, choose the OK button.</span></span> <span data-ttu-id="4f14a-117">De volgende stap in de wizard bestaat eruit uw gebruikersnaam en wachtwoord in te voeren.</span><span class="sxs-lookup"><span data-stu-id="4f14a-117">The next step in the wizard will be to enter your username and password.</span></span>

   > [!NOTE]  
>    <span data-ttu-id="4f14a-118">Als er andere verificatieopties beschikbaar zijn in de linkernavigatie, kiest u *Basis*.</span><span class="sxs-lookup"><span data-stu-id="4f14a-118">If there are other authentication options available in the left hand navigation, choose *Basic*.</span></span>
4. <span data-ttu-id="4f14a-119">Voer uw gebruikersnaam en wachtwoord in.</span><span class="sxs-lookup"><span data-stu-id="4f14a-119">Enter your username and password.</span></span> <span data-ttu-id="4f14a-120">U vindt deze informatie in het venster **Gebruikers** in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="4f14a-120">You can find this information in the **Users** window in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="4f14a-121">Gebruik **Webtoegangssleutel** als uw wachtwoord.</span><span class="sxs-lookup"><span data-stu-id="4f14a-121">Use the **Web Access Key** as your password.</span></span>

   <span data-ttu-id="4f14a-122">Uw gebruikersnaam is bijvoorbeeld *ADMIN* en de webservicetoegangssleutel die dient als uw wachtwoord, is *EgzeUFQ9Uv0o5O0lUMyqCzo1ueUW9yRF3SsLU=*.</span><span class="sxs-lookup"><span data-stu-id="4f14a-122">For example, your username is *ADMIN*, and the web service access key that serves as your password is *EgzeUFQ9Uv0o5O0lUMyqCzo1ueUW9yRF3SsLU=*.</span></span>
5. <span data-ttu-id="4f14a-123">Kies de knop **Verbinding** om door te gaan.</span><span class="sxs-lookup"><span data-stu-id="4f14a-123">Choose the **Connection** button to continue.</span></span> <span data-ttu-id="4f14a-124">De Power BI-wizard bevat een lijst met [!INCLUDE[d365fin](includes/d365fin_md.md)]-gegevensbronnen.</span><span class="sxs-lookup"><span data-stu-id="4f14a-124">The Power BI wizard shows a list of [!INCLUDE[d365fin](includes/d365fin_md.md)] data sources.</span></span> <span data-ttu-id="4f14a-125">Met deze gegevensbron worden alle webservices vertegenwoordigd die u hebt gepubliceerd vanuit uw [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="4f14a-125">These data source represent all the web services that you have published from your [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

   <span data-ttu-id="4f14a-126">U kunt ook een nieuwe webservice-URL in [!INCLUDE[d365fin](includes/d365fin_md.md)] maken met behulp van de actie **Gegevensset maken** op de pagina **Webservices** met de begeleide instelling **Rapportage instellen** of door de actie **Bewerken in Excel** in de lijsten te kiezen.</span><span class="sxs-lookup"><span data-stu-id="4f14a-126">Alternatively, create a new web service URL in [!INCLUDE[d365fin](includes/d365fin_md.md)] by using the **Create Data Set** action in the **Web Services** page, using the **Set Up Reporting** Assisted Setup guide, or by choosing the **Edit in Excel** action in any lists.</span></span>

6. <span data-ttu-id="4f14a-127">Geef de gegevens op die u aan uw gegevensmodel wilt toevoegen en kies vervolgens de knop **Laden**.</span><span class="sxs-lookup"><span data-stu-id="4f14a-127">Specify the data you want to add to your data model, and then choose the **Load** button.</span></span>
7. <span data-ttu-id="4f14a-128">Herhaal de vorige stappen om aanvullende [!INCLUDE[d365fin](includes/d365fin_md.md)]-gegevens aan uw Power BI-gegevensmodel toe te voegen.</span><span class="sxs-lookup"><span data-stu-id="4f14a-128">Repeat the previous steps to add additional [!INCLUDE[d365fin](includes/d365fin_md.md)] data to your Power BI data model.</span></span>

   > [!NOTE]  
>    <span data-ttu-id="4f14a-129">Zodra u verbinding hebt gemaakt met [!INCLUDE[d365fin](includes/d365fin_md.md)], wordt u niet weer gevraagd om de URL, gebruikersnaam of het wachtwoord van OData.</span><span class="sxs-lookup"><span data-stu-id="4f14a-129">Once you have successfully connected to [!INCLUDE[d365fin](includes/d365fin_md.md)], you will not be prompted again for the OData URL, username, or password.</span></span>

<span data-ttu-id="4f14a-130">Zodra de gegevens zijn geladen, worden deze in de rechternavigatie op de pagina weergegeven.</span><span class="sxs-lookup"><span data-stu-id="4f14a-130">Once the data is loaded it will appear in the right navigation on the page.</span></span> <span data-ttu-id="4f14a-131">Nu hebt u met succes een koppeling gemaakt naar uw Dynamics NAV-gegevens en kunt u uw Power BI-rapport gaan maken.</span><span class="sxs-lookup"><span data-stu-id="4f14a-131">At this point, you have successfully connected to your Dynamics NAV data and are ready to begin building your Power BI report.</span></span> <span data-ttu-id="4f14a-132">Zie de [Power BI-documentatie](https://powerbi.microsoft.com/documentation/powerbi-landing-page/) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="4f14a-132">For more information, see the [Power BI documentation](https://powerbi.microsoft.com/documentation/powerbi-landing-page/).</span></span>

## <a name="see-also"></a><span data-ttu-id="4f14a-133">Zie ook</span><span class="sxs-lookup"><span data-stu-id="4f14a-133">See Also</span></span>
[<span data-ttu-id="4f14a-134">Bedrijfsinformatie</span><span class="sxs-lookup"><span data-stu-id="4f14a-134">Business Intelligence</span></span>](bi.md)  
<span data-ttu-id="4f14a-135">[Welkom bij [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="4f14a-135">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span></span>  
[<span data-ttu-id="4f14a-136">Bedrijfsgegevens importeren uit andere financiële systemen</span><span class="sxs-lookup"><span data-stu-id="4f14a-136">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="4f14a-137">[Instellen van [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="4f14a-137">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
[<span data-ttu-id="4f14a-138">Financiën</span><span class="sxs-lookup"><span data-stu-id="4f14a-138">Finance</span></span>](finance.md)  

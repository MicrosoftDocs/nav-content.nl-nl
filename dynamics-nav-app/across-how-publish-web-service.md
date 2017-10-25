---
title: Objecten openstellen als webservices
description: Publiceer [!INCLUDE[d365fin](includes/d365fin_md.md)]-objecten als webservices om ze direct beschikbaar te maken op het netwerk.
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/01/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7c2bb65caeed819088382f811eb179eaeda35a7c
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-publish-a-web-service"></a><span data-ttu-id="34bfc-103">Procedure: Een webservice publiceren</span><span class="sxs-lookup"><span data-stu-id="34bfc-103">How to: Publish a Web Service</span></span>
<span data-ttu-id="34bfc-104">Webservices zijn een lichtgewicht manier om toepassingsfunctionaliteit aan allerlei externe systemen en gebruikers beschikbaar te maken.</span><span class="sxs-lookup"><span data-stu-id="34bfc-104">Web services are a lightweight way to make application functionality available to a variety of external systems and users.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="34bfc-105"> bevat een aantal objecten die standaard als webservices worden opengesteld vanwege de integratie met andere Microsoft-services, maar u kunt ook andere webservices toevoegen.</span><span class="sxs-lookup"><span data-stu-id="34bfc-105"> includes an number of objects that are exposed as web services by default due to integration with other Microsoft services, but you can also add other web services.</span></span>  

<span data-ttu-id="34bfc-106">U kunt een webservice in de Windows-client of de webclient instellen.</span><span class="sxs-lookup"><span data-stu-id="34bfc-106">You can set up a web service in the Windows client or in the Web client.</span></span> <span data-ttu-id="34bfc-107">U moet vervolgens de webservice publiceren zodat deze beschikbaar is voor service-aanvragen via het netwerk.</span><span class="sxs-lookup"><span data-stu-id="34bfc-107">You must then publish the web service so that it is available to service requests over the network.</span></span> <span data-ttu-id="34bfc-108">Gebruikers kunnen controleren of webservices actief zijn door een browser te laten kijken naar de serverlocatie en een overzicht van de beschikbare services aan te vragen.</span><span class="sxs-lookup"><span data-stu-id="34bfc-108">Users can discover web services by pointing a browser at the server location and requesting a list of available services.</span></span> <span data-ttu-id="34bfc-109">Wanneer u een webservice publiceert, is deze onmiddellijk beschikbaar via het netwerk voor geverifieerde gebruikers.</span><span class="sxs-lookup"><span data-stu-id="34bfc-109">When you publish a web service, it is immediately available over the network for authenticated users.</span></span> <span data-ttu-id="34bfc-110">Alle bevoegde gebruikers hebben toegang tot metagegevens voor webservices, maar alleen gebruikers die beschikken over voldoende machtigingen hebben toegang tot de werkelijke gegevens.</span><span class="sxs-lookup"><span data-stu-id="34bfc-110">All authorized users can access metadata for web services, but only users who have sufficient permissions can access actual data.</span></span>

## <a name="creating-and-publishing-a-web-service"></a><span data-ttu-id="34bfc-111">Een webservice maken en publiceren</span><span class="sxs-lookup"><span data-stu-id="34bfc-111">Creating and Publishing a Web Service</span></span>  
 <span data-ttu-id="34bfc-112">In de volgende stappen wordt uitgelegd hoe u een webservice maakt en publiceert.</span><span class="sxs-lookup"><span data-stu-id="34bfc-112">The following steps explain how to create and publish a web service.</span></span>  

#### <a name="to-create-and-publish-a-web-service"></a><span data-ttu-id="34bfc-113">Een webservice maken en publiceren</span><span class="sxs-lookup"><span data-stu-id="34bfc-113">To create and publish a web service</span></span>  

1.  <span data-ttu-id="34bfc-114">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Webservices** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="34bfc-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Web Services**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="34bfc-115">Kies op de pagina **Webservices** de optie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="34bfc-115">In the **Web Services** page, choose **New**.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    > [!NOTE]  
    >  <span data-ttu-id="34bfc-116">**Codeunit** en **Pagina** zijn geldige typen voor SOAP-webservices.</span><span class="sxs-lookup"><span data-stu-id="34bfc-116">**Codeunit** and **Page** are valid types for SOAP web services.</span></span> <span data-ttu-id="34bfc-117">**Pagina** en **Query** zijn geldige typen voor OData-webservices.</span><span class="sxs-lookup"><span data-stu-id="34bfc-117">**Page** and **Query** are valid types for OData web services.</span></span>  
    <span data-ttu-id="34bfc-118">Als de database meerdere bedrijven bevat, kunt u een specifieke object-id voor een van de bedrijven kiezen.</span><span class="sxs-lookup"><span data-stu-id="34bfc-118">Also, if the database contains multiple companies, you can choose an object ID that is specific to one of the companies.</span></span>  
    <span data-ttu-id="34bfc-119">De servicenaam is zichtbaar voor consumenten die uw webservice gebruiken en is de basis voor het identificeren en onderscheiden van webservices. Zorg dus dat de naam duidelijk is.</span><span class="sxs-lookup"><span data-stu-id="34bfc-119">Finally, the service name is visible to consumers of your web service and is the basis for identifying and distinguishing web services, so you should make the name meaningful.</span></span>

3.  <span data-ttu-id="34bfc-120">Schakel het selectievakje in de kolom **Gepubliceerd** in.</span><span class="sxs-lookup"><span data-stu-id="34bfc-120">Select the check box in the **Published** column.</span></span>  

     <span data-ttu-id="34bfc-121">Wanneer u de webservice publiceert, ziet u in de velden **OData-URL** en **SOAP-URL** de URL's die voor de webservice zijn gegenereerd.</span><span class="sxs-lookup"><span data-stu-id="34bfc-121">When you publish the web service, in the **OData URL** and **SOAP URL** fields, you can see the URLs that are generated for the web service.</span></span> <span data-ttu-id="34bfc-122">U kunt de webservice direct controleren door de koppelingen in de velden **OData-URL** en **SOAP-URL** te kiezen.</span><span class="sxs-lookup"><span data-stu-id="34bfc-122">You can test the web service immediately by choosing the links in the **OData URL** and **SOAP URL** fields.</span></span> <span data-ttu-id="34bfc-123">U kunt eventueel de waarde van het veld kopiëren en opslaan voor later gebruik.</span><span class="sxs-lookup"><span data-stu-id="34bfc-123">Optionally, you can copy the value of the field and save it for later use.</span></span>  

<span data-ttu-id="34bfc-124">Wanneer u een webservice publiceert, is deze beschikbaar voor externe partijen.</span><span class="sxs-lookup"><span data-stu-id="34bfc-124">After you publish a web service, it is available to external parties.</span></span> <span data-ttu-id="34bfc-125">U kunt de beschikbaarheid van de webservice verifiëren door een browser te gebruiken, of u kunt de koppeling in de velden **OData-URL** en **SOAP-URL** kiezen in het venster **Webservices**.</span><span class="sxs-lookup"><span data-stu-id="34bfc-125">You can verify the availability of that web service by using a browser, or you can choose the link in the **OData URL** and **SOAP URL** fields in the **Web Services** window.</span></span> <span data-ttu-id="34bfc-126">In de volgende procedure wordt beschreven hoe u de beschikbaarheid van de webservice kunt controleren voor later gebruik.</span><span class="sxs-lookup"><span data-stu-id="34bfc-126">The following procedure illustrates how you can verify the availability of the web service for later use.</span></span>  

#### <a name="to-verify-the-availability-of-a-web-service"></a><span data-ttu-id="34bfc-127">De beschikbaarheid van een webservice verifiëren</span><span class="sxs-lookup"><span data-stu-id="34bfc-127">To verify the availability of a web service</span></span>  

1.  <span data-ttu-id="34bfc-128">Voer in de browser de relevante URL in.</span><span class="sxs-lookup"><span data-stu-id="34bfc-128">In your browser, enter the relevant URL.</span></span> <span data-ttu-id="34bfc-129">De volgende tabel illustreert de soorten URL's die u kunt invullen.</span><span class="sxs-lookup"><span data-stu-id="34bfc-129">The following table illustrates the types of URLs that you can enter.</span></span> <span data-ttu-id="34bfc-130">Gebruik voor SOAP-webservices de volgende notatie voor uw URI.</span><span class="sxs-lookup"><span data-stu-id="34bfc-130">For SOAP web services, use the following format for your URI.</span></span>  

    <table>
    <tr>
    <th><span data-ttu-id="34bfc-131">Type webservice</span><span class="sxs-lookup"><span data-stu-id="34bfc-131">Web service type</span></span></th>
    <th><span data-ttu-id="34bfc-132">Syntaxis</span><span class="sxs-lookup"><span data-stu-id="34bfc-132">Syntax</span></span></th>
    <th><span data-ttu-id="34bfc-133">Opmerking</span><span class="sxs-lookup"><span data-stu-id="34bfc-133">Example</span></span></th>
    </tr>
    <tr>
    <td><span data-ttu-id="34bfc-134">SOAP</span><span class="sxs-lookup"><span data-stu-id="34bfc-134">SOAP</span></span></td>
    <td><span data-ttu-id="34bfc-135">https://*Server*:*SOAPWebServicePort*/*ServerInstance*/WS/*CompanyName*/salesDocuments/</span><span class="sxs-lookup"><span data-stu-id="34bfc-135">https://*Server*:*SOAPWebServicePort*/*ServerInstance*/WS/*CompanyName*/salesDocuments/</span></span></td>
    <td><span data-ttu-id="34bfc-136">https://mycompany.financials.dynamics.com:7047/MS/WS/MyCompany/Page/salesDocuments?tenant=mycompany.financials.dynamics.com</span><span class="sxs-lookup"><span data-stu-id="34bfc-136">https://mycompany.financials.dynamics.com:7047/MS/WS/MyCompany/Page/salesDocuments?tenant=mycompany.financials.dynamics.com</span></span></td>
    </tr>
    <tr>
    <td><span data-ttu-id="34bfc-137">OData</span><span class="sxs-lookup"><span data-stu-id="34bfc-137">OData</span></span></td>
    <td><span data-ttu-id="34bfc-138">https://*Server*:*ODataWebServicePort*/*ServerInstance*/OData/Company('*CompanyName*')</span><span class="sxs-lookup"><span data-stu-id="34bfc-138">https://*Server*:*ODataWebServicePort*/*ServerInstance*/OData/Company('*CompanyName*')</span></span></td>
    <td><span data-ttu-id="34bfc-139">https://MyCompany.financials.dynamics.com:7048/MS/OData/Company('MyCompany')/salesDocuments?tenant=MyCompany.financials.dynamics.com</span><span class="sxs-lookup"><span data-stu-id="34bfc-139">https://MyCompany.financials.dynamics.com:7048/MS/OData/Company('MyCompany')/salesDocuments?tenant=MyCompany.financials.dynamics.com</span></span>

         The company name is case-sensitive.</td>
    </tr>
    </table>

2.  <span data-ttu-id="34bfc-140">Controleer de informatie die verschijnt in de browser.</span><span class="sxs-lookup"><span data-stu-id="34bfc-140">Review the information that is displayed in the browser.</span></span> <span data-ttu-id="34bfc-141">Controleer of u de naam ziet van de webservice die u hebt gemaakt.</span><span class="sxs-lookup"><span data-stu-id="34bfc-141">Verify that you can see the name of the web service that you have created.</span></span>  

 <span data-ttu-id="34bfc-142">Als u toegang hebt tot een webservice en gegevens wilt terugschrijven naar [!INCLUDE[d365fin](includes/d365fin_md.md)], moet u de bedrijfsnaam opgeven.</span><span class="sxs-lookup"><span data-stu-id="34bfc-142">When you access a web service, and you want to write data back to [!INCLUDE[d365fin](includes/d365fin_md.md)], you must specify the company name.</span></span> <span data-ttu-id="34bfc-143">U kunt het bedrijf opgeven als onderdeel van URI zoals weergegeven in de volgende voorbeelden, of u kunt het bedrijf opgeven als onderdeel van de queryparameters.</span><span class="sxs-lookup"><span data-stu-id="34bfc-143">You can specify the company as part of the URI as shown in the examples, or you can specify the company as part of the query parameters.</span></span> <span data-ttu-id="34bfc-144">De volgende URI's wijzen bijvoorbeeld naar dezelfde OData-webservice en zijn beide geldige URI's.</span><span class="sxs-lookup"><span data-stu-id="34bfc-144">For example, the following URIs point to the same OData web service and are both valid URIs.</span></span>  

```  
https://localhost:7048/server/OData/Company('CRONUS International Ltd.')/Customer  
```  

```  
https://localhost:7048/server/OData/Customer?company='CRONUS International Ltd.'  
```  

## <a name="see-also"></a><span data-ttu-id="34bfc-145">Zie ook</span><span class="sxs-lookup"><span data-stu-id="34bfc-145">See Also</span></span>  
[<span data-ttu-id="34bfc-146">Installatie en beheer in Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="34bfc-146">Setup and Administration in Dynamics NAV</span></span>](admin-setup-and-administration.md)  


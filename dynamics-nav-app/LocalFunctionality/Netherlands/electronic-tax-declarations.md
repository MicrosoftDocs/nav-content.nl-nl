---
title: Elektronische belastingaangiften
description: Bedrijven moeten hun btw- en ICP-aangiften elektronisch aanleveren aan de belastingdienst.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: e4f8ee8c08b24d3e0113713694328e9f3deb8e98
ms.contentlocale: nl-nl
ms.lasthandoff: 12/01/2017

---
# <a name="electronic-tax-declarations"></a><span data-ttu-id="bad55-103">Elektronische belastingaangiften</span><span class="sxs-lookup"><span data-stu-id="bad55-103">Electronic Tax Declarations</span></span>
<span data-ttu-id="bad55-104">Bedrijven moeten hun btw- en ICP-aangiften elektronisch aanleveren aan de belastingdienst.</span><span class="sxs-lookup"><span data-stu-id="bad55-104">Companies must deliver their VAT and ICP declarations electronically to the tax authorities.</span></span>  

## <a name="prepare-for-electronic-declaration"></a><span data-ttu-id="bad55-105">Voorbereiding voor elektronische aangifte</span><span class="sxs-lookup"><span data-stu-id="bad55-105">Prepare for Electronic Declaration</span></span>  
 <span data-ttu-id="bad55-106">Voordat je elektronische aangiften kan versturen naar de belastingdienst moeten eerst de volgende taken zijn uitgevoerd:</span><span class="sxs-lookup"><span data-stu-id="bad55-106">Before you can send electronic declarations to the tax authorities you must perform the following tasks:</span></span>  

1.  <span data-ttu-id="bad55-107">Gebruikerscertificaten aanvragen bij de certificaatautoriteit (CA) en deze importeren in de toepassing.</span><span class="sxs-lookup"><span data-stu-id="bad55-107">Request user certificates from the certification authority (CA) and import them in the application.</span></span> <span data-ttu-id="bad55-108">Zie voor meer informatie de [website](http://go.microsoft.com/fwlink/?LinkID=223151) van de Nederlandse belastingdienst.</span><span class="sxs-lookup"><span data-stu-id="bad55-108">For more information, see the [website](http://go.microsoft.com/fwlink/?LinkID=223151) of the Dutch tax office.</span></span>  
2.  <span data-ttu-id="bad55-109">Aanmelden voor elektronische aangifte bij de belastingdienst.</span><span class="sxs-lookup"><span data-stu-id="bad55-109">Register at the tax authorities for electronic declaration.</span></span>  
3.  <span data-ttu-id="bad55-110">Algemene en persoonlijke gegevens, ontvangen van de belastingdienst, in het venster Elek. aangifte-instellingen invoeren.</span><span class="sxs-lookup"><span data-stu-id="bad55-110">Enter general data and personal data received from the tax authorities in the Elec. Tax Declaration Setup Window window.</span></span>  

<span data-ttu-id="bad55-111">Zie voor meer informatie [Elektronische btw- en ICP-aangiftes](electronic-vat-and-icp-declarations.md).</span><span class="sxs-lookup"><span data-stu-id="bad55-111">For more information, see [Electronic VAT and ICP Declarations](electronic-vat-and-icp-declarations.md).</span></span>  

## <a name="create-and-submit-electronic-declarations"></a><span data-ttu-id="bad55-112">Elektronische aangiftes maken en verzenden</span><span class="sxs-lookup"><span data-stu-id="bad55-112">Create and Submit Electronic Declarations</span></span>  
<span data-ttu-id="bad55-113">Als de hierboven vermelde taken zijn afgerond, kan de toepassing btw- en ICP-aangiften maken en verzenden naar de belastingdienst.</span><span class="sxs-lookup"><span data-stu-id="bad55-113">When the tasks stated above are finished the application can create and submit VAT and ICP declarations to the tax authorities.</span></span>  

<span data-ttu-id="bad55-114">De belastingdienst zal voor elke ontvangen aangifte een responsbericht sturen.</span><span class="sxs-lookup"><span data-stu-id="bad55-114">For each electronic declaration the tax authorities will send a response message.</span></span> <span data-ttu-id="bad55-115">Deze responsberichten worden opgehaald van de server bij de belastingdienst en verwerkt in de applicatie.</span><span class="sxs-lookup"><span data-stu-id="bad55-115">These messages must be received from the server of the tax authorities and processed.</span></span>  

## <a name="response-message-from-the-tax-authorities"></a><span data-ttu-id="bad55-116">Responsbericht van de belastingdienst</span><span class="sxs-lookup"><span data-stu-id="bad55-116">Response Message from the Tax Authorities</span></span>  
<span data-ttu-id="bad55-117">De belastingdienst zal een responsbericht sturen om het bedrijf te informeren over de status van de elektronische aangifte(n).</span><span class="sxs-lookup"><span data-stu-id="bad55-117">The tax authorities will send a response message to inform the company about the status of their electronic declarations.</span></span> <span data-ttu-id="bad55-118">Om te beginnen moet u de responsberichten van de belastingdienst in [!INCLUDE[navnow](../../includes/navnow_md.md)] importeren.</span><span class="sxs-lookup"><span data-stu-id="bad55-118">The first step is to import the response messages from the tax authorities in [!INCLUDE[navnow](../../includes/navnow_md.md)].</span></span> <span data-ttu-id="bad55-119">Vervolgens verwerkt u deze responsberichten.</span><span class="sxs-lookup"><span data-stu-id="bad55-119">The second step is processing the response messages.</span></span>  

<span data-ttu-id="bad55-120">Het responsbericht moeten aan de gerelateerde elektronische aangifte zijn gekoppeld.</span><span class="sxs-lookup"><span data-stu-id="bad55-120">The response message must be linked to the related electronic tax declaration.</span></span> <span data-ttu-id="bad55-121">Zie voor meer informatie de tabel Elek. aangiftekop.</span><span class="sxs-lookup"><span data-stu-id="bad55-121">For more information, see Elec. Tax Declaration Header Table.</span></span> <span data-ttu-id="bad55-122">Als er geen begeleidende elektronische aangifte wordt gevonden, wordt een foutmelding gegeven.</span><span class="sxs-lookup"><span data-stu-id="bad55-122">If no accompanying electronic tax declaration is found, an error message will appear.</span></span>  

<span data-ttu-id="bad55-123">Als de begeleidende elektronische belastingaangifte is gevonden moeten, afhankelijk van de responssoort, verschillende stappen worden uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="bad55-123">If the accompanying electronic tax declaration is found then, depending on the type of the response message, different steps must be performed.</span></span>  

## <a name="acknowledgement-response-message"></a><span data-ttu-id="bad55-124">Bevestiging van responsbericht</span><span class="sxs-lookup"><span data-stu-id="bad55-124">Acknowledgement Response Message</span></span>  
<span data-ttu-id="bad55-125">Als er geen fouten zijn gevonden in de elektronische aangifte en de gegevens zijn verwerkt door de belastingdienst, wordt het veld Status in de tabel **Elek. aangiftekop** gewijzigd in **Geaccepteerd**.</span><span class="sxs-lookup"><span data-stu-id="bad55-125">If no errors were found in the electronic declaration and the data has been processed by the tax authorities, the Status Field field in the **Elec. Tax Declaration Header** table will be changed into **Acknowledgement**.</span></span>  

## <a name="declaration-for-a-fiscal-entity"></a><span data-ttu-id="bad55-126">Aangifte voor een fiscale eenheid</span><span class="sxs-lookup"><span data-stu-id="bad55-126">Declaration for a Fiscal Entity</span></span>  
<span data-ttu-id="bad55-127">Als een bedrijf verscheidene bedrijven heeft geregistreerd als dochterondernemingen van een moedermaatschappij, hebben deze de mogelijkheid om de btw-aangifte afzonderlijk te doen of gecombineerd voor één fiscale eenheid.</span><span class="sxs-lookup"><span data-stu-id="bad55-127">If a company has several companies registered as subsidiaries of a holding company, they have the option to submit the VAT declaration individually or combined for one fiscal entity.</span></span> <span data-ttu-id="bad55-128">Ongeacht de keuze, moeten ICP-aangiften altijd afzonderlijk worden ingediend.</span><span class="sxs-lookup"><span data-stu-id="bad55-128">Regardless of the choice, the ICP declarations must always be submitted individually.</span></span>  

<span data-ttu-id="bad55-129">In het programma kunnen geen belastinggegevens van verschillende bedrijven worden gecombineerd tot één btw-aangifte.</span><span class="sxs-lookup"><span data-stu-id="bad55-129">The application cannot combine tax information for several companies into one electronic VAT declaration.</span></span> <span data-ttu-id="bad55-130">Als het bedrijf de belastinggegevens wil combineren, moet er een btw-aangifte op papier worden opgesteld voor elke dochteronderneming en moet het totale bedrag voor de moedermaatschappij worden berekend.</span><span class="sxs-lookup"><span data-stu-id="bad55-130">If the company wants to combine the tax information, they have to create a VAT statement on paper for each subsidiary company and calculate the total amount for the holding company.</span></span> <span data-ttu-id="bad55-131">Daarna moeten deze bedragen handmatig worden ingevoerd op de website van de belastingdienst.</span><span class="sxs-lookup"><span data-stu-id="bad55-131">After that these amounts can be manually entered on the website of the tax authorities.</span></span>  

<span data-ttu-id="bad55-132">Voor elke dochteronderneming kan een elektronische ICP-aangifte worden opgesteld en aan de belastingdienst worden gezonden.</span><span class="sxs-lookup"><span data-stu-id="bad55-132">For each subsidiary company an electronic ICP declaration can be created and submitted to the tax authorities.</span></span> <span data-ttu-id="bad55-133">Deze elektronische ICP-aangiften moeten het btw-nummer van de dochteronderneming en het veld Nr. fiscale eenheid</span><span class="sxs-lookup"><span data-stu-id="bad55-133">These electronic ICP declarations must contain the VAT Registration No. of the subsidiary company and the Fiscal Entity No.</span></span> <span data-ttu-id="bad55-134">van de moedermaatschappij uit de tabel Bedrijfsgegevens bevatten.</span><span class="sxs-lookup"><span data-stu-id="bad55-134">Field of the holding company out of the Company Information table.</span></span>  

<span data-ttu-id="bad55-135">Als u elektronische aangiften voor dochterondernemingen van een moedermaatschappij wilt instellen, moet u een vinkje plaatsen in het veld Deel van Fiscale eenheid in het venster Elek. aangifte-instellingen.</span><span class="sxs-lookup"><span data-stu-id="bad55-135">To setup electronic declarations for subsidiaries of a holding company, you must place a check mark in the field Part of Fiscal Entity Field in the Elec. Tax Declaration Setup Window window.</span></span>  

## <a name="see-also"></a><span data-ttu-id="bad55-136">Zie ook</span><span class="sxs-lookup"><span data-stu-id="bad55-136">See Also</span></span>  
 [<span data-ttu-id="bad55-137">Elektronische btw- en ICP-aangiften</span><span class="sxs-lookup"><span data-stu-id="bad55-137">Electronic VAT and ICP Declarations</span></span>](electronic-vat-and-icp-declarations.md) 


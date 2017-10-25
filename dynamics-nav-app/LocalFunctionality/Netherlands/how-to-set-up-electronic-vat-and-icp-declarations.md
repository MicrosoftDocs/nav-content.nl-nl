---
title: Elektronische btw- en ICP-aangiften instellen
description: Als u uw Digipoort-communicatie wilt laten werken, moet u mogelijk uw netwerkinstellingen aanpassen. Digipoort gebruikt een veilig communicatieprotocol en vereist gebruik van TCP-poort 443. Voordat u met de volgende procedure begint, stelt u uw netwerk in om deze poort te gebruiken.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 2f001f3bfcd80e443b1adee1b9dab28d32b5acc8
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-electronic-vat-and-icp-declarations"></a><span data-ttu-id="0de61-105">Procedure: Elektronische btw- en ICP-aangiften instellen</span><span class="sxs-lookup"><span data-stu-id="0de61-105">How to: Set Up Electronic VAT and ICP Declarations</span></span>
<span data-ttu-id="0de61-106">Als u uw Digipoort-communicatie wilt laten werken, moet u mogelijk uw netwerkinstellingen aanpassen.</span><span class="sxs-lookup"><span data-stu-id="0de61-106">To get your Digipoort communications to work, you may have to adjust your network settings.</span></span> <span data-ttu-id="0de61-107">Digipoort gebruikt een veilig communicatieprotocol en vereist gebruik van TCP-poort 443.</span><span class="sxs-lookup"><span data-stu-id="0de61-107">Digipoort uses a secure communication protocol and requires using TCP port 443.</span></span> <span data-ttu-id="0de61-108">Voordat u met de volgende procedure begint, stelt u uw netwerk in om deze poort te gebruiken.</span><span class="sxs-lookup"><span data-stu-id="0de61-108">Before proceeding with the following procedure, set up your network to use this port.</span></span>  
  
 <span data-ttu-id="0de61-109">Als u elektronische btw- en ICP-aangiften wilt kunnen maken en met de belastingdienst wilt kunnen communiceren, moet u eerst algemene gegevens over elektronische belastingaangiften instellen.</span><span class="sxs-lookup"><span data-stu-id="0de61-109">To be able to create electronic VAT and ICP declarations and communicate with the tax authorities, you must first set up general information about electronic tax declarations.</span></span> <span data-ttu-id="0de61-110">Uw bedrijf moet met de belastingdienst geregistreerd zijn voordat u elektronische aangiften kunt verzenden.</span><span class="sxs-lookup"><span data-stu-id="0de61-110">Your company must be registered with the tax authorities before you can send electronic declarations.</span></span>  
  
### <a name="to-set-up-electronic-tax-declarations"></a><span data-ttu-id="0de61-111">Elektronische belastingaangiften instellen</span><span class="sxs-lookup"><span data-stu-id="0de61-111">To set up electronic tax declarations</span></span>  
  
1.  <span data-ttu-id="0de61-112">Kies het pictogram ![Pictogram Zoeken naar pagina of rapport](media/ui-search/search_small.png "Pictogram Zoeken naar pagina of rapport"), voer **Elek. aangifte-instellingen** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="0de61-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Elec. Tax Declaration Setup**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="0de61-113">Selecteer in het venster **Elek. aangifte-instellingen** op het sneltabblad **Algemeen** de optie **BTW-contactpersoonsoort**.</span><span class="sxs-lookup"><span data-stu-id="0de61-113">In the **Elec. Tax Declaration Setup** window, on the **General** FastTab, select the **VAT Contact Type**.</span></span> <span data-ttu-id="0de61-114">De opties zijn **Belastingplichtige** en **Expediteur**.</span><span class="sxs-lookup"><span data-stu-id="0de61-114">The options include **Tax Payer** and **Agent**.</span></span> <span data-ttu-id="0de61-115">Als de contactsoort **Belastingplichtige** is, wordt de contact-id in de elektronische aangifte ingevuld met het btw-nummer van het bedrijf.</span><span class="sxs-lookup"><span data-stu-id="0de61-115">If the contact type is **Tax Payer**, the contact ID in the electronic declaration will be filled with the VAT Registration No. of the company.</span></span>  
  
3.  <span data-ttu-id="0de61-116">Selecteer het **ICP-contactpersoonsoort**.</span><span class="sxs-lookup"><span data-stu-id="0de61-116">Select the **ICP Contact Type**.</span></span> <span data-ttu-id="0de61-117">De opties zijn **Belastingplichtige** en **Expediteur**.</span><span class="sxs-lookup"><span data-stu-id="0de61-117">The options include **Tax Payer** and **Agent**.</span></span>  
  
4.  <span data-ttu-id="0de61-118">Als u elektronische ICP-aangiften voor een dochteronderneming van een fiscale eenheid wilt verzenden, schakelt u het veld **Deel van Fiscale eenheid** in.</span><span class="sxs-lookup"><span data-stu-id="0de61-118">If you want to send electronic ICP declarations for a subsidiary company of a fiscal entity, select the **Part of Fiscal Entity** field.</span></span>  
  
5.  <span data-ttu-id="0de61-119">Voer op het sneltabblad **Nummering** de nummerreeks voor het veld **Btw-aangiftenrs.** in.</span><span class="sxs-lookup"><span data-stu-id="0de61-119">On the **Numbering** FastTab, enter the number series for the **VAT Declaration Nos. Field** field.</span></span>  
  
6.  <span data-ttu-id="0de61-120">Voer op het sneltabblad **Digipoort** de benodigde gegevens in voor de Digipoort-verzendingen.</span><span class="sxs-lookup"><span data-stu-id="0de61-120">On the **Digipoort** FastTab, enter the data needed for the Digipoort submissions.</span></span>  
  
    1.  <span data-ttu-id="0de61-121">Voer in het veld **Naam certificaat Digipoort-client** de algemene (CN) naam in van het certificaat u voor gebruik met Digipoort hebt aangevraagd.</span><span class="sxs-lookup"><span data-stu-id="0de61-121">In the **Digipoort Client Cert. Name** field, enter the common name (CN) of the certificate you requested for use with Digipoort.</span></span> <span data-ttu-id="0de61-122">U kunt deze gegevens invoeren in de certificaateigenschappen van het persoonlijke certificaat dat u hebt geïnstalleerd onder de map **Persoonlijk** in de procedure [Procedure: Certificaten instellen voor gebruik met Digipoort](how-to-set-up-certificates-for-use-with-digipoort.md).</span><span class="sxs-lookup"><span data-stu-id="0de61-122">You can find this information in the certificate properties of the personal certificate that you installed under the **Personal** folder in the procedure [How to: Set Up Certificates for use with Digipoort](how-to-set-up-certificates-for-use-with-digipoort.md).</span></span>  
  
    2.  <span data-ttu-id="0de61-123">Voer in het veld **Naam certificaat Digipoort-service** de algemene naam in van het servicecertificaat, die gelijk kan zijn aan de naam van de server waarmee u communiceert voor de Nederlandse overheid.</span><span class="sxs-lookup"><span data-stu-id="0de61-123">In the **Digipoort Service Cert. Name** field, enter the common name of the service certificate, which may be equal to the name of the server that that you are communicating with for the Dutch government.</span></span> <span data-ttu-id="0de61-124">U kunt deze gegevens invoeren in de certificaateigenschappen van het openbare certificaat dat is geïnstalleerd in de map **Vertrouwde uitgevers** in de procedure [Procedure: Certificaten instellen voor gebruik met Digipoort](how-to-set-up-certificates-for-use-with-digipoort.md).</span><span class="sxs-lookup"><span data-stu-id="0de61-124">You can find this information in the certificate properties of the public certificate that was installed in the **Trusted Publishers** folder in the procedure [How to: Set Up Certificates for use with Digipoort](how-to-set-up-certificates-for-use-with-digipoort.md).</span></span>  
  
    3.  <span data-ttu-id="0de61-125">Geef in het veld **Directe leverings-URL** de URL op voor de productieversie van de Digipoort Aanlever-service.</span><span class="sxs-lookup"><span data-stu-id="0de61-125">In the **Digipoort Delivery URL** field, specify the URL for the production version of the Digipoort Aanlever service.</span></span> <span data-ttu-id="0de61-126">Zie voor meer informatie [http://www.logius.nl/producten/gegevensuitwisseling/digipoort](http://www.logius.nl/producten/gegevensuitwisseling/digipoort).</span><span class="sxs-lookup"><span data-stu-id="0de61-126">For more information, see [http://www.logius.nl/producten/gegevensuitwisseling/digipoort](http://www.logius.nl/producten/gegevensuitwisseling/digipoort).</span></span>  
  
    4.  <span data-ttu-id="0de61-127">Geef in het veld **Digipoort status-URL** de URL op voor de statusinformatie die komt van de Digipoort Statusinformatie-service.</span><span class="sxs-lookup"><span data-stu-id="0de61-127">In the **Digipoort Status URL** field, specify the URL for the status information that is coming from the Digipoort Statusinformatie service.</span></span>  
  
     <span data-ttu-id="0de61-128">Zie voor meer informatie [Overzicht van Digipoort](digipoort-overview.md).</span><span class="sxs-lookup"><span data-stu-id="0de61-128">For more information, see [Digipoort Overview](digipoort-overview.md).</span></span>  
  
 <span data-ttu-id="0de61-129">Momenteel zijn er twee sets URL's die door de Nederlandse belastingdienst worden verstrekt.</span><span class="sxs-lookup"><span data-stu-id="0de61-129">Currently, there are two sets of URLs that are provided by the Dutch Tax Administration.</span></span> <span data-ttu-id="0de61-130">Deze zijn echter voor wijzigingen vatbaar en u moet de website van de dienst regelmatig controleren op updates.</span><span class="sxs-lookup"><span data-stu-id="0de61-130">These are subject to change, however, and you should check the administration’s website regularly for updates.</span></span>  
  
 <span data-ttu-id="0de61-131">**Productiegebruik**</span><span class="sxs-lookup"><span data-stu-id="0de61-131">**Production Use**</span></span>  
  
-   <span data-ttu-id="0de61-132">URL van Digipoort-aanlevering: https://www.procesinfrastructuur.nl/wus/2.0/aanleverservice/1.2</span><span class="sxs-lookup"><span data-stu-id="0de61-132">Digipoort Delivery URL: https://www.procesinfrastructuur.nl/wus/2.0/aanleverservice/1.2</span></span>  
  
-   <span data-ttu-id="0de61-133">Status van Digipoort-aanlevering: https://www.procesinfrastructuur.nl/wus/2.0/statusinformatieservice/1.2</span><span class="sxs-lookup"><span data-stu-id="0de61-133">Digipoort Status URL: https://www.procesinfrastructuur.nl/wus/2.0/statusinformatieservice/1.2</span></span>  
  
 <span data-ttu-id="0de61-134">**Gebruik testen**</span><span class="sxs-lookup"><span data-stu-id="0de61-134">**Testing Use**</span></span>  
  
-   <span data-ttu-id="0de61-135">URL van Digipoort-aanlevering: https://preprod.procesinfrastructuur.nl/wus/2.0/aanleverservice/1.2</span><span class="sxs-lookup"><span data-stu-id="0de61-135">Digipoort Delivery URL: https://preprod.procesinfrastructuur.nl/wus/2.0/aanleverservice/1.2</span></span>  
  
-   <span data-ttu-id="0de61-136">URL van Digipoort-status: https://preprod.procesinfrastructuur.nl/wus/2.0/statusinformatieservice/1.2</span><span class="sxs-lookup"><span data-stu-id="0de61-136">Digipoort Status URL: https://preprod.procesinfrastructuur.nl/wus/2.0/statusinformatieservice/1.2</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="0de61-137">Zie ook</span><span class="sxs-lookup"><span data-stu-id="0de61-137">See Also</span></span>  
 <span data-ttu-id="0de61-138">[Procedure: Elektronische btw- en ICP-aangiften verzenden](how-to-submit-electronic-vat-and-icp-declarations.md) </span><span class="sxs-lookup"><span data-stu-id="0de61-138">[How to: Submit Electronic VAT and ICP Declarations](how-to-submit-electronic-vat-and-icp-declarations.md) </span></span>  
 [<span data-ttu-id="0de61-139">Procedure: Responsberichten van de belastingdienst verwerken</span><span class="sxs-lookup"><span data-stu-id="0de61-139">How to: Process Response Messages from Tax Authorities</span></span>](how-to-process-response-messages-from-tax-authorities.md)

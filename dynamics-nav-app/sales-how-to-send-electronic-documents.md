---
title: Elektronische documenten verzenden
description: Leer hoe u facturen elektronisch verzendt.
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: e912d461193b14c08c02c067b190bca93bda5376
ms.contentlocale: nl-nl
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-send-electronic-documents"></a><span data-ttu-id="be214-103">Procedure: Elektronische documenten verzenden</span><span class="sxs-lookup"><span data-stu-id="be214-103">How to: Send Electronic Documents</span></span>
<span data-ttu-id="be214-104">De algemene versie van [!INCLUDE[d365fin](includes/d365fin_md.md)] ondersteunt het verzenden van elektronische facturen en creditnota's in de PEPPOL-indeling, die wordt ondersteund door de grootste aanbieders van documentuitwisselingsservices.</span><span class="sxs-lookup"><span data-stu-id="be214-104">The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] supports sending electronic invoices and credit memos in the PEPPOL format, which is supported by the largest document exchange service providers.</span></span> <span data-ttu-id="be214-105">Een aanbieder van documentuitwisselingsservices verzendt elektronische documenten tussen handelspartners.</span><span class="sxs-lookup"><span data-stu-id="be214-105">A document exchange service provider dispatches electronic documents between trading partners.</span></span> <span data-ttu-id="be214-106">Om ondersteuning te bieden voor elektronische documentindelingen, gebruikt u het kader voor gegevensuitwisseling.</span><span class="sxs-lookup"><span data-stu-id="be214-106">To provide support for other electronic document formats, you use the data exchange framework.</span></span>  

 <span data-ttu-id="be214-107">In de algemene versie van [!INCLUDE[d365fin](includes/d365fin_md.md)] is een service voor documentuitwisseling vooraf geconfigureerd zodat u deze kunt instellen voor uw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="be214-107">In the generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)], a document exchange service is preconfigured and ready to be set up for your company.</span></span> <span data-ttu-id="be214-108">Zie [Procedure: Een service voor documentuitwisseling instellen](across-how-to-set-up-a-document-exchange-service.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="be214-108">For more information, see [How to: Set Up a Document Exchange Service](across-how-to-set-up-a-document-exchange-service.md).</span></span>  

 <span data-ttu-id="be214-109">Als u een verkoopfactuur als elektronisch PEPPOL-document wilt versturen, selecteert u de optie **Elektronisch document** in het dialoogvenster **Boeken en verzenden**. Hierin kunt u dit ook instellen als standaardprofiel voor documentverzending van de klant.</span><span class="sxs-lookup"><span data-stu-id="be214-109">To send a sales invoice as an electronic PEPPOL document, you select the **Electronic Document** option in the **Post and Send** dialog box from where you can also set up the customer’s default document sending profile.</span></span> <span data-ttu-id="be214-110">Eerst moet u diverse stamgegevens instellen, zoals bedrijfsgegevens, klanten, artikelen en eenheden.</span><span class="sxs-lookup"><span data-stu-id="be214-110">First, you must set up various master data, such as company information, customers, items, and units of measure.</span></span> <span data-ttu-id="be214-111">Deze worden gebruikt om de zakelijke partners en artikelen te identificeren wanneer gegevens worden geconverteerd in velden in [Procedure: Verzending en ontvangst van elektronische documenten instellen](across-how-to-set-up-electronic-document-sending-and-receiving.md).</span><span class="sxs-lookup"><span data-stu-id="be214-111">These are used to identify the business partners and items when converting data in fields in [How to: Set Up Electronic Document Sending and Receiving](across-how-to-set-up-electronic-document-sending-and-receiving.md).</span></span>  

### <a name="to-send-an-electronic-sales-invoice"></a><span data-ttu-id="be214-112">Een elektronische verkoopfactuur verzenden</span><span class="sxs-lookup"><span data-stu-id="be214-112">To send an electronic sales invoice</span></span>  

1.  <span data-ttu-id="be214-113">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Verkoopfacturen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="be214-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Invoices**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="be214-114">Maak een nieuwe verkoopfactuur.</span><span class="sxs-lookup"><span data-stu-id="be214-114">Create a new sales invoice.</span></span>  

3.  <span data-ttu-id="be214-115">Als de verkoopfactuur gereed is voor facturering, kiest u op het tabblad **Acties** in de groep **Boeken** de optie **Boeken en verzenden**.</span><span class="sxs-lookup"><span data-stu-id="be214-115">When the sales invoice is ready to be invoiced, on the **Actions** tab, in the **Posting** group, choose **Post and Send**.</span></span>  

     <span data-ttu-id="be214-116">Als het standaardverzendprofiel van de klant **Elektronisch document** is, wordt dit aangegeven in het dialoogvenster **Boeken en bevestiging verzenden** en hoeft u alleen maar de knop **Ja** te kiezen om de factuur te boeken en elektronisch te verzenden in de geselecteerde indeling.</span><span class="sxs-lookup"><span data-stu-id="be214-116">If the customer’s default sending profile is **Electronic Document**, then it will be shown in the **Post and Send Confirmation** dialog box and you just have to choose the **Yes** button to post and send the invoice electronically in the selected format.</span></span>  

4.  <span data-ttu-id="be214-117">In het dialoogvenster **Boeken en bevestiging verzenden** kiest u de Knop AssistEdit rechts van het veld **Document verzenden naar**.</span><span class="sxs-lookup"><span data-stu-id="be214-117">In the **Post and Send Confirmation** dialog box, choose the AssistEdit button to the right of the **Send Document to** field.</span></span>  

5.  <span data-ttu-id="be214-118">Kies in het dialoogvenster **Document verzenden naar** in het veld **Elektronisch document** de optie **Via service voor documentuitwisseling**.</span><span class="sxs-lookup"><span data-stu-id="be214-118">In the **Send Document to** dialog box, in the **Electronic Document** field, choose **Through Document Exchange Service**.</span></span>  

6.  <span data-ttu-id="be214-119">Kies in het veld **Indeling** de optie **PEPPOL**.</span><span class="sxs-lookup"><span data-stu-id="be214-119">In the **Format** field, choose **PEPPOL**.</span></span>  

7.  <span data-ttu-id="be214-120">Kies de knop **Ok**.</span><span class="sxs-lookup"><span data-stu-id="be214-120">Choose the **OK** button.</span></span> <span data-ttu-id="be214-121">Het dialoogvenster **Boeken en bevestiging verzenden** verschijnt.</span><span class="sxs-lookup"><span data-stu-id="be214-121">The **Post and Send Confirmation** dialog box appears.</span></span> <span data-ttu-id="be214-122">**Elektronisch document (PEPPOL)** is toegevoegd aan het veld **Document verzenden naar**.</span><span class="sxs-lookup"><span data-stu-id="be214-122">**Electronic Document (PEPPOL)** is added to the **Send Document to** field.</span></span>  

8.  <span data-ttu-id="be214-123">Kies de knop **Ja**.</span><span class="sxs-lookup"><span data-stu-id="be214-123">Choose the **Yes** button.</span></span>  

     <span data-ttu-id="be214-124">De verkoopfactuur wordt geboekt en aan de klant gezonden als elektronisch document in de indeling PEPPOL.</span><span class="sxs-lookup"><span data-stu-id="be214-124">The sales invoice is posted and sent to the customer as an electronic document in the PEPPOL format.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="be214-125">U kunt ook een geboekte verkoopfactuur als een elektronisch document verzenden.</span><span class="sxs-lookup"><span data-stu-id="be214-125">You can also send a posted sales invoice as an electronic document.</span></span> <span data-ttu-id="be214-126">De procedure is hetzelfde als beschreven in dit onderwerp voor niet-geboekte verkoopdocumenten.</span><span class="sxs-lookup"><span data-stu-id="be214-126">The procedure is the same as described in this topic for non-posted sales documents.</span></span> <span data-ttu-id="be214-127">Kies in het venster **Geboekte verkoopfactuur**, op het tabblad **Acties**, in de groep **Algemeen** de optie **Activiteitenlogbestand** om de status van het elektronische document te bekijken.</span><span class="sxs-lookup"><span data-stu-id="be214-127">In the **Posted Sales Invoice** window, on the **Actions** tab, in the **General** group, choose **Activity Log** to view the status of the electronic document.</span></span> <span data-ttu-id="be214-128">Zie voor meer informatie **Activiteitenlogbestand**.</span><span class="sxs-lookup"><span data-stu-id="be214-128">For more information, see **Activity Log**.</span></span>  

## <a name="see-also"></a><span data-ttu-id="be214-129">Zie ook</span><span class="sxs-lookup"><span data-stu-id="be214-129">See Also</span></span>  
[<span data-ttu-id="be214-130">Procedure: Verkopen factureren</span><span class="sxs-lookup"><span data-stu-id="be214-130">How to: Invoice Sales</span></span>](sales-how-invoice-sales.md)  
[<span data-ttu-id="be214-131">Procedure: Verzendprofielen voor documenten instellen</span><span class="sxs-lookup"><span data-stu-id="be214-131">How to: Set Up Document Sending Profiles</span></span>](sales-how-setup-document-send-profiles.md)  
[<span data-ttu-id="be214-132">Procedure: Verzending en ontvangst van elektronische documenten instellen</span><span class="sxs-lookup"><span data-stu-id="be214-132">How to: Set Up Electronic Document Sending and Receiving</span></span>](across-how-to-set-up-electronic-document-sending-and-receiving.md)  
[<span data-ttu-id="be214-133">Procedure: Een service voor documentuitwisseling instellen</span><span class="sxs-lookup"><span data-stu-id="be214-133">How to: Set Up a Document Exchange Service</span></span>](across-how-to-set-up-a-document-exchange-service.md)  
[<span data-ttu-id="be214-134">Procedure: Definities voor gegevensuitwisseling instellen</span><span class="sxs-lookup"><span data-stu-id="be214-134">How to: Set Up Data Exchange Definitions</span></span>](across-how-to-set-up-data-exchange-definitions.md)  
[<span data-ttu-id="be214-135">Gegevens elektronisch uitwisselen</span><span class="sxs-lookup"><span data-stu-id="be214-135">Exchanging Data Electronically</span></span>](across-data-exchange.md)  
[<span data-ttu-id="be214-136">Algemene bedrijfsfunctionaliteit</span><span class="sxs-lookup"><span data-stu-id="be214-136">General Business Functionality</span></span>](ui-across-business-areas.md)  


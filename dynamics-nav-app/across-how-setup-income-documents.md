---
title: 'Procedure: Inkomende documenten instellen'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: d55329b571e4c59d4821a86a39362ea58480b86a
ms.contentlocale: nl-nl
ms.lasthandoff: 09/11/2017

---

# <a name="how-to-set-up-incoming-documents"></a><span data-ttu-id="71362-102">Procedure: Inkomende documenten instellen</span><span class="sxs-lookup"><span data-stu-id="71362-102">How to: Set Up Incoming Documents</span></span>
<span data-ttu-id="71362-103">Als u dagboekregels van inkomende documentrecords maakt, moet u in het venster **Instellingen van inkomende documenten** vastleggen welke dagboeksjabloon en batch moeten worden gebruikt.</span><span class="sxs-lookup"><span data-stu-id="71362-103">If you create general journal lines from incoming document records, you must specify in the **Incoming Documents Setup** window which journal template and batch to use.</span></span>

<span data-ttu-id="71362-104">Als u niet wilt dat gebruikers facturen of dagboekregels maken van inkomende documentrecords, tenzij de documenten zijn goedgekeurd, moet u fiatteurs instellen in het venster **Fiatteurs inkomende documenten**.</span><span class="sxs-lookup"><span data-stu-id="71362-104">If you do not want users to create invoices or general journal lines from incoming document records unless the documents are first approved, you must set up approvers in the **Incoming Document Approvers** window.</span></span>

<span data-ttu-id="71362-105">Als u PDF- en afbeeldingsbestanden naar elektronische documenten wilt omzetten waarnaar u kunt converteren, bijvoorbeeld inkoopfacturen in Dynamics NAV, moet u eerst de OCR-functie instellen en de service inschakelen.</span><span class="sxs-lookup"><span data-stu-id="71362-105">To turn PDF and image files into electronic documents that you can convert to, for example, purchase invoices inside Dynamics NAV, you must first set up the OCR feature and enable the service.</span></span>

<span data-ttu-id="71362-106">Wanneer de functie Inkomende documenten is ingesteld, kunt u verschillende functies gebruiken om onkostenbewijzen te controleren, OCR-taken te beheren en inkomende documentbestanden handmatig of automatisch te converteren naar de relevante documenten of dagboekregels.</span><span class="sxs-lookup"><span data-stu-id="71362-106">When the Incoming Documents feature is set up, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="71362-107">De externe bestanden kunnen worden gekoppeld in elke procesfase, inclusief naar geboekte documenten en naar de resulterende leverancier, klant en grootboekposten.</span><span class="sxs-lookup"><span data-stu-id="71362-107">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span> <span data-ttu-id="71362-108">Zie voor meer informatie [Procedure: Inkomende documenten verwerken](across-process-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="71362-108">For more information, see [How to: Process Incoming Documents](across-process-income-documents.md).</span></span>

## <a name="to-set-up-the-incoming-documents-feature"></a><span data-ttu-id="71362-109">De functie Inkomende documenten instellen</span><span class="sxs-lookup"><span data-stu-id="71362-109">To set up the Incoming Documents feature</span></span>
1. <span data-ttu-id="71362-110">Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Instellingen van inkomende documenten** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="71362-110">In the top right corner, choose the **Search for Page or Report** icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="71362-111">Vul indien nodig de velden in.</span><span class="sxs-lookup"><span data-stu-id="71362-111">Fill in the fields as necessary.</span></span> <span data-ttu-id="71362-112">Kies een veld om een korte omschrijving van het veld of een koppeling naar meer informatie te lezen.</span><span class="sxs-lookup"><span data-stu-id="71362-112">Choose a field to read a short description of the field or link to more information.</span></span>

## <a name="to-set-up-approvers-of-incoming-document-records"></a><span data-ttu-id="71362-113">Fiatteurs van inkomende documentrecords instellen</span><span class="sxs-lookup"><span data-stu-id="71362-113">To set up approvers of incoming document records</span></span>
1. <span data-ttu-id="71362-114">Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Instellingen van inkomende documenten** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="71362-114">In the top right corner, choose the **Search for Page or Report** icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="71362-115">Kies in het venster **Instellingen van inkomende documenten** de actie **Fiatteurs**.</span><span class="sxs-lookup"><span data-stu-id="71362-115">In the **Incoming Documents Setup** window, choose the **Approvers** action.</span></span>

    <span data-ttu-id="71362-116">Het venster **Fiatteurs inkomende documenten** bevat alle gebruikers die zijn ingesteld in uw Dynamics NAV.</span><span class="sxs-lookup"><span data-stu-id="71362-116">The **Incoming Document Approvers** window shows all users that are set up in your Dynamics NAV .</span></span>  
3. <span data-ttu-id="71362-117">Selecteer een of meer gebruikers die een inkomend document kunnen goedkeuren voordat een verwant document of verwante dagboekregel kan worden gemaakt.</span><span class="sxs-lookup"><span data-stu-id="71362-117">Select one or more users that can approve an incoming document before a related document or journal line can be created.</span></span>

<span data-ttu-id="71362-118">Wanneer fiatteurs zijn ingesteld in het venster **Fiatteurs inkomende documenten**, kunnen alleen die gebruikers een inkomend document goedkeuren als het selectievakje **Goedkeuring vereist voor maken** is ingeschakeld in het venster **Instellingen inkomende documenten**.</span><span class="sxs-lookup"><span data-stu-id="71362-118">When approvers have been set up in the **Incoming Document Approvers** window, only those users can approve an incoming document if the **Require Approval To Create** check box in the **Incoming Documents Setup** window is selected.</span></span>

<span data-ttu-id="71362-119">**Opmerking**: deze goedkeuringsinstellingen zijn niet gerelateerd aan goedkeuringswerkstromen.</span><span class="sxs-lookup"><span data-stu-id="71362-119">**Note**: This approval setup is not related to approval workflows.</span></span> <span data-ttu-id="71362-120">Zie voor meer informatie [Procedure: Goedkeuringswerkstromen gebruiken](across-how-use-approval-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="71362-120">For more information, see [How to: Use Approval Workflows](across-how-use-approval-workflows.md).</span></span>

## <a name="to-set-up-an-ocr-service"></a><span data-ttu-id="71362-121">Een OCR-service instellen</span><span class="sxs-lookup"><span data-stu-id="71362-121">To set up an OCR service</span></span>
1. <span data-ttu-id="71362-122">Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Instellingen van OCR-service** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="71362-122">In the top right corner, choose the **Search for Page or Report** icon, enter **OCR Service Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="71362-123">Vul indien nodig de velden in.</span><span class="sxs-lookup"><span data-stu-id="71362-123">Fill in the fields as necessary.</span></span> <span data-ttu-id="71362-124">Kies een veld om een korte omschrijving van het veld of een koppeling naar meer informatie te lezen.</span><span class="sxs-lookup"><span data-stu-id="71362-124">Choose a field to read a short description of the field or link to more information.</span></span>


## <a name="to-encrypt-your-login-information"></a><span data-ttu-id="71362-125">Uw aanmeldgegevens versleutelen</span><span class="sxs-lookup"><span data-stu-id="71362-125">To encrypt your login information</span></span>
<span data-ttu-id="71362-126">We raden u aan de aanmeldgegevens te beveiligen die u invoert in het venster **Instellingen van OCR-service**.</span><span class="sxs-lookup"><span data-stu-id="71362-126">It is recommended that you protect the logon information that you enter in the **OCR Service Setup** window.</span></span> <span data-ttu-id="71362-127">U kunt gegevens op de server versleutelen door nieuwe encryptiesleutels te genereren of bestaande sleutels te importeren die u inschakelt op de serverinstantie die verbinding maakt met de database.</span><span class="sxs-lookup"><span data-stu-id="71362-127">You can encrypt data on the server by generating new or importing existing encryption keys that you enable on the server instance that connects to the database.</span></span>

1. <span data-ttu-id="71362-128">Kies in het venster **Instellingen van OCR-service** de actie **Versleutelingsbeheer**.</span><span class="sxs-lookup"><span data-stu-id="71362-128">In the **OCR Service Setup** window, choose the **Encryption Management** action.</span></span>
2. <span data-ttu-id="71362-129">Schakel in het venster **Beheer gegevensversleuteling** versleuteling van uw gegevens in.</span><span class="sxs-lookup"><span data-stu-id="71362-129">In the **Data Encryption Management** window, enable encryption of your data.</span></span>

## <a name="see-also"></a><span data-ttu-id="71362-130">Zie ook</span><span class="sxs-lookup"><span data-stu-id="71362-130">See Also</span></span>  
[<span data-ttu-id="71362-131">Inkomende documenten verwerken</span><span class="sxs-lookup"><span data-stu-id="71362-131">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="71362-132">Inkomende documenten</span><span class="sxs-lookup"><span data-stu-id="71362-132">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="71362-133">Inkoop beheren</span><span class="sxs-lookup"><span data-stu-id="71362-133">Manage Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="71362-134">Werken met Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="71362-134">Work With Dynamics NAV</span></span>](ui-work-product.md)


---
title: 'Procedure: Projectvoorraden beheren'
author: SorenGP
ms.custom: na
ms.date: 11/01/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 00b9ed8480f6b5ab9265beb0fe2dc0060b1c3192
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-manage-job-supplies"></a><span data-ttu-id="2da28-102">Procedure: Projectvoorraden beheren</span><span class="sxs-lookup"><span data-stu-id="2da28-102">How to: Manage Job Supplies</span></span>
<span data-ttu-id="2da28-103">Het beheren van projectgoederen van artikelen, services en onkosten is een integraal en zeer belangrijk aspect van de uitvoering van alle projecten.</span><span class="sxs-lookup"><span data-stu-id="2da28-103">Managing project supplies of items, services, and expenses is an integral and critical aspect of the execution of all jobs.</span></span> <span data-ttu-id="2da28-104">U kunt voorraadhoeveelheden gebruiken of projectspecifieke inkopen doen met behulp van inkooporders of inkoopfacturen.</span><span class="sxs-lookup"><span data-stu-id="2da28-104">You can use inventory quantities or make job-specific purchases using purchase orders or purchase invoices.</span></span> <span data-ttu-id="2da28-105">Stel bijvoorbeeld dat bij een serviceproject voor een computer een nieuwe schijf vereist is.</span><span class="sxs-lookup"><span data-stu-id="2da28-105">For example, a service job on a computer requires a new disk.</span></span> <span data-ttu-id="2da28-106">U maakt een inkoopfactuur om een nieuwe schijf te kopen en legt het project vast waarvoor deze wordt gebruikt.</span><span class="sxs-lookup"><span data-stu-id="2da28-106">You create a purchase invoice to buy a new disk and record the job that it will be used on.</span></span>

<span data-ttu-id="2da28-107">Als voor het inkoopproces de fysieke transactie niet apart hoeft te worden vastgelegd, kan een aankoop worden verwerkt in het venster **GB-dagboek project**.</span><span class="sxs-lookup"><span data-stu-id="2da28-107">If the purchase process does not require that the physical transaction be recorded separately, then a purchase may be processed in the **Job G/L Journal** window.</span></span> <span data-ttu-id="2da28-108">Zie voor meer informatie [Procedure: Gebruik vastleggen voor projecten](projects-how-record-job-usage.md).</span><span class="sxs-lookup"><span data-stu-id="2da28-108">For more information, see [How to: Record Usage for Jobs](projects-how-record-job-usage.md).</span></span>

## <a name="to-purchase-items-or-services-for-a-job"></a><span data-ttu-id="2da28-109">Artikelen of services inkopen voor een project</span><span class="sxs-lookup"><span data-stu-id="2da28-109">To purchase items or services for a job</span></span>
<span data-ttu-id="2da28-110">In de volgende procedure wordt beschreven hoe u een inkoopfactuur gebruikt om producten voor een project te kopen.</span><span class="sxs-lookup"><span data-stu-id="2da28-110">The following procedure shows how to use a purchase invoice to purchase products for a job.</span></span> <span data-ttu-id="2da28-111">Dezelfde stappen gelden bij gebruik van een inkooporder.</span><span class="sxs-lookup"><span data-stu-id="2da28-111">The same steps apply when using a purchase order.</span></span>  

1. <span data-ttu-id="2da28-112">Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Inkoopfacturen** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="2da28-112">In the top right corner, choose the **Search for Page or Report** icon, enter **Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="2da28-113">Kies de actie **Nieuw** en vul indien nodig de velden in.</span><span class="sxs-lookup"><span data-stu-id="2da28-113">Choose the **New** action and fill in the fields as necessary.</span></span> <span data-ttu-id="2da28-114">Zie voor meer informatie [Procedure: Inkopen vastleggen](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="2da28-114">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>
3. <span data-ttu-id="2da28-115">Selecteer in de velden **Projectnr.**</span><span class="sxs-lookup"><span data-stu-id="2da28-115">In the **Job No.**</span></span> <span data-ttu-id="2da28-116">en **Projecttaaknr.**</span><span class="sxs-lookup"><span data-stu-id="2da28-116">and **Job Task No.**</span></span> <span data-ttu-id="2da28-117">de gegevens van het project waarvoor u artikelen of services wilt inkopen.</span><span class="sxs-lookup"><span data-stu-id="2da28-117">fields, select the information of the job that you want to purchase items or services for.</span></span>  

    <span data-ttu-id="2da28-118">De waarde die u selecteert in het veld **Projectregelsoort** definieert of een planningsregel wordt gemaakt wanneer u het gebruik van het artikel boekt.</span><span class="sxs-lookup"><span data-stu-id="2da28-118">The value that you select in the **Job Line Type** field defines whether a planning line is created when you post the usage of the item.</span></span> <span data-ttu-id="2da28-119">Als het veld **Factureerbaar** bevat, worden projectplanningsregels gemaakt die gereed zijn om te worden gefactureerd aan de klant.</span><span class="sxs-lookup"><span data-stu-id="2da28-119">If the field contains **Billable**, then job planning lines that are ready to be invoiced to the customer are created.</span></span> <span data-ttu-id="2da28-120">Zie [Procedure: Projecten factureren](projects-how-invoice-jobs.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="2da28-120">For more information, see [How to: Invoice Jobs](projects-how-invoice-jobs.md).</span></span>

4. <span data-ttu-id="2da28-121">Kies de actie **Boeken**.</span><span class="sxs-lookup"><span data-stu-id="2da28-121">Choose the **Post** action.</span></span>

## <a name="to-view-the-value-of-purchases-for-a-job"></a><span data-ttu-id="2da28-122">De waarde van aankopen voor een project weergeven</span><span class="sxs-lookup"><span data-stu-id="2da28-122">To view the value of purchases for a job</span></span>  

1. <span data-ttu-id="2da28-123">Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Projecten** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="2da28-123">In the top right corner, choose the **Search for Page or Report** icon, enter **Jobs**, and then choose the related link.</span></span>
2. <span data-ttu-id="2da28-124">Open de betreffende projectkaart.</span><span class="sxs-lookup"><span data-stu-id="2da28-124">Open a relevant job card.</span></span>

    <span data-ttu-id="2da28-125">In het sneltabblad **Taken** bevat het veld **Openstaande orders** het totale uitstaande bedrag in de lokale valuta van voorraadartikelen en -services op inkoopdocumenten voor de projecttaakregel.</span><span class="sxs-lookup"><span data-stu-id="2da28-125">On the **Tasks** FastTab, the **Outstanding Orders** field shows the total outstanding amount, in local currency, of inventory items and services on purchase documents for the job task line.</span></span>  

    <span data-ttu-id="2da28-126">Het veld **Ontv./Niet gefact. bedrag** bevat de waarde van artikelen die worden geleverd op inkoopdocumenten, maar die nog niet zijn gefactureerd.</span><span class="sxs-lookup"><span data-stu-id="2da28-126">The **Amt. Rec. Not Invoiced** field shows the value of items delivered on purchase documents, but not yet invoiced.</span></span>  

3. <span data-ttu-id="2da28-127">Kies een van de velden om het venster **Inkoopregels** te openen. In dit venster kunt u informatie bekijken over de gerelateerde inkoopdocumentregels, inclusief welke artikelen of services zijn ontvangen.</span><span class="sxs-lookup"><span data-stu-id="2da28-127">Choose either of the fields to open the **Purchase Lines** window where you can review information about the related purchase document lines, including which items or services have been received.</span></span>

## <a name="to-post-a-job-related-expense"></a><span data-ttu-id="2da28-128">Projectkosten boeken</span><span class="sxs-lookup"><span data-stu-id="2da28-128">To post a job-related expense</span></span>  
<span data-ttu-id="2da28-129">Als u buitengewone of eenmalige projectkosten maakt, kunt u het venster **GB-dagboek project** gebruiken om ze direct te boeken naar de relevante projectrekening.</span><span class="sxs-lookup"><span data-stu-id="2da28-129">If you incur extraordinary or one-time job expenses, you can use the **Job G/L Journal** window to post them directly to the relevant job account.</span></span>

1. <span data-ttu-id="2da28-130">Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **GB-dagboeken voor project** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="2da28-130">In the top right corner, choose the **Search for Page or Report** icon, enter **Job G/L Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="2da28-131">Maak een nieuwe regel en voer gegevens over de kosten in, zoals informatie in de velden **Projectnr.**</span><span class="sxs-lookup"><span data-stu-id="2da28-131">Create a new line and enter information about the expense, including information in the **Job No.**</span></span> <span data-ttu-id="2da28-132">en **Projecttaaknr.**</span><span class="sxs-lookup"><span data-stu-id="2da28-132">and **Job Task No** fields.</span></span>  
3. <span data-ttu-id="2da28-133">Wanneer het dagboek compleet is, kiest u de actie **Boeken**.</span><span class="sxs-lookup"><span data-stu-id="2da28-133">When the journal is complete, choose the **Post** action.</span></span>


## <a name="see-also"></a><span data-ttu-id="2da28-134">Zie ook</span><span class="sxs-lookup"><span data-stu-id="2da28-134">See Also</span></span>
[<span data-ttu-id="2da28-135">Projecten beheren</span><span class="sxs-lookup"><span data-stu-id="2da28-135">Manage Projects</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="2da28-136">Financiën</span><span class="sxs-lookup"><span data-stu-id="2da28-136">Finance</span></span>](finance-setup.md)  
<span data-ttu-id="2da28-137">[Inkoop beheren](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="2da28-137">[Manage Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="2da28-138">[Verkoop beheren](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="2da28-138">[Manage Sales](sales-manage-sales.md)    </span></span>  
[<span data-ttu-id="2da28-139">Werken met Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="2da28-139">Work With Dynamics NAV</span></span>](ui-work-product.md)  


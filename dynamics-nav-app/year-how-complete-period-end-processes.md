---
title: Perioden afsluiten
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: ac1ed2d1dcf8bf780bda91fbf0a04e5c5e8d106a
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---
# <a name="close-periods"></a><span data-ttu-id="3d394-102">Perioden afsluiten</span><span class="sxs-lookup"><span data-stu-id="3d394-102">Close Periods</span></span>
<span data-ttu-id="3d394-103">U bent niet verplicht om perioden af te sluiten, maar er zijn echter vele maandeindeactiviteiten die u desgewenst kunt uitvoeren in de toepassing.</span><span class="sxs-lookup"><span data-stu-id="3d394-103">The application does not force you to close periods, however, there are many period-end (month-end) activities that can be performed in the application if you want.</span></span> <span data-ttu-id="3d394-104">In dit onderwerp vindt u een overzicht van deze processen en activiteiten die al dan niet nodig kunnen zijn voor uw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="3d394-104">This topic provides an overview of these processes and activities, which may or may not be necessary for your company.</span></span>

## <a name="general-ledger"></a><span data-ttu-id="3d394-105">Grootboek</span><span class="sxs-lookup"><span data-stu-id="3d394-105">General Ledger</span></span>
* <span data-ttu-id="3d394-106">Geef de boekingsperiode voor het gehele systeem of een specifieke gebruiker op.</span><span class="sxs-lookup"><span data-stu-id="3d394-106">Specify system-wide and user-specific posting period.</span></span>

    <span data-ttu-id="3d394-107">Hiermee worden de datums opgegeven tussen welke boekingen zijn toegestaan.</span><span class="sxs-lookup"><span data-stu-id="3d394-107">This specifies the dates between which postings are allowed.</span></span> <span data-ttu-id="3d394-108">Afhankelijk van uw zakelijke behoeften kunt u de boekingsdatumbereiken voor een gebruiker beperken aan het begin van het periode-eindeproces of op een later tijdstip aan het einde van de periode.</span><span class="sxs-lookup"><span data-stu-id="3d394-108">Depending on your business needs, you may want to restrict user posting date ranges at the start of the period-end process or at later time towards the end of the period.</span></span> <span data-ttu-id="3d394-109">Zie [Procedure: Boekingsperioden opgeven](finance-setup-how-specify-posting-periods.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="3d394-109">For more information, see [How to: Specify Posting Periods](finance-setup-how-specify-posting-periods.md).</span></span>
* <span data-ttu-id="3d394-110">Voer alle noodzakelijke grootboekherwaarderingen uit.</span><span class="sxs-lookup"><span data-stu-id="3d394-110">Make all necessary G/L adjustments.</span></span>
* <span data-ttu-id="3d394-111">Wijzig en boek periodieke dagboeken.</span><span class="sxs-lookup"><span data-stu-id="3d394-111">Update and post Recurring Journals.</span></span>
<!--* Process Consolidations-->
* <span data-ttu-id="3d394-112">Voer rapportageschema's als volgt uit:</span><span class="sxs-lookup"><span data-stu-id="3d394-112">Run account schedules as follows:</span></span>
  1. <span data-ttu-id="3d394-113">Open het venster **Rapportageschema** en kies de actie **Afdrukken**.</span><span class="sxs-lookup"><span data-stu-id="3d394-113">Open the **Account Schedule** window, and choose the **Print** action.</span></span>
  2. <span data-ttu-id="3d394-114">Vul het aanvraagvenster **Rapportageschema** in en kies de actie **Afdrukken**.</span><span class="sxs-lookup"><span data-stu-id="3d394-114">Fill the **Account Schedule** request window and choose the **Print** action.</span></span>

## <a name="sales--receivables"></a><span data-ttu-id="3d394-115">Verkopen en Klanten</span><span class="sxs-lookup"><span data-stu-id="3d394-115">Sales & Receivables</span></span>
* <span data-ttu-id="3d394-116">Boek alle verkooporders, facturen, creditnota's en retourorders.</span><span class="sxs-lookup"><span data-stu-id="3d394-116">Post all sales orders, invoices, credit memos, and return orders.</span></span>
* <span data-ttu-id="3d394-117">Boek alle ontvangstendagboeken.</span><span class="sxs-lookup"><span data-stu-id="3d394-117">Post all cash receipt journals.</span></span>
* <span data-ttu-id="3d394-118">Wijzig en boek periodieke dagboeken die zijn gerelateerd aan Verkoop.</span><span class="sxs-lookup"><span data-stu-id="3d394-118">Update and post recurring journals that are related to Sales & Receivables.</span></span>
* <span data-ttu-id="3d394-119">Reconcilieer klanten met het grootboek.</span><span class="sxs-lookup"><span data-stu-id="3d394-119">Reconcile accounts receivable to the general ledger.</span></span>
* <span data-ttu-id="3d394-120">Voer de batchverwerking **Gefactureerde verkooporders verwijderen** uit.</span><span class="sxs-lookup"><span data-stu-id="3d394-120">Run the **Delete Invoiced Sales Orders** batch job.</span></span>

## <a name="purchases--payables"></a><span data-ttu-id="3d394-121">Inkopen en Leveranciers</span><span class="sxs-lookup"><span data-stu-id="3d394-121">Purchases & Payables</span></span>
* <span data-ttu-id="3d394-122">Boek alle inkooporders, facturen, creditnota's en retourorders.</span><span class="sxs-lookup"><span data-stu-id="3d394-122">Post all purchase orders, invoices, credit memos, and return orders.</span></span>
* <span data-ttu-id="3d394-123">Boek alle betalingsdagboeken.</span><span class="sxs-lookup"><span data-stu-id="3d394-123">Post all payment journals.</span></span>
* <span data-ttu-id="3d394-124">Wijzig en boek periodieke dagboeken die zijn gerelateerd aan Inkoop.</span><span class="sxs-lookup"><span data-stu-id="3d394-124">Update and post recurring journals that are related to purchases & payables.</span></span>
* <span data-ttu-id="3d394-125">Voer het rapport **Vervallen betalingen** uit en reconcilieer leveranciers met het grootboek.</span><span class="sxs-lookup"><span data-stu-id="3d394-125">Run the **Aged Accounts Payable** report and reconcile accounts payable to the general ledger.</span></span>
* <span data-ttu-id="3d394-126">Voer de batchverwerking **Gefactureerde inkooporders verwijderen** uit.</span><span class="sxs-lookup"><span data-stu-id="3d394-126">Run the **Delete Invoiced Purchase Orders** batch job.</span></span>

<!-- ### Fixed Assets
* Post all maintenance costs have been posted through the fixed asset journals or invoices.
* Post adjustments.
* Post appreciation.
* Post depreciation.
* Update and post the recurring fixed asset journal.-->

<!--### Intercompany
* Process Intercompany Postings.-->

## <a name="calculate-and-process-sales-tax"></a><span data-ttu-id="3d394-127">Btw berekenen en verwerken</span><span class="sxs-lookup"><span data-stu-id="3d394-127">Calculate and Process Sales Tax</span></span>
*  <span data-ttu-id="3d394-128">Vul belastingaangiften in.</span><span class="sxs-lookup"><span data-stu-id="3d394-128">Complete Tax Statements.</span></span>

## <a name="see-also"></a><span data-ttu-id="3d394-129">Zie ook</span><span class="sxs-lookup"><span data-stu-id="3d394-129">See Also</span></span>
[<span data-ttu-id="3d394-130">Afsluitingsjaren en -perioden</span><span class="sxs-lookup"><span data-stu-id="3d394-130">Closing Years and Periods</span></span>](year-close-years-periods.md)  
[<span data-ttu-id="3d394-131">Boeken sluiten</span><span class="sxs-lookup"><span data-stu-id="3d394-131">Close Books</span></span>](year-close-books.md)


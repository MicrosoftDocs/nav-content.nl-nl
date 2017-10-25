---
title: "Bankafschriften importeren en reconciliëren"
description: "Banken bieden elektronische bankafschriften voor al uw financiële interacties. U kunt deze afschriften in het bank- of giroboek importeren."
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
ms.openlocfilehash: 21ac0420b8339bc94b6b13750838cd20ff9ba04e
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-import-and-reconcile-bank-statements"></a><span data-ttu-id="4d521-104">Procedure: Bankafschriften importeren en reconciliëren</span><span class="sxs-lookup"><span data-stu-id="4d521-104">How to: Import and Reconcile Bank Statements</span></span>
<span data-ttu-id="4d521-105">Banken bieden elektronische bankafschriften voor al uw financiële interacties.</span><span class="sxs-lookup"><span data-stu-id="4d521-105">Banks provide electronic bank statements for all your financial interactions.</span></span> <span data-ttu-id="4d521-106">U kunt deze afschriften in het bank- of giroboek importeren.</span><span class="sxs-lookup"><span data-stu-id="4d521-106">You can import these statements into the bank or giro journals.</span></span>  
  
 <span data-ttu-id="4d521-107">Het importbankafschrift wordt ondersteund door de volgende protocollen:</span><span class="sxs-lookup"><span data-stu-id="4d521-107">The import bank statement is supported by the following protocols:</span></span>  
  
-   <span data-ttu-id="4d521-108">Rabobank mut.asc</span><span class="sxs-lookup"><span data-stu-id="4d521-108">Rabobank mut.asc</span></span>  
  
-   <span data-ttu-id="4d521-109">Rabobank vvmut.ac</span><span class="sxs-lookup"><span data-stu-id="4d521-109">Rabobank vvmut.ac</span></span>  
  
-   <span data-ttu-id="4d521-110">Rabobank ASCII</span><span class="sxs-lookup"><span data-stu-id="4d521-110">Rabobank ASCII</span></span>  
  
-   <span data-ttu-id="4d521-111">SEPA CAMT</span><span class="sxs-lookup"><span data-stu-id="4d521-111">SEPA CAMT</span></span>  
  
 <span data-ttu-id="4d521-112">Zie Importprotocol voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="4d521-112">For more information, see Import Protocol.</span></span>  
  
### <a name="to-import-and-reconcile-bank-statements"></a><span data-ttu-id="4d521-113">Bankafschriften importeren en reconciliëren</span><span class="sxs-lookup"><span data-stu-id="4d521-113">To import and reconcile bank statements</span></span>  
  
1.  <span data-ttu-id="4d521-114">Kies het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Bankafschrift importeren** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="4d521-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Import Bank Statement**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="4d521-115">Selecteer in het venster **Importprotocoloverzicht** het vereiste importprotocol en kies vervolgens de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="4d521-115">In the **Import Protocol List** window, select the required import protocol, and then choose the **OK** button.</span></span>  
  
3.  <span data-ttu-id="4d521-116">Als u bankafschriften automatisch wilt laten reconciliëren tijdens het importeren, schakelt u op het sneltabblad **Opties** het selectievakje **Automatisch reconciliëren** in.</span><span class="sxs-lookup"><span data-stu-id="4d521-116">To reconcile the bank statements automatically when importing, on the **Options** FastTab, select the **Automatic Reconciliation** check box.</span></span>  
  
    > [!NOTE]  
    >  <span data-ttu-id="4d521-117">Deze functie werkt niet voor bankafschriftbestanden van de soort SEPA CAMT.</span><span class="sxs-lookup"><span data-stu-id="4d521-117">This function does not work for bank statement files of type SEPA CAMT.</span></span> <span data-ttu-id="4d521-118">Gebruik in plaats daarvan de actie **Automatisch afstemmen** in het venster **Bankreconciliatie**.</span><span class="sxs-lookup"><span data-stu-id="4d521-118">Instead, use the **Match Automatically** action in the **Bank Acc. Reconciliation** window.</span></span> <span data-ttu-id="4d521-119">Zie voor meer informatie [Procedure: Bankafschriftregels afstemmen met bankrekeningposten](how-to-match-bank-statement-lines-with-bank-account-ledger-entries.md)</span><span class="sxs-lookup"><span data-stu-id="4d521-119">For more information, see [How to: Match Bank Statement Lines with Bank Account Ledger Entries](how-to-match-bank-statement-lines-with-bank-account-ledger-entries.md).</span></span>  
  
4.  <span data-ttu-id="4d521-120">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="4d521-120">Choose the **OK** button.</span></span>  
  
5.  <span data-ttu-id="4d521-121">Als u het bestand wilt importeren dat het elektronische bankafschrift bevat, geeft u de bestandsnaam en het pad op en kiest u de knop **Openen**.</span><span class="sxs-lookup"><span data-stu-id="4d521-121">To import the file that contains the electronic bank statement, specify the file name and path, and then choose the **Open** button.</span></span>  
  
     <span data-ttu-id="4d521-122">Het elektronische bankafschrift wordt geïmporteerd in het bank- of giroboek.</span><span class="sxs-lookup"><span data-stu-id="4d521-122">The electronic bank statement is imported into the bank or giro journals.</span></span> <span data-ttu-id="4d521-123">Zie voor meer informatie [Elektronisch bankieren voor Nederland](dutch-electronic-banking.md).</span><span class="sxs-lookup"><span data-stu-id="4d521-123">For more information, see [Dutch Electronic Banking](dutch-electronic-banking.md).</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="4d521-124">Zie ook</span><span class="sxs-lookup"><span data-stu-id="4d521-124">See Also</span></span>  
 <span data-ttu-id="4d521-125">[Elektronisch bankieren voor Nederland](dutch-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="4d521-125">[Dutch Electronic Banking](dutch-electronic-banking.md) </span></span>  
 <span data-ttu-id="4d521-126">Importprotocol</span><span class="sxs-lookup"><span data-stu-id="4d521-126">Import Protocol</span></span>   
 <span data-ttu-id="4d521-127">Veld Reconciliatiestatus</span><span class="sxs-lookup"><span data-stu-id="4d521-127">Reconciliation Status Field</span></span>   
 <span data-ttu-id="4d521-128">Tabel KBG-afschriftregel</span><span class="sxs-lookup"><span data-stu-id="4d521-128">CBG Statement Line Table</span></span>   
 <span data-ttu-id="4d521-129">Venster Bank-/Giroboek</span><span class="sxs-lookup"><span data-stu-id="4d521-129">Bank-Giro Journal Window</span></span>   
 [<span data-ttu-id="4d521-130">Procedure: Bankafschriftregels afstemmen met bankrekeningposten</span><span class="sxs-lookup"><span data-stu-id="4d521-130">How to: Match Bank Statement Lines with Bank Account Ledger Entries</span></span>](how-to-match-bank-statement-lines-with-bank-account-ledger-entries.md)

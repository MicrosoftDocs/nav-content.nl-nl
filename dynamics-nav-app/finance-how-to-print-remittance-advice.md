---
title: 'Procedure: Overschrijvingsbericht afdrukken'
description: U kunt leveranciers helpen bij het uitvoeren van reconciliaties door het overschrijvingsbericht af te drukken voordat u een betalingsdagboek boekt en nadat u een betaling hebt geboekt.
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/26/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 7c7004ac5ded9436861bf5034f59a9c2bcd99dd0
ms.contentlocale: nl-nl
ms.lasthandoff: 12/01/2017

---

#<a name="how-to-print-remittance-advice"></a><span data-ttu-id="2c816-103">Procedure: Overschrijvingsbericht afdrukken</span><span class="sxs-lookup"><span data-stu-id="2c816-103">How to: Print Remittance Advice</span></span>
<span data-ttu-id="2c816-104">U kunt het overschrijvingsbericht afdrukken voordat u een betalingsdagboek boekt en nadat u een betaling hebt geboekt.</span><span class="sxs-lookup"><span data-stu-id="2c816-104">You can print remittance advice before posting a payment journal and after posting a payment.</span></span> <span data-ttu-id="2c816-105">Op het bericht worden de nummers van de leverancierfactuur weergegeven waarmee leveranciers reconciliaties kunnen uitvoeren.</span><span class="sxs-lookup"><span data-stu-id="2c816-105">This advice displays vendor invoice numbers, which helps vendors to perform reconciliations.</span></span>

##<a name="to-print-remittance-advice"></a><span data-ttu-id="2c816-106">Overschrijvingsbericht afdrukken</span><span class="sxs-lookup"><span data-stu-id="2c816-106">To print remittance advice</span></span>
1. <span data-ttu-id="2c816-107">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Betalingsdagboeken** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="2c816-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="2c816-108">In het venster **Betalingsdagboek** selecteert u de betaling waarvoor het overschrijvingsbericht wilt afdrukken.</span><span class="sxs-lookup"><span data-stu-id="2c816-108">In the **Payment Journal** window, select the payment for which remittance advice must be printed.</span></span>  
3. <span data-ttu-id="2c816-109">Kies de actie **Overschrijvingsbericht afdrukken**.</span><span class="sxs-lookup"><span data-stu-id="2c816-109">Choose the **Print Remittance Advice** action.</span></span>  
4. <span data-ttu-id="2c816-110">Kies de gewenste filters in de batchverwerking **Overschrijvingsbericht - dagboek** op het sneltabblad **Fin. dagboekregel**.</span><span class="sxs-lookup"><span data-stu-id="2c816-110">In the **Remittance Advice - Journal** batch job, on the **Fen. Journal Line** FastTab, choose the appropriate filters.</span></span>  
  
    >[!Note]
    > <span data-ttu-id="2c816-111">U kunt filteren met het externe documentnummer van de leverancier om betalingen af te stemmen met facturen.</span><span class="sxs-lookup"><span data-stu-id="2c816-111">You can filter using the vendor's external document number to match payments with invoices.</span></span>

5. <span data-ttu-id="2c816-112">Selecteer op het sneltabblad **Leverancier** de gewenste filters.</span><span class="sxs-lookup"><span data-stu-id="2c816-112">On the **Vendor** FastTab, choose the appropriate filters.</span></span>  
6. <span data-ttu-id="2c816-113">Kies **Afdrukken** om het rapport af te drukken of kies **Voorbeeld** om het nu weer te geven.</span><span class="sxs-lookup"><span data-stu-id="2c816-113">Choose **Print** to print the report, or choose **Preview** to view it now.</span></span>  

## <a name="using-remittance-advice-reports"></a><span data-ttu-id="2c816-114">Rapporten met overschrijvingsberichten gebruiken</span><span class="sxs-lookup"><span data-stu-id="2c816-114">Using Remittance Advice Reports</span></span>
<span data-ttu-id="2c816-115">De volgende tabel beschrijft de rapporten die u met overschrijvingsberichten kunt gebruiken:</span><span class="sxs-lookup"><span data-stu-id="2c816-115">The following table describes the reports that you can use with remittance advice:</span></span>

|<span data-ttu-id="2c816-116">Rapporteren</span><span class="sxs-lookup"><span data-stu-id="2c816-116">Report</span></span>|<span data-ttu-id="2c816-117">Description</span><span class="sxs-lookup"><span data-stu-id="2c816-117">Description</span></span>|
|----|----|
|<span data-ttu-id="2c816-118">Rapport Overschrijvingsbericht - dagboek</span><span class="sxs-lookup"><span data-stu-id="2c816-118">Remittance Advice - Journal Report</span></span>|<span data-ttu-id="2c816-119">Dit rapport geeft aan welke documenten in de betaling zijn opgenomen.</span><span class="sxs-lookup"><span data-stu-id="2c816-119">This report indicates which documents are included in the payment.</span></span> <span data-ttu-id="2c816-120">Voor dagboekregels kunt u de dagboeksjabloon en de dagboekbatch opgeven waaruit de overschrijvingsberichten moeten worden afgedrukt, de eerste datum van de activiteit kiezen om af te drukken en filtereren op een documentnummer.</span><span class="sxs-lookup"><span data-stu-id="2c816-120">For general journal lines, you can specify the journal template and journal batch from which the remittance advices will be printed, the date of the first activity to print, and filter on a document number.</span></span> <span data-ttu-id="2c816-121">Voor leveranciers kunt u de leveranciernummers opgeven die u wilt opnemen in het rapport.</span><span class="sxs-lookup"><span data-stu-id="2c816-121">For vendors, you can enter the vendor numbers to include in the report.</span></span> |
|<span data-ttu-id="2c816-122">Rapport Overschrijvingsbericht - posten</span><span class="sxs-lookup"><span data-stu-id="2c816-122">Remittance Advice - Entries Report</span></span>| <span data-ttu-id="2c816-123">Dit rapport geeft aan welke documenten in de betaling zijn opgenomen.</span><span class="sxs-lookup"><span data-stu-id="2c816-123">This report indicates which documents are included in the payment.</span></span> <span data-ttu-id="2c816-124">U kunt de rapportinhoud bepalen met behulp van filters.</span><span class="sxs-lookup"><span data-stu-id="2c816-124">You define the report contents by setting filters.</span></span> <span data-ttu-id="2c816-125">Stel extra velden in op het tabblad door het veld **Veld** te kiezen.</span><span class="sxs-lookup"><span data-stu-id="2c816-125">You can set additional fields on the tab by choosing the **Field** field.</span></span> <span data-ttu-id="2c816-126">Voor leveranciersposten kunt u opgeven welke leveranciers u in het rapport wilt opnemen, de datum van de eerste activiteit om af te drukken, de valuta en het op te nemen volgnummer.</span><span class="sxs-lookup"><span data-stu-id="2c816-126">For vendor ledger entries, you can specify the vendors to include in the report, the date of the first activity to print, the currency, and the entry number to include.</span></span> |

> [!Note]
> <span data-ttu-id="2c816-127">Het rapport Overschrijvingsbericht - dagboek ondersteunt geen scenario's met verschillende valuta's of betalingstoleranties.</span><span class="sxs-lookup"><span data-stu-id="2c816-127">The Remittance Advice - Journal Report does not support cross currency application scenarios or payment tolerances.</span></span> <span data-ttu-id="2c816-128">Zie [Procedure: Vereffening van posten in verschillende valuta's inschakelen](finance-how-enable-application-ledger-entries-different-currencies.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="2c816-128">For more information, see [How to: Enable Application of Ledger Entries in Different Currencies](finance-how-enable-application-ledger-entries-different-currencies.md).</span></span>

> [!Tip]
> <span data-ttu-id="2c816-129">Voor meer informatie over het werken met rapporten zie [Controlelijsten weergeven vóór boeken](ui-how-view-test-reports-posting.md), [Werken met rapporten](ui-work-report.md) en [Gegevens zoeken, filteren en sorteren](ui-enter-criteria-filters.md).</span><span class="sxs-lookup"><span data-stu-id="2c816-129">For more information about how to work with reports, see [Viewing Test Reports before Posting](ui-how-view-test-reports-posting.md), [Work with Reports](ui-work-report.md), and [Searching, Filtering, and Sorting Data](ui-enter-criteria-filters.md).</span></span>

##<a name="see-also"></a><span data-ttu-id="2c816-130">Zie ook</span><span class="sxs-lookup"><span data-stu-id="2c816-130">See Also</span></span>  
[<span data-ttu-id="2c816-131">Welkom bij Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="2c816-131">Welcome to Dynamics NAV</span></span>](across-get-started.md)

---
title: Leveranciersbetalingen elektronisch versturen in de betalingsindeling SEPA ISO 20022
description: In [!INCLUDE[navnow](../../includes/navnow_md.md)] kunt u elektronische SEPA-leveranciersbetalingen (Single Euro Payments Area) ISO 20022 maken en verzenden.
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
ms.openlocfilehash: 6f44cb5380481cc73116790dbd61d459ea7384b3
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-submit-vendor-payments-electronically-in-sepa-iso-20022-payment-format"></a><span data-ttu-id="0491e-103">Procedure: Leverancierbetalingen elektronisch versturen in SEPA ISO 20022-betalingsindeling</span><span class="sxs-lookup"><span data-stu-id="0491e-103">How to: Submit Vendor Payments Electronically in SEPA ISO 20022 Payment Format</span></span>
<span data-ttu-id="0491e-104">In [!INCLUDE[navnow](../../includes/navnow_md.md)] kunt u elektronische SEPA-leveranciersbetalingen (Single Euro Payments Area) ISO 20022 maken en verzenden.</span><span class="sxs-lookup"><span data-stu-id="0491e-104">In [!INCLUDE[navnow](../../includes/navnow_md.md)], you can create and submit Single Euro Payments Area (SEPA) ISO 20022 vendor payments electronically.</span></span>  
  
 <span data-ttu-id="0491e-105">Voordat u SEPA-leveranciersbetalingen kunt maken en verzenden, moet u SEPA-betalingen activeren.</span><span class="sxs-lookup"><span data-stu-id="0491e-105">Before you can create and submit SEPA vendor payments, you must enable SEPA payments.</span></span> <span data-ttu-id="0491e-106">Zie [Procedure: SEPA-betalingen activeren](how-to-activate-sepa-payments.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="0491e-106">For more information, see [How to: Activate SEPA Payments](how-to-activate-sepa-payments.md).</span></span>  
  
### <a name="to-submit-vendor-payments-electronically-in-sepa-iso-20022-payment-format"></a><span data-ttu-id="0491e-107">Leverancierbetalingen elektronisch versturen in SEPA ISO 20022-betalingsindeling</span><span class="sxs-lookup"><span data-stu-id="0491e-107">To submit vendor payments electronically in SEPA ISO 20022 payment format</span></span>  
  
1.  <span data-ttu-id="0491e-108">Kies het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Telebankieren - bankoverzicht** in en kies de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="0491e-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Telebank-Bank Overview**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="0491e-109">Selecteer de relevante bankrekening en kies vervolgens op het tabblad **Navigeren** in de groep **Telebankieren** de optie **Voorstel**.</span><span class="sxs-lookup"><span data-stu-id="0491e-109">Select the relevant bank account, and then, on the **Navigate** tab, in the **Telebank** group, choose **Proposal**.</span></span>  
  
3.  <span data-ttu-id="0491e-110">Selecteer de relevante leveranciersbankrekening en kies vervolgens op het tabblad **Navigeren** in de groep **Voorstel** de optie **Posten ophalen**.</span><span class="sxs-lookup"><span data-stu-id="0491e-110">Select the relevant vendor bank account, and then, on the **Navigate** tab, in the **Proposal** group, choose **Get Entries**.</span></span>  
  
4.  <span data-ttu-id="0491e-111">Vul op het sneltabblad **Opties** van de batchverwerking **Voorstelposten ophalen** de velden in, zoals wordt beschreven in de volgende tabel.</span><span class="sxs-lookup"><span data-stu-id="0491e-111">In the **Get Proposal Entries** batch job, on the **Options** FastTab, fill in the fields as described in the following table.</span></span>  
  
    |<span data-ttu-id="0491e-112">Veld</span><span class="sxs-lookup"><span data-stu-id="0491e-112">Field</span></span>|<span data-ttu-id="0491e-113">Description</span><span class="sxs-lookup"><span data-stu-id="0491e-113">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="0491e-114">**Valutadatum**</span><span class="sxs-lookup"><span data-stu-id="0491e-114">**Currency Date**</span></span>|<span data-ttu-id="0491e-115">Hier geeft u de valutadatum op.</span><span class="sxs-lookup"><span data-stu-id="0491e-115">Specify the currency date.</span></span>|  
    |<span data-ttu-id="0491e-116">**Vervaldatum contantkort.**</span><span class="sxs-lookup"><span data-stu-id="0491e-116">**Pmt. Discount Date**</span></span>|<span data-ttu-id="0491e-117">Hier geeft u de vervaldatum voor de contantkorting op.</span><span class="sxs-lookup"><span data-stu-id="0491e-117">Specify the payment discount date.</span></span>|  
  
5.  <span data-ttu-id="0491e-118">Selecteer in het sneltabblad **Transactiemodus** de gewenste filters.</span><span class="sxs-lookup"><span data-stu-id="0491e-118">On the **Transaction Mode** FastTab, select the appropriate filters.</span></span>  
  
6.  <span data-ttu-id="0491e-119">Selecteer in het sneltabblad **Klantenpost** de gewenste filters.</span><span class="sxs-lookup"><span data-stu-id="0491e-119">On the **Cust. Ledger Entry** FastTab, select the appropriate filters.</span></span>  
  
7.  <span data-ttu-id="0491e-120">Selecteer op het sneltabblad **Leverancierspost** het filter **Leveranciersnr.** en selecteer een leveranciersnummer.</span><span class="sxs-lookup"><span data-stu-id="0491e-120">On the **Vendor Ledger Entry** FastTab, select the **Vendor No.** filter, and then select a vendor number.</span></span>  
  
    > [!NOTE]  
    >  <span data-ttu-id="0491e-121">Selecteer eventuele overige vereiste filters.</span><span class="sxs-lookup"><span data-stu-id="0491e-121">Select other appropriate filters if required.</span></span>  
  
8.  <span data-ttu-id="0491e-122">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="0491e-122">Choose the **OK** button.</span></span>  
  
     <span data-ttu-id="0491e-123">De voorstelregels worden opgenomen in het venster **Telebankierenvoorstel**.</span><span class="sxs-lookup"><span data-stu-id="0491e-123">The proposal lines populate in the **Telebank Proposal** window.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="0491e-124">Zie ook</span><span class="sxs-lookup"><span data-stu-id="0491e-124">See Also</span></span>  
 <span data-ttu-id="0491e-125">[Procedure: SEPA-betalingen activeren](how-to-activate-sepa-payments.md) </span><span class="sxs-lookup"><span data-stu-id="0491e-125">[How to: Activate SEPA Payments](how-to-activate-sepa-payments.md) </span></span>  
 <span data-ttu-id="0491e-126">[Single EURO Payments Area (SEPA)](single-euro-payments-area-sepa-.md) </span><span class="sxs-lookup"><span data-stu-id="0491e-126">[Single EURO Payments Area (SEPA)](single-euro-payments-area-sepa-.md) </span></span>  
 <span data-ttu-id="0491e-127">Venster Telebankieren - bankoverzicht</span><span class="sxs-lookup"><span data-stu-id="0491e-127">Telebank - Bank Overview Window</span></span>   
 <span data-ttu-id="0491e-128">Venster Telebankierenvoorstel</span><span class="sxs-lookup"><span data-stu-id="0491e-128">Telebank Proposal Window</span></span>

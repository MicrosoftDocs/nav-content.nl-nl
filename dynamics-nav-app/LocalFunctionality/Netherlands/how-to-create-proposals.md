---
title: Voorstellen maken
description: Voorstellen kunnen handmatig of automatisch worden gegenereerd op basis van leveranciers- of klantenposten.
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
ms.openlocfilehash: a73c3d1bc53f787a36f5d16e73879f387e953306
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-proposals"></a><span data-ttu-id="8d5f5-103">Procedure: Voorstellen maken</span><span class="sxs-lookup"><span data-stu-id="8d5f5-103">How to: Create Proposals</span></span>
<span data-ttu-id="8d5f5-104">Voorstellen kunnen handmatig of automatisch worden gegenereerd op basis van leveranciers- of klantenposten.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-104">Proposals can be generated manually or automatically based on either vendor or customer ledger entries.</span></span>  
  
> [!IMPORTANT]  
>  <span data-ttu-id="8d5f5-105">Als u een voorstel maakt, moet u het veld **Rekeninghouder** in de vensters Bankrekening leverancier en Bankrekening klant gebruiken.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-105">To create a proposal, you must use the **Owner Information** field in the Vendor Bank Account Card and Customer Bank Account Card windows.</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="8d5f5-106">U kunt op elk moment en op elk niveau, voorafgaand aan de verwerking van een voorstel, de transactiewijze en bankrekening wijzigen.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-106">At any time and at any level, before processing a proposal, the transaction mode and bank account can be modified.</span></span> <span data-ttu-id="8d5f5-107">Op het laagste niveau in de desbetreffende leveranciers- of klantenposten.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-107">At the lowest level on the relevant vendor or customer ledger entries.</span></span>  
  
#### <a name="to-create-proposals-manually"></a><span data-ttu-id="8d5f5-108">Handmatig voorstellen maken</span><span class="sxs-lookup"><span data-stu-id="8d5f5-108">To create proposals manually</span></span>  
  
1.  <span data-ttu-id="8d5f5-109">Kies het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Telebankieren - bankoverzicht** in en kies de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Telebank - Bank Overview**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="8d5f5-110">Selecteer de gewenste bankrekening.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-110">Select the relevant bank account.</span></span> <span data-ttu-id="8d5f5-111">Kies op het tabblad **Acties** in de groep **Telebankieren** de optie **Voorstel**.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-111">On the **Actions** tab, in the **Telebank** group, choose **Proposal**.</span></span>  
  
3.  <span data-ttu-id="8d5f5-112">U moet minimaal de velden **Rekeningsoort**, **Rekeningnr.**, **Transactiewijze**, **Bankrekeningnr.** en **Bedrag** invullen.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-112">At a minimum, you must fill in the **Account Type**, **Account No.**, **Transaction Mode**, **Bank Account No.**, and **Amount** fields.</span></span>  
  
       
  
4.  <span data-ttu-id="8d5f5-113">Als u de detailregels van het voorstel wilt bekijken of aanpassen, kies u in het gedeelte **Regels** op de werkbalk **Detailinformatie**.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-113">If you want to view or adjust the proposal's detail lines, in the **Lines** part, in the toolbar, choose **Detail Information**.</span></span> <span data-ttu-id="8d5f5-114">Als u wilt terugkeren naar het voorstel, sluit u het venster **Voorsteldetailregel**.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-114">To return to the proposal, close the **Proposal Detail Line** window.</span></span>  
  
#### <a name="to-create-proposals-automatically-from-sales"></a><span data-ttu-id="8d5f5-115">Automatisch voorstellen maken op basis van verkoop</span><span class="sxs-lookup"><span data-stu-id="8d5f5-115">To create proposals automatically from sales</span></span>  
  
1.  <span data-ttu-id="8d5f5-116">Stel voor de klant die de factuur heeft verstuurd een kaart in met de juiste waarden voor de velden **Valutacode**, **Transactiewijze** en **Bankrekening**.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-116">Set up a card for the customer who sent the invoice with appropriate values for the **Currency Code**, **Transaction Mode**, and **Bank Account** fields.</span></span>  
  
       
  
2.  <span data-ttu-id="8d5f5-117">Maak een verkoopfactuur of creditnota, vul de klant en relevante items in en boek de factuur.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-117">Create a sales invoice or credit memo, enter the customer and relevant items and post the invoice.</span></span> <span data-ttu-id="8d5f5-118">Controleer of de velden **Valutacode**, **Transactiewijze** en **Bankrekening** van de factuur/creditnota de juiste waarden bevatten.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-118">Check whether the **Currency Code**, **Transaction Mode**, and **Bank Account** fields of the invoice/credit memo contain appropriate values.</span></span> <span data-ttu-id="8d5f5-119">Standaard worden deze gekopieerd vanuit de klantenkaart.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-119">By default, they will be copied from the customer card.</span></span>  
  
       
  
3.  <span data-ttu-id="8d5f5-120">Kies het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Telebankieren - bankoverzicht** in en kies de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-120">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Telebank - Bank Overview**, and then choose the related link.</span></span>  
  
4.  <span data-ttu-id="8d5f5-121">Selecteer de gewenste bankrekening.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-121">Select the relevant bank account.</span></span> <span data-ttu-id="8d5f5-122">Kies op het tabblad **Acties** in de groep **Telebankieren** de optie **Voorstel**.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-122">On the **Actions** tab, in the **Telebank** group, choose **Proposal**.</span></span>  
  
5.  <span data-ttu-id="8d5f5-123">Klik op het tabblad **Acties** in de groep **Voorstel** op **Posten ophalen**.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-123">On the **Actions** tab, in the **Proposal** group, choose **Get Entries**.</span></span>  
  
     <span data-ttu-id="8d5f5-124">U kunt de batchverwerking Voorstelposten ophalen gebruiken om voorstelregels te genereren op basis van relevante klantenposten.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-124">You can use the Get Proposal Entries Batch Job batch job to generate proposal lines based on relevant customer ledger entries.</span></span>  
  
    > [!NOTE]  
    >  <span data-ttu-id="8d5f5-125">Alleen voor posten die een transactiewijze van het rekeningsoort **Klant** hebben en die aan de actieve bankrekening zijn gekoppeld, worden voorstelregels gemaakt.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-125">Only proposal lines will be created for ledger entries that have a transaction mode of account type **Customer** and a link to the active bank account.</span></span>  
  
6.  <span data-ttu-id="8d5f5-126">Als u de detailregels van het voorstel wilt bekijken of aanpassen, kies u in het gedeelte **Regels** op de werkbalk **Detailinformatie**.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-126">If you want to view or adjust the proposal's detail lines, in the **Lines** part, in the toolbar, choose **Detail Information**.</span></span> <span data-ttu-id="8d5f5-127">Als u wilt terugkeren naar het voorstel, sluit u het venster **Voorsteldetailregel**.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-127">To return to the proposal, close the **Proposal Detail Line** window.</span></span>  
  
#### <a name="to-create-proposals-automatically-from-purchases"></a><span data-ttu-id="8d5f5-128">Automatisch voorstellen maken op basis van inkoop</span><span class="sxs-lookup"><span data-stu-id="8d5f5-128">To create proposals automatically from purchases</span></span>  
  
1.  <span data-ttu-id="8d5f5-129">Stel voor de leverancier die de factuur heeft verstuurd een kaart in met de juiste waarden voor de velden **Valutacode**, **Transactiewijze** en **Bankrekening**.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-129">Set up a card for the vendor that sent the invoice with appropriate values for **Currency Code**, **Transaction Mode**, and **Bank Account** fields.</span></span>  
  
       
  
2.  <span data-ttu-id="8d5f5-130">Maak een inkoopfactuur of creditnota en voer de leverancier en relevante items in.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-130">Create a purchase invoice or credit memo, enter the vendor and relevant items.</span></span> <span data-ttu-id="8d5f5-131">Boek de factuur.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-131">Post the invoice.</span></span> <span data-ttu-id="8d5f5-132">Controleer of de velden **Valutacode**, **Transactiewijze** en **Bankrekening** van de factuur/creditnota de juiste waarden bevatten.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-132">Check whether the **Currency Code**, **Transaction Mode**, and **Bank Account** fields of the invoice/credit memo contain appropriate values.</span></span> <span data-ttu-id="8d5f5-133">Standaard worden deze gekopieerd vanuit de leverancierskaart.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-133">By default, they will be copied from the vendor card.</span></span>  
  
       
  
3.  <span data-ttu-id="8d5f5-134">Kies het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Telebankieren - bankoverzicht** in en kies de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-134">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Telebank - Bank Overview**, and then choose the related link.</span></span>  
  
4.  <span data-ttu-id="8d5f5-135">Selecteer de gewenste bankrekening.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-135">Select the relevant bank account.</span></span> <span data-ttu-id="8d5f5-136">Kies op het tabblad **Acties** in de groep **Telebankieren** de optie **Voorstel**.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-136">On the **Actions** tab, in the **Telebank** group, choose **Proposal**.</span></span>  
  
5.  <span data-ttu-id="8d5f5-137">Klik op het tabblad **Acties** in de groep **Voorstel** op **Posten ophalen**.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-137">On the **Actions** tab, in the **Proposal** group, choose **Get Entries**.</span></span>  
  
     <span data-ttu-id="8d5f5-138">U kunt de batchverwerking Voorstelposten ophalen gebruiken om voorstelregels te genereren op basis van relevante leveranciersposten.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-138">You can use the Get Proposal Entries Batch Job batch job to generate proposal lines based on relevant vendor ledger entries.</span></span>  
  
    > [!NOTE]  
    >  <span data-ttu-id="8d5f5-139">Alleen voor posten die een transactiewijze van het rekeningsoort **Leverancier** hebben en die aan de actieve bankrekening zijn gekoppeld, worden voorstelregels gemaakt.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-139">Only proposal lines will be created for ledger entries that have a transaction mode of account type **Vendor** and a link to the active bank account.</span></span>  
  
6.  <span data-ttu-id="8d5f5-140">Als u de detailregels van het voorstel wilt bekijken of aanpassen, kies u in het gedeelte **Regels** op de werkbalk **Detailinformatie**.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-140">If you want to view or adjust the proposal's detail lines, in the **Lines** part, in the toolbar, choose **Detail Information**.</span></span> <span data-ttu-id="8d5f5-141">Als u wilt terugkeren naar het voorstel, sluit u het venster **Voorsteldetailregel**.</span><span class="sxs-lookup"><span data-stu-id="8d5f5-141">To return to the proposal, close the **Proposal Detail Line** window.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="8d5f5-142">Zie ook</span><span class="sxs-lookup"><span data-stu-id="8d5f5-142">See Also</span></span>  
 <span data-ttu-id="8d5f5-143">[Procedure: Nieuwe klanten registreren](how-to-register-new-customers.md) </span><span class="sxs-lookup"><span data-stu-id="8d5f5-143">[How to: Register New Customers](how-to-register-new-customers.md) </span></span>  
 <span data-ttu-id="8d5f5-144">[Procedure: Verkoop factureren](how-to-invoice-sales.md) </span><span class="sxs-lookup"><span data-stu-id="8d5f5-144">[How to: Invoice Sales](how-to-invoice-sales.md) </span></span>  
 <span data-ttu-id="8d5f5-145">[Inkoopfacturen vastleggen](record-purchase-invoices.md) </span><span class="sxs-lookup"><span data-stu-id="8d5f5-145">[Record Purchase Invoices](record-purchase-invoices.md) </span></span>  
 [<span data-ttu-id="8d5f5-146">Procedure: Betalingsrun maken en exporteren</span><span class="sxs-lookup"><span data-stu-id="8d5f5-146">How to: Create and Export Payment History</span></span>](how-to-create-and-export-payment-history.md)

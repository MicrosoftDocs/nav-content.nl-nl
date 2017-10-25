---
title: Betalingsscenario 1 - binnenlandse betalingen (LV naar LV).
description: U kunt telebankieren gebruiken voor handel met binnenlandse en buitenlandse klanten en leveranciers. Dit onderwerp beschrijft een scenario waarin de handel geschiedt met binnenlandse klanten en leveranciers.
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
ms.openlocfilehash: 40693482dda3bb293f21ca28d2b0646bd083fcfe
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="payment-scenario-1---domestic-payments-lcy-to-lcy"></a><span data-ttu-id="a368c-104">Betalingsscenario 1 - binnenlandse betalingen (LV naar LV).</span><span class="sxs-lookup"><span data-stu-id="a368c-104">Payment Scenario 1 - Domestic Payments (LCY to LCY)</span></span>
<span data-ttu-id="a368c-105">U kunt telebankieren gebruiken voor handel met binnenlandse en buitenlandse klanten en leveranciers.</span><span class="sxs-lookup"><span data-stu-id="a368c-105">You can use telebanking for trade with domestic and foreign customers and vendors.</span></span> <span data-ttu-id="a368c-106">Dit onderwerp beschrijft een scenario waarin de handel geschiedt met binnenlandse klanten en leveranciers.</span><span class="sxs-lookup"><span data-stu-id="a368c-106">This topic describes a scenario where the trade is with domestic customers and vendors.</span></span>  
  
 <span data-ttu-id="a368c-107">De volgende lijst bevat de belangrijkste stappen:</span><span class="sxs-lookup"><span data-stu-id="a368c-107">The following list describes the main steps:</span></span>  
  
1.  <span data-ttu-id="a368c-108">Leverancier/klant maken.</span><span class="sxs-lookup"><span data-stu-id="a368c-108">Create Vendor/Customer.</span></span>  
  
2.  <span data-ttu-id="a368c-109">Bankrekening leverancier/klant maken.</span><span class="sxs-lookup"><span data-stu-id="a368c-109">Create Vendor/Customer Bank Account.</span></span>  
  
3.  <span data-ttu-id="a368c-110">Inkoopfactuur voor leverancier of verkoopfactuur voor klant maken en boeken.</span><span class="sxs-lookup"><span data-stu-id="a368c-110">Create and Post Purchase Invoice for Vendor or Sales Invoice for Customer.</span></span>  
  
4.  <span data-ttu-id="a368c-111">Voorstel maken.</span><span class="sxs-lookup"><span data-stu-id="a368c-111">Create Proposal.</span></span>  
  
5.  <span data-ttu-id="a368c-112">Betaalrun maken.</span><span class="sxs-lookup"><span data-stu-id="a368c-112">Create Payment History.</span></span>  
  
6.  <span data-ttu-id="a368c-113">Betaalrun exporteren.</span><span class="sxs-lookup"><span data-stu-id="a368c-113">Export Payment History.</span></span>  
  
7.  <span data-ttu-id="a368c-114">Bankafschrift importeren.</span><span class="sxs-lookup"><span data-stu-id="a368c-114">Import Bank Statement.</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="a368c-115">In de volgende voorbeelden zijn enkele standaard-CRONUS-gegevens gebruikt.</span><span class="sxs-lookup"><span data-stu-id="a368c-115">In the examples below some standard CRONUS data is being used.</span></span> <span data-ttu-id="a368c-116">En in plaats van een leverancier/klant en een Bankrekening leverancier/klant te maken, zou u ook bestaande gegevens kunnen gebruiken.</span><span class="sxs-lookup"><span data-stu-id="a368c-116">Likewise instead of creating a vendor/customer and a vendor/customer bank account you could use existing data.</span></span>  
  
## <a name="create-vendorcustomer"></a><span data-ttu-id="a368c-117">Leverancier/klant maken</span><span class="sxs-lookup"><span data-stu-id="a368c-117">Create Vendor/Customer</span></span>  
 <span data-ttu-id="a368c-118">Maak een leverancier/klant en vul alle noodzakelijke gegevens in.</span><span class="sxs-lookup"><span data-stu-id="a368c-118">Create vendor/customer and enter all necessary information.</span></span> <span data-ttu-id="a368c-119">Besteed extra aandacht aan het volgende:</span><span class="sxs-lookup"><span data-stu-id="a368c-119">Special attention should be paid to:</span></span>  
  
-   <span data-ttu-id="a368c-120">**Valutacode**: laat dit veld leeg, het wordt ingesteld op de lokale valuta (LV).</span><span class="sxs-lookup"><span data-stu-id="a368c-120">**Currency Code**: leave empty - i.e. it is set to the local currency (LCY).</span></span>  
  
-   <span data-ttu-id="a368c-121">**Transactiewijze**: selecteer een geschikte standaardtransactiewijze, dat wil zeggen, een transactiewijze die geschikt is voor betalingen in lokale valuta voor uw bank.</span><span class="sxs-lookup"><span data-stu-id="a368c-121">**Transaction Mode**: select an appropriate, default transaction mode - i.e. one that can deal with local currency payments for your bank.</span></span>  
  
-   <span data-ttu-id="a368c-122">**Bankrekening van voorkeur**: selecteer een geschikte standaardbankrekening van leveranciers/klanten met dezelfde valutacode als de leverancier/klant zelf.</span><span class="sxs-lookup"><span data-stu-id="a368c-122">**Preferred Bank Account**: select an appropriate, default vendor/customer bank account having the same Currency Code as the vendor/customer itself.</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="a368c-123">U kunt alleen een bankrekening in het veld **Bankrekening** invullen als er Bankrekeningen leverancier/klant beschikbaar zijn.</span><span class="sxs-lookup"><span data-stu-id="a368c-123">In order to be able to enter a bank account in the **Bank Account** vendor/customer bank accounts must be available.</span></span> <span data-ttu-id="a368c-124">Zie hieronder.</span><span class="sxs-lookup"><span data-stu-id="a368c-124">See below.</span></span>  
  
### <a name="example"></a><span data-ttu-id="a368c-125">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="a368c-125">Example</span></span>  
 <span data-ttu-id="a368c-126">Olek Johansson (code *OLEK*) is een van uw lokale leveranciers.</span><span class="sxs-lookup"><span data-stu-id="a368c-126">Olek Johansson (code *OLEK*) is one of our local vendors.</span></span> <span data-ttu-id="a368c-127">Inkoopfacturen worden door middel van onze nationale bankrekening (code *ABN*) aan zijn bankrekening (code *OJBA*) betaald.</span><span class="sxs-lookup"><span data-stu-id="a368c-127">Purchase invoices will be paid through our national bank account (code *ABN*) to his bank account (code *OJBA*).</span></span> <span data-ttu-id="a368c-128">Zowel bankrekening ABN als bankrekening OJBA worden uitgedrukt in lokale valuta (LV).</span><span class="sxs-lookup"><span data-stu-id="a368c-128">Both bank account ABN and OJBA are denominated in local currency (LCY).</span></span> <span data-ttu-id="a368c-129">Daarom laten we op de leverancierskaart van Olek Johansson het veld *Valutacode* leeg, vullen we in het veld *Transactiewijze* *ABN* in die is gekoppeld aan onze bankrekening *ABN* en stellen we het veld *Bankrekening* in op *OJBA*.</span><span class="sxs-lookup"><span data-stu-id="a368c-129">Therefore on Olek Johansson's Vendor Card we leave the *Currency Code* field empty, fill the *Transaction Mode* field with *ABN* that is linked to our bank account *ABN* and set the *Bank Account* field to *OJBA*.</span></span>  
  
## <a name="create-vendorcustomer-bank-account"></a><span data-ttu-id="a368c-130">Bankrekening leverancier/klant maken</span><span class="sxs-lookup"><span data-stu-id="a368c-130">Create Vendor/Customer Bank Account</span></span>  
 <span data-ttu-id="a368c-131">Maak een Bankrekening leverancier/klant en vul alle noodzakelijke gegevens in.</span><span class="sxs-lookup"><span data-stu-id="a368c-131">Create vendor/customer bank account and enter all necessary information.</span></span> <span data-ttu-id="a368c-132">Besteed extra aandacht aan het volgende:</span><span class="sxs-lookup"><span data-stu-id="a368c-132">Special attention should be paid to:</span></span>  
  
-   <span data-ttu-id="a368c-133">**Bankrekening van voorkeur**: voer een geldig bankrekeningnummer in.</span><span class="sxs-lookup"><span data-stu-id="a368c-133">**Preferred Bank Account**: enter a valid bank account number.</span></span>  
  
-   <span data-ttu-id="a368c-134">**Valutacode**: laat dit veld leeg; het wordt ingesteld op de lokale valuta (LV).</span><span class="sxs-lookup"><span data-stu-id="a368c-134">**Currency Code**: leave empty - i.e. it is set to the local currency (LCY).</span></span>  
  
-   <span data-ttu-id="a368c-135">**Rekeninghouder**:zorg ervoor dat alle gegevens zijn ingevuld.</span><span class="sxs-lookup"><span data-stu-id="a368c-135">**Owner Information**:be sure all owner information has been entered.</span></span>  
  
### <a name="example"></a><span data-ttu-id="a368c-136">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="a368c-136">Example</span></span>  
 <span data-ttu-id="a368c-137">De bankrekening van Olek Johansson (code *OJBA*) wordt uitgedrukt in lokale valuta (LV).</span><span class="sxs-lookup"><span data-stu-id="a368c-137">Olek Johansson's bank account (code *OJBA*) is denominated in local currency (LCY).</span></span> <span data-ttu-id="a368c-138">Daarom vullen we op de bankrekeningkaart leverancier van Olek Johansson een geldig nummer in het veld *Bankrekeningnr.* in *,* laten we het veld *Valutacode* leeg en vullen we in de velden op het tabblad Rekeninghouder de juiste waarden in.</span><span class="sxs-lookup"><span data-stu-id="a368c-138">Therefore on Olek Johansson's Vendor Bank Account Card we enter a valid number in the *Bank Account No.* field *,* leave the *Currency Code* field empty and fill the fields on the Owner Information tab with appropriate values.</span></span>  
  
## <a name="create-and-post-purchase-invoice-for-vendor-or-sales-invoice-for-customer"></a><span data-ttu-id="a368c-139">Inkoopfactuur voor leverancier of verkoopfactuur voor klant maken en boeken</span><span class="sxs-lookup"><span data-stu-id="a368c-139">Create and Post Purchase Invoice for Vendor or Sales Invoice for Customer</span></span>  
 <span data-ttu-id="a368c-140">Maak een inkoop-/verkoopfactuur en vul alle noodzakelijke gegevens in.</span><span class="sxs-lookup"><span data-stu-id="a368c-140">Create a purchase/sales invoice and enter all necessary information.</span></span> <span data-ttu-id="a368c-141">Besteed extra aandacht aan het volgende:</span><span class="sxs-lookup"><span data-stu-id="a368c-141">Special attention should be paid to:</span></span>  
  
-   <span data-ttu-id="a368c-142">**Valutacode**: laat dit veld leeg; het wordt ingesteld op de lokale valuta (LV).</span><span class="sxs-lookup"><span data-stu-id="a368c-142">**Currency Code**: leave empty - i.e. it is set to the local currency (LCY).</span></span>  
  
-   <span data-ttu-id="a368c-143">**Transactiewijze**: selecteer een geschikte standaardtransactiewijze, dat wil zeggen, een transactiewijze die geschikt is voor betalingen in lokale valuta voor uw bank.</span><span class="sxs-lookup"><span data-stu-id="a368c-143">**Transaction Mode**: select an appropriate, default transaction mode - i.e. one that can deal with local currency payments for your bank.</span></span>  
  
-   <span data-ttu-id="a368c-144">**Bankrekening van voorkeur**: selecteer een geschikte standaardbankrekening van leveranciers/klanten met dezelfde valutacode als de leverancier/klant zelf.</span><span class="sxs-lookup"><span data-stu-id="a368c-144">**Preferred Bank Account**: select an appropriate, default vendor/customer bank account having the same Currency Code is the vendor/customer itself.</span></span>  
  
 <span data-ttu-id="a368c-145">Standaard zijn in deze drie velden waarden ingevuld die zijn overgenomen uit de leveranciers-/klantenkaart.</span><span class="sxs-lookup"><span data-stu-id="a368c-145">By default these three fields will be populated with values taken from the vendor/customer card.</span></span>  
  
 <span data-ttu-id="a368c-146">Als de factuur is voltooid, kan deze worden geboekt.</span><span class="sxs-lookup"><span data-stu-id="a368c-146">When the invoice is finished it can be posted.</span></span>  
  
### <a name="example"></a><span data-ttu-id="a368c-147">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="a368c-147">Example</span></span>  
 <span data-ttu-id="a368c-148">Als we een inkoopfactuur voor Olek Johansson maken, vullen we *OLEK* in het veld ***Orderleveranciersnr.*** in.</span><span class="sxs-lookup"><span data-stu-id="a368c-148">When creating a purchase invoice for Olek Johansson we enter *OLEK* in the ***Buy-from Vendor No.*** field.</span></span> <span data-ttu-id="a368c-149">Standaard zijn in de velden *Valutacode*, *Transactiewijze* en *Bankrekening* waarden ingevuld die zijn overgenomen uit de leverancierskaart van Olek Johansson.</span><span class="sxs-lookup"><span data-stu-id="a368c-149">By default the *Currency Code*, *Transaction Mode* and *Bank Account* fields will be populated with values taken from the Olek Johansson's vendor card.</span></span> <span data-ttu-id="a368c-150">Daarom zijn de velden *Valutacode*, *Transactiewijze* en *Bankrekening* respectievelijk *<empty>*, *ABN* en *OJBA*.</span><span class="sxs-lookup"><span data-stu-id="a368c-150">Therefore the *Currency Code*, *Transaction Mode* and *Bank Account* fields will be *<empty>*, *ABN* and *OJBA* respectively.</span></span> <span data-ttu-id="a368c-151">Deze waarden kunnen echter worden gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="a368c-151">Nevertheless, these values can be changed.</span></span>  
  
## <a name="create-proposal"></a><span data-ttu-id="a368c-152">Voorstel maken</span><span class="sxs-lookup"><span data-stu-id="a368c-152">Create Proposal</span></span>  
 <span data-ttu-id="a368c-153">Open het venster Telebankieren - bankoverzicht en blader naar de bank die we voor onze betaling willen gebruiken.</span><span class="sxs-lookup"><span data-stu-id="a368c-153">Open the Telebank - Bank Overview Window window and browse to the bank through which we want to perform our payment.</span></span> <span data-ttu-id="a368c-154">Open het venster Voorstel en genereer betalingsvoorstellen met de batchverwerking Voorstelposten ophalen.</span><span class="sxs-lookup"><span data-stu-id="a368c-154">Open the Proposal window and generate payment proposals using the Get Proposal Entries batch job.</span></span>  
  
### <a name="example"></a><span data-ttu-id="a368c-155">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="a368c-155">Example</span></span>  
 <span data-ttu-id="a368c-156">Door middel van het venster Telebank - bankoverzicht openen we het venster Voorstel voor onze bank *ABN*.</span><span class="sxs-lookup"><span data-stu-id="a368c-156">Through the Telebank - Bank Overview window we open the Proposal window for our bank *ABN*.</span></span> <span data-ttu-id="a368c-157">Met de batchverwerking wordt één voorstelregel gemaakt voor de inkoopfactuur die we zojuist voor leverancier *OLEK* hebben gemaakt en geboekt.</span><span class="sxs-lookup"><span data-stu-id="a368c-157">Using the batch job one proposal line will be created for the purchase invoice we just created and posted for vendor *OLEK*.</span></span>  
  
## <a name="create-payment-history"></a><span data-ttu-id="a368c-158">Betaalrun maken</span><span class="sxs-lookup"><span data-stu-id="a368c-158">Create Payment History</span></span>  
 <span data-ttu-id="a368c-159">Vanuit het venster Voorstel verwerken we ons voorstel in een betaalrun.</span><span class="sxs-lookup"><span data-stu-id="a368c-159">From the Proposal window we process our proposal into a payment history.</span></span> <span data-ttu-id="a368c-160">Het voorstel verdwijnt en kan worden gevonden in het venster Betaalrunoverzicht voor dezelfde bank.</span><span class="sxs-lookup"><span data-stu-id="a368c-160">The proposal will disappear and can be found in the Payment History Overview window for the same bank.</span></span>  
  
### <a name="example"></a><span data-ttu-id="a368c-161">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="a368c-161">Example</span></span>  
 <span data-ttu-id="a368c-162">We verwerken ons voorstel met betrekking tot de betaling aan leverancier *OLEK* en openen het venster Betaalrunoverzicht voor onze bank *ABN*.</span><span class="sxs-lookup"><span data-stu-id="a368c-162">We process our proposal concerning the payment to vendor *OLEK* and open the Payment History Overview window for our bank *ABN*.</span></span> <span data-ttu-id="a368c-163">De laatste betaalrun is de betaalrun die we zojuist hebben gemaakt.</span><span class="sxs-lookup"><span data-stu-id="a368c-163">The last payment history is the one we just created.</span></span>  
  
## <a name="export-payment-history"></a><span data-ttu-id="a368c-164">Betaalrun exporteren</span><span class="sxs-lookup"><span data-stu-id="a368c-164">Export Payment History</span></span>  
 <span data-ttu-id="a368c-165">Open het venster Betaalrunoverzicht, blader naar de relevante betaalrun en klik op **Exporteren**.</span><span class="sxs-lookup"><span data-stu-id="a368c-165">Open the Payment History Overview Window window, browse to the relevant payment history and choose **Export**.</span></span> <span data-ttu-id="a368c-166">De exportbatchverwerking voor het exportprotocol dat aan deze betaling is gekoppeld, verschijnt.</span><span class="sxs-lookup"><span data-stu-id="a368c-166">The export batch job will appear for the export protocol that is linked to this payment.</span></span> <span data-ttu-id="a368c-167">Voor deze export zijn de juiste filters al automatisch ingevuld.</span><span class="sxs-lookup"><span data-stu-id="a368c-167">For this export the system already has entered appropriate filters.</span></span> <span data-ttu-id="a368c-168">Controleer desgewenst velden van het tabblad Opties en klik op OK om de betaling te exporteren.</span><span class="sxs-lookup"><span data-stu-id="a368c-168">Check, if wanted, any of the fields on the Options tab and click OK to export the payment.</span></span> <span data-ttu-id="a368c-169">Er wordt een tekstbestand gegenereerd met een bestandsnaam zoals die is gedefinieerd in het veld Standaardbestandsnamen van het exportprotocol, dat nu gereed is voor verzending naar onze bank.</span><span class="sxs-lookup"><span data-stu-id="a368c-169">The system will generate a text file using a filename as defined in the Default File Names Field field of the export protocol, which now is ready to be sent to our bank.</span></span>  
  
### <a name="example"></a><span data-ttu-id="a368c-170">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="a368c-170">Example</span></span>  
 <span data-ttu-id="a368c-171">Aangezien de transactiewijze die aan onze betaling is gekoppeld *ABN* is, verschijnt de batchverwerking CLIEOP03.</span><span class="sxs-lookup"><span data-stu-id="a368c-171">As the transaction mode associated with our payment is *ABN* the CLIEOP03 batch job will appear.</span></span>  
  
## <a name="import-bank-statement"></a><span data-ttu-id="a368c-172">Bankafschrift importeren</span><span class="sxs-lookup"><span data-stu-id="a368c-172">Import Bank Statement</span></span>  
 <span data-ttu-id="a368c-173">Nadat we elektronische bankafschriften van onze bank hebben ontvangen, kunnen we ze importeren door vanuit het venster Importprotocoloverzicht het betreffende importprotocol uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="a368c-173">After receiving electronic bank statements from our bank we can import them by running the appropriate import protocol from the Import Protocol List window.</span></span>  
  
### <a name="example"></a><span data-ttu-id="a368c-174">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="a368c-174">Example</span></span>  
 <span data-ttu-id="a368c-175">Het bankafschrift met onze betaling aan Olek Johansson wordt door onze bank *ABN* naar ons gestuurd.</span><span class="sxs-lookup"><span data-stu-id="a368c-175">The bank statement containing our payment to Olek Johansson will be sent to us by our bank *ABN*.</span></span> <span data-ttu-id="a368c-176">Daarom moeten we *OFFICE NET EXTRA* als het juiste importprotocol kiezen.</span><span class="sxs-lookup"><span data-stu-id="a368c-176">Therefore we should chose *OFFICE NET EXTRA* as the appropriate import protocol.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="a368c-177">Zie ook</span><span class="sxs-lookup"><span data-stu-id="a368c-177">See Also</span></span>  
 <span data-ttu-id="a368c-178">[Procedure: Voorstellen maken](how-to-create-proposals.md) </span><span class="sxs-lookup"><span data-stu-id="a368c-178">[How to: Create Proposals](how-to-create-proposals.md) </span></span>  
 [<span data-ttu-id="a368c-179">Procedure: Betalingsrun maken en exporteren</span><span class="sxs-lookup"><span data-stu-id="a368c-179">How to: Create and Export Payment History</span></span>](how-to-create-and-export-payment-history.md)

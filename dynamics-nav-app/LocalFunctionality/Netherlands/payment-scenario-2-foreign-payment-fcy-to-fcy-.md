---
title: Betalingsscenario 2 - buitenlandse betaling (VV naar VV)
description: U kunt telebankieren gebruiken voor handel met binnenlandse en buitenlandse klanten en leveranciers. Dit onderwerp beschrijft een scenario waarin de handel met buitenlandse klanten en leveranciers geschiedt die dezelfde vreemde valuta gebruiken als waarvoor uw bankrekening is ingesteld.
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
ms.openlocfilehash: f0ce9c3e83ed41fd25cd06abea8607f3f2d79563
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="payment-scenario-2---foreign-payment-fcy-to-fcy"></a><span data-ttu-id="a8f5c-104">Betalingsscenario 2 - buitenlandse betaling (VV naar VV)</span><span class="sxs-lookup"><span data-stu-id="a8f5c-104">Payment Scenario 2 - Foreign Payment (FCY to FCY)</span></span>
<span data-ttu-id="a8f5c-105">U kunt telebankieren gebruiken voor handel met binnenlandse en buitenlandse klanten en leveranciers.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-105">You can use telebanking for trade with domestic and foreign customers and vendors.</span></span> <span data-ttu-id="a8f5c-106">Dit onderwerp beschrijft een scenario waarin de handel met buitenlandse klanten en leveranciers geschiedt die dezelfde vreemde valuta gebruiken als waarvoor uw bankrekening is ingesteld.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-106">This topic describes a scenario where the trade is with foreign customers and vendor that use the same foreign currency as your bank account is set up to use.</span></span>  
  
 <span data-ttu-id="a8f5c-107">De volgende lijst bevat de belangrijkste stappen:</span><span class="sxs-lookup"><span data-stu-id="a8f5c-107">The following list describes the main steps:</span></span>  
  
1.  <span data-ttu-id="a8f5c-108">Leverancier/klant maken.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-108">Create Vendor/Customer.</span></span>  
  
2.  <span data-ttu-id="a8f5c-109">Bankrekening leverancier/klant maken.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-109">Create Vendor/Customer Bank Account.</span></span>  
  
3.  <span data-ttu-id="a8f5c-110">Inkoopfactuur voor leverancier of verkoopfactuur voor klant maken en boeken.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-110">Create and Post Purchase Invoice for Vendor or Sales Invoice for Customer.</span></span>  
  
4.  <span data-ttu-id="a8f5c-111">Voorstel maken.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-111">Create Proposal.</span></span>  
  
5.  <span data-ttu-id="a8f5c-112">Betaalrun maken.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-112">Create Payment History.</span></span>  
  
6.  <span data-ttu-id="a8f5c-113">Betaalrun exporteren.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-113">Export Payment History.</span></span>  
  
7.  <span data-ttu-id="a8f5c-114">Bankafschrift importeren.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-114">Import Bank Statement.</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="a8f5c-115">In de volgende voorbeelden zijn enkele standaard-CRONUS-gegevens gebruikt.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-115">In the examples below some standard CRONUS data is being used.</span></span> <span data-ttu-id="a8f5c-116">En in plaats van een leverancier/klant en een Bankrekening leverancier/klant te maken, zou u ook bestaande gegevens kunnen gebruiken.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-116">Likewise instead of creating a vendor/customer and a vendor/customer bank account you could use existing data.</span></span>  
  
## <a name="create-vendorcustomer"></a><span data-ttu-id="a8f5c-117">Leverancier/klant maken</span><span class="sxs-lookup"><span data-stu-id="a8f5c-117">Create Vendor/Customer</span></span>  
 <span data-ttu-id="a8f5c-118">Maak een leverancier/klant en vul alle noodzakelijke gegevens in.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-118">Create vendor/customer and enter all necessary information.</span></span> <span data-ttu-id="a8f5c-119">Besteed extra aandacht aan het volgende:</span><span class="sxs-lookup"><span data-stu-id="a8f5c-119">Special attention should be paid to:</span></span>  
  
-   <span data-ttu-id="a8f5c-120">**Valutacode**: stel in dit veld de vreemde valuta (VV) in.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-120">**Currency Code**: set it to the foreign currency (FCY).</span></span>  
  
-   <span data-ttu-id="a8f5c-121">**Transactiewijze**: selecteer een geschikte standaardtransactiewijze, dat wil zeggen, een transactiewijze die geschikt is voor betalingen in vreemde valuta voor uw buitenlandse bank.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-121">**Transaction Mode**: select an appropriate, default transaction mode - i.e. one that can deal with foreign currency payments for your foreign bank.</span></span>  
  
-   <span data-ttu-id="a8f5c-122">**Bankrekening van voorkeur**: selecteer een geschikte standaardbankrekening van leveranciers/klanten met dezelfde valutacode als de leverancier/klant zelf.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-122">**Preferred Bank Account**: select an appropriate, default vendor/customer bank account having the same Currency Code as the vendor/customer itself.</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="a8f5c-123">U kunt alleen een bankrekening in het veld **Bankrekening** invullen als er Bankrekeningen leverancier/klant beschikbaar zijn.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-123">In order to be able to enter a bank account in the **Bank Account** vendor/customer bank accounts must be available.</span></span> <span data-ttu-id="a8f5c-124">Zie hieronder.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-124">See below.</span></span>  
  
### <a name="example"></a><span data-ttu-id="a8f5c-125">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="a8f5c-125">Example</span></span>  
 <span data-ttu-id="a8f5c-126">Jannet Carter (code *JANNET*) is een van onze Amerikaanse leveranciers.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-126">Jannet Carter (code *JANNET*) is one of our US vendors.</span></span> <span data-ttu-id="a8f5c-127">Inkoopfacturen worden door middel van onze buitenlandse bankrekening (code *ABN-USD*) aan haar bankrekening (code *JCBA*) betaald.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-127">Purchase invoices will be paid through our foreign bank account (code *ABN-USD*) to her bank account (code *JCBA*).</span></span> <span data-ttu-id="a8f5c-128">Zowel bankrekening ABN-USD als bankrekening JCBA worden uitgedrukt in dezelfde vreemde valuta (VV), in dit geval Amerikaanse dollars (USD).</span><span class="sxs-lookup"><span data-stu-id="a8f5c-128">Both bank account ABN-USD and JCBA are denominated in the same foreign currency (FCY) - i.e. USD.</span></span> <span data-ttu-id="a8f5c-129">Daarom stellen we op de leverancierskaart van Jannet Carter het veld *Valutacode* in op *USD*, vullen we in het veld *Transactiewijze* *ABN-USD* in die aan onze bankrekening *ABN-USD* is gekoppeld en stellen we het veld *Bankrekening* in op *JCBA*.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-129">Therefore on Jannet Carter's Vendor Card we set the *Currency Code* field to *USD*, fill the *Transaction Mode* field with *ABN-USD* that is linked to our bank account *ABN-USD* and set the *Bank Account* field to *JCBA*.</span></span>  
  
## <a name="create-vendorcustomer-bank-account"></a><span data-ttu-id="a8f5c-130">Bankrekening leverancier/klant maken</span><span class="sxs-lookup"><span data-stu-id="a8f5c-130">Create Vendor/Customer Bank Account</span></span>  
 <span data-ttu-id="a8f5c-131">Maak een bankrekening leverancier/klant en vul alle noodzakelijke gegevens in.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-131">Create vendor/customer bank account and enter all necessary information.</span></span> <span data-ttu-id="a8f5c-132">Besteed extra aandacht aan het volgende:</span><span class="sxs-lookup"><span data-stu-id="a8f5c-132">Special attention should be paid to:</span></span>  
  
-   <span data-ttu-id="a8f5c-133">**Bankrekening van voorkeur**: voer een geldig bankrekeningnummer in.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-133">**Preferred Bank Account**: enter a valid bank account number.</span></span>  
  
-   <span data-ttu-id="a8f5c-134">**Valutacode**: stel in dit veld de vreemde valuta (VV) in.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-134">**Currency Code**: set it to the foreign currency (FCY).</span></span>  
  
-   <span data-ttu-id="a8f5c-135">**Rekeninghouder**: zorg ervoor dat alle gegevens zijn ingevuld.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-135">**Owner Information**:be sure all owner information has been entered.</span></span>  
  
### <a name="example"></a><span data-ttu-id="a8f5c-136">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="a8f5c-136">Example</span></span>  
 <span data-ttu-id="a8f5c-137">De bankrekening van Jannet Carter (code *JCBA*) wordt uitgedrukt in vreemde valuta (VV), in dit geval USD.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-137">Jannet Carter's bank account (code *JCBA*) is denominated in foreign currency (FCY) - i.e. USD.</span></span> <span data-ttu-id="a8f5c-138">Daarom vullen we op de bankrekeningkaart leverancier van Jannet Carter een geldig nummer in het veld *Bankrekeningnr.* in *,* stellen we het veld *Valutacode* in op *USD* en vullen we in de velden op het tabblad Rekeninghouder de juiste waarden in.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-138">Therefore on Jannet Carter's Vendor Bank Account Card we enter a valid number in the *Bank Account No.* field *,* set the *Currency Code* field to *USD* and fill the fields on the Owner Information tab with appropriate values.</span></span>  
  
## <a name="create-and-post-purchase-invoice-for-vendor-or-sales-invoice-for-customer"></a><span data-ttu-id="a8f5c-139">Inkoopfactuur voor leverancier of verkoopfactuur voor klant maken en boeken</span><span class="sxs-lookup"><span data-stu-id="a8f5c-139">Create and Post Purchase Invoice for Vendor or Sales Invoice for Customer</span></span>  
 <span data-ttu-id="a8f5c-140">Maak een inkoop-/verkoopfactuur en vul alle noodzakelijke gegevens in.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-140">Create a purchase/sales invoice and enter all necessary information.</span></span> <span data-ttu-id="a8f5c-141">Besteed extra aandacht aan het volgende:</span><span class="sxs-lookup"><span data-stu-id="a8f5c-141">Special attention should be paid to:</span></span>  
  
-   <span data-ttu-id="a8f5c-142">**Valutacode**: stel in dit veld de vreemde valuta (VV) in.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-142">**Currency Code**: set it to the foreign currency (FCY).</span></span>  
  
-   <span data-ttu-id="a8f5c-143">**Transactiewijze**: selecteer een geschikte standaardtransactiewijze, dat wil zeggen, een transactiewijze die geschikt is voor betalingen in vreemde valuta voor uw buitenlandse bank.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-143">**Transaction Mode**: select an appropriate, default transaction mode - i.e. one that can deal with foreign currency payments for your foreign bank.</span></span>  
  
-   <span data-ttu-id="a8f5c-144">**Bankrekening van voorkeur**: selecteer een geschikte standaardbankrekening van leveranciers/klanten met dezelfde valutacode als de leverancier/klant zelf.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-144">**Preferred Bank Account**: select an appropriate, default vendor/customer bank account having the same Currency Code is the vendor/customer itself.</span></span>  
  
 <span data-ttu-id="a8f5c-145">Standaard zijn in deze drie velden waarden ingevuld die zijn overgenomen uit de leveranciers-/klantenkaart.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-145">By default these three fields will be populated with values taken from the vendor/customer card.</span></span>  
  
 <span data-ttu-id="a8f5c-146">Als de factuur is voltooid, kan deze worden geboekt.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-146">When the invoice is finished it can be posted.</span></span>  
  
### <a name="example"></a><span data-ttu-id="a8f5c-147">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="a8f5c-147">Example</span></span>  
 <span data-ttu-id="a8f5c-148">Als we een inkoopfactuur voor Jannet Carter maken, vullen we *JANNET* in het veld ***Orderleveranciersnr.*** in.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-148">When creating a purchase invoice for Jannet Carter we enter *JANNET* in the ***Buy-from Vendor No.*** field.</span></span> <span data-ttu-id="a8f5c-149">Standaard zijn in de velden *Valutacode*, *Transactiewijze* en *Bankrekening* waarden overgenomen vanuit de leverancierskaart van Jannet Carter.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-149">By default the *Currency Code*, *Transaction Mode* and *Bank Account* fields will be populated with values taken from the Jannet Carter's vendor card.</span></span> <span data-ttu-id="a8f5c-150">Daarom is in de velden *Valutacode*, *Transactiewijze* en *Bankrekening* respectievelijk *USD*, *ABN-USD* en *JCBA* ingevuld.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-150">Therefore the *Currency Code*, *Transaction Mode* and *Bank Account* fields will be *USD*, *ABN-USD* and *JCBA* respectively.</span></span> <span data-ttu-id="a8f5c-151">Deze waarden kunnen echter worden gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-151">Nevertheless, these values can be changed.</span></span>  
  
## <a name="create-proposal"></a><span data-ttu-id="a8f5c-152">Voorstel maken</span><span class="sxs-lookup"><span data-stu-id="a8f5c-152">Create Proposal</span></span>  
 <span data-ttu-id="a8f5c-153">Open het venster Telebankieren - bankoverzicht en blader naar de bank die we voor onze betaling willen gebruiken.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-153">Open the Telebank - Bank Overview Window window and browse to the bank through which we want to perform our payment.</span></span> <span data-ttu-id="a8f5c-154">Open het venster Voorstel en genereer betalingsvoorstellen met de batchverwerking Voorstelposten ophalen.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-154">Open the Proposal window and generate payment proposals using the Get Proposal Entries batch job.</span></span>  
  
### <a name="example"></a><span data-ttu-id="a8f5c-155">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="a8f5c-155">Example</span></span>  
 <span data-ttu-id="a8f5c-156">Door middel van het venster Telebank - bankoverzicht openen we het venster Voorstel voor onze bank *ABN*.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-156">Through the Telebank - Bank Overview window we open the Proposal window for our bank *ABN-USD*.</span></span> <span data-ttu-id="a8f5c-157">Met de batchverwerking wordt één voorstelregel gemaakt voor de inkoopfactuur die we zojuist voor leverancier *JANNET* hebben gemaakt en geboekt.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-157">Using the batch job one proposal line will be created for the purchase invoice we just created and posted for vendor *JANNET*.</span></span>  
  
## <a name="create-payment-history"></a><span data-ttu-id="a8f5c-158">Betaalrun maken</span><span class="sxs-lookup"><span data-stu-id="a8f5c-158">Create Payment History</span></span>  
 <span data-ttu-id="a8f5c-159">Vanuit het venster Voorstel verwerken we ons voorstel in een betaalrun.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-159">From the Proposal window we process our proposal into a payment history.</span></span> <span data-ttu-id="a8f5c-160">Het voorstel verdwijnt en kan worden gevonden in het venster Betaalrunoverzicht voor dezelfde bank.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-160">The proposal will disappear and can be found in the Payment History Overview window for the same bank.</span></span>  
  
### <a name="example"></a><span data-ttu-id="a8f5c-161">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="a8f5c-161">Example</span></span>  
 <span data-ttu-id="a8f5c-162">We verwerken ons voorstel met betrekking tot de betaling aan leverancier *JANNET* en openen het venster Betaalrunoverzicht voor onze bank *ABN-USD*.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-162">We process our proposal concerning the payment to vendor *JANNET* and open the Payment History Overview window for our bank *ABN-USD*.</span></span> <span data-ttu-id="a8f5c-163">De laatste betaalrun is de betaalrun die we zojuist hebben gemaakt.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-163">The last payment history is the one we just created.</span></span>  
  
## <a name="export-payment-history"></a><span data-ttu-id="a8f5c-164">Betaalrun exporteren</span><span class="sxs-lookup"><span data-stu-id="a8f5c-164">Export Payment History</span></span>  
 <span data-ttu-id="a8f5c-165">Open het venster Betaalrunoverzicht, blader naar de relevante betaalrun en klik op **Exporteren**.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-165">Open the Payment History Overview Window window, browse to the relevant payment history and choose **Export**.</span></span> <span data-ttu-id="a8f5c-166">De exportbatchverwerking voor het exportprotocol dat aan deze betaling is gekoppeld, verschijnt.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-166">The export batch job will appear for the export protocol that is linked to this payment.</span></span> <span data-ttu-id="a8f5c-167">Voor deze export zijn de juiste filters al automatisch ingevuld.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-167">For this export the system already has entered appropriate filters.</span></span> <span data-ttu-id="a8f5c-168">Controleer desgewenst velden van het tabblad Opties en klik op OK om de betaling te exporteren.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-168">Check, if wanted, any of the fields on the Options tab and click OK to export the payment.</span></span> <span data-ttu-id="a8f5c-169">Er wordt een tekstbestand gegenereerd met een bestandsnaam zoals die is gedefinieerd in het veld Standaardbestandsnamen van het exportprotocol, dat nu gereed is voor verzending naar onze bank.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-169">The system will generate a text file using a filename as defined in the Default File Names Field field of the export protocol, which now is ready to be sent to our bank.</span></span>  
  
### <a name="example"></a><span data-ttu-id="a8f5c-170">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="a8f5c-170">Example</span></span>  
 <span data-ttu-id="a8f5c-171">Aangezien de transactiewijze die aan onze betaling is gekoppeld *ABN-USD* is, verschijnt de batchverwerking BBV of PAYMUL.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-171">As the transaction mode associated with our payment is *ABN-USD* the BBV or PAYMUL batch job will appear.</span></span>  
  
## <a name="import-bank-statement"></a><span data-ttu-id="a8f5c-172">Bankafschrift importeren</span><span class="sxs-lookup"><span data-stu-id="a8f5c-172">Import Bank Statement</span></span>  
 <span data-ttu-id="a8f5c-173">Nadat we elektronische bankafschriften van onze bank hebben ontvangen, kunnen we ze importeren door vanuit het venster Importprotocoloverzicht het betreffende importprotocol uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-173">After receiving electronic bank statements from our bank we can import them by running the appropriate import protocol from the Import Protocol List window.</span></span>  
  
### <a name="example"></a><span data-ttu-id="a8f5c-174">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="a8f5c-174">Example</span></span>  
 <span data-ttu-id="a8f5c-175">Het bankafschrift met onze betaling aan Jannet Carter wordt door onze bank *ABN-USD* naar ons gestuurd.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-175">The bank statement containing our payment to Jannet Carter will be sent to us by our bank *ABN-USD*.</span></span> <span data-ttu-id="a8f5c-176">Daarom moeten we *OFFICE NET EXTRA* als het juiste importprotocol kiezen.</span><span class="sxs-lookup"><span data-stu-id="a8f5c-176">Therefore we should chose *OFFICE NET EXTRA* as the appropriate import protocol.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="a8f5c-177">Zie ook</span><span class="sxs-lookup"><span data-stu-id="a8f5c-177">See Also</span></span>  
 <span data-ttu-id="a8f5c-178">[Procedure: Voorstellen maken](how-to-create-proposals.md) </span><span class="sxs-lookup"><span data-stu-id="a8f5c-178">[How to: Create Proposals](how-to-create-proposals.md) </span></span>  
 [<span data-ttu-id="a8f5c-179">Procedure: Betalingsrun maken en exporteren</span><span class="sxs-lookup"><span data-stu-id="a8f5c-179">How to: Create and Export Payment History</span></span>](how-to-create-and-export-payment-history.md)

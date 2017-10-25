---
title: Betalingsscenario 3 - een buitenlandse betaling (LV naar VV)
description: U kunt telebankieren gebruiken voor handel met binnenlandse en buitenlandse klanten en leveranciers. Dit onderwerp beschrijft een scenario waarin de handel met buitenlandse klanten en leveranciers geschiedt die een andere valuta dan uw lokale valuta gebruiken.
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
ms.openlocfilehash: 5d16a7daee6b79b92a8e7a21d317efbda6fd6167
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="payment-scenario-3---foreign-payment-lcy--to-fcy"></a><span data-ttu-id="f938a-104">Betalingsscenario 3 - een buitenlandse betaling (LV naar VV)</span><span class="sxs-lookup"><span data-stu-id="f938a-104">Payment Scenario 3 - Foreign Payment (LCY  to FCY)</span></span>
<span data-ttu-id="f938a-105">U kunt telebankieren gebruiken voor handel met binnenlandse en buitenlandse klanten en leveranciers.</span><span class="sxs-lookup"><span data-stu-id="f938a-105">You can use telebanking for trade with domestic and foreign customers and vendors.</span></span> <span data-ttu-id="f938a-106">Dit onderwerp beschrijft een scenario waarin de handel met buitenlandse klanten en leveranciers geschiedt die een andere valuta dan uw lokale valuta gebruiken.</span><span class="sxs-lookup"><span data-stu-id="f938a-106">This topic describes a scenario where the trade is with foreign customers and vendors that use a different currency than your local currency.</span></span>  
  
1.  <span data-ttu-id="f938a-107">Leverancier/klant maken.</span><span class="sxs-lookup"><span data-stu-id="f938a-107">Create Vendor/Customer.</span></span>  
  
2.  <span data-ttu-id="f938a-108">Bankrekening leverancier/klant maken.</span><span class="sxs-lookup"><span data-stu-id="f938a-108">Create Vendor/Customer Bank Account.</span></span>  
  
3.  <span data-ttu-id="f938a-109">Inkoopfactuur voor leverancier of verkoopfactuur voor klant maken en boeken.</span><span class="sxs-lookup"><span data-stu-id="f938a-109">Create and Post Purchase Invoice for Vendor or Sales Invoice for Customer.</span></span>  
  
4.  <span data-ttu-id="f938a-110">Voorstel maken.</span><span class="sxs-lookup"><span data-stu-id="f938a-110">Create Proposal.</span></span>  
  
5.  <span data-ttu-id="f938a-111">Betaalrun maken.</span><span class="sxs-lookup"><span data-stu-id="f938a-111">Create Payment History.</span></span>  
  
6.  <span data-ttu-id="f938a-112">Betaalrun exporteren.</span><span class="sxs-lookup"><span data-stu-id="f938a-112">Export Payment History.</span></span>  
  
7.  <span data-ttu-id="f938a-113">Bankafschrift importeren.</span><span class="sxs-lookup"><span data-stu-id="f938a-113">Import Bank Statement.</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="f938a-114">In de volgende voorbeelden zijn enkele standaard-CRONUS-gegevens gebruikt.</span><span class="sxs-lookup"><span data-stu-id="f938a-114">In the examples below some standard CRONUS data is being used.</span></span> <span data-ttu-id="f938a-115">En in plaats van een leverancier/klant en een Bankrekening leverancier/klant te maken, zou u ook bestaande gegevens kunnen gebruiken.</span><span class="sxs-lookup"><span data-stu-id="f938a-115">Likewise instead of creating a vendor/customer and a vendor/customer bank account you could use existing data.</span></span>  
  
## <a name="create-vendorcustomer"></a><span data-ttu-id="f938a-116">Leverancier/klant maken</span><span class="sxs-lookup"><span data-stu-id="f938a-116">Create Vendor/Customer</span></span>  
 <span data-ttu-id="f938a-117">Maak een leverancier/klant en vul alle noodzakelijke gegevens in.</span><span class="sxs-lookup"><span data-stu-id="f938a-117">Create vendor/customer and enter all necessary information.</span></span> <span data-ttu-id="f938a-118">Besteed extra aandacht aan het volgende:</span><span class="sxs-lookup"><span data-stu-id="f938a-118">Special attention should be paid to:</span></span>  
  
-   <span data-ttu-id="f938a-119">**Valutacode**: stel in dit veld de vreemde valuta (VV) in.</span><span class="sxs-lookup"><span data-stu-id="f938a-119">**Currency Code**: set it to the foreign currency (FCY).</span></span>  
  
-   <span data-ttu-id="f938a-120">**Transactiewijze**: selecteer een geschikte standaardtransactiewijze, dat wil zeggen, een transactiewijze die geschikt is voor betalingen in vreemde valuta voor uw lokale bank.</span><span class="sxs-lookup"><span data-stu-id="f938a-120">**Transaction Mode**: select an appropriate, default transaction mode - i.e. one that can deal with foreign currency payments for your local bank.</span></span>  
  
-   <span data-ttu-id="f938a-121">**Bankrekening van voorkeur**: selecteer een geschikte standaardbankrekening van leveranciers/klanten met dezelfde valutacode als de leverancier/klant zelf.</span><span class="sxs-lookup"><span data-stu-id="f938a-121">**Preferred Bank Account**: select an appropriate, default vendor/customer bank account having the same Currency Code as the vendor/customer itself.</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="f938a-122">U kunt alleen een bankrekening in het veld **Bankrekening** invullen als er Bankrekeningen leverancier/klant beschikbaar zijn.</span><span class="sxs-lookup"><span data-stu-id="f938a-122">In order to be able to enter a bank account in the **Bank Account** vendor/customer bank accounts must be available.</span></span> <span data-ttu-id="f938a-123">Zie hieronder.</span><span class="sxs-lookup"><span data-stu-id="f938a-123">See below.</span></span>  
  
### <a name="example"></a><span data-ttu-id="f938a-124">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="f938a-124">Example</span></span>  
 <span data-ttu-id="f938a-125">Hernandez Ortiz (code *ORTIZ*) is een van onze Mexicaanse leveranciers.</span><span class="sxs-lookup"><span data-stu-id="f938a-125">Hernandez Ortiz (code *ORTIZ*) is one of our Mexican vendors.</span></span> <span data-ttu-id="f938a-126">Inkoopfacturen worden door middel van onze nationale bankrekening (code *ABN*) aan zijn bankrekening (code *HOBA*) betaald.</span><span class="sxs-lookup"><span data-stu-id="f938a-126">Purchase invoices will be paid through our national bank account (code *ABN*) to his bank account (code *HOBA*).</span></span> <span data-ttu-id="f938a-127">Terwijl onze bankrekening ABN in lokale valuta (LV) wordt uitgedrukt, wordt de bankrekening van Hernandez Ortiz, HOBA, in Mexicaanse peso's (MXN) uitgedrukt.</span><span class="sxs-lookup"><span data-stu-id="f938a-127">While our bank account ABN is denominated in local currency (LCY), Hernandez Ortiz's bank account HOBA is denominated in Mexican peso (MXN).</span></span> <span data-ttu-id="f938a-128">Daarom stellen we op de leverancierskaart van Hernandez Ortiz het veld *Valutacode* in op *MXN*, vullen we in het veld *Transactiewijze* *ABN* in die aan onze bankrekening *ABN* is gekoppeld en stellen we het veld *Bankrekening* in op *HOBA*.</span><span class="sxs-lookup"><span data-stu-id="f938a-128">Therefore on Hernandez Ortiz's Vendor Card we set the *Currency Code* field to *MXN*, fill the *Transaction Mode* field with *ABN* that is linked to our bank account *ABN* and set the *Bank Account* field to *HOBA*.</span></span>  
  
## <a name="create-vendorcustomer-bank-account"></a><span data-ttu-id="f938a-129">Bankrekening leverancier/klant maken</span><span class="sxs-lookup"><span data-stu-id="f938a-129">Create Vendor/Customer Bank Account</span></span>  
 <span data-ttu-id="f938a-130">Maak een bankrekening leverancier/klant en vul alle noodzakelijke gegevens in.</span><span class="sxs-lookup"><span data-stu-id="f938a-130">Create vendor/customer bank account and enter all necessary information.</span></span> <span data-ttu-id="f938a-131">Besteed extra aandacht aan het volgende:</span><span class="sxs-lookup"><span data-stu-id="f938a-131">Special attention should be paid to:</span></span>  
  
-   <span data-ttu-id="f938a-132">**Bankrekening van voorkeur**: voer een geldig bankrekeningnummer in.</span><span class="sxs-lookup"><span data-stu-id="f938a-132">**Preferred Bank Account**: enter a valid bank account number.</span></span>  
  
-   <span data-ttu-id="f938a-133">**Valutacode**: stel in dit veld de vreemde valuta (VV) in.</span><span class="sxs-lookup"><span data-stu-id="f938a-133">**Currency Code**: set it to the foreign currency (FCY).</span></span>  
  
-   <span data-ttu-id="f938a-134">**Rekeninghouder**: zorg ervoor dat alle gegevens zijn ingevuld.</span><span class="sxs-lookup"><span data-stu-id="f938a-134">**Owner Information**:be sure all owner information has been entered.</span></span>  
  
### <a name="example"></a><span data-ttu-id="f938a-135">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="f938a-135">Example</span></span>  
 <span data-ttu-id="f938a-136">De bankrekening van Hernandez Ortiz (code *HOBA*) wordt uitgedrukt in *MXN*.</span><span class="sxs-lookup"><span data-stu-id="f938a-136">Hernandez Ortiz's bank account (code *HOBA*) is denominated in *MXN*.</span></span> <span data-ttu-id="f938a-137">Daarom vullen we op de bankrekeningkaart leverancier van Hernandez Ortiz een geldig nummer in het veld *Bankrekeningnr.* in *,* stellen we het veld *Valutacode* in op *MXN* en vullen we in de velden op het tabblad Rekeninghouder de juiste waarden in.</span><span class="sxs-lookup"><span data-stu-id="f938a-137">Therefore on Hernandez Ortiz's Vendor Bank Account Card we enter a valid number in the *Bank Account No.* field *,* set the *Currency Code* field to *MXN* and fill the fields on the Owner Information tab with appropriate values.</span></span>  
  
## <a name="create-and-post-purchase-invoice-for-vendor-or-sales-invoice-for-customer"></a><span data-ttu-id="f938a-138">Inkoopfactuur voor leverancier of verkoopfactuur voor klant maken en boeken</span><span class="sxs-lookup"><span data-stu-id="f938a-138">Create and Post Purchase Invoice for Vendor or Sales Invoice for Customer</span></span>  
 <span data-ttu-id="f938a-139">Maak een inkoop-/verkoopfactuur en vul alle noodzakelijke gegevens in.</span><span class="sxs-lookup"><span data-stu-id="f938a-139">Create a purchase/sales invoice and enter all necessary information.</span></span> <span data-ttu-id="f938a-140">Besteed extra aandacht aan het volgende:</span><span class="sxs-lookup"><span data-stu-id="f938a-140">Special attention should be paid to:</span></span>  
  
-   <span data-ttu-id="f938a-141">**Valutacode**: stel in dit veld de vreemde valuta (VV) in.</span><span class="sxs-lookup"><span data-stu-id="f938a-141">**Currency Code**: set it to the foreign currency (FCY).</span></span>  
  
-   <span data-ttu-id="f938a-142">**Transactiewijze**: selecteer een geschikte standaardtransactiewijze, dat wil zeggen, een transactiewijze die geschikt is voor betalingen in lokale valuta voor uw lokale bank.</span><span class="sxs-lookup"><span data-stu-id="f938a-142">**Transaction Mode**: select an appropriate, default transaction mode - i.e. one that can deal with local currency payments for your local bank.</span></span>  
  
-   <span data-ttu-id="f938a-143">**Bankrekening van voorkeur**: selecteer een geschikte standaardbankrekening van leveranciers/klanten met dezelfde valutacode als de leverancier/klant zelf.</span><span class="sxs-lookup"><span data-stu-id="f938a-143">**Preferred Bank Account**: select an appropriate, default vendor/customer bank account having the same Currency Code is the vendor/customer itself.</span></span>  
  
 <span data-ttu-id="f938a-144">Standaard zijn in deze drie velden waarden ingevuld die zijn overgenomen uit de leveranciers-/klantenkaart.</span><span class="sxs-lookup"><span data-stu-id="f938a-144">By default these three fields will be populated with values taken from the vendor/customer card.</span></span>  
  
 <span data-ttu-id="f938a-145">Als de factuur is voltooid, kan deze worden geboekt.</span><span class="sxs-lookup"><span data-stu-id="f938a-145">When the invoice is finished it can be posted.</span></span>  
  
### <a name="example"></a><span data-ttu-id="f938a-146">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="f938a-146">Example</span></span>  
 <span data-ttu-id="f938a-147">Als we een inkoopfactuur voor Hernandez Ortiz maken, vullen we *ORTIZ* in het veld ***Orderleveranciersnr.*** in.</span><span class="sxs-lookup"><span data-stu-id="f938a-147">When creating a purchase invoice for Hernandez Ortiz we enter *ORTIZ* in the ***Buy-from Vendor No.*** field.</span></span> <span data-ttu-id="f938a-148">Standaard zijn in de velden *Valutacode*, *Transactiewijze* en *Bankrekening* waarden overgenomen vanuit de leveranciers kaart van Hernandez Ortiz.</span><span class="sxs-lookup"><span data-stu-id="f938a-148">By default the *Currency Code*, *Transaction Mode* and *Bank Account* fields will be populated with values taken from the Hernandez Ortiz's vendor card.</span></span> <span data-ttu-id="f938a-149">Daarom is in de velden *Valutacode*, *Transactiewijze* en *Bankrekening* respectievelijk *MXN*, *ABN* en *HOBA* ingevuld.</span><span class="sxs-lookup"><span data-stu-id="f938a-149">Therefore the *Currency Code*, *Transaction Mode* and *Bank Account* fields will be *MXN*, *ABN* and *HOBA* respectively.</span></span> <span data-ttu-id="f938a-150">Deze waarden kunnen echter worden gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="f938a-150">Nevertheless, these values can be changed.</span></span>  
  
## <a name="create-proposal"></a><span data-ttu-id="f938a-151">Voorstel maken</span><span class="sxs-lookup"><span data-stu-id="f938a-151">Create Proposal</span></span>  
 <span data-ttu-id="f938a-152">Open het venster Telebank - bankoverzicht en blader naar de bank die we voor onze betaling willen gebruiken.</span><span class="sxs-lookup"><span data-stu-id="f938a-152">Open the Telebank - Bank Overview window and browse to the bank through which we want to perform our payment.</span></span> <span data-ttu-id="f938a-153">Open het venster Voorstel en genereer betalingsvoorstellen met de batchverwerking Voorstelposten ophalen.</span><span class="sxs-lookup"><span data-stu-id="f938a-153">Open the Proposal window and generate payment proposals using the Get Proposal Entries batch job.</span></span>  
  
### <a name="example"></a><span data-ttu-id="f938a-154">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="f938a-154">Example</span></span>  
 <span data-ttu-id="f938a-155">Door middel van het venster Telebank - bankoverzicht openen we het venster Voorstel voor onze bank *ABN*.</span><span class="sxs-lookup"><span data-stu-id="f938a-155">Through the Telebank - Bank Overview window we open the Proposal window for our bank *ABN*.</span></span> <span data-ttu-id="f938a-156">Met de batchverwerking wordt één voorstelregel gemaakt voor de inkoopfactuur die we zojuist voor leverancier *ORTIZ* hebben gemaakt en geboekt.</span><span class="sxs-lookup"><span data-stu-id="f938a-156">Using the batch job one proposal line will be created for the purchase invoice we just created and posted for vendor *ORTIZ*.</span></span> <span data-ttu-id="f938a-157">Het bedrag van de betaling wordt uitgedrukt in lokale valuta (LV).</span><span class="sxs-lookup"><span data-stu-id="f938a-157">The amount of the payment will be in local currency (LCY).</span></span>  
  
## <a name="create-payment-history"></a><span data-ttu-id="f938a-158">Betaalrun maken</span><span class="sxs-lookup"><span data-stu-id="f938a-158">Create Payment History</span></span>  
 <span data-ttu-id="f938a-159">Vanuit het venster Voorstel verwerken we ons voorstel in een betaalrun.</span><span class="sxs-lookup"><span data-stu-id="f938a-159">From the Proposal window we process our proposal into a payment history.</span></span> <span data-ttu-id="f938a-160">Het voorstel verdwijnt en kan worden gevonden in het venster Betaalrunoverzicht voor dezelfde bank.</span><span class="sxs-lookup"><span data-stu-id="f938a-160">The proposal will disappear and can be found in the Payment History Overview window for the same bank.</span></span>  
  
### <a name="example"></a><span data-ttu-id="f938a-161">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="f938a-161">Example</span></span>  
 <span data-ttu-id="f938a-162">We verwerken ons voorstel met betrekking tot de betaling aan leverancier *ORTIZ* en openen het venster Betaalrunoverzicht voor onze bank *ABN*.</span><span class="sxs-lookup"><span data-stu-id="f938a-162">We process our proposal concerning the payment to vendor *ORTIZ* and open the Payment History Overview window for our bank *ABN*.</span></span> <span data-ttu-id="f938a-163">De laatste betaalrun is de betaalrun die we zojuist hebben gemaakt.</span><span class="sxs-lookup"><span data-stu-id="f938a-163">The last payment history is the one we just created.</span></span>  
  
## <a name="export-payment-history"></a><span data-ttu-id="f938a-164">Betaalrun exporteren</span><span class="sxs-lookup"><span data-stu-id="f938a-164">Export Payment History</span></span>  
 <span data-ttu-id="f938a-165">Open het venster Betaalrunoverzicht, blader naar de relevante betaalrun en klik op **Exporteren**.</span><span class="sxs-lookup"><span data-stu-id="f938a-165">Open the Payment History Overview Window window, browse to the relevant payment history and choose **Export**.</span></span> <span data-ttu-id="f938a-166">De exportbatchverwerking voor het exportprotocol dat aan deze betaling is gekoppeld, verschijnt.</span><span class="sxs-lookup"><span data-stu-id="f938a-166">The export batch job will appear for the export protocol that is linked to this payment.</span></span> <span data-ttu-id="f938a-167">Voor deze export zijn de juiste filters al automatisch ingevuld.</span><span class="sxs-lookup"><span data-stu-id="f938a-167">For this export the system already has entered appropriate filters.</span></span> <span data-ttu-id="f938a-168">Controleer desgewenst velden van het tabblad Opties en klik op OK om de betaling te exporteren.</span><span class="sxs-lookup"><span data-stu-id="f938a-168">Check, if wanted, any of the fields on the Options tab and click OK to export the payment.</span></span> <span data-ttu-id="f938a-169">Er wordt een tekstbestand gegenereerd met een bestandsnaam zoals die is gedefinieerd in het veld Standaardbestandsnamen van het exportprotocol, dat nu gereed is voor verzending naar onze bank.</span><span class="sxs-lookup"><span data-stu-id="f938a-169">The system will generate a text file using a filename as defined in the Default File Names Field field of the export protocol, which now is ready to be sent to our bank.</span></span>  
  
### <a name="example"></a><span data-ttu-id="f938a-170">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="f938a-170">Example</span></span>  
 <span data-ttu-id="f938a-171">Aangezien de transactiewijze die aan onze betaling is gekoppeld *ABN* is, verschijnt de batchverwerking BBV of PAYMUL.</span><span class="sxs-lookup"><span data-stu-id="f938a-171">As the transaction mode associated with our payment is *ABN* the BBV or PAYMUL batch job will appear.</span></span>  
  
## <a name="import-bank-statement"></a><span data-ttu-id="f938a-172">Bankafschrift importeren</span><span class="sxs-lookup"><span data-stu-id="f938a-172">Import Bank Statement</span></span>  
 <span data-ttu-id="f938a-173">Nadat we elektronische bankafschriften van onze bank hebben ontvangen, kunnen we ze importeren door vanuit het venster Importprotocoloverzicht het betreffende importprotocol uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="f938a-173">After receiving electronic bank statements from our bank we can import them by running the appropriate import protocol from the Import Protocol List window.</span></span>  
  
### <a name="example"></a><span data-ttu-id="f938a-174">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="f938a-174">Example</span></span>  
 <span data-ttu-id="f938a-175">Het bankafschrift met onze betaling aan Hernandez Ortiz wordt door onze bank *ABN* naar ons gestuurd.</span><span class="sxs-lookup"><span data-stu-id="f938a-175">The bank statement containing our payment to Hernandez Ortiz will be sent to us by our bank *ABN*.</span></span> <span data-ttu-id="f938a-176">Daarom moeten we *OFFICE NET EXTRA* als het juiste importprotocol kiezen.</span><span class="sxs-lookup"><span data-stu-id="f938a-176">Therefore we should chose *OFFICE NET EXTRA* as the appropriate import protocol.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="f938a-177">Zie ook</span><span class="sxs-lookup"><span data-stu-id="f938a-177">See Also</span></span>  
 <span data-ttu-id="f938a-178">[Procedure: Voorstellen maken](how-to-create-proposals.md) </span><span class="sxs-lookup"><span data-stu-id="f938a-178">[How to: Create Proposals](how-to-create-proposals.md) </span></span>  
 [<span data-ttu-id="f938a-179">Procedure: Betalingsrun maken en exporteren</span><span class="sxs-lookup"><span data-stu-id="f938a-179">How to: Create and Export Payment History</span></span>](how-to-create-and-export-payment-history.md)

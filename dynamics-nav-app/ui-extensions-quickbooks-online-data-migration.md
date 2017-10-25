---
title: De extensie QuickBooks-migratie gebruiken
description: Beschrijft hoe u de extensie gebruikt om klanten, leveranciers, artikelen en rekeningen van QuickBooks Online naar Dynamics NAV te migreren.
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: extension, migrate, data, QuickBooks, import
ms.date: 05/24/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: ff8f8f0c529966fc108d2d4c86e2d0681b1fc005
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---

# <a name="the-quickbooks-online-data-migration-extension-for-dynamics-nav"></a><span data-ttu-id="0cbc8-103">De extensie QuickBooks Online-gegevensmigratie voor Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="0cbc8-103">The QuickBooks Online Data Migration Extension for Dynamics NAV</span></span>
<span data-ttu-id="0cbc8-104">Deze extensie wordt opgenomen in de begeleide instelling **Gegevensmigratie**, om u te helpen belangrijke bedrijfsgegevens te migreren van QuickBooks Online naar [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="0cbc8-104">This extension is included in the **Data Migration** assisted setup guide to help you migrate important business data from QuickBooks Online to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="0cbc8-105">Dat is bijvoorbeeld handig als uw bedrijf groeit en u hebt besloten uw app voor bedrijfsmanagement te upgraden door [!INCLUDE[d365fin](includes/d365fin_md.md)] te gaan gebruiken.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-105">For example, this is useful when your business is growing, and you've decided to upgrade your business management app by starting to use [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

## <a name="what-data-can-i-import-from-quickbooks-online"></a><span data-ttu-id="0cbc8-106">Welke gegevens kan ik uit QuickBooks Online importeren?</span><span class="sxs-lookup"><span data-stu-id="0cbc8-106">What data can I import from QuickBooks Online?</span></span>
<span data-ttu-id="0cbc8-107">U kunt de volgende gegevens uit QuickBooks Online importeren naar [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span><span class="sxs-lookup"><span data-stu-id="0cbc8-107">You can import the following data from QuickBooks Online to [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span></span>  

* <span data-ttu-id="0cbc8-108">Klanten</span><span class="sxs-lookup"><span data-stu-id="0cbc8-108">Customers</span></span>
* <span data-ttu-id="0cbc8-109">Leveranc.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-109">Vendors</span></span>
* <span data-ttu-id="0cbc8-110">Artikelen</span><span class="sxs-lookup"><span data-stu-id="0cbc8-110">Items</span></span>
* <span data-ttu-id="0cbc8-111">Rekeningschema</span><span class="sxs-lookup"><span data-stu-id="0cbc8-111">Chart of accounts</span></span> 
* <span data-ttu-id="0cbc8-112">Beginsaldotransactie in het grootboek</span><span class="sxs-lookup"><span data-stu-id="0cbc8-112">Beginning balance transaction in the general ledger</span></span>
* <span data-ttu-id="0cbc8-113">In voorraad aantallen voor voorraadartikelen</span><span class="sxs-lookup"><span data-stu-id="0cbc8-113">On-hand quantities for inventory items</span></span>
* <span data-ttu-id="0cbc8-114">Open documenten voor klanten en leveranciers, zoals facturen, creditnota's en betalingen</span><span class="sxs-lookup"><span data-stu-id="0cbc8-114">Open documents for customers and vendors, such as invoices, credit memos, and payments</span></span>

<span data-ttu-id="0cbc8-115">Wij migreren alleen hele bedragen op verkoop- en inkoopdocumenten.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-115">We migrate only full amounts on sales and purchase documents.</span></span> <span data-ttu-id="0cbc8-116">We werken geen gedeeltelijk betaalde bedragen bij.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-116">We do not update partially paid amounts.</span></span> <span data-ttu-id="0cbc8-117">Als een klant bijvoorbeeld 300 van een totaal van 500 euro op een verkoopfactuur heeft voldaan, migreren we de hele 500.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-117">For example, if a customer has paid 300 of a total of 500 dollars on a sales invoice, we migrate the full 500.</span></span> <span data-ttu-id="0cbc8-118">Wanneer u gedeeltelijke betalingen hebt ontvangen, moet u deze handmatig bijwerken, voordat of nadat u gegevens migreert.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-118">If you have received partial payments, you must update these manually, either before or after you migrate data.</span></span> <span data-ttu-id="0cbc8-119">Het is raadzaam openstaande transacties te vereffenen voordat u migreert, om zaken achteraf gemakkelijker te maken.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-119">We recommend that you apply outstanding transactions before you migrate, just to make things easier afterward.</span></span>

> [!NOTE]  
>   <span data-ttu-id="0cbc8-120">Wij migreren geen inkooporders of verkooporders.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-120">We do not migrate purchase orders or sales orders.</span></span>

## <a name="before-you-start"></a><span data-ttu-id="0cbc8-121">Voordat u begint</span><span class="sxs-lookup"><span data-stu-id="0cbc8-121">Before you start</span></span>
<span data-ttu-id="0cbc8-122">Een belangrijk deel van het migratieproces is de rekeningen opgeven waarnaar transacties moeten worden gemigreerd.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-122">An important part of the migration process is to specify the accounts to migrate transactions to.</span></span> <span data-ttu-id="0cbc8-123">Het is aan te raden deze koppeling te plannen voordat u gegevens migreert.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-123">It's a good idea to plan this mapping before you migrate data.</span></span> <span data-ttu-id="0cbc8-124">Bijvoorbeeld, de rekeningen waarnaar u transacties boekt voor:</span><span class="sxs-lookup"><span data-stu-id="0cbc8-124">For example, the accounts where you post transactions for:</span></span>  
  
* <span data-ttu-id="0cbc8-125">De verkoop van artikelen of services aan klanten.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-125">The sale of items or services to customers.</span></span>
* <span data-ttu-id="0cbc8-126">De aankoop van artikelen of services van leveranciers.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-126">The purchase of items or services from vendors.</span></span>  
* <span data-ttu-id="0cbc8-127">Herwaarderingen in het grootboek.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-127">Adjustments in the general ledger.</span></span>  

[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="0cbc8-128"> vereist dat aan grootboekrekeningen rekeningnummers zijn toegewezen.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-128"> requires that general ledger accounts have account numbers assigned to them.</span></span> <span data-ttu-id="0cbc8-129">Zorg ervoor dat rekeningnummers zijn toegewezen aan uw rekeningen in QuickBooks Online.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-129">Make sure that account numbers are assigned to your accounts in QuickBooks Online.</span></span>

<span data-ttu-id="0cbc8-130">Als transacties in QuickBooks Online belastingbedragen hebben, moet u eerst een belastingrekening instellen voor uw belastingjurisdictie in [!INCLUDE[d365fin](includes/d365fin_md.md)], voordat u transacties kunt boeken.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-130">If transactions in QuickBooks Online have tax amounts, you must set up a tax account for your tax jurisdictions in [!INCLUDE[d365fin](includes/d365fin_md.md)] before you can post transactions.</span></span>

## <a name="how-do-i-start-using-the-extension"></a><span data-ttu-id="0cbc8-131">Hoe kan ik beginnen de extensie te gebruiken?</span><span class="sxs-lookup"><span data-stu-id="0cbc8-131">How do I start using the extension?</span></span>
<span data-ttu-id="0cbc8-132">Aan de slag gaan is eenvoudig.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-132">Getting started is easy.</span></span> <span data-ttu-id="0cbc8-133">Het enige wat u moet doen is de begeleide instelling **Gegevensmigratie** uitvoeren.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-133">All you need to do is run the **Data Migration** assisted setup guide.</span></span> <span data-ttu-id="0cbc8-134">U doet dat als volgt:</span><span class="sxs-lookup"><span data-stu-id="0cbc8-134">Here's how:</span></span>

1. <span data-ttu-id="0cbc8-135">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Begeleide instelling** in en kies vervolgens **Bedrijfsgegevens migreren**.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-135">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Assisted Setup**, and then choose **Migrate business data**.</span></span>
2. <span data-ttu-id="0cbc8-136">Volg de instructies in elke stap in de begeleide instelling.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-136">Follow the instructions on each step in the assisted setup guide.</span></span>

## <a name="what-do-i-do-after-i-migrate-data"></a><span data-ttu-id="0cbc8-137">Wat doe ik nadat ik gegevens heb gemigreerd?</span><span class="sxs-lookup"><span data-stu-id="0cbc8-137">What do I do after I migrate data?</span></span>
<span data-ttu-id="0cbc8-138">Nadat u gegevens migreert, hebben transacties de status **Niet geboekt**, zodat u deze kunt controleren en correcties kunt aanbrengen.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-138">After you migrate data, transactions have the status **Unposted**, so you can review them and make adjustments.</span></span> <span data-ttu-id="0cbc8-139">Als u de transacties wilt controleren, gaat u naar de pagina waar u deze normaal zou vinden.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-139">To review the transactions, go to the page where you would normally find them.</span></span> <span data-ttu-id="0cbc8-140">Als u bijvoorbeeld ongeboekte verkoopfacturen wilt controleren, gaat u naar de pagina **Verkoopfacturen**.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-140">For example, to review unposted sales invoices, go to the **Sales Invoices** page.</span></span> <span data-ttu-id="0cbc8-141">Als u betalingsdagboeken wilt controleren, gaat u naar de pagina **Betalingsdagboeken**.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-141">To review payment journals, go to the **Payment Journals** page.</span></span>   

<span data-ttu-id="0cbc8-142">Er zijn enkele dingen die u met name moet doen:</span><span class="sxs-lookup"><span data-stu-id="0cbc8-142">There are a few things in particular that you should do:</span></span>

* <span data-ttu-id="0cbc8-143">Als de transacties in QuickBooks Online opslag- of kortingsbedragen bevatten, moet u de bedragen handmatig toevoegen aan de gerelateerde transacties in [!INCLUDE[d365fin](includes/d365fin_md.md)] voordat u deze boekt.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-143">If the transactions in QuickBooks Online had markup or discount amounts, you must manually add the amounts to the related transactions in [!INCLUDE[d365fin](includes/d365fin_md.md)] before you post them.</span></span>
* <span data-ttu-id="0cbc8-144">Als u btw gebruikt, hebt u mogelijk een bedrijfsboekingsgroep en een productboekingsgroep in de boekingsinstellingen nodig, zodat u btw-bedragen kunt boeken.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-144">If you are using value added tax (VAT), you may need to add a business posting group and a product posting group to the posting setup so that you can post VAT amounts.</span></span>
* <span data-ttu-id="0cbc8-145">Controleer de beginsaldi voor de rekeningen in het grootboek.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-145">Verify the beginning balances for accounts in the general ledger.</span></span> <span data-ttu-id="0cbc8-146">Online QuickBooks slaat het huidige saldo van alle rekeningen niet op, dus u moet mogelijk beginsaldi corrigeren.</span><span class="sxs-lookup"><span data-stu-id="0cbc8-146">QuickBooks Online does not store the current balance for all accounts, so you might need to correct beginning balances.</span></span>

## <a name="see-also"></a><span data-ttu-id="0cbc8-147">Zie ook</span><span class="sxs-lookup"><span data-stu-id="0cbc8-147">See Also</span></span>
[<span data-ttu-id="0cbc8-148">Bedrijfsgegevens importeren uit andere financiële systemen</span><span class="sxs-lookup"><span data-stu-id="0cbc8-148">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="0cbc8-149">[[!INCLUDE[d365fin](includes/d365fin_md.md)] aanpassen met behulp van extensies](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="0cbc8-149">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  


---
title: 'Procedure: Werken met cheques'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 421516a7580a90d6eabc8ecfcc841215839994c9
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-work-with-checks"></a><span data-ttu-id="4b174-102">Procedure: Werken met cheques</span><span class="sxs-lookup"><span data-stu-id="4b174-102">How to: Work With Checks</span></span>
<span data-ttu-id="4b174-103">Dynamics NAV ondersteunt het elektronisch en handmatig verzenden van cheques.</span><span class="sxs-lookup"><span data-stu-id="4b174-103">Dynamics NAV supports electronic and manual check issuance.</span></span> <span data-ttu-id="4b174-104">Bij beide methoden wordt het betalingsdagboek gebruikt om cheques te verzenden naar leveranciers.</span><span class="sxs-lookup"><span data-stu-id="4b174-104">Both methods use the payment journal to issue checks to vendors.</span></span> <span data-ttu-id="4b174-105">Daarnaast kunt u cheques nietig verklaren en chequeposten weergeven.</span><span class="sxs-lookup"><span data-stu-id="4b174-105">You can also void checks and view check ledger entries.</span></span>

<span data-ttu-id="4b174-106">Bij het proces voor het uitgeven van cheques worden betalingen voorgesteld, worden posten gemaakt en worden de computercheques afgedrukt.</span><span class="sxs-lookup"><span data-stu-id="4b174-106">The process of issuing checks suggests payments, creates ledger entries, and prints the computer checks.</span></span>

<span data-ttu-id="4b174-107">De printer moet correct zijn ingesteld op het afdrukken van chequeformulieren en u moet bepalen welke indeling wordt gebruikt.</span><span class="sxs-lookup"><span data-stu-id="4b174-107">Your printer must be correctly set up with the check forms, and you must define which check layout to use.</span></span> <span data-ttu-id="4b174-108">Zie voor meer informatie [Procedure: Cheque-indelingen definiëren](finance-setup-how-define-check-layouts.md)</span><span class="sxs-lookup"><span data-stu-id="4b174-108">For more information, see [How to: Define Check Layouts](finance-setup-how-define-check-layouts.md)</span></span>

## <a name="to-issue-checks"></a><span data-ttu-id="4b174-109">Cheques uitgeven</span><span class="sxs-lookup"><span data-stu-id="4b174-109">To issue checks</span></span>
1. <span data-ttu-id="4b174-110">Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Betalingsdagboeken** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="4b174-110">In the top right corner, choose the **Search for Page or Report** icon, enter **Payment Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="4b174-111">Vul het dagboek met relevante betalingen, bijvoorbeeld met behulp van de functie Leveranciersbetalingen voorstellen.</span><span class="sxs-lookup"><span data-stu-id="4b174-111">Fill in the journal with relevant payments, for example by using the Suggest Vendor Payments function.</span></span> <span data-ttu-id="4b174-112">Zie voor meer informatie [Procedure: Leveranciersbetalingen voorstellen](payables-how-suggest-vendor-payments.md).</span><span class="sxs-lookup"><span data-stu-id="4b174-112">For more information, see [How to: Suggest Vendor Payments](payables-how-suggest-vendor-payments.md).</span></span>
3. <span data-ttu-id="4b174-113">Selecteer een van de volgende opties in het veld **Betalingssoort** op dagboekregels voor betalingen die u wilt doen met cheques:</span><span class="sxs-lookup"><span data-stu-id="4b174-113">In the **Bank Payment Type** field on journal lines for payment that you want to make with checks, select one of the following options:</span></span>

 - <span data-ttu-id="4b174-114">**Automatische cheque**: selecteer deze optie als u een cheque wilt afdrukken voor het bedrag op de betalingsdagboekregel.</span><span class="sxs-lookup"><span data-stu-id="4b174-114">**Computer Check**: Select this option if you want to print a check for the amount on the payment journal line.</span></span> <span data-ttu-id="4b174-115">U moet de cheques afdrukken voordat u de dagboekregels kunt boeken.</span><span class="sxs-lookup"><span data-stu-id="4b174-115">You must print the checks before you can post the journal lines.</span></span> <span data-ttu-id="4b174-116">U kunt **Automatische cheque** alleen selecteren als het **Tegenrekeningsoort** of het **Rekeningsoort** **Bankrekening** is.</span><span class="sxs-lookup"><span data-stu-id="4b174-116">You can only select **Computer Check** if the **Bal. Account Type** or the **Account Type** is **Bank Account**.</span></span>

 - <span data-ttu-id="4b174-117">**Handmatige cheque**: selecteer deze optie als u handmatig een cheque hebt gemaakt en er een bijbehorende chequepost moet worden gemaakt voor dit bedrag.</span><span class="sxs-lookup"><span data-stu-id="4b174-117">**Manual Check**: Select this option if you have created a check manually and want to create a corresponding check ledger entry for this amount.</span></span> <span data-ttu-id="4b174-118">Met deze optie kunt u geen cheques afdrukken vanuit Dynamics NAV.</span><span class="sxs-lookup"><span data-stu-id="4b174-118">By using this option, you cannot print checks from Dynamics NAV.</span></span> <span data-ttu-id="4b174-119">U kunt **Handmatige cheque** alleen selecteren als het **Tegenrekeningsoort** of het **Rekeningsoort** **Bankrekening** is.</span><span class="sxs-lookup"><span data-stu-id="4b174-119">You can only select **Manual Check** if the **Bal. Account Type** or the **Account Type** is **Bank Account**.</span></span>

    <span data-ttu-id="4b174-120">**Opmerking**: u moet automatische cheques afdrukken voordat u de gerelateerde dagboekregels boekt.</span><span class="sxs-lookup"><span data-stu-id="4b174-120">**Note**: You must print computer checks before you post the related journal lines.</span></span>
4. <span data-ttu-id="4b174-121">In het geval van automatische cheques kiest u **Cheque afdrukken**.</span><span class="sxs-lookup"><span data-stu-id="4b174-121">In case of computer checks, choose **Print Check**.</span></span>
5. <span data-ttu-id="4b174-122">Vul indien nodig de velden in het venster **Cheque** in.</span><span class="sxs-lookup"><span data-stu-id="4b174-122">In the **Check** window, fill in the fields as necessary.</span></span> <span data-ttu-id="4b174-123">Kies een veld om een korte omschrijving van het veld of een koppeling naar meer informatie te lezen.</span><span class="sxs-lookup"><span data-stu-id="4b174-123">Choose a field to read a short description of the field or link to more information.</span></span>
6. <span data-ttu-id="4b174-124">Klik op **Afdrukken**.</span><span class="sxs-lookup"><span data-stu-id="4b174-124">Choose the **Print** button.</span></span>

<span data-ttu-id="4b174-125">**Opmerking**: als u cheques in meerdere valuta's van verschillende bankrekeningen wilt afdrukken, moet u de batchverwerking **Cheque afdrukken** voor elke valuta afzonderlijk uitvoeren en de juiste bankrekening opgeven.</span><span class="sxs-lookup"><span data-stu-id="4b174-125">**Note**: If you want to print checks in more than one currency from different bank accounts, you must run the **Print Check** batch job separately for each currency and specify the appropriate bank account.</span></span>

## <a name="to-cancel-printed-checks-that-are-not-posted"></a><span data-ttu-id="4b174-126">Afgedrukte cheques annuleren die niet zijn geboekt</span><span class="sxs-lookup"><span data-stu-id="4b174-126">To cancel printed checks that are not posted</span></span>
<span data-ttu-id="4b174-127">U kunt niet-geboekte cheques annuleren nadat ze zijn afgedrukt door de actie **Ongeldige cheque** in het venster **Betalingsdagboek** te gebruiken.</span><span class="sxs-lookup"><span data-stu-id="4b174-127">You can cancel non-posted checks after they have been printed by using the **Void Check** action in the **Payment Journal** window.</span></span>
1. <span data-ttu-id="4b174-128">Kies in het venster **Betalingsdagboek** de actie **Ongeldige cheque** en kies vervolgens welke cheques u wilt annuleren.</span><span class="sxs-lookup"><span data-stu-id="4b174-128">In the **Payment Journal** window, choose the **Void Check**, and then choose which checks to cancel.</span></span>

## <a name="to-void-checks"></a><span data-ttu-id="4b174-129">Cheques nietig verklaren</span><span class="sxs-lookup"><span data-stu-id="4b174-129">To void checks</span></span>
<span data-ttu-id="4b174-130">Wanneer chequebetaling is geboekt, kunt u cheques alleen annuleren (nietig verklaren) vanuit de resulterende bankposten.</span><span class="sxs-lookup"><span data-stu-id="4b174-130">When check payment have been posted, you can only cancel (void) checks from the resulting bank ledger entries.</span></span>

1. <span data-ttu-id="4b174-131">Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, voer **Bankrekeningen** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="4b174-131">In the top right corner, choose the **Search for Page or Report** icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="4b174-132">Selecteer de betreffende bankrekening, kies de actie **Bewerken** en kies vervolgens de actie **Chequeposten**.</span><span class="sxs-lookup"><span data-stu-id="4b174-132">Select the relevant bank account, choose the **Edit** action, and then choose the **Check Ledger Entries** action.</span></span>
3. <span data-ttu-id="4b174-133">Kies in het venster **Chequeposten** de actie **Ongeldige cheque**.</span><span class="sxs-lookup"><span data-stu-id="4b174-133">In the **Check Ledger Entries** window, choose the **Void Check** action.</span></span>
4. <span data-ttu-id="4b174-134">Schakel het selectievakje **Cheque alleen nietig verklaren** in.</span><span class="sxs-lookup"><span data-stu-id="4b174-134">Select the **Void Check Only** check box.</span></span>
5. <span data-ttu-id="4b174-135">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="4b174-135">Choose the **OK**button.</span></span>

## <a name="see-also"></a><span data-ttu-id="4b174-136">Zie ook</span><span class="sxs-lookup"><span data-stu-id="4b174-136">See Also</span></span>
[<span data-ttu-id="4b174-137">Betalingsverplichtingen beheren</span><span class="sxs-lookup"><span data-stu-id="4b174-137">Manage Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="4b174-138">Bankieren instellen</span><span class="sxs-lookup"><span data-stu-id="4b174-138">Set Up Banking</span></span>](bank-setup-banking.md)  


---
title: Automatisch recordinteracties met contacten vastleggen
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
ms.openlocfilehash: 50e5d44cc9575dbfcb3181c465e2d16d6d135369
ms.contentlocale: nl-nl
ms.lasthandoff: 06/26/2017

---
# <a name="prepare-pre-closing-reports"></a><span data-ttu-id="784db-102">Rapporten voorbereiden die voorafgaan aan een afsluiting</span><span class="sxs-lookup"><span data-stu-id="784db-102">Prepare Pre-Closing Reports</span></span>
<span data-ttu-id="784db-103">Er staan veel standaardrapporten tot uw beschikking voor het verifiëren van de nauwkeurigheid van de rekeningen voor u de boeken sluit aan het eind van een jaar of een periode.</span><span class="sxs-lookup"><span data-stu-id="784db-103">There are many standard reports that you can use to verify the accuracy of the accounts before closing the books at the end of a year or period.</span></span> <span data-ttu-id="784db-104">U kunt bijvoorbeeld het rapport **Klant - Proefbalans** gebruiken om na te gaan of het saldo van een klantboekingsgroep gelijk is aan het saldo op de overeenkomstige grootboekrekening op een bepaalde datum.</span><span class="sxs-lookup"><span data-stu-id="784db-104">For example, you can use the **Customer - Trial Balance** report to verify that the balance for a customer posting group is equal to the balance on the corresponding general ledger account on a certain date.</span></span>

<span data-ttu-id="784db-105">In de volgende tabel wordt een beschrijving gegeven van een aantal rapporten die nuttig kunnen zijn in dit proces, samen met de rapportnaam.</span><span class="sxs-lookup"><span data-stu-id="784db-105">The following table describes a number of reports that may be useful in this process along with the report name.</span></span>

|<span data-ttu-id="784db-106">Als u dit wilt doen</span><span class="sxs-lookup"><span data-stu-id="784db-106">To</span></span>     |<span data-ttu-id="784db-107">Dit rapport raadplegen</span><span class="sxs-lookup"><span data-stu-id="784db-107">See this report</span></span>       |
|-------|----------------------|
|<span data-ttu-id="784db-108">Een gedetailleerd proefbalansrapport af te drukken van één of meer bankrekeningen met aanvullende informatie over afzonderlijke posten.</span><span class="sxs-lookup"><span data-stu-id="784db-108">Print a detailed trial balance report for one or more bank accounts with additional information about individual entries.</span></span>|<span data-ttu-id="784db-109">Bankrekening</span><span class="sxs-lookup"><span data-stu-id="784db-109">Bank Acc.</span></span> <span data-ttu-id="784db-110">- gedetailleerde proefbalans</span><span class="sxs-lookup"><span data-stu-id="784db-110">- Detail Trial Bal.</span></span>|
|<span data-ttu-id="784db-111">Een gedetailleerd proefbalansrapport af te drukken voor bepaalde klanten.</span><span class="sxs-lookup"><span data-stu-id="784db-111">Print a detail trial balance for selected customers.</span></span>|<span data-ttu-id="784db-112">Klant: proefbalans</span><span class="sxs-lookup"><span data-stu-id="784db-112">Customer - Trial Balance</span></span>|
|<span data-ttu-id="784db-113">Een gedetailleerd proefbalansrapport af te drukken met uitvoerige informatie over afzonderlijke posten, voor bepaalde klanten gedurende een bepaalde periode.</span><span class="sxs-lookup"><span data-stu-id="784db-113">Print a detail trial balance with detailed information about individual entries, for selected customers during a selected period.</span></span>|<span data-ttu-id="784db-114">Klant - Historie</span><span class="sxs-lookup"><span data-stu-id="784db-114">Customer - Detail Trial Bal.</span></span>|
|<span data-ttu-id="784db-115">Een gedetailleerd proefbalansrapport af te drukken voor bepaalde leveranciers.</span><span class="sxs-lookup"><span data-stu-id="784db-115">Print a detail trial balance for selected vendors.</span></span>|<span data-ttu-id="784db-116">Leverancier - Proefbalans</span><span class="sxs-lookup"><span data-stu-id="784db-116">Vendor - Trial Balance</span></span>|
|<span data-ttu-id="784db-117">Een gedetailleerd proefbalansrapport af te drukken met uitvoerige informatie over afzonderlijke posten, voor bepaalde leveranciers gedurende een bepaalde periode.</span><span class="sxs-lookup"><span data-stu-id="784db-117">Print a detail trial balance with detailed information about individual entries, for selected vendors during a selected period.</span></span>|<span data-ttu-id="784db-118">Leverancier - Historie</span><span class="sxs-lookup"><span data-stu-id="784db-118">Vendor - Detail Trial Balance</span></span>|
|<span data-ttu-id="784db-119">Een proefbalans af te drukken met de cijfers van het huidige en het voorgaande jaar.</span><span class="sxs-lookup"><span data-stu-id="784db-119">Print a trial balance with the current year's and the previous year's figures.</span></span>|<span data-ttu-id="784db-120">Proefbalans afsluiten</span><span class="sxs-lookup"><span data-stu-id="784db-120">Closing Trial Balance</span></span>|
|<span data-ttu-id="784db-121">Een gedetailleerd proefbalansrapport af te drukken voor saldo's van grootboekrekeningen.</span><span class="sxs-lookup"><span data-stu-id="784db-121">Print a detailed trial balance report for general ledger account balances.</span></span>|<span data-ttu-id="784db-122">Proefbalans Detail</span><span class="sxs-lookup"><span data-stu-id="784db-122">Detail Trial Balance</span></span>|
|<span data-ttu-id="784db-123">Een proefbalansrapport af te drukken met saldo's en nettowijzigingen van grootboekrekeningen.</span><span class="sxs-lookup"><span data-stu-id="784db-123">Print a trial balance report with balances and net changes for general ledger accounts.</span></span>|<span data-ttu-id="784db-124">Proefbalans</span><span class="sxs-lookup"><span data-stu-id="784db-124">Trial Balance</span></span>|
|<span data-ttu-id="784db-125">Een proefbalans af te drukken voor een geconsolideerd bedrijf.</span><span class="sxs-lookup"><span data-stu-id="784db-125">Print a trial balance for a consolidated company.</span></span>|<span data-ttu-id="784db-126">Consolidatie - Proefbalans</span><span class="sxs-lookup"><span data-stu-id="784db-126">Consolidated Trial Balance</span></span>|
<span data-ttu-id="784db-127">Als u een rapport wilt bekijken, kiest u in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport**, typt u de naam zoals deze in de tabel wordt weergegeven en kiest u vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="784db-127">To see a report, in the top right corner, choose the **Search for Page or Report** icon, type the name as it appears in the table, and then choose the related link.</span></span>

## <a name="see-also"></a><span data-ttu-id="784db-128">Zie ook</span><span class="sxs-lookup"><span data-stu-id="784db-128">See Also</span></span>
[<span data-ttu-id="784db-129">Jaren en perioden afsluiten</span><span class="sxs-lookup"><span data-stu-id="784db-129">Close Years and Periods</span></span>](year-close-years-periods.md)


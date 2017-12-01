---
title: Elektronische btw- en ICP-aangiften maken
description: Als u elektronische btw- en ICP-aangiften wilt maken, moet u eerst de aangifte instellen met het venster **Elek. aangifte-instellingen**. Vervolgens kunt u ze naar de belastingdienst verzenden.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: e2829359f76092488cc165f0b15b9ba1cbd3aae8
ms.contentlocale: nl-nl
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-create-electronic-vat-and-icp-declarations"></a><span data-ttu-id="f251b-104">Procedure: Elektronische btw- en ICP-aangiften maken</span><span class="sxs-lookup"><span data-stu-id="f251b-104">How to: Create Electronic VAT and ICP Declarations</span></span>
<span data-ttu-id="f251b-105">Als u elektronische btw- en ICP-aangiften wilt maken, moet u eerst de aangifte instellen met het venster **Elek. aangifte-instellingen**.</span><span class="sxs-lookup"><span data-stu-id="f251b-105">To create electronic VAT and ICP declarations, you must first set up the declaration using the **Elec. Tax Declaration Setup** window.</span></span> <span data-ttu-id="f251b-106">Vervolgens kunt u ze naar de belastingdienst verzenden.</span><span class="sxs-lookup"><span data-stu-id="f251b-106">Then you can submit them to the tax authorities.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="f251b-107">Als u het veld **Deel van Fiscale eenheid** in het venster **Elek. aangifte-instellingen** hebt geselecteerd, kunt u een elektronische aangifte voor slechts één bedrijf maken.</span><span class="sxs-lookup"><span data-stu-id="f251b-107">If you have selected the **Part of Fiscal Entity** field in the **Elec. Tax Declaration Setup** window, then you can create an electronic declaration for only one company.</span></span> <span data-ttu-id="f251b-108">Als u de btw-gegevens van alle dochterondernemingen van een moedermaatschappij wilt combineren, moet u een btw-aangifte op papier opstellen voor elke dochteronderneming en handmatig de totaalbedragen voor de moedermaatschappij berekenen.</span><span class="sxs-lookup"><span data-stu-id="f251b-108">If you want to combine the tax information for all subsidiaries of a holding company, you must create a VAT statement on paper for each subsidiary company and manually calculate the total amounts for the holding company.</span></span> <span data-ttu-id="f251b-109">Deze totaalbedragen van de moedermaatschappij moeten worden ingevoerd op de website van de belastingdienst.</span><span class="sxs-lookup"><span data-stu-id="f251b-109">These total amounts of the holding company must be entered on the website of the tax authorities.</span></span> <span data-ttu-id="f251b-110">U kunt geen belastinggegevens van ICP-aangiften combineren.</span><span class="sxs-lookup"><span data-stu-id="f251b-110">You cannot combine tax information for ICP declarations.</span></span> <span data-ttu-id="f251b-111">ICP-aangiften moeten altijd afzonderlijk worden ingediend.</span><span class="sxs-lookup"><span data-stu-id="f251b-111">ICP declarations must always be submitted individually.</span></span>  

<span data-ttu-id="f251b-112">Als er geen intracommunautaire leveringen zijn geweest in de aangifteperiode, dan wordt er een elektronische ICP-aangifte aangemaakt zonder XML-elementen voor de leveringen.</span><span class="sxs-lookup"><span data-stu-id="f251b-112">If there are no intra-community deliveries in the declaration period, then an electronic ICP declaration is created without XML elements for the deliveries.</span></span> <span data-ttu-id="f251b-113">Als u een dergelijke aangifte verzendt, wordt een foutbericht weergegeven.</span><span class="sxs-lookup"><span data-stu-id="f251b-113">If you submit such a declaration, an error message will be displayed.</span></span>  

## <a name="to-create-an-electronic-vat-or-icp-declaration"></a><span data-ttu-id="f251b-114">Een elektronische btw- of ICP-aangifte maken</span><span class="sxs-lookup"><span data-stu-id="f251b-114">To create an electronic VAT or ICP declaration</span></span>  

1.  <span data-ttu-id="f251b-115">Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Elektronische aangiften** in en kies de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="f251b-115">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Elec. Tax Declarations**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f251b-116">Kies in het venster **Overzicht elektronische aangiften** de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="f251b-116">In the **Elec. Tax Declaration List** window, choose the **New** action.</span></span>  
3.  <span data-ttu-id="f251b-117">Vul in het venster **Elektronische aangiftekaart** op het sneltabblad **Algemeen** de vereiste velden in zoals beschreven in de volgende tabel.</span><span class="sxs-lookup"><span data-stu-id="f251b-117">In the **Elec. Tax Declaration Card** window, on the **General** FastTab, fill in the required fields as described in the following table.</span></span>  

    |<span data-ttu-id="f251b-118">Veld</span><span class="sxs-lookup"><span data-stu-id="f251b-118">Field</span></span>|<span data-ttu-id="f251b-119">Description</span><span class="sxs-lookup"><span data-stu-id="f251b-119">Description</span></span>|  
    |-----------------------------------|---------------------------------------|  
    |<span data-ttu-id="f251b-120">**Sjabloonnaam**</span><span class="sxs-lookup"><span data-stu-id="f251b-120">**Template Name**</span></span>|<span data-ttu-id="f251b-121">De naam van de sjabloon die wordt gebruikt om de elektronische aangifte te maken.</span><span class="sxs-lookup"><span data-stu-id="f251b-121">The name of the template that will be used to create the electronic declaration.</span></span>|  
    |<span data-ttu-id="f251b-122">**Aangifte**</span><span class="sxs-lookup"><span data-stu-id="f251b-122">**Statement Name**</span></span>|<span data-ttu-id="f251b-123">De naam van het afschrift dat wordt gebruikt om de elektronische aangifte te maken.</span><span class="sxs-lookup"><span data-stu-id="f251b-123">The name of the statement that will be used to create the electronic declaration.</span></span>|  

6.  <span data-ttu-id="f251b-124">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="f251b-124">Choose the **OK** button.</span></span>  

<span data-ttu-id="f251b-125">De XML-elementen met de bijbehorende gegevens van de elektronische aangifte worden weergegeven op het sneltabblad **Regels** in het venster **Elektronische aangiftekaart**.</span><span class="sxs-lookup"><span data-stu-id="f251b-125">The XML elements and the accompanying data of the electronic declaration are displayed on the **Lines** FastTab in the **Elec. Tax Declaration Card** window.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f251b-126">Zie ook</span><span class="sxs-lookup"><span data-stu-id="f251b-126">See Also</span></span>  
 <span data-ttu-id="f251b-127">[Elektronische belastingaangiften](electronic-tax-declarations.md) </span><span class="sxs-lookup"><span data-stu-id="f251b-127">[Electronic Tax Declarations](electronic-tax-declarations.md) </span></span>  
 <span data-ttu-id="f251b-128">[Elektronische btw- en ICP-aangiften](electronic-vat-and-icp-declarations.md) </span><span class="sxs-lookup"><span data-stu-id="f251b-128">[Electronic VAT and ICP Declarations](electronic-vat-and-icp-declarations.md) </span></span>  
 [<span data-ttu-id="f251b-129">Procedure: Btw-categorieën instellen</span><span class="sxs-lookup"><span data-stu-id="f251b-129">How to: Set Up VAT Categories</span></span>](how-to-set-up-vat-categories.md)


---
title: "Btw-categorieën instellen"
description: Als u de elektronische btw-aangifte wilt gebruiken, moet u een btw-categoriecode voor alle XML-elementen in de elektronische btw-aangifte instellen.
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
ms.openlocfilehash: c1f85bc8bec383ab97f4ddf89ac157f33f248259
ms.contentlocale: nl-nl
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-set-up-vat-categories"></a><span data-ttu-id="63847-103">Procedure: Btw-categorieën instellen</span><span class="sxs-lookup"><span data-stu-id="63847-103">How to: Set Up VAT Categories</span></span>
<span data-ttu-id="63847-104">Als u de elektronische btw-aangifte wilt gebruiken, moet u een btw-categoriecode voor alle XML-elementen in de elektronische btw-aangifte instellen.</span><span class="sxs-lookup"><span data-stu-id="63847-104">To use the electronic VAT declaration, you must set up a VAT category code for all XML elements in the electronic VAT declaration.</span></span>  

<span data-ttu-id="63847-105">U moet alle mogelijke categorie- en subcategoriecombinaties instellen die een XML-element in de elektronische btw-aangifte voorstellen.</span><span class="sxs-lookup"><span data-stu-id="63847-105">You must set up all of the possible category and subcategory combinations that represent an XML element in the electronic VAT declaration.</span></span> <span data-ttu-id="63847-106">Vervolgens kunt u de btw-aangiftegegevens direct aan een XML-element toewijzen.</span><span class="sxs-lookup"><span data-stu-id="63847-106">Then, you can map the VAT statement data directly to an XML element.</span></span>  

## <a name="to-set-up-a-vat-category"></a><span data-ttu-id="63847-107">Een btw-categorie instellen</span><span class="sxs-lookup"><span data-stu-id="63847-107">To set up a VAT category</span></span>  

1.  <span data-ttu-id="63847-108">Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Elektronische aangifte btw-categorieën** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="63847-108">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Elec. Tax. Decl. VAT Categories**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="63847-109">Kies in het venster **Elektronische aangifte btw-categorieën** de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="63847-109">In the **Elec. Tax. Decl. VAT Categories** window, choose the **New** action.</span></span>  
3.  <span data-ttu-id="63847-110">Vul de velden in zoals beschreven in de volgende tabel.</span><span class="sxs-lookup"><span data-stu-id="63847-110">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="63847-111">Veld</span><span class="sxs-lookup"><span data-stu-id="63847-111">Field</span></span>|<span data-ttu-id="63847-112">Description</span><span class="sxs-lookup"><span data-stu-id="63847-112">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="63847-113">**Code**</span><span class="sxs-lookup"><span data-stu-id="63847-113">**Code**</span></span>|<span data-ttu-id="63847-114">De unieke code voor elke categorie- en subcategoriecombinatie.</span><span class="sxs-lookup"><span data-stu-id="63847-114">The unique code for each category and subcategory combination.</span></span> <span data-ttu-id="63847-115">U kunt maximaal 10 alfanumerieke tekens invoeren.</span><span class="sxs-lookup"><span data-stu-id="63847-115">You can enter a maximum of 10 alphanumeric characters.</span></span>|  
    |<span data-ttu-id="63847-116">**Categorie**</span><span class="sxs-lookup"><span data-stu-id="63847-116">**Category**</span></span>|<span data-ttu-id="63847-117">Geef de hoofdcategorieoptie voor de btw-aangifte op.</span><span class="sxs-lookup"><span data-stu-id="63847-117">Specify the main category option for the VAT statement.</span></span>|  
    |<span data-ttu-id="63847-118">**Door ons (Binnenland)**</span><span class="sxs-lookup"><span data-stu-id="63847-118">**By Us (Domestic)**</span></span>|<span data-ttu-id="63847-119">De subcategorie voor de btw-aangifte.</span><span class="sxs-lookup"><span data-stu-id="63847-119">The subcategory for the VAT Statement.</span></span><br /><br /> <span data-ttu-id="63847-120">Selecteer hier een subcategorie als het veld **Categorie** **Door ons (Binnenland)** bevat.</span><span class="sxs-lookup"><span data-stu-id="63847-120">Select a subcategory here if the **Category** field displays **By Us (Domestic)**.</span></span>|  
    |<span data-ttu-id="63847-121">**Aan ons (Binnenland)**</span><span class="sxs-lookup"><span data-stu-id="63847-121">**To Us (Domestic)**</span></span>|<span data-ttu-id="63847-122">De subcategorie voor de btw-aangifte.</span><span class="sxs-lookup"><span data-stu-id="63847-122">The subcategory for the VAT Statement.</span></span><br /><br /> <span data-ttu-id="63847-123">Selecteer hier een subcategorie als het veld **Categorie** **Aan ons (Binnenland)** bevat.</span><span class="sxs-lookup"><span data-stu-id="63847-123">Select a subcategory here if the **Category** field displays **To Us (Domestic)**.</span></span>|  
    |<span data-ttu-id="63847-124">**Door ons (Buitenland)**</span><span class="sxs-lookup"><span data-stu-id="63847-124">**By Us (Foreign)**</span></span>|<span data-ttu-id="63847-125">De subcategorie voor de btw-aangifte.</span><span class="sxs-lookup"><span data-stu-id="63847-125">The subcategory for the VAT Statement.</span></span><br /><br /> <span data-ttu-id="63847-126">Selecteer hier een subcategorie als het veld **Categorie** **Door ons (Buitenland)** bevat.</span><span class="sxs-lookup"><span data-stu-id="63847-126">Select a subcategory here if the **Category** field displays **By Us (Foreign)**.</span></span>|  
    |<span data-ttu-id="63847-127">**Aan ons (Buitenland)**</span><span class="sxs-lookup"><span data-stu-id="63847-127">**To Us (Foreign)**</span></span>|<span data-ttu-id="63847-128">De subcategorie voor de btw-aangifte.</span><span class="sxs-lookup"><span data-stu-id="63847-128">The subcategory for the VAT Statement.</span></span><br /><br /> <span data-ttu-id="63847-129">Selecteer hier een subcategorie als het veld **Categorie** **Aan ons (Buitenland)** bevat.</span><span class="sxs-lookup"><span data-stu-id="63847-129">Select a subcategory here if the **Category** field displays **To Us (Foreign)**.</span></span>|  
    |<span data-ttu-id="63847-130">**Berekening**</span><span class="sxs-lookup"><span data-stu-id="63847-130">**Calculation**</span></span>|<span data-ttu-id="63847-131">De subcategorie voor de btw-aangifte.</span><span class="sxs-lookup"><span data-stu-id="63847-131">The subcategory for the VAT Statement.</span></span><br /><br /> <span data-ttu-id="63847-132">Selecteer hier een subcategorie als het veld **Categorie** **Berekening** bevat.</span><span class="sxs-lookup"><span data-stu-id="63847-132">Select a subcategory here if the **Category** field displays **Calculation**.</span></span>|  
    |<span data-ttu-id="63847-133">**Optioneel**</span><span class="sxs-lookup"><span data-stu-id="63847-133">**Optional**</span></span>|<span data-ttu-id="63847-134">Schakel dit in om aan te geven dat het XML-element dat aangeduid wordt met de categoriecode, niet verplicht is in de elektronische btw-aangifte.</span><span class="sxs-lookup"><span data-stu-id="63847-134">Select to indicate that the XML element that is represented by the category code is not required in the electronic VAT declaration.</span></span>|  

4.  <span data-ttu-id="63847-135">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="63847-135">Choose the **OK** button.</span></span>  

<span data-ttu-id="63847-136">U kunt nu de btw-aangiftegegevens direct aan een XML-element toewijzen.</span><span class="sxs-lookup"><span data-stu-id="63847-136">You can now map the VAT statement data directly to an XML element.</span></span>  

## <a name="see-also"></a><span data-ttu-id="63847-137">Zie ook</span><span class="sxs-lookup"><span data-stu-id="63847-137">See Also</span></span>  
 <span data-ttu-id="63847-138">[Elektronische btw- en ICP-aangiften](electronic-vat-and-icp-declarations.md) </span><span class="sxs-lookup"><span data-stu-id="63847-138">[Electronic VAT and ICP Declarations](electronic-vat-and-icp-declarations.md) </span></span>  
 [<span data-ttu-id="63847-139">Procedure: Elektronische btw- en ICP-aangiften maken</span><span class="sxs-lookup"><span data-stu-id="63847-139">How to: Create Electronic VAT and ICP Declarations</span></span>](how-to-create-electronic-vat-and-icp-declarations.md)


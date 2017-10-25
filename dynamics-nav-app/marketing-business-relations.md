---
title: "Zakenrelatiecodes definiëren voor contacten"
description: "Gebruik zakenrelaties in Dynamics NAV om met marketing te helpen en de zakenrelatie aan te geven die u hebt met uw prospects, cliënten, en klanten, bijvoorbeeld, een bank- of serviceleverancier."
documentationcenter: 
author: jswymer
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: marketing, prospect, contact, client, customer
ms.date: 06/06/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 36e77c794e7aa92d5d323d93a7703359018efd39
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="setting-up-business-relations-on-contact-companies"></a><span data-ttu-id="d3e9e-103">Zakenrelaties instellen voor contactbedrijven</span><span class="sxs-lookup"><span data-stu-id="d3e9e-103">Setting Up Business Relations on Contact Companies</span></span>
<span data-ttu-id="d3e9e-104">U kunt zakenrelaties gebruiken om de zakenrelatie aan te geven die u hebt met uw contacten bijvoorbeeld een prospect, bank, serviceleverancier, enzovoort.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-104">You can use business relations to indicate the business relationship you have with your contacts, for example, a prospect, bank, consultant, service supplier, and so on.</span></span>

<span data-ttu-id="d3e9e-105">Zakenrelaties gebruiken voor contacten is een proces van twee stappen.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-105">Using business relations on contacts is a two-step process.</span></span> <span data-ttu-id="d3e9e-106">Eerst definieert u de zakenrelatiecode.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-106">First, you define the business relation code.</span></span> <span data-ttu-id="d3e9e-107">U hoeft deze stap slechts eenmaal uit te voeren voor elke zakenrelatie.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-107">You only have to perform this step one time for each business relation.</span></span> <span data-ttu-id="d3e9e-108">Als u een zakenrelatie hebt, kunt u beginnen de code toe te wijzen aan contactbedrijven.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-108">Once you have a business relation code, you can start to assign the code to contact companies.</span></span>

> [!NOTE]  
>   <span data-ttu-id="d3e9e-109">Als u de contacten wilt synchroniseren met leveranciers, klanten of bankrekeningen in een ander onderdeel van de toepassing, kunt u een zakenrelatie instellen.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-109">If you plan to synchronize your contacts with vendors, customers, or bank accounts in other parts of the application, you may want to set up a business relation for them.</span></span>

## <a name="to-define-a-business-relation-code"></a><span data-ttu-id="d3e9e-110">Een zakenrelatiecode definiëren</span><span class="sxs-lookup"><span data-stu-id="d3e9e-110">To define a business relation code</span></span>
<span data-ttu-id="d3e9e-111">De zakenrelatiecode geeft een categorie of soort aan van de zakenrelatie, zoals BANK of JURIDISCH.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-111">The business relation code defines a category or type of the business relationship, such as BANK or Law.</span></span> <span data-ttu-id="d3e9e-112">U kunt meerdere zakenrelatiecodes hebben.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-112">You can have several business relation codes.</span></span> <span data-ttu-id="d3e9e-113">Als u de zakenrelatie wilt definiëren, gebruikt u het venster **Zakenrelaties**.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-113">To define the business relation, you use the **Business Relations** window.</span></span>

1. <span data-ttu-id="d3e9e-114">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Zakenrelaties** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Business Relations**, and then choose the related link.</span></span>
2. <span data-ttu-id="d3e9e-115">Kies de actie **Nieuw** en vul een code en een beschrijving in.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-115">Choose the **New** action, and fill in a code and description.</span></span> <span data-ttu-id="d3e9e-116">De code kan maximaal uit 11 tekens bestaan en kan elke combinatie zijn van cijfers en letters.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-116">The code can be a maximum of 11 characters, and can be any combination of numbers and letters.</span></span>

## <span data-ttu-id="d3e9e-117"><a name="AssignBusRelContact"></a> Zakenrelaties toewijzen aan contacten</span><span class="sxs-lookup"><span data-stu-id="d3e9e-117"><a name="AssignBusRelContact"></a> To assign business relations to a contact</span></span>
<span data-ttu-id="d3e9e-118">U kunt geen zakenrelaties toewijzen aan een contactpersoon, alleen aan contactbedrijven.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-118">You cannot assign business relations to a contact person - only companies.</span></span>

1. <span data-ttu-id="d3e9e-119">Open het contact.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-119">Open the contact.</span></span>
2. <span data-ttu-id="d3e9e-120">Kies de actie **Bedrijf** en kies vervolgens de actie **Zakenrelaties**.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-120">Choose the **Company** action, and then the **Business Relations** action.</span></span>

    <span data-ttu-id="d3e9e-121">Het venster **Zakenrelaties (Relatie)** wordt weergegeven.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-121">The **Contact Business Relations** window opens.</span></span>
3. <span data-ttu-id="d3e9e-122">Selecteer in het veld **Zakenrelatiecode** de zakenrelatie die u wilt toewijzen.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-122">In the **Business Relation Code** field, select the business relation you want to assign.</span></span>

<span data-ttu-id="d3e9e-123">Herhaal deze stappen om het gewenste aantal zakenrelaties toe te wijzen.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-123">Repeat these steps to assign as many business relations as you want.</span></span> <span data-ttu-id="d3e9e-124">U kunt zakenrelaties ook toewijzen in het contactoverzicht door dezelfde procedure te volgen.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-124">You can also assign business relations from the contact list by following the same procedure.</span></span>

<span data-ttu-id="d3e9e-125">Het aantal zakenrelaties dat u aan het contact hebt toegewezen, wordt weergegeven in het veld **Aantal zakenrelaties** in het gedeelte **Segmentatie** van het venster **Contact**.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-125">The number of business relations you have assigned to the contact is displayed in the **No. of Business Relations** field in the **Segmentation** section in the **Contact** window.</span></span>

<span data-ttu-id="d3e9e-126">Nadat u zakenrelaties hebt toegewezen aan de contacten, kunt u deze gegevens gebruiken om contacten voor de segmenten te selecteren.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-126">After you have assigned business relations to your contacts, you can use this information to select contacts for your segments.</span></span> <span data-ttu-id="d3e9e-127">Zie voor meer informatie [Procedure: Contacten toevoegen aan segmenten](marketing-add-contact-segment.md).</span><span class="sxs-lookup"><span data-stu-id="d3e9e-127">For more information, see [How to: Add Contacts to Segments](marketing-add-contact-segment.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="d3e9e-128">Zie ook</span><span class="sxs-lookup"><span data-stu-id="d3e9e-128">See Also</span></span>
[<span data-ttu-id="d3e9e-129">Contactbedrijven maken</span><span class="sxs-lookup"><span data-stu-id="d3e9e-129">Creating Contact Companies</span></span>](marketing-create-contact-companies.md)  
<span data-ttu-id="d3e9e-130">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d3e9e-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>


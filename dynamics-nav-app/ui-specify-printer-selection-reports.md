---
title: Printerselectie opgeven voor rapporten
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 56a5c1428651162293e56d71e2369fe55d291594
ms.contentlocale: nl-nl
ms.lasthandoff: 09/11/2017

---
    
# <a name="specify-printer-selection-for-reports"></a><span data-ttu-id="e12da-102">Printerselectie opgeven voor rapporten</span><span class="sxs-lookup"><span data-stu-id="e12da-102">Specify Printer Selection for Reports</span></span>
<span data-ttu-id="e12da-103">U kunt rapporten instellen zodat ze op een specifieke printer worden afgedrukt.</span><span class="sxs-lookup"><span data-stu-id="e12da-103">You can set up reports so that they must be printed on a specific printer.</span></span> <span data-ttu-id="e12da-104">Hier volgen enkele toepassingen van de printerselectie:</span><span class="sxs-lookup"><span data-stu-id="e12da-104">The following are some uses of printer selection:</span></span> 

- <span data-ttu-id="e12da-105">U kunt rapporten afdrukken op speciaal briefpapier van het bedrijf.</span><span class="sxs-lookup"><span data-stu-id="e12da-105">You can print reports on special company letterhead.</span></span>
- <span data-ttu-id="e12da-106">U kunt rapporten afdrukken op verschillende papierformaten.</span><span class="sxs-lookup"><span data-stu-id="e12da-106">You can print reports on different paper sizes.</span></span>
- <span data-ttu-id="e12da-107">U kunt rapporten afdrukken op de standaardprinter van een opgegeven werknemer.</span><span class="sxs-lookup"><span data-stu-id="e12da-107">You can print reports on the default printer of a specified employee.</span></span>

<span data-ttu-id="e12da-108">U gebruikt het venster **Printerselecties** om verschillende waarden in te stellen om verschillende uitvoer te verkrijgen.</span><span class="sxs-lookup"><span data-stu-id="e12da-108">You use the **Printer Selections** window to set different values to obtain different output.</span></span> <span data-ttu-id="e12da-109">Als u een specifieke printer selecteert, heeft dat voorrang op een meer algemene printerselectie.</span><span class="sxs-lookup"><span data-stu-id="e12da-109">If you set a specific printer selection, then it takes precedence over a more general printer selection.</span></span> <span data-ttu-id="e12da-110">Zo kunt u instellen printerselectie met de waarden in de **Gebruikersnaam**, **Rapport-ID**, en **Printernaam**.</span><span class="sxs-lookup"><span data-stu-id="e12da-110">For example, you can set a printer selection that has values in the **User ID**, **Report ID**, and **Printer Name** fields.</span></span> <span data-ttu-id="e12da-111">Deze printerselectie heeft voorrang op een printerselectie met lege velden **Gebruikersnaam** of **Rapport-ID**.</span><span class="sxs-lookup"><span data-stu-id="e12da-111">This printer selection takes precedence over a printer selection that has blank entries in the **User ID** or **Report ID** fields.</span></span> 

<span data-ttu-id="e12da-112">De volgende tabel beschrijft de combinatie van waarden wanneer u printerinstellingen instelt voor een rapport.</span><span class="sxs-lookup"><span data-stu-id="e12da-112">The following table describes the combination of values to specify when you set up printer selections for a report.</span></span>

|<span data-ttu-id="e12da-113">Als u dit wilt doen</span><span class="sxs-lookup"><span data-stu-id="e12da-113">To</span></span>                                                 |<span data-ttu-id="e12da-114">Stel de volgende waarden in</span><span class="sxs-lookup"><span data-stu-id="e12da-114">Set the following values</span></span>                                             |
|---------------------------------------------------|---------------------------------------------------------------------|
|<span data-ttu-id="e12da-115">Een rapport afdrukken naar een specifieke printer voor alle gebruikers</span><span class="sxs-lookup"><span data-stu-id="e12da-115">Print a report to a specific printer for all users</span></span> |<span data-ttu-id="e12da-116">Geef waarden op in de velden **Rapport-ID** en **Printernaam** en laat het veld **Gebruikersnaam** leeg.</span><span class="sxs-lookup"><span data-stu-id="e12da-116">Specify values in the **Report ID** and **Printer Name** fields and leave the **User ID** field blank.</span></span>|
|<span data-ttu-id="e12da-117">Alle rapporten naar een specifieke printer afdrukken voor een specifieke gebruiker</span><span class="sxs-lookup"><span data-stu-id="e12da-117">Print all reports to a specific printer for a specific user</span></span>|<span data-ttu-id="e12da-118">Geef waarden op in de velden **Gebruikers-ID** en **Printernaam** en laat het veld **Rapport-ID** leeg.</span><span class="sxs-lookup"><span data-stu-id="e12da-118">Specify values in the **User ID** and **Printer Name** fields and leave the **Report ID** field blank.</span></span>|
|<span data-ttu-id="e12da-119">De standaardprinter voor alle rapporten instellen</span><span class="sxs-lookup"><span data-stu-id="e12da-119">Set the default printer for all reports</span></span>|<span data-ttu-id="e12da-120">Geef een waarde op in het veld **Printernaam** en laat de velden **Gebruikers-ID** en **Rapport-ID** leeg.</span><span class="sxs-lookup"><span data-stu-id="e12da-120">Specify a value in the **Printer Name** field and leave the **User ID** and **Report ID** fields blank.</span></span>|
|<span data-ttu-id="e12da-121">Een specifiek rapport afdrukken naar de standaardprinter van de gebruiker</span><span class="sxs-lookup"><span data-stu-id="e12da-121">Print a specific report to the user’s default printer</span></span>|<span data-ttu-id="e12da-122">Geef een waarde op in het veld **Rapport-ID** en laat de velden **Printernaam** en **Gebruikers-ID** leeg.</span><span class="sxs-lookup"><span data-stu-id="e12da-122">Specify a value in the **Report ID** field and leave the **Printer Name** and **User ID** fields blank.</span></span>|
|<span data-ttu-id="e12da-123">Een specifiek rapport naar een specifieke printer afdrukken voor een specifieke gebruiker</span><span class="sxs-lookup"><span data-stu-id="e12da-123">Print a specific report to a specific printer for a specific user</span></span>|<span data-ttu-id="e12da-124">Geef waarden in alle drie de velden op.</span><span class="sxs-lookup"><span data-stu-id="e12da-124">Specify values in all three fields.</span></span>|

## <a name="see-also"></a><span data-ttu-id="e12da-125">Zie ook</span><span class="sxs-lookup"><span data-stu-id="e12da-125">See Also</span></span>
[<span data-ttu-id="e12da-126">Werken met Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="e12da-126">Work with Dynamics NAV</span></span>](ui-work-product.md)


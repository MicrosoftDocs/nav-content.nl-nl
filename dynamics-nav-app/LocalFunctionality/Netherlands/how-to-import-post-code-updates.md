---
title: Postcode-updates importeren
description: "Elke maand ontvangt u een postcodebestand met alle postcodemutaties in een maand. Dit postcodebestand kan worden geïmporteerd en kan de relevante gegevens in de tabel **Postcodereeks** bijwerken."
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
ms.openlocfilehash: 891257ce2854a6da38377391333258b5d731af02
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-import-post-code-updates"></a><span data-ttu-id="c2af9-104">Procedure: Postcode-updates importeren</span><span class="sxs-lookup"><span data-stu-id="c2af9-104">How to: Import Post Code Updates</span></span>
<span data-ttu-id="c2af9-105">Elke maand ontvangt u een postcodebestand met alle postcodemutaties in een maand.</span><span class="sxs-lookup"><span data-stu-id="c2af9-105">Every month a post code file will be delivered with all post code mutations in a month.</span></span> <span data-ttu-id="c2af9-106">Dit postcodebestand kan worden geïmporteerd en kan de relevante gegevens in de tabel **Postcodereeks** bijwerken.</span><span class="sxs-lookup"><span data-stu-id="c2af9-106">This post code file can be imported and update the relevant data of the **Post Code Range** table.</span></span>  
  
### <a name="to-import-the-update-file"></a><span data-ttu-id="c2af9-107">Het updatebestand importeren</span><span class="sxs-lookup"><span data-stu-id="c2af9-107">To import the update file</span></span>  
  
1.  <span data-ttu-id="c2af9-108">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Postcode-updates** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="c2af9-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Post Codes Updates**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="c2af9-109">Kies in het venster **Postcode-updates** op het tabblad **Acties** in de groep **Functies** de optie **Postcodes-update importeren**.</span><span class="sxs-lookup"><span data-stu-id="c2af9-109">In the **Post Codes Updates** window, on the **Actions** tab, in the **Functions** group, choose **Import Post Codes Update**.</span></span>  
  
3.  <span data-ttu-id="c2af9-110">Geef het pad en de naam op van het postcode-updatebestand en kies vervolgens de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="c2af9-110">Specify the path and name of the post code update file, and then choose the **OK** button.</span></span> <span data-ttu-id="c2af9-111">Als u het bestand niet wilt importeren, kiest u de knop **Annuleren** om het venster te sluiten.</span><span class="sxs-lookup"><span data-stu-id="c2af9-111">If you do not want to import the file, choose the **Cancel** button to close the window.</span></span>  
  
 <span data-ttu-id="c2af9-112">Als geen bestand met een volledige set postcodegegevens is geïmporteerd, verschijnt er een bericht.</span><span class="sxs-lookup"><span data-stu-id="c2af9-112">If there is no file imported with a full set of post code data, then a message appears.</span></span>  
  
 <span data-ttu-id="c2af9-113">Voordat de postcodes worden bijgewerkt, worden de volgende controles uitgevoerd:</span><span class="sxs-lookup"><span data-stu-id="c2af9-113">Before updating the post codes the following checks will be performed:</span></span>  
  
-   <span data-ttu-id="c2af9-114">Is er al een updatebestand geïmporteerd met een recenter datumveld dan de datum van dit nieuwe updatebestand?</span><span class="sxs-lookup"><span data-stu-id="c2af9-114">Is there already an update file imported with a Date Field later then the date of this new update file?</span></span> <span data-ttu-id="c2af9-115">Als dat het geval is, wordt het proces gestopt.</span><span class="sxs-lookup"><span data-stu-id="c2af9-115">If so then the process will stop.</span></span>  
  
-   <span data-ttu-id="c2af9-116">Is er een lange periode tussen de datum van dit bestand en de waarde in het datumveld van het laatst geïmporteerde bestand?</span><span class="sxs-lookup"><span data-stu-id="c2af9-116">Is there a gap between the date of this file and the value in the Date Field field for the last imported file?</span></span> <span data-ttu-id="c2af9-117">Als dat het geval is, verschijnt er een bericht.</span><span class="sxs-lookup"><span data-stu-id="c2af9-117">If there is a gap then a message appears.</span></span> <span data-ttu-id="c2af9-118">U kunt kiezen of u het updatebestand nog steeds wilt importeren.</span><span class="sxs-lookup"><span data-stu-id="c2af9-118">You can choose if you still want to import the update file.</span></span>  
  
 <span data-ttu-id="c2af9-119">Gegevens over de geïmporteerde postcode worden opgeslagen in de tabel Postcode-update logpost.</span><span class="sxs-lookup"><span data-stu-id="c2af9-119">Information about the imported post code will be saved in the Post Code Update Log Entry Table table.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="c2af9-120">Zie ook</span><span class="sxs-lookup"><span data-stu-id="c2af9-120">See Also</span></span>  
 <span data-ttu-id="c2af9-121">[Nederlandse postcodes](dutch-post-codes.md) </span><span class="sxs-lookup"><span data-stu-id="c2af9-121">[Dutch Post Codes](dutch-post-codes.md) </span></span>  
 <span data-ttu-id="c2af9-122">Tabel Postcode-update logpost</span><span class="sxs-lookup"><span data-stu-id="c2af9-122">Post Code Update Log Entry Table</span></span>   
 <span data-ttu-id="c2af9-123">Venster Postcode-updates</span><span class="sxs-lookup"><span data-stu-id="c2af9-123">Post Code Updates Window</span></span>   
 <span data-ttu-id="c2af9-124">Tabel Postcodereeks</span><span class="sxs-lookup"><span data-stu-id="c2af9-124">Post Code Range Table</span></span>

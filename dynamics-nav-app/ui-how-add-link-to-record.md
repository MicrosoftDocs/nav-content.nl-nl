---
title: Koppelen vanuit records naar externe gegevens of programma's
description: Koppel een hyperlink aan een document of een website aan een bepaalde record, zoals een klant of document.
documentationcenter: 
author: jswymer
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 903d8710a8c77348e1366d9a9a29b75395887198
ms.contentlocale: nl-nl
ms.lasthandoff: 10/16/2017

---
# <a name="adding-links-to-websites-documents-or-programs-on-records"></a><span data-ttu-id="d0a03-103">Koppelingen naar websites, documenten of programma's voor records toevoegen</span><span class="sxs-lookup"><span data-stu-id="d0a03-103">Adding Links to Websites, Documents, or Programs on Records</span></span>
<span data-ttu-id="d0a03-104">Voor een bepaalde record, zoals een klant, document of verkooporder, kunt u een koppeling naar een extern document, een website of een programma toevoegen.</span><span class="sxs-lookup"><span data-stu-id="d0a03-104">On a specific record, such as a customer, document, or sales order, you can add a link to an external document, website, or program.</span></span> <span data-ttu-id="d0a03-105">Of u wilt een koppeling die wordt geopend, e-mailen naar een bepaalde geadresseerde als u het selecteert.</span><span class="sxs-lookup"><span data-stu-id="d0a03-105">Or, you may want a link that opens a new empty email to a specific recipient when you select it.</span></span> <span data-ttu-id="d0a03-106">De kaartpagina voor sommige records, zoals klanten- en leverancierskaarten, bevatten een veld **Startpagina** waarin u een internetadres (URL) kunt opgeven.</span><span class="sxs-lookup"><span data-stu-id="d0a03-106">The card page for some records, such as customer and vendor cards, include a **Home Page** field where you can enter an Internet address (URL).</span></span> <span data-ttu-id="d0a03-107">Als u andere koppelingen wilt opnemen, kunt u de methode gebruiken die in dit artikel wordt beschreven.</span><span class="sxs-lookup"><span data-stu-id="d0a03-107">To include other links, you can use the method described in this article.</span></span>

<span data-ttu-id="d0a03-108">Stel dat u afgedrukte facturen van leveranciers ontvangt.</span><span class="sxs-lookup"><span data-stu-id="d0a03-108">Another example could be when you receive printed invoices from vendors.</span></span> <span data-ttu-id="d0a03-109">U kunt deze scannen en als PDF-bestanden opslaan op een SharePoint-site.</span><span class="sxs-lookup"><span data-stu-id="d0a03-109">You can scan them and store them as .pdf files on a SharePoint site.</span></span> <span data-ttu-id="d0a03-110">Vervolgens kunt u in [!INCLUDE[d365fin_md](includes/d365fin_md.md)] een koppeling vanuit een inkoopfactuur naar de betreffende factuur in SharePoint maken.</span><span class="sxs-lookup"><span data-stu-id="d0a03-110">Then you can make a link from a purchase invoice in [!INCLUDE[d365fin_md](includes/d365fin_md.md)] to the corresponding invoice on  SharePoint.</span></span> <span data-ttu-id="d0a03-111">Ook kunt u een koppeling maken van een artikelkaart naar de overeenkomstige pagina in de onlinecatalogus van uw leverancier.</span><span class="sxs-lookup"><span data-stu-id="d0a03-111">Or, you can make a link from an item card to the corresponding page in your vendor's online catalog.</span></span>
  
## <a name="to-add-a-link-on-a-record"></a><span data-ttu-id="d0a03-112">Een koppeling aan een record toevoegen</span><span class="sxs-lookup"><span data-stu-id="d0a03-112">To add a link on a record</span></span>   
  
1.  <span data-ttu-id="d0a03-113">Open de record waaraan u de koppeling wilt koppelen, zoals een klantenkaart of een verkooporder.</span><span class="sxs-lookup"><span data-stu-id="d0a03-113">Open the record that you want to attach the link to, such as a customer card or sales order.</span></span> <span data-ttu-id="d0a03-114">Als u de koppeling aan een bepaalde regel wilt koppelen, bijvoorbeeld aan een regel in een dagboek, selecteert u de regel.</span><span class="sxs-lookup"><span data-stu-id="d0a03-114">If you want to attach the link to a specific line, such as a journal line, select the line.</span></span>  
  
2.  <span data-ttu-id="d0a03-115">Kies de actie **Koppelingen** om het venster **Koppelingen** te openen met alle koppelingen die aan die record zijn toegevoegd.</span><span class="sxs-lookup"><span data-stu-id="d0a03-115">Choose the **Links** action to open the **Links** windows that shows all the current links that are added to the record.</span></span>

3. <span data-ttu-id="d0a03-116">Als u een nieuwe koppeling wilt toevoegen, kiest u **+nieuw**.</span><span class="sxs-lookup"><span data-stu-id="d0a03-116">To add a new link, choose **+new**.</span></span> 
  
4.  <span data-ttu-id="d0a03-117">Voer in het veld **Koppelingsadres** het volgende in</span><span class="sxs-lookup"><span data-stu-id="d0a03-117">In the **Link Address** field, enter</span></span>

    -   <span data-ttu-id="d0a03-118">Als u een koppeling met een bestand op uw computer of netwerk wilt toevoegen, voert u het volledige pad en de bestandsnaam in, bijvoorbeeld **C:My Documentsinvoice1.doc**.</span><span class="sxs-lookup"><span data-stu-id="d0a03-118">To link to a file on your computer or network, enter the full path and file name, such as  **C:My Documentsinvoice1.doc**.</span></span>
    -   <span data-ttu-id="d0a03-119">Als u een koppeling met een website wilt toevoegen, voert u het internetadres (URL) in, bijvoorbeeld **www.microsoft.com**.</span><span class="sxs-lookup"><span data-stu-id="d0a03-119">To link to website, enter the Internet address (URL), such as **www.microsoft.com**.</span></span> 
    -   <span data-ttu-id="d0a03-120">Als u een koppeling met een website wilt toevoegen, voert u het internetadres (URL) in, bijvoorbeeld **www.microsoft.com**.</span><span class="sxs-lookup"><span data-stu-id="d0a03-120">To link to website, enter the Internet address (URL), such as **www.microsoft.com**.</span></span> 
    -   <span data-ttu-id="d0a03-121">Als u een koppeling met een programma wilt toevoegen, voert u een bepaalde tekenreeks in om het programma te openen.</span><span class="sxs-lookup"><span data-stu-id="d0a03-121">To link to a program, enter a specific string to open the program.</span></span> <span data-ttu-id="d0a03-122">Als u OneNote op een bepaalde pagina wilt openen, voert u bijvoorbeeld **onenote:///C:My Documentstest.one** in.</span><span class="sxs-lookup"><span data-stu-id="d0a03-122">For example, to open OneNote with a specific page, enter **onenote:///C:My Documentstest.one**.</span></span> <span data-ttu-id="d0a03-123">Als u Outlook wilt openen met een nieuwe lege e-mail naar een bepaalde alias, voert u **mailto:testalias** in.</span><span class="sxs-lookup"><span data-stu-id="d0a03-123">Or, to open Outlook with a new empty email to a specific alias, enter **mailto:testalias**.</span></span>  
  
5.  <span data-ttu-id="d0a03-124">Vul het veld **Beschrijving** in met informatie over de koppeling.</span><span class="sxs-lookup"><span data-stu-id="d0a03-124">Fill in the **Description** field with information about the link.</span></span>  
  
6.  <span data-ttu-id="d0a03-125">Kies de knop **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="d0a03-125">Choose the **Save** button.</span></span>  
  
## <a name="to-delete-a-link-from-a-record"></a><span data-ttu-id="d0a03-126">Een koppeling uit een record verwijderen</span><span class="sxs-lookup"><span data-stu-id="d0a03-126">To delete a link from a record</span></span>  
  
<span data-ttu-id="d0a03-127">Als u een koppeling wilt verwijderen, kunt u in het venster **Koppelingen** eerst **…** en vervolgens **Verwijderen** selecteren.</span><span class="sxs-lookup"><span data-stu-id="d0a03-127">To delete a link, in the **Links** window, you can select **...** and then **Delete**.</span></span>

<span data-ttu-id="d0a03-128">Als u één record verwijdert, bijvoorbeeld een verkooporderregel, een verkooporder of een klant, worden alle koppelingen verwijderd die aan die record zijn gekoppeld.</span><span class="sxs-lookup"><span data-stu-id="d0a03-128">If you delete a single record, such as a sales order line, a sales order, or a customer, then all the links attached to the record are deleted.</span></span> <span data-ttu-id="d0a03-129">Als u records echter verwijdert met een batchtaak, zoals de batchtaak **Gefact. verk.-orders verw.**, worden de koppelingen nog wel opgeslagen in de database.</span><span class="sxs-lookup"><span data-stu-id="d0a03-129">However, if you delete records using a batch job, such as the **Delete Invoiced Sales Orders** batch job, then the links are still stored in the database.</span></span> <span data-ttu-id="d0a03-130">U kunt ze uit de database verwijderen door de code-unit **Bestandskoppelingen zonder recordreferentie verwijderen** uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="d0a03-130">To delete the links from the database, run the **Delete Orphaned Record Links** codeunit.</span></span> <span data-ttu-id="d0a03-131">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Koppelingen zonder recordreferentie verwijderen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="d0a03-131">To do this, choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delete Orphaned Record Links**, and then choose the related link.</span></span>   
  
<!-- ### To run delete orphaned record links  
  
1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Data Deletion**, and then choose the related link.  
  
2.  On the **Data Deletion** page, choose **Tasks**, and then choose **Delete Orphaned Record Links**.  -->
  
## <a name="see-also"></a><span data-ttu-id="d0a03-132">Zie ook</span><span class="sxs-lookup"><span data-stu-id="d0a03-132">See Also</span></span>  
<span data-ttu-id="d0a03-133">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d0a03-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
